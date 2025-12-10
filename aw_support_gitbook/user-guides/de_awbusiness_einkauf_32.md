---
title: "DE AWBusiness Einkauf 3.2"
category: "user_manuals"
product: "Unknown"
doc_type: "Unknown"
language: "EN"
tags: ["DE_AWBusiness_Einkauf_3.2"]
version: "1.0"
last_updated: "2025-12-10"
description: "Einkauf            D                        deutsch               A+W Business                                                                                                                 Vorspann                                             Vorspann                                         In diesem Teil der Dokumentation finden Sie editorische Notizen.                                           Revisionsübersicht                                         Part             Beschreibung"
source_file: "DE_AWBusiness_Einkauf_3.2.pdf"
---


# DE AWBusiness Einkauf 3.2

Einkauf            D




                   deutsch




          A+W Business
                                                                                                                Vorspann




                                        Vorspann
                                        In diesem Teil der Dokumentation finden Sie editorische Notizen.


                                        Revisionsübersicht
                                        Part             Beschreibung
                                        Version/Datum

                                        3.30/04-2020     Wareneingang aktualisiert.

                                        3.20/11-2019     Softwarereferenz: Aktualisierung Dialog Wareneingang,
                                                         Tutorial: Kapitel für Kisten in den Part Kistenmanagement
                                                         verschoben.

                                        3.10/10-2017     Strukturelle Überarbeitung, neuer Dialog Nachbestellung, Dialog
                                                         AB-Lieferant aktualisiert.

                                        3.01/01-2017     Produkt- und Firmennamen angepasst.

                                        3.00/06-2013     Vollständige Überarbeitung der ALFAK-Dokumentation und
                                                         Anpassung auf A+W Business.

                                        2.10/02-2012     Aktualisierung der Kapitel zum Wareneingang

                                        2.00/02-2010     Aktualisierung und Umstellung auf Doku-Konzept 2010

                                        1.00/10-2008     Part Einkauf neu
                                                         Aus Part Dokumente ausgegliedert



                                        Editorial
                                        Das Editorial enthält Informationen zu folgenden Themen:
                                        •   Anmerkungen zu diesem Dokument
                                        •   Urheberrechte
                                        •   Warenzeichen
                                        •   Kontakte

                                        Anmerkungen zu diesem Dokument
                                        Diese Veröffentlichung ist ausschließlich für Endanwender von A+W Business
                                        gedacht.
                                        Diese Dokumentation und die darin beschriebene Software wird nur in Lizenz
                                        vergeben und darf nur gemäß dieser Lizenz verwendet und kopiert werden.
                                        Der Inhalt der Dokumentation dient nur der Information und kann jederzeit
                                        ohne Vorankündigung geändert werden. Bei der Zusammenstellung von Tex-
                                        ten und Abbildungen wurde mit größter Sorgfalt vorgegangen. Trotzdem kön-
3.30 / 04-2020




                                        nen Fehler nicht vollständig ausgeschlossen werden. A+W Software GmbH
                                        übernimmt keine Haftung für Fehler oder Ungenauigkeiten, es sei denn, diese
                                        beruhen auf vorsätzlichem oder grobfahrlässigem Handeln.



                 A+W Business Einkauf                                                                                D-3
                 Vorspann




                            Dieses Dokument beschreibt die volle Ausbaustufe von A+W Business.

                            Urheberrechte
                            © 2017, A+W Software GmbH, alle Rechte, auch des Nachdrucks, der Her-
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

                               +49 6404 2051-0

                               +49 6404 2051-877

                            aw.zentrale@a-w.com

                            http://www.a-w.com
3.30 / 04-2020




                 D-4                                                              A+W Business Einkauf
                                                                                                                                                            Inhalt




                                        Inhalt
                                        Vorspann ................................................................................................................ D-3
                                         Revisionsübersicht .............................................................................................. D-3
                                         Editorial ............................................................................................................... D-3

                                        Tutorial                                                                                                            D-9
                                        Überblick ............................................................................................................... D-11
                                          Dokumentation .................................................................................................. D-12
                                            Aufbau des Tutorials ...................................................................................... D-12
                                            Darstellungskonventionen .............................................................................. D-13
                                          Menü-Übersicht ................................................................................................. D-14
                                        Grundgedanken zum Einkauf ............................................................................... D-17
                                        Stammdaten für den Einkauf ................................................................................ D-20
                                          Produktdefinition ................................................................................................ D-21
                                            Bestellkennzeichen ........................................................................................ D-22
                                            Stammdaten eines Produkts prüfen ............................................................... D-25
                                            Lagermaß anlegen ......................................................................................... D-27
                                          Lieferanten ........................................................................................................ D-30
                                            Marktpartner Lieferant .................................................................................... D-31
                                            Stammdaten eines Lieferanten prüfen ........................................................... D-32
                                            Lieferantenkartei anpassen ............................................................................ D-33
                                          EK-Preise .......................................................................................................... D-36
                                            Preislisten ...................................................................................................... D-37
                                            Stammdaten der Preise prüfen ...................................................................... D-38
                                          Dokumentenstatus ............................................................................................ D-40
                                            Statuszuordnung ............................................................................................ D-41
                                            Statusvergabe ................................................................................................ D-42
                                        Bestellungen ......................................................................................................... D-43
                                          Bestellübergabe vs. manuelle Bestellung ......................................................... D-44
                                            Dokument Bestellung ..................................................................................... D-45
                                            Voreinstellungen für Bestellungen prüfen ...................................................... D-47
                                          Bestellpositionen im Auftrag .............................................................................. D-50
                                            Kundenbestellung .......................................................................................... D-51
                                            Lieferant für Auftragsposition ......................................................................... D-52
                                            Änderung in bestellten Positionen ................................................................. D-53
                                            Bestellposition im Auftrag erfassen ................................................................ D-54
                                            Lieferanten im Auftrag ändern ....................................................................... D-56
                                            Bestellte Auftragsposition ändern .................................................................. D-57
                                          Bestellübergabe ................................................................................................ D-60
                                            Bestellpool ..................................................................................................... D-62
                                            Dokument in den Bestellpool stellen .............................................................. D-68
                                            Bestellung im Bestellpool ändern ................................................................... D-72
                                            Preise im Bestellpool vergleichen .................................................................. D-74
                                            Auftrags- und Bestell-Info .............................................................................. D-78
                                          Manuelle Bestellung .......................................................................................... D-79
                                            Unabhängige Bestellungen ............................................................................ D-80
                                            Unabhängige Bestellung erfassen ................................................................. D-81
                                            Lagerbestellung erfassen ............................................................................... D-83
                                          Auftragsbestätigung des Lieferanten ................................................................. D-86
                                            Lieferanten-AB ............................................................................................... D-87
                                            Überfällige Lieferungen .................................................................................. D-88
3.30 / 04-2020




                                            Auftragsbestätigung erfassen ........................................................................ D-89
                                            AB erfassen und Preise prüfen ...................................................................... D-93
                                            Lieferanten anmahnen ................................................................................... D-97



                 A+W Business Einkauf                                                                                                                         D-5
                 Inhalt




                            Lieferterminkontrolle ........................................................................................ D-100
                               Prüfung und Korrektur von Lieferterminen ................................................... D-101
                               Liefertermine ändern und Kunden benachrichtigen ..................................... D-102
                               Alle Termine prüfen und ändern .................................................................. D-105
                            Anfrage ............................................................................................................ D-110
                               Anfrage zu Bestellpositionen oder Bestellungen ......................................... D-111
                               Anfrage zu einer Bestellposition erzeugen .................................................. D-112
                               Bestellung aus unabhängiger Anfrage erstellen .......................................... D-115
                            Übungen .......................................................................................................... D-117
                          Lieferungen im Wareneingang ............................................................................ D-119
                            Wareneingang ................................................................................................. D-120
                               Lieferungen .................................................................................................. D-121
                               Voreinstellungen für Wareneingang prüfen ................................................. D-126
                               Wareneingang erfassen ............................................................................... D-127
                               Wareneingang kontrollieren ......................................................................... D-133
                            Wareneingang von Kisten ............................................................................... D-135
                               Kistengeschäft ............................................................................................. D-136
                               Firmendaten prüfen ...................................................................................... D-136
                               Einstellungen für Identnummern prüfen ....................................................... D-137
                               Wareneingang von Kisten erfassen ............................................................. D-138
                            Preis- und Rechnungskontrolle ....................................................................... D-143
                               Eingangsrechnung ....................................................................................... D-144
                               Rechnung kontrollieren ................................................................................ D-146
                            Übungen .......................................................................................................... D-149
                          Elektronischer Dokumentenaustausch ............................................................... D-150
                            Export/Import (openTRANS) ........................................................................... D-151
                               Dokumentenaustausch ................................................................................ D-153
                               Dokumentenkontrolle ................................................................................... D-156
                               Dienste prüfen .............................................................................................. D-159
                               Statusvergabe .............................................................................................. D-160
                               Voreinstellungen für Datenaustausch prüfen ............................................... D-161
                               Währungseinstellungen prüfen .................................................................... D-162
                               Statusdefinitionen prüfen ............................................................................. D-163
                               Datenexport per openTRANS einstellen ...................................................... D-166
                               Partnerstammdaten prüfen .......................................................................... D-168
                               Elektronisches Dokument einlesen .............................................................. D-169
                               Elektronisches Dokument prüfen ................................................................. D-170
                               Teillieferung aus elektronischem Dokument erstellen ................................. D-172
                               Positionen im elektronischen Dokument zuordnen ...................................... D-173
                               Zuschläge/Rabatte manuell zuordnen ......................................................... D-175
                            Datenexport/-import (EDI) ............................................................................... D-177
                               Datenaustausch im ASC-Format ................................................................. D-178
                               Firmendaten prüfen ...................................................................................... D-178
                               Einstellungen prüfen .................................................................................... D-178
                               Bestellung exportieren ................................................................................. D-182

                          Softwarereferenz                                                                                             D-183
                          Übersicht ............................................................................................................. D-185
                          Anfrage (Menü) ................................................................................................... D-186
                            Anfrage (Dokumentenverwaltung) ................................................................... D-187
                          Bestellung (Menü) ............................................................................................... D-188
                            Bestellung (Dokumentenverwaltung) .............................................................. D-190
                            Nachbestellung ................................................................................................ D-191
3.30 / 04-2020




                            Export (EDI) ..................................................................................................... D-193
                              Menü Funktionen ......................................................................................... D-194
                              Export – Export ............................................................................................ D-195
                              Export – Pool ............................................................................................... D-196


                 D-6                                                                                            A+W Business Einkauf
                                                                                                                                                         Inhalt




                                          AB-Lieferant .................................................................................................... D-197
                                            Menü Optionen ............................................................................................ D-197
                                            AB-Lieferant – Dokumente ........................................................................... D-198
                                            AB-Lieferant – Positionen ............................................................................ D-202
                                            AB-Lieferant – Liefertermine ändern ............................................................ D-203
                                        Auftragsbestätigung ............................................................................................ D-204
                                          Preiskontrolle ................................................................................................... D-205
                                            Menü Funktionen ......................................................................................... D-205
                                            Menü Optionen ............................................................................................ D-206
                                            Preiskontrolle – Bestellungen ...................................................................... D-207
                                            Preiskontrolle – Position .............................................................................. D-210
                                            Preiskontrolle – Stückliste ............................................................................ D-212
                                          Elektronische Preiskontrolle ............................................................................ D-213
                                            Menü Funktionen ......................................................................................... D-214
                                            Menü Optionen ............................................................................................ D-214
                                            Elektronische Preiskontrolle – Dokumentenimport ...................................... D-216
                                            Elektronische Preiskontrolle – Positionsübersicht ....................................... D-219
                                          Auswahl (Prod. Nr. für Ausgleichspos.) ........................................................... D-220
                                          Einstellungen für Xternal ................................................................................. D-221
                                          Positionen manuell zuordnen .......................................................................... D-221
                                          Fußzuschläge/-rabatte verteilen ...................................................................... D-222
                                          Filtereinstellungen ........................................................................................... D-223
                                          Mahnung ......................................................................................................... D-225
                                        Wareneingang .................................................................................................... D-227
                                          Wareneingang (Dialog) ................................................................................... D-227
                                            Menü Funktionen ......................................................................................... D-228
                                            Menü Optionen ............................................................................................ D-228
                                            Menü Druck .................................................................................................. D-229
                                            Wareneingang – Auswahl ............................................................................ D-230
                                            Wareneingang – Komplett ........................................................................... D-232
                                            Wareneingang – Positionsweise .................................................................. D-234
                                            Wareneingang – Identnummer .................................................................... D-237
                                            Wareneingang – Protokoll (Identnummern) ................................................. D-239
                                          Einstellungen (ID) ............................................................................................ D-240
                                          Eingangskontrolle ............................................................................................ D-241
                                            Eingangskontrolle – Komplette Bestellungen .............................................. D-241
                                            Eingangskontrolle – Mengendiskrepanzen .................................................. D-243
                                        Rechnung ........................................................................................................... D-245
                                          Rechnungskontrolle ......................................................................................... D-245
                                            Menü Funktionen ......................................................................................... D-246
                                            Menü Optionen ............................................................................................ D-246
                                            Rechnungskontrolle – Bestellungen ............................................................ D-248
                                            Rechnungskontrolle – Positionen ................................................................ D-251
                                            Rechnungskontrolle – Stückliste .................................................................. D-253
                                          Rechnungsdatum ............................................................................................ D-255
                                          Elektronische Rechnungskontrolle .................................................................. D-256
                                            Menü Funktionen ......................................................................................... D-256
                                            Menü Optionen ............................................................................................ D-257
                                            Elektronische Rechnungskontrolle – Dokumentenimport ............................ D-259
                                            Elektronische Rechnungskontrolle – Positionsübersicht ............................. D-262
                                        Basisglasverrechnung ........................................................................................ D-264
3.30 / 04-2020




                 A+W Business Einkauf                                                                                                                      D-7
                 Inhalt




                          Partindex                                                                                                  D-265
                          Index Einkauf ...................................................................................................... D-267
3.30 / 04-2020




                 D-8                                                                                          A+W Business Einkauf
Einkauf              D

                 Tutorial




          A+W Business
                 Tutorial                                                                                    Überblick




                                        Überblick
                                        Das Tutorial zum Modul Einkauf beschäftigt sich mit den Grundlagen des Ein-
                                        kaufs in A+W Business. Das Tutorial baut auf den Kenntnissen zu den
                                        Stammdaten und zum Verkauf auf.

                                            Funktionen sind von den freigeschalteten Modulen abhängig
                                            Bitte beachten Sie, dass die unterschiedlichen Funktionen nur dann zur
                                            Verfügung stehen, wenn die zugehörigen Module und Schnittstellen instal-
                                            liert und freigeschaltet sind.

                                            Wenn Sie in dieser Beschreibung Funktionen finden, die in Ihrer Installati-
                                            on nicht zugänglich sind, wenden Sie sich bitte an die A+W Software
                                            GmbH.

                                        Themenblöcke
                                        In diesem Tutorial finden Sie folgende Themenblöcke:
                                        •   Grundgedanken zum Einkauf
                                        •   Stammdaten für den Einkauf
                                        •   Bestellungen
                                        •   Lieferungen im Wareneingang
                                        •   Elektronischer Dokumentenaustausch

                                        Vorausgesetzte Kenntnisse
                                        Das Tutorial richtet sich an Teilnehmer, die in A+W Business den Einkauf
                                        abwickeln. Die Teilnehmer müssen das Konzept der Stammdaten in
                                        A+W Business und den Dialog Dokumentenverwaltung kennen.
3.30 / 04-2020




                 A+W Business Einkauf                                                                            D-11
                 Überblick                                                                              Tutorial




                             Dokumentation
                             Für das Modul Einkauf stehen folgende Dokumente zur Verfügung:

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
3.30 / 04-2020




                 D-12                                                                  A+W Business Einkauf
                 Tutorial                                                                                      Überblick




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
                                                                 Dokumente > Bestellung > Export.

                                        []                       Eckige Klammern bezeichnen Schaltflächen im Dialog,
                                                                 z. B.: Mit [OK] speichern Sie die Daten.

                                        <>                       Spitze Klammern bezeichnen Tasten oder
                                                                 Tastenkombinationen auf der Tastatur, z. B.: Mit <F1>
                                                                 öffnen Sie die Online-Hilfe.
3.30 / 04-2020




                 A+W Business Einkauf                                                                              D-13
                 Überblick                                                                                      Tutorial




                                         Menü-Übersicht
                                         In diesem Abschnitt finden Sie eine kurze Übersicht über die Programmberei-
                                         che, die in den Themenblöcken dieser Schulung angesprochen werden.
                                         Im Menü Dokumente finden Sie auch die Programmbereiche, mit denen Sie
                                         den Verkauf abwickeln. Diese werden im Part Verkauf beschrieben.




                 Abb. D-1    Modul Dokumente – Menü Bestellung


                                         Bestellung
                                         In diesem Bereich erstellen und verwalten Sie Bestellungen.
                                          “Bestellungen” auf Seite D-43

                                         Nachbestellung
                                         In diesem Dialog verwalten Sie Aufträge mit Bestellteilen, die als Bruch gemel-
                                         det sind und entscheiden ob diese nachbestellt, reklamiert, verrechnet oder
                                         von der Auftragsmenge abgezogen werden sollen.
3.30 / 04-2020




                                          Softwarereferenz, “Nachbestellung” auf Seite D-191




                 D-14                                                                           A+W Business Einkauf
                 Tutorial                                                                                   Überblick




                                        Druck Bestellung
                                        In diesem Dialog drucken Sie die Bestellungen, die Sie an Lieferanten senden
                                        wollen. Diese Funktion ist ausführlich im Part Verkauf beschrieben.
                                         Verkauf, “Druck” auf Seite C-190

                                        Export
                                        In diesem Dialog exportieren Sie Bestellungen, um sie über die EDI-Schnitt-
                                        stelle an den betreffenden Lieferanten zu übertragen.
                                         “Bestellung exportieren” auf Seite D-182

                                        Journal
                                        In diesem Dialog verschaffen Sie sich einen Überblick über die Bestellungen.
                                        Diese Funktion ist ausführlich im Part Verkauf beschrieben.
                                         Verkauf, “Journal” auf Seite C-384

                                        AB Lieferant
                                        In diesem Dialog erfassen Sie die Auftragsbestätigungen, die Ihre Lieferanten
                                        gesendet haben.
                                         “Lieferanten-AB” auf Seite D-87

                                        Auftragsbestätigung
                                        In diesem Bereich prüfen Sie die Preise von Auftragsbestätigungen.
                                         “Rechnung kontrollieren” auf Seite D-146

                                        Wareneingang
                                        In diesem Bereich prüfen und erfassen Sie den Wareneingang zu Ihren Be-
                                        stellungen.
                                         “Wareneingang” auf Seite D-120

                                        Rechnung
                                        In diesem Bereich erfassen und kontrollieren Sie die Lieferantenrechnungen.
                                         “Elektronisches Dokument prüfen” auf Seite D-170

                                        FIBU-Übergabe
                                        In diesem Dialog übergeben Sie die eingegangenen Rechnungen an Ihre Fi-
                                        nanzbuchhaltung. Diese Funktion ist ausführlich im Part Verkauf beschrieben.
                                         Verkauf, “Sollstellung FiBu” auf Seite C-682

                                        Übergabe Archiv
                                        In diesem Dialog übergeben Sie Ihre Bestellungen an das Archiv. Diese Funk-
3.30 / 04-2020




                                        tion ist ausführlich im Part Verkauf beschrieben.
                                         Verkauf, “Übergabe Archiv” auf Seite C-686




                 A+W Business Einkauf                                                                          D-15
                 Überblick                                                                          Tutorial




                             Dokumentendaten
                             In diesem Dialog können Sie sich Übersichten über Bestellungen und korres-
                             pondierende Aufträge anzeigen lassen und ggf. die Termine korrigieren. Diese
                             Funktion ist ausführlich im Part Verkauf beschrieben.
                              Verkauf, “Dokumentendaten” auf Seite C-737

                             Lagersuche
                             In diesem Dialog können Sie die Verfügbarkeit von Produkten prüfen und nach
                             Lagermaßen suchen. Diese Funktion ist ausführlich im Part Verkauf beschrie-
                             ben.
                              Verkauf, “Lagersuche” auf Seite C-741

                             Artikel-Info
                             In diesem Dialog können Sie sich Informationen zu den Produkten anzeigen
                             lassen, die in A+W Business angelegt sind. Sie können dabei den Produktauf-
                             bau, die Preise und die Verfügbarkeit prüfen. Diese Funktion ist ausführlich im
                             Part Verkauf beschrieben.
                              Verkauf, “Artikel-Informationen” auf Seite C-602

                             Faxnachricht
                             In diesem Dialog können Sie direkt aus A+W Business Faxnachrichten an Ihre
                             Kunden und Lieferanten erstellen und versenden. Diese Funktion ist ausführ-
                             lich im Part Überblick beschrieben.
                              Einleitung, “Standard-Menüs” auf Seite A-53
3.30 / 04-2020




                 D-16                                                              A+W Business Einkauf
                 Tutorial                                                                Grundgedanken zum Einkauf




                                          Grundgedanken zum Einkauf
                                          Der Einkauf gehört zu den kaufmännischen Aufgaben im Unternehmen. Ein
                                          typischer Einkauf ist in A+W Business so oder ähnlich aufgebaut:




                                                                          Anfrage




                                                       Bestellung                      Kunden-
                                                                                       Auftrag

                                                                        Übergabe




                                                  AB + Preiskontrolle




                             Lager                    Wareneingang                               Produktion




                                                  AB + Preiskontrolle




                  Legende:                 Dokument                  Bereich                 optional



                 Abb. D-2     Schema des Einkaufs in A+W Business


                                          Alle kaufmännischen Vorgänge in A+W Business basieren auf den Stamm-
                                          daten. Nur wenn diese korrekt gepflegt sind, kann der Einkauf problemlos ab-
                                          gewickelt werden:
3.30 / 04-2020




                 A+W Business Einkauf                                                                           D-17
                 Grundgedanken zum Einkauf                                                                   Tutorial




                                      •   Anfrage:
                                          Mit der Anfrage holen Sie Angebote Ihrer Lieferanten ein. Wenn Sie das
                                          Angebot überzeugt, können Sie aus der Anfrage direkt die Bestellung er-
                                          zeugen, ohne die Daten erneut eingeben zu müssen.
                                           “Anfrage” auf Seite D-110
                                      •   Bestellung:
                                          Als manuelle Bestellung erfassen Sie die Bestellpositionen und wählen
                                          den gewünschten Lieferanten aus.
                                          Die referenzierte Bestellung wird aus dem Kundenauftrag über den Bestell-
                                          pool erzeugt.
                                           “Manuelle Bestellung” auf Seite D-79
                                      •   Auftragsbestätigung (AB) vom Lieferanten:
                                          Sie erfassen die Nummer der AB und prüfen die Preise und Liefertermine.
                                          Bei Verzögerungen benachrichtigen Sie ggf. den Kunden. Geänderte und
                                          bestätigte Preise können in die EK-Kalkulation zurückgeschrieben werden.
                                           “Auftragsbestätigung und Liefertermin” auf Seite D-87
                                      •   Wareneingang:
                                          Sie prüfen den Wareneingang und buchen automatisch die Lagerbestel-
                                          lungen in den Lagerbestand. Referenzierte Bestellungen werden als Ein-
                                          gang an die Produktion und/oder den Verkauf übergeben, um den
                                          zugehörigen Kundenauftrag weiterzubearbeiten oder abzuschließen.
                                           “Wareneingang erfassen” auf Seite D-127
                                      •   Rechnungskontrolle:
                                          Sie prüfen die Rechnung und korrigieren ggf. Ihre Einkaufspreise, sofern
                                          Sie die geänderten Preise akzeptieren. Anschließend kann die Rechnung
                                          zur Anweisung freigegeben werden.
                                           “Preis- und Rechnungskontrolle” auf Seite D-143

                                      Handlungsablauf im Einkauf
                                      Üblicherweise bearbeiten Sie ein Einkaufsdokument in folgenden Schritten:
                                      •   Anfrage erstellen (optional)
                                      •   Bestellung
                                          – Kopfdaten erfassen
                                          – Positionen erfassen
                                          – Stückliste bearbeiten
                                      •   Bestellung drucken (senden per Fax, E-Mail, elektronisch)
                                      •   Auftragsbestätigung vom Lieferanten erfassen
                                      •   Preise prüfen
                                      •   Termine und Tourenplanung nach Rückmeldungen korrigieren
                                      •   Wareneingang erfassen
                                      •   Rechnung prüfen
                                      •   Übergabe an Archiv und Statistik
                                      •   Dokument aus der Hauptdatenbank löschen
                                      Wenn die Bestellung durch die Bestellübergabe aus einem Kundenauftrag er-
                                      zeugt wurde, müssen die Daten nicht manuell erfasst werden.
3.30 / 04-2020




                 D-18                                                                          A+W Business Einkauf
                 Tutorial                                                          Grundgedanken zum Einkauf




                                        Täglicher Arbeitsablauf
                                        Am einfachsten gestalten Sie Ihren täglichen Arbeitsablauf über die Num-
                                        mernverwalter. Leeren Sie dazu den entsprechenden Nummernverwalter
                                        oder legen Sie für den aktuellen Tag einen neuen an.
                                        Erstellen Sie dann die neuen Dokumente in diesem Nummernverwalter.
                                        Auf diese Weise behalten Sie am besten im Blick, welche Dokumente neu
                                        sind und weiterverarbeitet werden können oder müssen.
3.30 / 04-2020




                 A+W Business Einkauf                                                                     D-19
                 Stammdaten für den Einkauf                                                              Tutorial




                                        Stammdaten für den Einkauf
                                        In diesem Themenblock lernen Sie, wie Sie die Stammdaten für den Einkauf
                                        anpassen.
                                        Dazu gehören folgende Lerneinheiten:
                                        •     “Produktdefinition” auf Seite D-21
                                        •     “Lieferanten” auf Seite D-30
                                        •     “EK-Preise” auf Seite D-36
                                        •     “Dokumentenstatus” auf Seite D-40
3.30 / 04-2020




                 D-20                                                                     A+W Business Einkauf
                 Tutorial                                                                   Stammdaten für den Einkauf




                                        Produktdefinition
                                        Lernziele

                                        • Stammdaten der Produkte für den Einkauf anpassen.
                                        • Beschaffungsarten für Bestellung kennenlernen.
                                        • Nutzen des Bestellkennzeichens im Auftrag kennenlernen.


                                        Nutzen

                                        • Anhand des Bestellkennzeichens erkennt A+W Business die Produkte, die bestellt
                                          werden müssen.
                                        • Über das Bestellkennzeichen wird zu einem Kundenauftrag im Bestellpool
                                          automatisch eine Bestellung erzeugt. Die Bestellung muss daher nicht manuell
                                          erfasst werden.


                                        Merke

                                        Beschaffungsart           Das Kennzeichen Beschaffungsart legt fest, wie das im
                                                                  Auftrag oder in der Bestellung erfasste Produkt beschafft
                                                                  werden soll, z. B. durch Produktion, Lagerentnahme,
                                                                  Bestellung.

                                        Bestellkennzeichen        Als Bestellkennzeichen werden folgende
                                                                  Beschaffungsarten bezeichnet:
                                                                  • Bestellung
                                                                  • Bestellung (komplett)

                                        Bestellung (komplett)     Dieses Kennzeichen wird bei Produkten mit Stückliste
                                                                  verwendet, die als Ganzes bestellt werden sollen, z. B.
                                                                  eine komplette Tür mit Beschlägen.

                                        Bestellung                Dieses Kennzeichen wird bei Produkten verwendet,
                                                                  deren einzelne Komponenten bestellt werden sollen,
                                                                  z. B. nur die Beschläge.

                                        Voreinstellungen          Stammdaten
                                                                  Produktverwaltung:
                                                                  • Register Preis/Zuschlag
                                                                  • Register Lager/Einkauf
                                                                  Firmendaten:
                                                                  •   Register Lager/EK/EDI
                                                                  •   Register Dokumente
                                                                  •   Register Parameter
                                                                  •   Register Kalkulation
3.30 / 04-2020




                 A+W Business Einkauf                                                                                D-21
                 Stammdaten für den Einkauf                                                                      Tutorial




                                        Bestellkennzeichen
                                        Der Einkauf bezieht sich auf die Produkte, die in A+W Business verwaltet wer-
                                        den. Um ein Produkt einzukaufen, muss es in einer Bestellung erfasst werden.
                                        Zu jedem Produkt legen Sie fest, wie es für die Preisberechnung, die Rabatt-
                                        findung, die Fertigung oder Bestellung usw. herangezogen wird. Nur mit den
                                        entsprechenden Kennzeichen sind z. B. automatische Übergaben an die
                                        Schnittstellen, Berechnungen und Druck in den Dokumenten möglich.
                                        Im Rahmen des Einkaufs muss die Beschaffungsart gesondert betrachtet wer-
                                        den, denn über sie erkennt A+W Business, wenn ein Produkt oder eine Kom-
                                        ponente eines Produkts eingekauft werden muss.
                                        •     Bestellartikel (komplett):
                                              Bestellung erfolgt inklusive aller Bearbeitungen, die in der Stückliste er-
                                              fasst wurden. Besteht z. B. ein VSG aus einem Float 5 mm, einer Folie und
                                              einem ESG 5 mm, so wird das VSG als Ganzes bestellt. (Beachten Sie
                                              hierzu auch die Abgrenzung zu Bestellartikel.)
                                        •     Bestellartikel:
                                              Nur das betreffende Produkt wird bestellt, ohne den Inhalt der Stückliste
                                              (z. B. Bearbeitungen) zu beachten. Besteht wiederum z. B. ein VSG aus ei-
                                              nem Float, einer Folie und einem ESG und ist das Kennzeichen Bestellar-
                                              tikel nun für das ESG gesetzt, so wird nur das ESG beim Lieferanten
                                              bestellt. Das VSG wird in Eigenfertigung produziert.
                                        Dieses Bestellkennzeichen wird automatisch in die Auftragsposition übernom-
                                        men. Im Auftrag kann aber außerdem jeder Position ein Bestellkennzeichen
                                        zugeordnet werden.
3.30 / 04-2020




                 D-22                                                                            A+W Business Einkauf
                 Tutorial                                                                        Stammdaten für den Einkauf




                                            Beschaffungsart
                                            Diese Beschaffungsarten für die Bestellung (Bestellkennzeichen) werden in
                                            den Stammdaten der Produkte festgelegt. Es wird standardmäßig herangezo-
                                            gen, wenn ein Produkt im Dokument erfasst wird. Im Auftrag und in der Bestel-
                                            lung kann es überschrieben werden.


                    * = Bestellung, ** Bestellung komplett

                                                                                            Float 4 Bronze wird gesäumt
                      ISO 150000                                                            ISO wird produziert
                      • Float_5
                      • SZR
                                                              Float 4 Bronze wird
                      • Float_4_Bronze *
                                                              ungesäumt geliefert
                        - Kanten gesäumt
                      • Stufung


                      ISO 150000                                                            ISO wird produziert
                      • Float_5
                      • SZR
                                                              Float 4 Bronze wird
                      • Float_4_Bronze **
                                                              gesäumt geliefert
                        - Kanten gesäumt
                      • Stufung


                      ISO 150000 **                           ISO wird komplett geliefert
                      • Float_5
                      • SZR
                      • Float_4_Bronze
                        - Kanten gesäumt
                      • Stufung



                 Abb. D-3     Bestellkennzeichen in der Stückliste


                                            Wenn eine Hauptposition oder eine übergeordnete Stücklisten-Komponente
                                            mit der Beschaffungsart Bestellung (komplett) gekennzeichnet ist, werden die
                                            zugehörigen Stücklisten-Komponenten nicht vom Lager abgebucht, wenn de-
                                            ren Beschaffungsart auf Lagerentnahme eingestellt ist. Die Beschaffungsart
                                            dieser Komponenten kann dann nicht geändert werden.
3.30 / 04-2020




                 A+W Business Einkauf                                                                                     D-23
                 Stammdaten für den Einkauf                                                               Tutorial




                                        Die Beschaffungsart kann pro Mandant und/oder AV-Bereich festgelegt wer-
                                        den. In diesem Fall muss in den Firmendaten die Option Abweichende Be-
                                        schaffungsart pro Mandant/AV-Bereich aktivieren aktiviert werden.




                                        A

                                        A Abweichende Beschaffungsart pro Mandant oder AV-Bereich
                                        Abb. D-4    Firmendaten – Register Parameter


                                        Preise und Zuschläge
                                        Preistabellen werden sowohl für den Einkauf als auch für den Verkauf ange-
                                        legt. Sie müssen jedem einzelnen Produkt zugewiesen werden, damit die ent-
                                        sprechenden Preise automatisch berechnet werden.
3.30 / 04-2020




                 D-24                                                                       A+W Business Einkauf
                 Tutorial                                                                  Stammdaten für den Einkauf




                                          Stammdaten eines Produkts prüfen
                                          Für den Einkauf müssen besonders all die Produktdaten vollständig erfasst
                                          sein, die standardmäßig bestellt werden.
                                          Im Part Stammdaten ist ausführlich beschrieben, wie Sie die Stammdaten zu
                                          Ihren Produkten anlegen. In der folgenden Beschreibung wird daher nur auf
                                          die Besonderheiten eingegangen, die Sie für den Einkauf beachten müssen.


                                           So prüfen Sie die Stammdaten eines Produkts
                                          1 Wählen Sie Stammdaten > Produkte > Artikel > Artikel.
                                             Der Dialog Produktverwaltung wird geöffnet.
                                              Stammdaten, “Produktverwaltung – Lager/Einkauf” auf Seite B-608
                                          2 Suchen Sie das Produkt, das Sie prüfen möchten, und wechseln Sie zum
                                            Register Preis/Zuschlag.




                                                                                                                   A


                                                                                                                   B




                    A Preisberechnung für den Verkauf                  B Preisberechnung für den Einkauf
                    Abb. D-5    Produktverwaltung – Preis/Zuschlag


                                          3 Prüfen Sie, ob die Preistabellen und die Checkboxen Preisrelevant für VK
                                            (A) und EK (B) richtig gewählt sind.
3.30 / 04-2020




                                             Die Checkbox Preisrelevant EK muss nur dann markiert sein, wenn Sie mit
                                             der EK-Kalkulation arbeiten.



                 A+W Business Einkauf                                                                            D-25
                 Stammdaten für den Einkauf                                                                      Tutorial




                                              Weitere Informationen zu den Preisen finden Sie unter:
                                               “EK-Preise” auf Seite D-36
                                         4 Wechseln Sie zum Register Lager/Einkauf.




                                                                                                                       A




                                                                                                                       B




                   A Auswahl der Beschaffungsart                         B Auswahl bei abweichenden Kennzeichen
                   Abb. D-6    Produktverwaltung – Lager/Einkauf


                                         5 Prüfen Sie, ob die Beschaffungsart (A) richtig eingestellt ist.
                                              Für Bestellartikel können Sie folgende Einträge auswählen:
                                              •   Bestellung (komplett):
                                                  Produkt mit Stückliste und Produkt, das als Ganzes bestellt wird, z. B.
                                                  eine komplette Tür mit Beschlägen.
                                              •   Bestellung:
                                                  Produkt ohne Stückliste und Produkt, das als Stücklisten-Komponenten
                                                  (ganz oder teilweise) bestellt wird.
                                         6 Wählen Sie im Menü Start > Speichern, um die Daten zu speichern.
                                              Die Daten werden gespeichert.
3.30 / 04-2020




                 D-26                                                                            A+W Business Einkauf
                 Tutorial                                                                     Stammdaten für den Einkauf




                                             Lagermaß anlegen
                                             Für die korrekte Preisberechnung können Sie Lagermaße zu den Produkten
                                             anlegen, z. B. Gläser mit festen Maßen. Wenn ein Produkt auch als Lagerar-
                                             tikel geführt werden soll, müssen Sie es außerdem in der Lagerverwaltung an-
                                             legen. Eine Beschreibung dazu finden Sie im Part Lagerwirtschaft.


                                              So legen Sie Lagermaße in den Stammdaten an
                                             1 Wählen Sie Stammdaten > Produkte > Artikel > Lagermaße.
                                                Der Dialog Produktverwaltung Lagermaße wird geöffnet.
                                                 Stammdaten, “Lagermaße” auf Seite B-637
                                             2 Wählen Sie im Menü Start > Neu, um in den Erfassungs-Modus zu wech-
                                               seln.


                                         B                A




                 C

                 D




                 A Maße der Platte                                  C Preistabellen für Verkauf und Einkauf einstellen
                 B Inhalt bei Kisten                                D Preisermittlung im Lager
                 Abb. D-7     Felder für Lagermaß freigeschaltet


                                             3 Geben Sie die Maße (A) an.
3.30 / 04-2020




                                                Falls Sie in der Lagerverwaltung bereits einen entsprechenden Lagerarti-
                                                kel definiert haben sollten, tragen Sie die gleichen Werte für Breite und
                                                Höhe ein.


                 A+W Business Einkauf                                                                                    D-27
                 Stammdaten für den Einkauf                                                                  Tutorial




                                        4 Wenn das Lagermaß als Kiste verwaltet wird, geben Sie an, wie viele Blät-
                                          ter (B) in der Kiste enthalten sind.
                                        5 Sie können zusätzlich folgende abweichende Angaben einstellen:
                                              •   Preisschlüssel (C) für den Verkauf und den Einkauf.
                                              •   Bezeichnung und Kurzbezeichnung (Matchcode), z. B. um den Lager-
                                                  artikel besser identifizieren zu können.
                                              •   Beschaffungsart, z. B. Lagerentnahme bei Lagermaßen, die auch als
                                                  Lagerartikeln vorhanden sind.
                                              Wenn Sie das Lagermaß auch als Lagerartikel anlegen wollen, müssen Sie
                                              entscheiden, ob die Preisermittlung auch im Lager durchgeführt werden
                                              soll.
                                        6 Markieren Sie die Checkbox EK Suche Lager (D), wenn das Lagermaß in
                                          die Preisermittlung einbezogen werden soll.




                   Abb. D-8    Neues Lagermaß für die Preisberechnung


                                        7 Wählen Sie im Menü Start > Speichern, um die Daten zu speichern.
                                              Die Daten werden gespeichert. Anschließend wird die Abfrage angezeigt,
                                              ob Sie dieses Lagermaß auch als Lagerartikel anlegen möchten.
                                        8 Wählen Sie [Ja], wenn das Lagermaß auch als Lagerartikel verwaltet wer-
3.30 / 04-2020




                                          den soll.




                 D-28                                                                         A+W Business Einkauf
                 Tutorial                                                                Stammdaten für den Einkauf




                                        Der Dialog Lagerverwaltung wird geöffnet. Wie Sie Lagerartikel anlegen,
                                        ist ausführlich im Part Lagerwirtschaft beschrieben.
                                         Lagerwirtschaft, “Lagerartikel anlegen” auf Seite G-74
3.30 / 04-2020




                 A+W Business Einkauf                                                                        D-29
                 Stammdaten für den Einkauf                                                                       Tutorial




                                        Lieferanten
                                        Lernziele

                                        • Lieferanten als Marktpartner anlegen.
                                        • Standard-Lieferant zuordnen.
                                        • Lieferantenkartei kennenlernen.


                                        Nutzen

                                        • Bestellungen können über die hinterlegten Kommunikationswege direkt an den
                                          Lieferanten gesendet werden.
                                        • Standard-Lieferanten werden in der Bestellung automatisch erfasst. Sie können
                                          jedoch geändert werden, wenn dies erforderlich ist.
                                        • Über die Angaben zur Lieferdauer werden die Termine für Bestellungen und
                                          referenzierte Aufträge errechnet.


                                        Merke

                                        Marktpartner               Alle Lieferanten werden im Dialog Partnerverwaltung
                                                                   angelegt.

                                        Lieferantenkartei          In der Lieferantenkartei wird festgelegt, welche
                                                                   Lieferanten welche Produkte bzw. Warengruppen liefern.
                                                                   Diese Angaben werden u. a. für die Übergabe von
                                                                   Bestellpositionen an den Einkauf benötigt.

                                        Standard-Lieferant         Wenn für ein Produkt oder eine Warengruppe mehrere
                                                                   Lieferanten eingetragen sind, wird ein Standard-
                                                                   Lieferant festgelegt.

                                        Voreinstellungen           Stammdaten:
                                                                   • Lieferantendaten (Marktpartner)
                                                                   • Lieferantenkartei
3.30 / 04-2020




                 D-30                                                                            A+W Business Einkauf
                 Tutorial                                                                 Stammdaten für den Einkauf




                                        Marktpartner Lieferant
                                        Lieferanten werden in A+W Business angelegt, damit Bestellungen automati-
                                        siert abgearbeitet werden können. Bei der Erfassung von Aufträgen und Be-
                                        stellungen müssen die Daten der Lieferanten daher nicht gesondert erfasst
                                        werden.
                                        Lieferanten werden wie die Kunden im Dialog Partnerverwaltung angelegt. In
                                        den Stammdaten der Lieferanten müssen die Daten für die Kommunikation
                                        korrekt hinterlegt sein, damit Dokumente direkt aus A+W Business heraus
                                        versendet werden können.

                                        Lieferantenkartei
                                        In der Lieferantenkartei wird festgelegt, welche Lieferanten welche Produkte
                                        bzw. Warengruppen liefern. Werden für einen Lieferanten ein Produkt und die
                                        dazugehörigen Warengruppen angegeben, berücksichtigt die Bestellüberga-
                                        be das Produkt vorrangig.
                                        Die Angaben aus der Lieferantenkartei werden ignoriert, wenn im Dokumen-
                                        tenkopf zu einer Position oder zu einer Stücklisten-Komponente ein abwei-
                                        chender Lieferant eingegeben ist.
                                        Wenn für ein Produkt mehrere Lieferanten angegeben sind, kann bei der Be-
                                        stellübergabe ein Preisvergleich gestartet werden. Gleichzeitig wird die Liefer-
                                        dauer angezeigt, so dass auch hinterlegte Lieferzeiten berücksichtig werden
                                        können.

                                        Standard-Lieferant
                                        Wenn ein Standard-Lieferant festgelegt ist, muss die Bestellung nicht über den
                                        Bestellpool gesendet werden. Der Standard-Lieferant wird mit der Rangnum-
                                        mer 1 gekennzeichnet, alle weiteren Lieferanten erhalten die Folgenummern
                                        in der Reihenfolge, die ihrer Bedeutung für den Einkauf entspricht.
                                        Pro Produkt gibt es nur einen Standard-Lieferanten. Wenn aber ein bestimm-
                                        tes Produkt in großer Stückzahl bestellt wird, die der Standard-Lieferant nicht
                                        produzieren kann, kann zusätzlich ein Standard-Lieferant für Serienaufträge
                                        angelegt werden. In der Auftragserfassung aktivieren Sie in einem solchen
                                        Fall den Dokumententyp Serienauftrag. Bei der Bestellübergabe wird dann
                                        automatisch der Lieferant für Serienaufträge herangezogen.
3.30 / 04-2020




                 A+W Business Einkauf                                                                             D-31
                 Stammdaten für den Einkauf                                                                       Tutorial




                                         Stammdaten eines Lieferanten prüfen
                                         Damit die Bestellungen korrekt abgewickelt werden können, müssen Sie die
                                         Stammdaten eines Lieferanten und die Zuordnung von Produkten zu Lieferan-
                                         ten einrichten.
                                         Im Part Stammdaten ist ausführlich beschrieben, wie Sie die Stammdaten zu
                                         Ihren Partnern anlegen. In der folgenden Beschreibung wird daher nur auf die
                                         Besonderheiten eingegangen, die Sie für den Einkauf beachten müssen.


                                          So prüfen Sie die Stammdaten der Lieferanten
                                         1 Wählen Sie Stammdaten > Marktpartner > Lieferant > Lieferanten.
                                               Stammdaten, “Partnerverwaltung” auf Seite B-756
                                         2 Suchen Sie den Lieferanten, dessen Daten Sie prüfen wollen.




                                                                                                                             B




                    A




                   A E-Mail-Adresse des Lieferanten                 B Sprache, in der Formulare gedruckt werden
                   Abb. D-9    Stammdaten – Lieferanten


                                         3 Prüfen Sie im Register Adresse, ob die Daten für den Schriftverkehr und
                                           die Kommunikation vollständig und aktuell sind.
3.30 / 04-2020




                                              Die E-Mail-Adresse kann auch für den Austausch von elektronischen Do-
                                              kumenten genutzt werden, z. B. von PDF-Dateien. Achten Sie auf die kor-
                                              rekte und vollständige Schreibweise.



                 D-32                                                                             A+W Business Einkauf
                 Tutorial                                                                     Stammdaten für den Einkauf




                                          4 Wechseln Sie zum Register Auftrag und prüfen Sie, ob der Dokumenten-
                                            versand richtig aktiviert ist.




                                                   A       B
                                             A Bestellung per Fax-Versand            B Anfrage per E-Mail-Versand
                                             Abb. D-10     Fax- und E-Mail-Versand (Beispiel für Einstellungen)


                                          5 Wählen Sie im Menü Start > Speichern, um die Änderungen zu speichern.
                                             Die Daten werden gespeichert.


                                          Lieferantenkartei anpassen
                                          In der Lieferantenkartei legen Sie fest, welche Lieferanten welche Produkte
                                          bzw. Warengruppen liefern und wie lange die Lieferzeiten sind.


                                           So prüfen Sie die Lieferantenkartei
                                          1 Wählen Sie Stammdaten > Marktpartner > Lieferant > Kartei.
                                             Der Dialog Lieferantenkartei wird mit dem Register Produkte geöffnet.
                                          2 Wählen Sie im Menü Start > Filter, um in den Such-Modus zu wechseln.




                    A
                    B
3.30 / 04-2020




                    A Option Produkt                               B Auswahl der Varianten
                    Abb. D-11   Lieferantenkartei – Produktsuche


                 A+W Business Einkauf                                                                               D-33
                 Stammdaten für den Einkauf                                                                       Tutorial




                                         3 Wählen Sie die Option Produkt (A) und tragen Sie die Nummer des Pro-
                                           dukts ein.
                                         4 Wählen Sie im Menü Start > Suchen, um in die Suche zu starten.
                                              Im Bereich Produkt - Lieferanten werden alle Lieferanten aufgeführt, die
                                              das gewählte Produkt liefern können. Mit dem Rang 1 ist der Standard-Lie-
                                              ferant gekennzeichnet.




                    A

                    B




                                                              C                    D
                   A Abweichende Bezeichnungen                    C Rang 1 = Standard-Lieferant
                   B Lieferzeit                                   D Rangfolge ändern
                   Abb. D-12   Lieferantenkartei – Produkte


                                         5 Tragen Sie die Anzahl (B) der Tage ein, die zur Berechnung der Lieferzeit
                                           herangezogen werden soll.
                                              Die Lieferzeit wird bei der Bestellübergabe im Preisvergleich und bei der
                                              Lieferterminkontrolle berücksichtigt.
                                         6 Prüfen Sie die Rangfolge der Lieferanten und korrigieren Sie diese ggf., in-
                                           dem Sie einen Eintrag markieren und mit den Pfeilschaltflächen (D) nach
                                           oben oder unten verschieben.
                                              Die Rangnummer 1 (C) bezeichnet den Standard-Lieferanten. Er wird au-
                                              tomatisch bei Bestellungen eingesetzt, die nicht im Bestellpool geprüft wer-
                                              den.
                                         7 Wenn Ihr Lieferant abweichende Produktbezeichnungen benutzt, tragen
3.30 / 04-2020




                                           Sie diese ein (A).
                                              Diese Bezeichnungen werden in der Bestellung aufgeführt und helfen,
                                              Missverständnisse zu vermeiden.


                 D-34                                                                             A+W Business Einkauf
                 Tutorial                                                           Stammdaten für den Einkauf




                                        8 Wählen Sie im Menü Start > Speichern, um die Änderungen zu speichern.
                                          Wenn Sie ganze Warengruppen prüfen möchten, wechseln Sie zum Regis-
                                          ter Warengruppen und verfahren analog.
3.30 / 04-2020




                 A+W Business Einkauf                                                                    D-35
                 Stammdaten für den Einkauf                                                                           Tutorial




                                        EK-Preise
                                        Lernziele

                                        • Preisjahrgang, Preisschlüssel und Tarife für Einkaufspreise (EK) kennenlernen.
                                        • EK-Preise bearbeiten.


                                        Nutzen

                                        • Einkaufspreise werden bei der Erfassung von Aufträgen und Bestellungen
                                          berechnet, so dass der Deckungsbeitrag automatisch berechnet werden kann.
                                        • EK-Preise können in der Bestellung überschrieben werden.


                                        Merke

                                        Preisliste                 Preisjahrgänge, -schlüssel und Tarife bilden den
                                                                   Rahmen für die Preislisten.

                                        Individualpreise           Individuelle Preise von Lieferanten können Sie mit allen
                                                                   Bezugsgrößen einrichten, die auch für die allgemeinen
                                                                   Preislisten und Zuschläge gelten.

                                        Voreinstellungen           Stammdaten:
                                                                   •   Jahrgang
                                                                   •   Schlüssel
                                                                   •   Tarife
                                                                   •   Preise
                                                                   Firmendaten:
                                                                   • Register Lager / EK / EDI
                                                                   • Register Preisberechnung
                                                                   • Register Fibu
                                                                   Referenzen:
                                                                   • Preisimport VEGLA
                                                                   Utilities:
                                                                   • Preislistenimport
3.30 / 04-2020




                 D-36                                                                             A+W Business Einkauf
                 Tutorial                                                                 Stammdaten für den Einkauf




                                        Preislisten
                                        Die Preisberechnung in A+W Business ist aus flexiblen Bausteinen zusam-
                                        mengesetzt, die alle Berechnungsmöglichkeiten abdecken. Sie können jedem
                                        Produkt die passende Art der Preisberechnung zuordnen.
                                        Preisjahrgänge, -schlüssel und Tarife bilden den Rahmen für die Preislisten.
                                        In den Preistabellen selbst sind die Beträge hinterlegt, die in den Dokumenten
                                        herangezogen werden.
                                        Preise legen Sie als Standard-Preislisten oder als Preislisten für bestimmte
                                        Kunden- oder Lieferantengruppen, für einzelne Kunden oder für einzelne Lie-
                                        feranten fest.
                                        Im Einkauf arbeiten Sie in der Regel nur mit einem Preisschlüssel, z. B. dem
                                        Schlüssel EK. Sie können aber auch im Einkaufsbereich nach verschiedenen
                                        Preisschlüsseln differenzieren.
                                        Bei der Preisfindung wird folgende Hierarchie durchlaufen:
                                        •   Manuelle Preiseingaben im Auftrag oder Angebot (oberste Priorität)
                                        •   Objektbezogene Vereinbarungen
                                        •   Kunden-/lieferantenbezogene Vereinbarungen
                                        •   Gruppenspezifische Vereinbarungen
                                        •   Allgemeine Vereinbarungen
                                        Innerhalb dieser Hierarchiestufen können allgemeine Preise, Sonderbedin-
                                        gungen für Warengruppen und einzelne Produkte, Austauschpreise und Zu-
                                        schläge für Modelle und Sprossen hinterlegt werden.

                                        Individualpreise
                                        Bei der Gestaltung individueller Preise für Kunden und Lieferanten können Sie
                                        alle Bezugsgrößen nutzen, die auch für die allgemeinen Preislisten und
                                        Zuschläge gelten. So können Sie entweder Preistabellen für Ihre einzelnen
                                        Kunden oder Lieferanten anlegen oder die Preise im Dokument vereinba-
                                        rungsgemäß anpassen.

                                        Preislistenimport
                                        Preislisten Ihrer Lieferanten können Sie importieren, wenn diese als Datei vor-
                                        liegen.

                                            Historie der Preisänderungen
                                            Wenn Sie mit einer Gupta-Datenbank arbeiten, können Sie Änderungen
                                            der Preise in einer Historie verfolgen. Diese Funktion ist im Part Stammda-
                                            ten beschrieben.
3.30 / 04-2020




                 A+W Business Einkauf                                                                            D-37
                 Stammdaten für den Einkauf                                                                     Tutorial




                                          Stammdaten der Preise prüfen
                                          In Bestellungen können die Preise nur berechnet werden, wenn die Einkaufs-
                                          preise korrekt sind. Im Part Stammdaten ist ausführlich beschrieben, wie Sie
                                          die Stammdaten zu Ihren Preisen anlegen. In der folgenden Beschreibung
                                          wird daher nur auf die Besonderheiten eingegangen, die Sie für den Einkauf
                                          beachten müssen.


                                           So prüfen Sie die Stammdaten Ihrer Preislisten
                                          1 Wählen Sie Stammdaten > Preise > Preise und prüfen Sie, ob der Jahr-
                                            gang, der Schlüssel und der Tarif für die Einkaufspreise (EK) richtig defi-
                                            niert sind.
                                          2 Wechseln Sie zum Dialog Preise und lassen Sie sich die Tabelle und den
                                            Tarif für die EK-Preise anzeigen.
                                              Wenn Sie die Suche nicht einschränken, werden alle Preistabellen aufge-
                                              listet.


                                     A                                   B




                 A Einzelpreis                                     B Preistabelle
3.30 / 04-2020




                 Abb. D-13   EK-Preistabellen – Preisauswahl


                                               Stammdaten, “Preise – Preisauswahl” auf Seite B-715



                 D-38                                                                            A+W Business Einkauf
                 Tutorial                                                                   Stammdaten für den Einkauf




                                          3 Markieren Sie die Preistabelle (B), die Sie prüfen wollen, und wechseln Sie
                                            zu dem Register, in dem der Preis festgelegt ist.
                                             In diesem Beispiel ist der Einzelpreis (A) geprüft.


                                                             A   B                                    C




                    A Preis                          B Preiseinheit                    C Währung
                    Abb. D-14   Preisauswahl – Einzelpreis


                                             In der Übersicht sind alle Tarife der ausgewählten Preistabelle aufgeführt.
                                             Die nicht definierten Preise sind in roter Schrift angezeigt.
                                          4 Prüfen Sie, ob der Preis auf dem aktuellen Stand ist, oder korrigieren Sie
                                            ihn. Setzen Sie dazu den Cursor in die Zelle Preis und überschreiben Sie
                                            den Eintrag.
                                          5 Wählen Sie im Menü Start > Speichern, um die Daten zu speichern.
                                             Die Daten werden gespeichert.


                                          Ergänzende Informationen
                                           Stammdaten, “Stammdaten für Preise” auf Seite B-211
3.30 / 04-2020




                                           Stammdaten, “Einzelpreise anlegen” auf Seite B-236
                                           Stammdaten, “Firmendaten – Kalkulation” auf Seite B-981




                 A+W Business Einkauf                                                                             D-39
                 Stammdaten für den Einkauf                                                                           Tutorial




                                        Dokumentenstatus
                                        Lernziele

                                        • Statusumsetzung von referenzierten Dokumenten kennenlernen.
                                        • Statuszuordnung prüfen.


                                        Nutzen

                                        • Statuszuordnungen für referenzierte Dokumente werden neben den
                                          Statuszuordnungen für unabhängige Dokumente gepflegt. Anhand des Status
                                          kann also erkannt werden, ob eine Bestellung referenziert ist.
                                        • Wareneingänge zu einer Bestellung setzen den Status des referenzierten Auftrags
                                          um. So kann am Auftrag der aktuelle Stand erkannt werden.


                                        Merke

                                        Statuszuordnungen          Statuszuordnungen für referenzierte Dokumente müssen
                                                                   den gleichen Mindeststatus haben.

                                        Statusumsetzung            Der Status des referenzierten Auftrags wird beim
                                                                   Wareneingang der Bestellung umgesetzt.

                                        Voreinstellungen           Stammdaten:
                                                                   • Statuszuordnung
3.30 / 04-2020




                 D-40                                                                            A+W Business Einkauf
                 Tutorial                                                                   Stammdaten für den Einkauf




                                        Statuszuordnung
                                        Die Einkaufsdokumente durchlaufen von der Erfassung bis zur Archivierung
                                        mehrere Programmpunkte, die jeweils durch einen Status gekennzeichnet
                                        sind. An diesen Status können Bedingungen und Sperren geknüpft sein.
                                        Wie Sie die Statuspunkte und -zuordnungen einrichten, hängt von den Ge-
                                        schäftsabläufen in Ihrem Unternehmen ab. Eine ausführliche Beschreibung
                                        finden Sie dazu im Part Stammdaten.




                                                                                                                       A




                                                                                                                       B




                                        A Status für Auftrag mit referenzierter   B Korrespondierender Status für
                                          Bestellung                                Bestellung
                                        Abb. D-15     Statuszuordnung für referenzierte Dokumente


                                        Statuszuordnungen werden für referenzierte Dokumente und für unabhängige
                                        Dokumente getrennt eingerichtet, z. B. für den Wareneingang.
3.30 / 04-2020




                 A+W Business Einkauf                                                                               D-41
                 Stammdaten für den Einkauf                                                                           Tutorial




                                        Statusvergabe
                                        Der Status der Dokumente wird in der Regel umgesetzt, wenn eine Bestellung
                                        geändert, versendet usw. wird. Dabei wird unterschieden, ob die Bestellung
                                        durch einen Auftrag oder unabhängig erzeugt wurde.

                                              Beispiele

                                              für Aufträge                          für Bestellungen

                                              30 - Auftrag in Einkauf übergeben

                                              31 - AB Lieferant teilweise/Auftrag   62 - AB Lieferant teilweise/Bestellung

                                              32 - AB Lieferant komplett/Auftrag    63 - AB Lieferant komplett/Bestellung

                                              33 - Wareneingang teilweise/Auftrag   64 - Wareneingang teilweise/Bestellung

                                              34 - Wareneingang komplett/Auftrag    65 - Wareneingang komplett/Bestellung

                                                                                    66 - Rechnungskontrolle


                                        Wenn im Wareneingang die Nummer der Auftragsbestätigung (AB) des Liefe-
                                        ranten eingegeben ist, wird der Status der Bestellung umgesetzt.
                                        Wenn ein Wareneingang zu einer Bestellung aus einem Kundenauftrag (refe-
                                        renzierte Bestellung) verbucht wird, zu dem weitere Bestellungen noch offen
                                        sind, wird der Status des Auftrages auf Wareneingang teilweise/Auftrag ge-
                                        setzt.


                                        Ergänzende Informationen
                                         Verkauf, “Status” auf Seite C-221
                                         Stammdaten, “Geschäftsabläufe abbilden” auf Seite B-420
                                         Stammdaten, “Statuszuordnung” auf Seite B-887
3.30 / 04-2020




                 D-42                                                                               A+W Business Einkauf
                 Tutorial                                                                              Bestellungen




                                        Bestellungen
                                        In diesem Themenblock lernen Sie, wie Sie Bestellungen erzeugen und Ter-
                                        mine prüfen.
                                        Dazu gehören folgende Lerneinheiten:
                                        •   “Bestellübergabe vs. manuelle Bestellung” auf Seite D-44
                                        •   “Bestellpositionen im Auftrag” auf Seite D-50
                                        •   “Bestellübergabe” auf Seite D-60
                                        •   “Manuelle Bestellung” auf Seite D-79
                                        •   “Auftragsbestätigung des Lieferanten” auf Seite D-86
                                        •   “Lieferterminkontrolle” auf Seite D-100
                                        •   “Anfrage” auf Seite D-110
                                        Üblicherweise erfassen Sie eine Bestellung in folgenden Schritten:
                                        •   Anfrage erstellen (optional)
                                        •   Bestellung erfassen
                                        •   Bestellung an den Lieferanten senden
                                        •   Auftragsbestätigung vom Lieferanten erfassen
                                            – Preise prüfen
                                            – Termine und Tourenplanung nach Rückmeldungen korrigieren
                                            – Kunden über Terminänderungen informieren
                                        •   Auftragsbestätigung des Lieferanten anmahnen
                                        Diese Reihenfolge entspricht im Wesentlichen auch der Reihenfolge der Dia-
                                        loganordnung in A+W Business. Einige der Schritte können jedoch über meh-
                                        rere Dialoge ausgeführt werden. Sie sind daher in einer Lerneinheit
                                        zusammengefasst.
                                        Die Preise können bereits auf einer Auftragsbestätigung des Lieferanten ge-
                                        prüft werden. In der Praxis kann durchaus vorkommen, dass Auftragsbestäti-
                                        gung und Lieferung zusammen mit der Rechnung eintreffen. Da die Dialoge
                                        für die Preiskontrolle und die Rechnungskontrolle identisch sind, wird das
                                        Konzept der Preis- und Rechnungskontrolle im Themenblock Wareneingang
                                        beschrieben.
                                         “Eingangsrechnung” auf Seite D-144
                                        Eine Anfrage wird logischerweise vor der Bestellung erstellt, sie ist jedoch
                                        nicht zwingend erforderlich. In diesem Tutorial wird die Anfrage nach den Be-
                                        stellungen behandelt, weil Sie dann bereits mit allen Details der Bestellung
                                        vertraut sind.
3.30 / 04-2020




                 A+W Business Einkauf                                                                          D-43
                 Bestellungen                                                                             Tutorial




                                Bestellübergabe vs. manuelle Bestel-
                                lung
                                Lernziele

                                • Unterschied zwischen automatischer (referenzierter) und unabhängiger Bestellung
                                  kennenlernen.


                                Nutzen

                                • Auftragspositionen, die bestellt werden müssen, können automatisch in eine
                                  (referenzierte) Bestellung geleitet werden.
                                • Lagerbestände werden durch Lagerbestellungen ergänzt. Diese werden manuell
                                  erfasst. Sie können auch durch Unterschreitung von Mindestbeständen angelegt
                                  werden. (Diese Funktion ist im Part Lagerwirtschaft beschrieben.)


                                Merke

                                Bestellung aus Auftrag     Auftragspositionen, die bestellt werden müssen, werden
                                                           im Bestellpool an den Einkauf übergeben. Mit der
                                                           Übergabe wird automatisch eine Bestellung erzeugt.

                                Referenzierte Bestellung   Aus einer Auftragsposition, die an den Einkauf
                                                           übergeben wurde, wird eine referenzierte Bestellung mit
                                                           einer eigenen Dokumentennummer erzeugt.

                                Unabhängige Bestellung     Unabhängige Bestellungen werden manuell erfasst.
                                                           Bei unabhängigen Bestellungen wird der Lagerbestand
                                                           nicht aktualisiert, wenn der Wareneingang gebucht wird.

                                Lagerbestellung            Lagerbestellungen dienen dazu, den Lagerbestand
                                                           aufzufüllen. Sie können manuell erfasst werden.

                                Voreinstellungen           Stammdaten:
                                                           • Lieferantendaten (Marktpartner)
                                                           • Lieferantenkartei
                                                           Firmendaten:
                                                           • Register Dokumente
                                                           • Register Parameter
                                                           • Register Lager/EK/EDI
3.30 / 04-2020




                 D-44                                                                    A+W Business Einkauf
                 Tutorial                                                                                    Bestellungen




                                             Dokument Bestellung
                                             Bestellungen können entweder auftragsabhängig oder unabhängig
                                             eingegeben werden:
                                             •   Auftragsabhängige (referenzierte) Bestellungen beziehen sich auf eine Po-
                                                 sition im Kundenauftrag. Sie werden durch die Bestellübergabe erzeugt. Im
                                                 Bestellpool schlägt A+W Business aufgrund der Daten aus der Lieferan-
                                                 tenkartei einen Lieferanten vor.
                                             •   Unabhängige Bestellungen dienen in der Regel nicht dazu, den Lagerbe-
                                                 stand aufzufüllen, da der Wareneingang nicht automatisch den Lagerbe-
                                                 stand aktualisiert. Sie werden manuell erfasst.
                                             •   Lagerbestellungen dienen dazu, den Lagerbestand aufzufüllen. Sie kön-
                                                 nen manuell erfasst oder durch Unterschreitung eines Mindestbestands er-
                                                 zeugt werden.




                     Auftragsabhängige
                     Bestellung                                                           Auftrag

                                                               Wareneingang
                     Unabhängige
                     Bestellung




                     Manuelle
                     Lagerbestellung
                                                               Wareneingang
                     Automatische
                     Lagerbestellung



                                                            Lager
                                                            • Float 3
                            Mindestbestand                  • Float 4
                                                            • Float 5
                                                            • …




                 Abb. D-16     Arten der Bestellung


                                             In dieser vereinfachten Darstellung sehen Sie, wozu die unterschiedlichen Be-
                                             stellungen erfasst werden. In den folgenden Einheiten werden die auftragsab-
                                             hängigen und die unabhängigen Bestellungen ausführlich beschrieben.
3.30 / 04-2020




                                             Lagerbestellungen werden ausführlich im Part Lagerwirtschaft beschrieben.




                 A+W Business Einkauf                                                                               D-45
                 Bestellungen                                                                          Tutorial




                                Alle Bestellungen sind eigene Dokumente mit einem eigenen Nummernkreis.
                                Sie werden im Dialog zur Dokumentenverwaltung angezeigt und können un-
                                abhängig davon, wie sie erzeugt wurden, bearbeitet werden.




                                A




                                B




                                C




                                A Anlieferung durch den            C Dokumententyp:
                                  Lieferanten                        - <k. A.>: automatische oder manuelle
                                B Zusatz-Informationen, z. B.          Bestellung
                                  Referenz auf Auftrag               - Lagerbestellung

                                Abb. D-17    Dokument Bestellung


                                Bestellungen müssen an den Lieferanten gesendet werden. Dazu steht neben
                                dem Fax- und dem E-Mail-Versand auch die Datenübertragung über Schnitt-
                                stellen zur Verfügung.
3.30 / 04-2020




                 D-46                                                                 A+W Business Einkauf
                 Tutorial                                                                                 Bestellungen




                                          Voreinstellungen für Bestellungen prüfen
                                          Für die Bestellungen müssen Sie die Voreinstellungen in den Firmendaten
                                          prüfen. Im Part Stammdaten ist ausführlich beschrieben, wie Sie die Stamm-
                                          daten zu Ihrer Firma einrichten. In der folgenden Beschreibung wird daher nur
                                          auf die Besonderheiten eingegangen, die Sie für den Einkauf beachten müs-
                                          sen.

                                             A+W Business neu starten
                                             Nach Änderungen der Firmendaten sollten Sie A+W Business neu starten.


                                           So prüfen Sie die Einstellungen für Bestellungen
                                          1 Wählen Sie Stammdaten > Firma > Firmendaten.
                                             Der Dialog Firmendaten wird geöffnet.
                                              Stammdaten, “Firmendaten” auf Seite B-918
                                          2 Wechseln Sie zum Register Dokumente und prüfen Sie die Einstellungen
                                            für den Fax- und E-Mail-Versand.




                 A
                 B                                                                                                  C




                 A Faxversand einzeln oder gesammelt pro           B E-Mailversand einzeln oder gesammelt pro
3.30 / 04-2020




                   Lieferant/Kunde                                   Lieferant/Kunde
                                                                   C Dateiformat, das als E-Mail-Anhang gesendet wird.
                 Abb. D-18   Firmendaten – Dokumente



                 A+W Business Einkauf                                                                             D-47
                 Bestellungen                                                                                       Tutorial




                                          3 Wechseln Sie zum Register Parameter und prüfen Sie die Einstellungen
                                            wie in der folgenden Abbildung gezeigt.




                                                                                                                             D
                                                                                                                             C

                                                                                                                             B


                    A




                   A Änderungen in einer Position in das referenzierte C   Positionen mit Maßen über den Lagermaßen
                     Dokument übernehmen                                   automatisch als Bestellung kennzeichnen
                   B Bestelltexte aus dem Kundenauftrag für den        D   Virtuelle Positionsnummern für den Wareneingang
                     openTRANS-Austausch übernehmen                        von Kisten
                   Abb. D-19    Firmendaten – Parameter


                                              Die Einstellungen werden in separaten Einheiten ausführlich beschrieben.
                                              •   Checkbox A:
                                                   “Bestellte Auftragsposition ändern” auf Seite D-57
                                              •   Checkboxen B und D:
                                                   “Kistengeschäft” auf Seite D-136
                                                   “Export/Import (openTRANS)” auf Seite D-151
                                              •   Lagerbestellungen (C) sind ausführlich im Part Lagerwirtschaft be-
                                                  schrieben.
3.30 / 04-2020




                 D-48                                                                               A+W Business Einkauf
                 Tutorial                                                                                    Bestellungen




                                           4 Wechseln Sie zum Register Lager/EK/EDI und prüfen Sie die Einstellung
                                             im Bereich Einkauf.




                    A
                    B




                    A Bestellkennzeichen bei ISO-Einheiten mit         B Positionen aus Lagerbestellungen anzeigen,
                      Bearbeitungen                                      obwohl sie keine Lagerartikel sind.
                    Abb. D-20    Firmendaten – Lager/EK/EDI


                                           5 Markieren Sie die Checkbox ISO als Bestellartikel (Bearb. können Eigen-
                                             fertigung sein) (A).
                                              Wenn bei Isolierglas (ISO) Bearbeitungen mit der Beschaffungsart Produk-
                                              tion (Eigenfertigung) in der Stückliste vorhanden sind, können diese mit be-
                                              stellt werden. Diese Einstellung ist sinnvoll, wenn Sie ISO-Einheiten nur bei
                                              Engpässen in der Produktion bestellen.
                                           6 Wählen Sie im Menü Start > Speichern, um die Änderungen zu speichern.
                                              Die Daten werden gespeichert.
3.30 / 04-2020




                 A+W Business Einkauf                                                                                 D-49
                 Bestellungen                                                                               Tutorial




                                Bestellpositionen im Auftrag
                                Lernziele

                                •   Bestellposition erfassen und Kennzeichen zuordnen.
                                •   Lieferanten in der Auftragsposition ändern.
                                •   Lieferanten für den gesamten Auftrag ändern.
                                •   Bestellte Position ändern.


                                Nutzen

                                • Aus Auftragspositionen können Bestellungen erzeugt werden, ohne die Positionen
                                  als Bestellung neu zu erfassen.


                                Merke

                                Bestellposition             Bestellpositionen aus Aufträgen erzeugen pro Standard-
                                                            Lieferant eine eigene Bestellung.

                                Bestellkennzeichen          Als Bestellkennzeichen werden folgende
                                                            Beschaffungsarten bezeichnet:
                                                            • Bestellung
                                                            • Bestellung (komplett)

                                Bestellung (komplett)       Dieses Kennzeichen wird bei Produkten mit Stückliste
                                                            verwendet, die als Ganzes bestellt werden sollen, z. B.
                                                            eine komplette Tür mit Beschlägen.

                                Bestellung                  Dieses Kennzeichen wird bei Produkten verwendet,
                                                            deren einzelne Komponenten bestellt werden sollen,
                                                            z. B. nur die Beschläge.

                                Voreinstellungen            Stammdaten:
                                                            • Lieferantendaten (Marktpartner)
                                                            • Lieferantenkartei
                                                            Firmendaten:
                                                            • Register Dokumente
                                                            • Register Parameter
                                                            • Register Lager/EK/EDI
3.30 / 04-2020




                 D-50                                                                     A+W Business Einkauf
                 Tutorial                                                                                   Bestellungen




                                           Kundenbestellung
                                           Im Kundenauftrag können Positionen enthalten sein, die aus unterschiedli-
                                           chen Gründen bestellt werden müssen, z. B., weil das Produkt nicht im Lager
                                           geführt wird oder weil Engpässe in der Produktion den Liefertermin gefährden
                                           und darum die Position komplett bestellt werden muss. Grundsätzlich kann
                                           also jede Position eines Auftrags bestellt werden.
                                           Bestellungen zu Auftragspositionen können aus den Aufträgen heraus er-
                                           zeugt werden. Dazu muss mindestens eine Stücklisten-Komponente oder die
                                           gesamte Position als Bestellung gekennzeichnet sein.
                                           Bestellungen werden nicht automatisch an den Einkauf übergeben. Sind Be-
                                           stellartikel in einem Auftrag enthalten, können Sie sich dies durch eine Mel-
                                           dung anzeigen lassen, wenn Sie die Positionserfassung schließen.




                                 A                                                B
                 A Stücklisten-Komponente soll bestellt werden        B Beschaffungsart der Komponente geändert in
                                                                        Bestellung
                 Abb. D-21    Bestellkennzeichen für Stücklisten-Komponente


                                           Für die Bestellpositionen in einem Auftrag wird ein neues Dokument erzeugt:
                                           eine Bestellung. Dieses Dokument wird durch die Übergabe des Auftrags an
                                           den Einkauf erzeugt. Die Bestellübergabe ist einer separaten Einheit be-
                                           schrieben.
                                            “Bestellübergabe” auf Seite D-60
                                           Sind in einem Auftrag verschiedene Bestellpositionen enthalten, werden so
                                           viele Bestellungen erzeugt, wie unterschiedliche Standard-Lieferanten aus der
                                           Lieferantenkartei ausgelesen wurden.
3.30 / 04-2020




                 A+W Business Einkauf                                                                                D-51
                 Bestellungen                                                                            Tutorial




                                Lieferant für Auftragsposition
                                Achten Sie im Auftrag darauf, dass Sie für Bestellartikel den gewünschten Lie-
                                feranten auswählen. Sie haben dazu verschiedene Möglichkeiten:
                                •   Dokumentenerfassung – Register Konditionen:




                                    Diese Einstellung gilt übergreifend für alle Positionen im aktuellen Auftrag,
                                    sofern sie nicht (anschließend) auf den Ebenen der Position oder der
                                    Stückliste überschrieben werden.
                                •   Positionserfassung – Register Zusatz:




                                    Diese Einstellung gilt nur für die jeweils markierte Position.
                                •   Positionserfassung – Register Stückliste:




                                    Diese Einstellung gilt nur für die jeweils markierte Stücklisten-Komponente.
                                •   Bestellübergabe:
                                    Wenn bei den oben genannten Möglichkeiten keine Angaben gemacht
                                    sind, wird in der Bestellung automatisch der Standard-Lieferant eingesetzt.
                                    Die Einstellungen aus dem Auftrag und/oder den Produktstammdaten kön-
                                    nen im Bestellpool überschrieben werden.
                                    Die Bestellübergabe ist einer separaten Einheit beschrieben.
                                     “Bestellübergabe” auf Seite D-60
3.30 / 04-2020




                 D-52                                                                    A+W Business Einkauf
                 Tutorial                                                                               Bestellungen




                                        Änderung in bestellten Positionen
                                        Auftragspositionen, die bereits bestellt wurden, werden für die weitere Bear-
                                        beitung gesperrt. Sie können nachträglich in der Positionserfassung des Auf-
                                        trags (oder der Bestellung) erst geändert werden, wenn die Sperrung manuell
                                        aufgehoben wird. Änderungen können sich z. B. auf Preise, Mengen oder
                                        Maße beziehen. Der Tarif kann trotz der Sperrung geändert werden.
                                        Die Änderungen müssen in die referenzierten Bestellungen übernommen wer-
                                        den. Wenn Sie Maße oder Stückzahl einer bestellten Position ändern, können
                                        Sie die Änderungen in der ursprünglichen Bestellung eintragen. Die Bestel-
                                        lung muss dann mit einem Hinweis auf die Änderungen erneut an den Liefe-
                                        ranten gesendet werden.
                                        Der geänderte Auftrag muss anschließend wieder über den Bestellpool an den
                                        Einkauf übergeben werden.
3.30 / 04-2020




                 A+W Business Einkauf                                                                          D-53
                 Bestellungen                                                                                   Tutorial




                                            Bestellposition im Auftrag erfassen
                                            In einer Auftragsposition können Komponenten oder ganze Positionen erfasst
                                            sein, aus denen eine Bestellung erzeugt werden muss. Dazu muss die richtige
                                            Beschaffungsart (Bestellkennzeichen) zugewiesen sein.


                                             So erfassen Sie im Auftrag eine Position zur Bestellung
                                            1 Erfassen Sie den Auftragskopf und wechseln Sie zum Register Positionen.
                                            2 Erfassen Sie das Produkt, das Ihr Kunde haben möchte.




                 A


                 B




                 A Beschaffungsart für markierte Position            B Auftragsposition erfasst
                 Abb. D-22    Bestellposition im Auftrag


                                            3 Prüfen Sie die korrekte Einstellung der Beschaffungsart (A).
                                            4 Wählen Sie im Menü Start > Speichern, um die Daten zu speichern.
                                            5 Erfassen Sie eine weitere Position, in der jedoch nur eine Komponente der
                                              Stückliste bestellt werden soll.
                                            6 Wechseln Sie zum Register Stückliste.
3.30 / 04-2020




                 D-54                                                                             A+W Business Einkauf
                 Tutorial                                                                                       Bestellungen




                 A




                 B

                 C




                 A Stücklisten-Komponente, die bestellt werden muss        C Beschaffungsart
                 B Lieferant für die Komponente
                 Abb. D-23    Beschaffungsart für Stücklisten-Komponente


                                           7 Markieren Sie die Komponente (A), die bestellt werden muss.
                                           8 Wählen Sie die Beschaffungsart (C) und den Lieferanten (B) aus.
                                           9 Wählen Sie im Menü Start > Speichern, um die Änderungen zu speichern.
                                              Sie können jetzt weitere Positionen erfassen oder die erfassten Positionen
                                              ändern.
                                              Wenn Sie alle Bestellpositionen bei demselben Lieferanten bestellen wol-
                                              len, wählen im Auftragskopf Sie im Register Konditionen den neuen Liefe-
                                              ranten aus.
                                               “So ändern Sie den Lieferanten aller Bestellpositionen” auf Seite D-56
                                           10 Schließen Sie die Positionserfassung.
                                              Wenn für die Bestellpositionen kein Standard-Lieferant angegeben war,
                                              muss der Lieferant im Dialog Bestellübergabe – Bestellpool angegeben
                                              werden.
3.30 / 04-2020




                                               “So erzeugen Sie eine Bestellung zu einem Kundenauftrag” auf Seite D-68




                 A+W Business Einkauf                                                                                    D-55
                 Bestellungen                                                                                       Tutorial




                                             Lieferanten im Auftrag ändern
                                             Sie können im Auftragskopf einen anderen Lieferanten für die Bestellungen
                                             auswählen. Dieser Lieferant gilt dann für alle Bestellpositionen des Auftrags.

                                                 Bestellkennzeichen im Nummernverwalter ändern
                                                 Wenn Sie in mehreren Aufträgen das Bestellkennzeichen ändern müssen,
                                                 können Sie diese Aufträge in einem neuen Nummernverwalter sammeln.
                                                 In diesem Nummernverwalter können Sie über das Menü Funktionen >
                                                 Kennzeichenänderung die Beschaffungsart und den Lieferanten für alle
                                                 Dokumente gemeinsam ändern.


                                              So ändern Sie den Lieferanten aller Bestellpositionen
                                             1 Öffnen Sie den Auftrag mit den Bestellpositionen.
                                             2 Wechseln Sie zum Register Konditionen.




                                                                                                                         A




                 A Lieferant für alle Bestellpositionen
                 Abb. D-24     Auftragskopf – Register Konditionen


                                             3 Wählen Sie den gewünschten Lieferanten (A) aus.
3.30 / 04-2020




                                             4 Wählen Sie im Menü Start > Speichern, um die Daten zu speichern.




                 D-56                                                                              A+W Business Einkauf
                 Tutorial                                                                                Bestellungen




                                           Die Abfrage wird angezeigt: Soll das Bestellkennzeichen komplett für alle
                                           Positionen gesetzt werden.
                                        5 Wählen Sie:
                                           •   [Ja]: Der gesamte Auftrag wird an den Einkauf zur Bestellung bei dem
                                               gewählten Lieferanten übergeben.
                                           •   [Nein]: Nur die Bestellpositionen werden an den Einkauf übergeben.
                                        6 Schließen Sie den Auftrag.
                                           Sie können jetzt die Bestellungen an den Einkauf übergeben.
                                            “So erzeugen Sie eine Bestellung zu einem Kundenauftrag” auf Seite D-68


                                        Bestellte Auftragsposition ändern
                                        Sie können eine bestellte Position im Auftrag nachträglich ändern und die Be-
                                        stellung neu erzeugen. Vergessen Sie dabei nicht, dem Lieferanten deutlich
                                        zu machen, welche Bestellung neu ist und welche frühere Bestellung durch sie
                                        ersetzt wird.

                                           Bestellte Position ändern
                                           Sie können eine bestellte Position nur so lange ändern, wie keine Auftrags-
                                           bestätigung des Lieferanten oder ein Wareneingang erfasst wurde oder ein
                                           Sperrstatus erreicht ist.
3.30 / 04-2020




                 A+W Business Einkauf                                                                            D-57
                 Bestellungen                                                                                       Tutorial




                                             So ändern Sie eine bestellte Position
                                            1 Öffnen Sie das Dokument, in dem Sie eine bestellte Position ändern möch-
                                              ten, und wechseln Sie zur Positionserfassung.
                                            2 Markieren Sie die Position, die Sie ändern wollen.




                                                                                                                         A




                                                                                                                         B




                 A Produktaufbau gesperrt                                 B Position gesperrt, nur Preis änderbar
                 Abb. D-25   Beschaffungsart für Stücklisten-Komponente


                                               Die Felder (A) der bestellten Positionen sind gesperrt. In der Spalte Hin-
                                               weis (B) wird der entsprechende Text angezeigt.
                                            3 Wählen Sie im Menü Funktionen > Gruppe Position > Gesperrte Position
                                              ändern.
                                               Die Felder werden freigeschaltet.
                                            4 Geben Sie die Änderungen ein, z. B. die Stückzahl.
                                            5 Wählen Sie im Menü Start > Speichern, um die Änderung zu speichern.
                                               Die Änderungen werden gespeichert. Sie können weitere Änderungen ein-
                                               tragen.
3.30 / 04-2020




                                            6 Schließen Sie die Positionserfassung.




                 D-58                                                                               A+W Business Einkauf
                 Tutorial                                                                                   Bestellungen




                                              Der Dialog Bestellübergabe – Bestellpool wird geöffnet und Sie können die
                                              Bestellungen an den Einkauf übergeben.
                                               “So erzeugen Sie eine Bestellung zu einem Kundenauftrag” auf Seite D-68




                 Abb. D-26   Bestellübergabe – Bestellpool

                                               Verkauf, “Bestellübergabe” auf Seite C-654
                                          7 Übergeben Sie die geänderte Bestellung wie unter Bestellung übergeben
                                            beschrieben.
                                               “Dokument in den Bestellpool stellen” auf Seite D-68

                                              Lieferanten informieren
                                              Vergessen Sie nicht, Ihren Lieferanten über die Änderung zu informieren,
                                              wenn Sie die ursprüngliche Bestellung bereits an ihn weitergeleitet hatten.
3.30 / 04-2020




                 A+W Business Einkauf                                                                               D-59
                 Bestellungen                                                                                    Tutorial




                                Bestellübergabe
                                Lernziele

                                •   Auftrag mit Bestellpositionen in den Bestellpool stellen.
                                •   Bestellpositionen im Bestellpool prüfen.
                                •   Lieferant und Liefertermin ändern.
                                •   Bestellpositionen an den Einkauf übergeben.


                                Nutzen

                                • Auftragspositionen können direkt an den Einkauf übergeben werden. Die
                                  Bestellpositionen brauchen nicht im Bestellpool geprüft zu werden.
                                • Im Bestellpool kann ein Preisvergleich geöffnet werden, um den günstigsten (oder
                                  schnellsten) Lieferanten auszuwählen.
                                • Termine, Preise und Lieferanten von Bestellungen können vor der Übergabe
                                  geprüft werden.


                                Merke

                                Bestellübergabe               Durch die Bestellübergabe werden die Bestellungen zu
                                                              Auftragspositionen erzeugt.
                                                              Die Übergabe einer Bestellung muss manuell
                                                              angestoßen werden. Aus dem Bestellpool werden nur
                                                              die Auftragspositionen mit einem Bestellkennzeichen an
                                                              den Einkauf übergeben.

                                Bestellpool                   Der Bestellpool wird manuell gefüllt. Er listet immer alle
                                                              Dokumente auf, die im gewählten Nummernverwalter
                                                              stehen.

                                Bestellungen                  Bestellpositionen aus verschiedenen Aufträgen können
                                                              zu einer Sammelbestellung zusammengefasst werden,
                                                              wenn für diese Positionen der Lieferant und das
                                                              Lieferdatum identisch sind.

                                Lieferant                     Wenn in einem Auftrag mehrere Positionen mit
                                                              Bestellkennzeichen erfasst wurden, wird für jeden
                                                              Lieferanten eine eigene Bestellung erzeugt.

                                Preisvergleich                Vor der Übergabe der Bestellung können Sie die Preise
                                                              der Lieferanten vergleichen, die das Produkt liefern
                                                              können. Dazu muss die Lieferantenkartei gepflegt
                                                              werden.

                                Terminänderung                Wird im Bestellpool das Anlieferdatum beim Kunden
                                                              geändert, wird diese Änderung auch in den
                                                              referenzierten Auftrag übernommen.

                                Bestellung senden             Bestellungen, die über den Bestellpool erzeugt wurden,
                                                              müssen über den Dialog Formular-/ Etikettendruck
                                                              gedruckt und an den Lieferanten gesendet werden.
3.30 / 04-2020




                 D-60                                                                           A+W Business Einkauf
                 Tutorial                                                                            Bestellungen




                                        Merke

                                        Voreinstellungen   Bestellübergabe > Menü Optionen:
                                                           • Auftragsbezogene Übergabe:
                                                             Die Bestellungen werden pro Auftrag übergeben.
                                                             Wenn diese Option nicht aktiviert ist, können
                                                             Sammelbestellungen erzeugt werden.
                                                           • Bestellnummer = Auftragsnummer:
                                                             Diese Option ist nur freigeschaltet, wenn die Option
                                                             Auftragsbezogene Übergabe aktiviert ist. Diese
                                                             Einstellung darf nicht aktiviert sein, wenn
                                                             unterschiedliche Lieferanten in einem Auftrag erfasst
                                                             sind.
                                                           Stammdaten:
                                                           • Nummernkreise
                                                           • Lieferantenkartei
                                                           Firmendaten:
                                                           • Register Produktion (Profit-Center-Abrechnung)
                                                           • Register Lager/EK/EDI (Abstandhalter mitbestellen)
3.30 / 04-2020




                 A+W Business Einkauf                                                                        D-61
                 Bestellungen                                                                                  Tutorial




                                           Bestellpool
                                           Bestellungen aus Kundenaufträgen werden automatisch erzeugt.


                        A    B         C                D         E                F            G    H




                 A Auftragsnummer                   D Produktbezeichnung               G Dokumentennummer nach der
                 B Positionsnummer aus Auftrag      E Bestellung erzeugen                Übergabe
                 C (Standard-)Lieferant             F Anfrage erzeugen                 H Stückliste anzeigen

                 Abb. D-27   Bestellpositionen im Bestellpool


                                           Dazu werden die Auftragspositionen über den Bestellpool an den Einkauf
                                           übergeben. Auftragspositionen ohne Bestellartikel werden nicht weiterverar-
                                           beitet. Anhand des Dokumentenstatus erkennt das Programm, welche Positi-
                                           onen zur Bestellung übergeben werden können.
                                           Die Prüfung der Kundenaufträge im Bestellpool bezieht sich nur auf Produkte
                                           mit der Beschaffungsart Bestellung oder Bestellung (komplett).
3.30 / 04-2020




                 D-62                                                                           A+W Business Einkauf
                 Tutorial                                                                                       Bestellungen




                             Auftrag




                            Bestellpool




                            Prüfung auf
                            Bestellteile



                                              nein                                   nein         untergeordnete
                        Hauptposition                             Stückliste
                                                                 Komponente                        Komponente


                                   ja                                    ja                                ja


                                                         Pro Lieferant eine Bestellung



                 Abb. D-28       Ablauf der Prüfung von Aufträgen im Bestellpool


                                              Die Kundenaufträge werden zunächst auf der Ebene der Hauptposition und
                                              dann auf der Ebene der Stückliste nach Komponenten mit einer der beiden
                                              Beschaffungsarten durchsucht. Die Produkte werden dabei nach einfachen
                                              Bestellteilen und solchen Bestellteilen unterschieden, bei denen alle unterge-
                                              ordneten Produkte mitbestellt werden.
                                              Wenn in einem Kundenauftrag mehrere Positionen erfasst sind, die bei unter-
                                              schiedlichen Lieferanten bestellt werden, wird für jeden Lieferanten eine eige-
                                              ne Bestellung erzeugt.
                                              Wenn in einem Kundenauftrag Lagerartikel in einer Stückzahl angegeben
                                              sind, die den aktuellen Lagerbestand überschreitet, müssen diese Lagerarti-
                                              kel durch eine (manuelle) Lagerbestellung erfasst und bestellt werden.

                                              Prüfungen
                                              Über das Menü Optionen können verschiedene Prüfungen aktiviert werden,
                                              z. B.:
                                              •   Lieferterminprüfung:
                                                  Der Liefertermin wird automatisch geprüft. Ändern Sie einen Liefertermin,
                                                  der nicht an einem Tourentag liegt, wird eine entsprechende Meldung an-
                                                  gezeigt.
                                              •   Lieferantentour berücksichtigen:
                                                  Wenn die Bestellung auf einen Liefertermin fällt, der nicht an einem Tou-
3.30 / 04-2020




                                                  rentag liegt, wird eine entsprechende Meldung angezeigt. Dazu müssen
                                                  die Lieferantentouren in den Stammdaten hinterlegt werden.




                 A+W Business Einkauf                                                                                  D-63
                 Bestellungen                                                                          Tutorial




                                •   Vorlauftage mit Kombiwarengruppe ermitteln:
                                    Wenn in den Kombiwarengruppen Vorlauftage hinterlegt sind, sollen diese
                                    zur Berechnung des Liefertermins herangezogen werden.
                                     Stammdaten, “Vorlauftage” auf Seite B-568
                                •   Produktbezeichnung aus Lieferantenkartei:
                                    Die Bezeichnung der bestellten Produkte wird aus der Lieferantenkartei
                                    übernommen.
                                •   Keine Kostenrückschreibung:
                                    Die Kosten werden nicht in die EK-Preise des Auftrags zurückgeschrieben.
                                •   Maßzuschläge berücksichtigen:
                                    Bei der Bestellung sollen die Maßzuschläge mit übergeben werden.

                                Bestellübergabe
                                Vor der Übergabe der Bestellpositionen können Sie den Modus auswählen.




                                Abb. D-29     Bestellmodus




                                                        NV
                                                      Aufträge


                                             Bestellübergabe
                                             • Sofort anfragen                Anfrage erzeugen

                                             • Sofort bestellen               Bestellung erzeugen

                                             • Pool füllen



                                                     Bestellpool              Termin OK
                                                                              Lieferant OK


                                    Preisvergleich          Terminproblem



                                               Lieferant ändern




                                Abb. D-30     Lieferanten im Bestellpool ändern
3.30 / 04-2020




                                Mit der Option Sofort bestellen, werden die Bestellungen erzeugt, ohne sie in
                                den Bestellpool zu stellen. Im Bestellpool können die Termine und die Liefe-
                                ranten geändert werden.



                 D-64                                                                    A+W Business Einkauf
                 Tutorial                                                                                     Bestellungen




                                            Lieferantenauswahl und Preisvergleich
                                            Bei gefährdeten Terminen können andere Lieferanten ausgewählt werden.
                                            Diese werden aus der Lieferantenkartei ausgelesen. Wenn dort auch Preise
                                            pro Lieferant hinterlegt sind, ist ein Preisvergleich möglich, so dass Sie unab-
                                            hängig von Terminproblemen auch zu dem günstigsten Lieferanten wechseln
                                            können.


                                                             Preisvergleich
                                                             Lieferant ändern


                   NV                                   Bestellpool


                   Aufträge                 Bestell-               Standard-                  Sammel-
                                            Postionen              Lieferant                  Bestellungen
                   •   12301
                                            • 12301 - 2            • 4004               Lieferant 4004   • 12301 - 3
                   •   12302
                                                    -3             • 5001                                • 12304 - 3
                   •   12303
                   •   12304                • 12304 - 1            • 7890
                   •   …                            -3             • 4004               Lieferant 5001   • 12304 - 1
                                                    -5             • 6731                                        -5

                                                                                        Lieferant 2468   • 12301 - 2

                                                             Terminproblem
                                                             Lieferant ändern


                 Abb. D-31     Lieferanten im Bestellpool ändern


                                            Liefertermine
                                            Damit Liefertermine berechnet werden können, muss in der Lieferantenkartei
                                            die Lieferzeit für jeden einzelnen Lieferanten hinterlegt sein. Bei der Übergabe
                                            von Kundenaufträgen wird der Termin der Auslieferung beim Kunden geprüft.
                                            Dazu wird angezeigt, ob der Lieferant aufgrund seiner spezifischen Lieferzeit
                                            in der Lage ist, die Bestellung rechtzeitig zu liefern.
                                            Der Liefertermin des Lieferanten im Bestellpool wird aus dem Versandtag mi-
                                            nus der hinterlegten Vorlauftage zur jeweiligen WGR ermittelt.
                                            Dabei werden die Wochentage und die Tour berücksichtigt. Wenn keine Vor-
                                            lauftage eintragen sind, wird der Versandtag als Liefertermin übernommen.
                                            Im Bestellpool wird farblich hervorgehoben, wenn ein Liefertermin aus dem
                                            Auftrag aufgrund der Liefertage aus der Lieferantenkartei für die Bestellung
                                            nicht eingehalten werden kann.
                                            Der Lieferant und/oder der Liefertermin kann dann schon im Bestellpool geän-
                                            dert werden. Die Änderungen werden in den Auftrag zurückgeschrieben.
3.30 / 04-2020




                 A+W Business Einkauf                                                                                  D-65
                 Bestellungen                                                                        Tutorial




                                Erzeugte Bestellungen
                                Nachdem die Übergabe abgeschlossen ist, zeigt eine Meldung an, wie viele
                                Dokumente nicht übergeben (verarbeitet) wurden.




                                Abb. D-32    Fehlerhafte Dokumente


                                Diese müssen Sie dann einzeln prüfen und ggf. korrigieren. Dies können z. B.
                                folgende Fehler sein:
                                •   Keine Bestellkennzeichen gefunden.
                                •   Auftrag ist noch geöffnet.
                                •   Status lässt die Übergabe nicht zu.
                                Aus den Auftragspositionen mit Bestellkennzeichen wurden Bestellungen er-
                                zeugt, die Sie in der Dokumentenverwaltung für Bestellungen öffnen und prü-
                                fen können. Diese Bestellungen senden Sie auf die übliche Weise an die
                                betreffenden Lieferanten.
                                Für alle übergebenen Positionen wird der Status umgesetzt. In den referen-
                                zierten Aufträgen wird der Status umgesetzt.

                                Bestellnummern
                                Üblicherweise erhalten die automatisch erzeugten Bestellungen Nummern
                                aus dem entsprechenden Nummernkreis. Sie können bei der Übergabe je-
                                doch entscheiden, ob die Auftragsnummer auch als Bestellnummer verwen-
                                det werden soll.
3.30 / 04-2020




                 D-66                                                                A+W Business Einkauf
                 Tutorial                                                                                Bestellungen




                                        Sammelbestellungen pro Lieferant
                                        Bestellungen aus verschiedenen Aufträgen an denselben Lieferanten werden
                                        zu Sammelbestellungen zusammengefasst. Dabei orientiert sich das System
                                        an der Reihenfolge, in der die Einträge im Bestellpool aufgeführt sind. In die-
                                        sem Fall darf jedoch die Auftragsnummer nicht als Bestellnummer übernom-
                                        men werden.
                                        Wenn Sie im Bestellpool alle Positionen für einen Lieferanten markiert haben,
                                        können diese zu einer Sammelbestellung zusammengefasst werden.
                                        Dazu müssen folgende Voraussetzungen erfüllt sein:
                                        •   Identischer Lieferant
                                        •   Identischer Liefertermin
                                        •   Das Kennzeichen für Sammelbestellungen in den Lieferantenstammdaten
                                            muss gesetzt sein (Register Auftrag).
                                        Im Menü Funktionen > Markierungsoptionen legen Sie fest, für welchen Liefe-
                                        ranten die Sammelbestellung erzeugt werden soll.




                                        Abb. D-33    Markierungsoptionen für Sammelbestellung


                                        Mit den Markierungsoptionen werden alle entsprechenden Positionen im Be-
                                        stellpool automatisch markiert. Damit die Sammelbestellung erzeugt werden
                                        kann, muss im Menü Optionen > Gruppe Übergabe > Auftragsbezogene Über-
                                        gabe deaktiviert sein.
3.30 / 04-2020




                 A+W Business Einkauf                                                                            D-67
                 Bestellungen                                                                                 Tutorial




                                         Dokument in den Bestellpool stellen
                                         Für die Übergabe werden die Aufträge in einem Nummernverwalter gesam-
                                         melt. Der Bestellpool greift auf den Nummernverwalter zu, den Sie auswählen.
                                         Mit der Bestellübergabe kann ein neuer Nummernverwalter erstellt werden, in
                                         den die erfolgreichen Bestellungen gestellt werden. Die Bestellungen können
                                         nur erzeugt werden, wenn die Aufträge vor der Übergabe geschlossen sind.


                                          So erzeugen Sie eine Bestellung zu einem Kundenauftrag
                                         1 Wählen Sie Dokumente > Auftrag > Bestellübergabe.


                                                                                              A




                    B




                    C                                                                                                D

                   A Nummernverwalter mit Aufträgen B Modus der Übergabe              D Ziel-Nummernkreis
                     für die Übergabe               C Ziel-Nummernverwalter
                   Abb. D-34    Aufträge aus dem Nummernverwalter übergeben


                                         2 Wählen Sie den Modus (B) aus:
                                            •   Pool füllen:
                                                Mit dieser Option werden die Aufträge im Register Bestellpool ange-
                                                zeigt und können vor der Übergabe geprüft und geändert werden.
3.30 / 04-2020




                                            •   Sofort bestellen:
                                                Mit dieser Option werden die Daten sofort als Bestellung beim Stan-
                                                dard-Lieferanten erzeugt. Diese Option ist dann sinnvoll, wenn Sie zu-
                                                vor keine Preise oder Liefertermine prüfen möchten.


                 D-68                                                                         A+W Business Einkauf
                 Tutorial                                                                                  Bestellungen




                                                  Die Bestellungen können Sie anschließend drucken und auf die ge-
                                                  wohnte Art an den Lieferanten senden, z. B. per E-Mail-Anhang.
                                              •   Sofort anfragen:
                                                  Mit dieser Option werden die Daten als Anfrage beim Standard-Liefe-
                                                  ranten erzeugt.
                                              In diesem Beispiel werden die Aufträge zunächst im Bestellpool geprüft.
                                          3 Wählen Sie den Nummernverwalter (A) aus, in dem die Aufträge mit Be-
                                            stellpositionen stehen.
                                          4 Wählen Sie den Ziel-Nummernverwalter (C) aus, in den die erzeugten Be-
                                            stellungen gestellt werden.
                                              Sie können einen neuen Namen eingeben und so einen neuen Nummern-
                                              verwalter anlegen. Wenn Sie dazu einen anderen Mitarbeiter auswählen,
                                              wird der Nummernverwalter diesem zugeordnet.
                                          5 Wählen Sie ggf. einen anderen Ziel-Nummernkreis (D) aus.
                                          6 Wählen Sie im Menü Start > Ausführen, um die Aufträge in den Bestellpool
                                            zu stellen.




                    Abb. D-35   Auftragspositionen im Bestellpool
3.30 / 04-2020




                                              Der Bestellpool wird gefüllt. Pro Auftrag werden die Bestellpositionen an-
                                              gezeigt.




                 A+W Business Einkauf                                                                              D-69
                 Bestellungen                                                                                  Tutorial




                                          7 Markieren Sie die Positionen, die Sie an den Einkauf übergeben möchten.
                                             Klicken Sie dazu doppelt in den jeweiligen Zeilenkopf.




                   Abb. D-36    Markierte Auftragspositionen übergeben


                                             Nur die Positionen sind markiert, die mit einem X gekennzeichnet sind.
                                          8 Wählen Sie im Menü Start > Ausführen, um die Aktion zu starten.
                                             Die aktivierten Prüfungen werden durchgeführt. Dies kann je nach Anzahl
                                             der Aufträge einige Momente dauern. Bestätigen Sie die jeweiligen Hinwei-
                                             se mit [Ja] oder [Nein], um die Prüfungen fortzusetzen. Wenn alle Prüfun-
                                             gen abgeschlossen sind, werden die zugehörigen Bestellungen angelegt
                                             und sind damit an den Einkauf übergeben.
                                             Die übergebenen Positionen werden aus dem Bestellpool gelöscht.
                                             Der Auftragsstatus wird hochgesetzt. In der Auftragshistorie wird die Num-
                                             mer der Bestellung als Referenz angegeben.
3.30 / 04-2020




                 D-70                                                                          A+W Business Einkauf
                 Tutorial                                                                             Bestellungen




                    Abb. D-37   Bestellnummern nach der Übergabe


                                            Nach der Übergabe der Positionen wird die Bestellnummer zum Auftrag
                                            angezeigt.
                                            Die erzeugten Bestellungen können Sie unter Dokumente > Bestellung öff-
                                            nen und weiterbearbeiten. Drucken Sie die neue Bestellung und senden
                                            Sie sie an den Lieferanten.
3.30 / 04-2020




                 A+W Business Einkauf                                                                        D-71
                 Bestellungen                                                                                    Tutorial




                                          Bestellung im Bestellpool ändern
                                          Wenn zu einer Position Terminschwierigkeiten angezeigt werden, können Sie
                                          im Bestellpool einen anderen Lieferanten auswählen. Den Dialog zur Ände-
                                          rung des Lieferanten können Sie auch ohne Terminschwierigkeiten öffnen, um
                                          einen anderen als den vorgeschlagenen Standard-Lieferanten auszuwählen.


                                           So ändern Sie den Liefertermin und den Lieferanten
                                          1 Wählen Sie Dokumente > Auftrag > Bestellübergabe.
                                          2 Stellen Sie die Aufträge in den Bestellpool.
                                              Dieser Vorgang ist in der vorausgegangenen Einheit beschrieben.
                                               “Dokument in den Bestellpool stellen” auf Seite D-68
                                          3 Markieren Sie die Position, zu der Sie den Liefertermin ändern wollen.
                                              Klicken Sie dazu doppelt in den jeweiligen Zeilenkopf.




                   Abb. D-38    Position für die Änderung des Lieferanten markiert


                                              Nur die Positionen sind markiert, die mit einem X gekennzeichnet sind.
                                          4 Wählen Sie im Menü Funktionen > Lieferant/Liefertermine ändern.
3.30 / 04-2020




                 D-72                                                                              A+W Business Einkauf
                 Tutorial                                                                              Bestellungen




                                           Sie können jetzt folgende Angaben ändern:
                                           •   den Lieferanten
                                           •   den Liefertermin des Lieferanten
                                           •   den Termin der Anlieferung beim Kunden.
                                        5 Klicken Sie auf [OK], um die Änderung zu übernehmen.
                                           Der Dialog Lieferant und Liefertermine ändern wird geschlossen. Im Be-
                                           stellpool wird die Auftragsposition mit dem neuen Termin und/oder Liefe-
                                           ranten angezeigt.
                                        6 Wählen Sie im Menü Start > Ausführen, um die Position an den Einkauf zu
                                          übergeben.
                                           Die aktivierten Prüfungen werden durchgeführt. Dies kann je nach Anzahl
                                           der Aufträge einige Momente dauern. Bestätigen Sie die jeweiligen Hinwei-
                                           se mit [Ja] oder [Nein], um die Prüfungen fortzusetzen. Wenn alle Prüfun-
                                           gen abgeschlossen sind, werden die zugehörigen Bestellungen angelegt
                                           und sind damit an den Einkauf übergeben.
                                           Die geänderten Termine werden in den Auftrag zurückgeschrieben.
                                           Nach der Übergabe der Positionen wird die Bestellnummer zum Auftrag
                                           angezeigt.
                                           Die erzeugte Bestellung können Sie unter Dokumente > Bestellung öffnen
                                           und weiterbearbeiten. Drucken Sie die neue Bestellung und senden Sie sie
                                           an den Lieferanten.
3.30 / 04-2020




                 A+W Business Einkauf                                                                         D-73
                 Bestellungen                                                                                    Tutorial




                                          Preise im Bestellpool vergleichen
                                          Wenn zu einem Produkt mehrere Lieferanten hinterlegt sind, können Sie im
                                          Bestellpool die Preise vergleichen und einen anderen Lieferanten auswählen.


                                           So vergleichen Sie die Preise im Bestellpool
                                          1 Wählen Sie Dokumente > Auftrag > Bestellübergabe.
                                          2 Stellen Sie die Aufträge in den Bestellpool.
                                              Dieser Vorgang ist in der vorausgegangenen Einheit beschrieben.
                                               “Dokument in den Bestellpool stellen” auf Seite D-68
                                          3 Markieren Sie die Position, zu der Sie die EK-Preise vergleichen wollen.
                                              Klicken Sie dazu doppelt in den jeweiligen Zeilenkopf.




                   Abb. D-39    Position für den Preisvergleich markiert


                                              Nur die Positionen sind markiert, die mit einem X gekennzeichnet sind.
                                          4 Wählen Sie im Menü Funktionen > Lieferantenpreise.
3.30 / 04-2020




                 D-74                                                                              A+W Business Einkauf
                 Tutorial                                                                                         Bestellungen




                                                          A

                                    B
                                    C
                                    D

                    A !!! Bei allen Textfarben:                        C Textfarbe grün:
                      Liefertermin gefährdet                             preisgünstigster Lieferant
                    B Textfarbe rot:                                   D Textfarbe blau:
                      Standard-Lieferant                                 Standard-Lieferant ist preisgünstigster Lieferant
                    Abb. D-40     Preisvergleich für Position


                                             5 Markieren Sie die Checkbox links des Lieferanten, an den die Bestellung
                                               der Position gesendet werden soll.
                                             6 Klicken Sie auf [OK], um die Änderung zu übernehmen.
                                                  Der Dialog Preisvergleich wird geschlossen. Im Bestellpool wird die Auf-
                                                  tragsposition mit dem neuen Lieferanten angezeigt.
                                             7 Markieren Sie die Aufträge oder Auftragspositionen, die Sie an den Einkauf
                                               übergeben möchten.
                                                  Klicken Sie dazu doppelt in den jeweiligen Zeilenkopf.
3.30 / 04-2020




                 A+W Business Einkauf                                                                                        D-75
                 Bestellungen                                                                                 Tutorial




                   Abb. D-41    Position mit geändertem Lieferanten


                                             Nur die Positionen sind markiert, die mit einem X gekennzeichnet sind.
                                          8 Wählen Sie im Menü Start > Ausführen, um die Übergabe zu starten.
                                             Die aktivierten Prüfungen werden durchgeführt. Dies kann je nach Anzahl
                                             der Aufträge einige Momente dauern. Bestätigen Sie die jeweiligen Hinwei-
                                             se mit [Ja] oder [Nein], um die Prüfungen fortzusetzen. Wenn alle Prüfun-
                                             gen abgeschlossen sind, werden die zugehörigen Bestellungen angelegt
                                             und sind damit an den Einkauf übergeben.
                                             Übergebene Positionen werden aus dem Bestellpool gelöscht.
3.30 / 04-2020




                 D-76                                                                         A+W Business Einkauf
                 Tutorial                                                                               Bestellungen




                    A




                    B




                    A Erste Bestellnummer                          B Zweite Bestellnummer
                    Abb. D-42   Bestellnummern nach der Übergabe


                                            Nach der Übergabe der Positionen werden die alte und die neue Bestell-
                                            nummer zum Auftrag angezeigt.
                                            Die Bestellungen können Sie unter Dokumente > Bestellung öffnen und
                                            weiterbearbeiten. Drucken Sie die neue Bestellung und senden Sie sie an
                                            den Lieferanten.
                                            Vergessen Sie nicht, den alten Lieferanten über die Änderung zu informie-
                                            ren.
3.30 / 04-2020




                 A+W Business Einkauf                                                                          D-77
                 Bestellungen                                                                                        Tutorial




                                           Auftrags- und Bestell-Info
                                           Zu jedem Auftrag und zu jeder Bestellung können die referenzierten Doku-
                                           mente in einer Übersicht angezeigt werden. Diese Funktion steht in der Be-
                                           stellung (Kopfdaten) über das Menü Funktion > Auftrags-/Bestell-Info zur
                                           Verfügung.




                 Abb. D-43   Auftrags- und Bestellinfo – Übersicht über die referenzierten Dokumente


                                           Dieser Dialog ist im Part Verkauf beschrieben.
                                            Verkauf, “Auftrags-/Bestell-Info” auf Seite C-562
3.30 / 04-2020




                 D-78                                                                                  A+W Business Einkauf
                 Tutorial                                                                                    Bestellungen




                                        Manuelle Bestellung
                                        Lernziele

                                        • Bestellung manuell erfassen.
                                        • Dokumententyp Lagerbestellung kennenlernen.


                                        Nutzen

                                        • Lagerbestellungen werden für die Bestandspflege im Lager erfasst. Sie können
                                          neben den Lagerartikeln auch Artikel enthalten, die nicht als Bestand im Lager
                                          gepflegt werden.


                                        Merke

                                        Manuelle Bestellung        Bestellungen, die nicht durch die Bestellübergabe aus
                                                                   einer Auftragsposition erzeugt werden, müssen manuell
                                                                   erfasst werden.

                                        Unabhängige Bestellung     In unabhängigen Bestellungen können Sie sämtliche
                                                                   Produkte erfassen, die eingekauft werden können.
                                                                   Unabhängige Bestellungen beziehen sich nicht auf einen
                                                                   Auftrag.

                                        Lagerbestellungen          Lagerbestellungen sind ein eigener Dokumententyp. Sie
                                                                   dienen dazu, den Lagerbestand aufzufüllen.

                                        Voreinstellungen           Stammdaten:
                                                                   • Lieferantenkartei
                                                                   Lieferanten
                                                                   • Register Auftrag
                                                                   • Register Finanzen
                                                                   • Register Saldo
                                                                   Firmendaten:
                                                                   • Register Parameter
                                                                   • Register Lager/EK/EDI
3.30 / 04-2020




                 A+W Business Einkauf                                                                                D-79
                 Bestellungen                                                                        Tutorial




                                Unabhängige Bestellungen
                                Alle Bestellungen zu Produkten, die nicht das Bestellkennzeichen Bestellung
                                oder Bestellung (komplett) haben und nicht aus einem Auftrag heraus erzeugt
                                werden, müssen manuell erfasst werden.
                                Als Bestellung können Sie alle Produkte erfassen, die zur Produktion oder
                                zum Verkauf benötigt werden. Dabei wird unterschieden, ob Sie Artikel bestel-
                                len, die als Lagerware verbucht werden können oder solche, die zwar im
                                Lager vorgehalten, jedoch nicht in den Bestandslisten geführt werden. Bestel-
                                lungen von Lagerartikeln und Kisten müssen mit dem Dokumententyp Lager-
                                bestellung erfasst werden, damit der Wareneingang korrekt verbucht werden
                                kann.
                                Wenn Sie für Ihre Lieferanten entsprechende Konditionen hinterlegen, werden
                                in den Bestellungen sofort die aktuellen EK-Preise ausgewiesen. Diese die-
                                nen zur Kontrolle von Preisen in Auftragsbestätigungen (AB) und Rechnungen
                                Ihrer Lieferanten.

                                Lagerbestellungen
                                Lagerbestellungen werden als eigener Dokumententyp erfasst und können als
                                Positionen alle Zukaufartikel, Lagermaße, Kisten und Sondergrößen enthal-
                                ten, die als Lagerartikel geführt werden. Die Wareneingänge von Lagerartikeln
                                aus Lagerbestellungen werden direkt in den Lagerbestand gebucht.
                                Wenn Sie Lagerbestellungen mit Positionen erfassen, die nicht als Lagerarti-
                                kel geführt werden, werden diese im Wareneingang nicht angezeigt. Sie kön-
                                nen in den Firmendaten jedoch die entsprechende Option aktivieren.
                                Die Lagerbestellungen sind ausführlich im Part Lagerwirtschaft beschrieben.

                                Einkaufspreise
                                Der EK wird aus den Preislisten für den Einkauf herangezogen. Bei der Erfas-
                                sung von Bestellpositionen werden die entsprechenden Preise angezeigt und
                                bei Änderungen aktualisiert.
3.30 / 04-2020




                 D-80                                                                A+W Business Einkauf
                 Tutorial                                                                                 Bestellungen




                                           Unabhängige Bestellung erfassen
                                           Sie können in einer unabhängigen Bestellung alle Produkte erfassen, die in
                                           den Stammdaten hinterlegt sind.

                                               Arbeiten mit Nummernverwaltern
                                               Richten Sie sich für die Bestellungen die Nummernverwalter so ein, dass
                                               die Dokumente nach eindeutigen Kriterien zusammengefasst werden,
                                               z. B. nach Lieferanten, nach Datum, nach Lagerbestellungen, nach kom-
                                               plett gelieferten Bestellungen.


                                            So erfassen Sie eine unabhängige Bestellung
                                           1 Wählen Sie Dokumente > Bestellung > Bestellung.
                                               Der Dialog Dokumentenverwaltung wird geöffnet.
                                                Verkauf, “Dokument – Kopfdaten” auf Seite C-417
                                           2 Prüfen Sie im Menü Funktionen > NV Auswahl, ob der richtige Nummern-
                                             verwalter eingestellt ist, und korrigieren Sie ggf. die Einstellung.
                                           3 Erfassen Sie den Dokumentenkopf, indem Sie den Lieferanten auswählen.




                                                                                                                    A




                                                                                                                    B
3.30 / 04-2020




                 A Termin der Anlieferung durch den Lieferanten      B Dokumententyp
                 Abb. D-44    Unabhängige Bestellung erfassen




                 A+W Business Einkauf                                                                            D-81
                 Bestellungen                                                                              Tutorial




                                4 Prüfen Sie den Termin für die Anlieferung (A).
                                   Dies ist der Termin, zu dem Sie die Lieferung bei sich erwarten.
                                5 Wählen Sie im Feld Typ (B) den Eintrag <k.A.>.
                                   Wenn Sie den Typ auf <k.A.> einstellen, wird der Wareneingang nicht auf
                                   das Lager gebucht.
                                   Die Lagerbestellung ist in einer separaten Einheit beschrieben.
                                    “So erfassen Sie eine Lagerbestellung mit Kisten” auf Seite D-83
                                6 Erfassen Sie die Positionen, wie im Kapitel Bestellpositionen im Auftrag be-
                                  schrieben.
                                    “So erfassen Sie im Auftrag eine Position zur Bestellung” auf Seite D-54
                                7 Drucken und versenden Sie die Bestellung.
                                   Die Bestellung steht nun in dem von Ihnen bestimmten Nummernverwalter.
                                   Zu ihr kann später eine Auftragsbestätigung vom Lieferanten und/oder ein
                                   Wareneingang erfasst werden.
                                    “Wareneingang erfassen” auf Seite D-127
3.30 / 04-2020




                 D-82                                                                    A+W Business Einkauf
                 Tutorial                                                                                   Bestellungen




                                        Lagerbestellung erfassen
                                        Sie können in einer Lagerbestellung auch Artikel bestellen, die nicht als Lager-
                                        artikel verbucht werden können. Ein Hinweis macht Sie beim Speichern auf
                                        solche Bestellpositionen aufmerksam. Diese Artikel werden beim Warenein-
                                        gang jedoch nicht automatisch als Lagerbestand verbucht.
                                        In der nachfolgenden Handlungsanleitung wird eine Lagerbestellung für Kis-
                                        ten erfasst. Diese Kistenbestellungen können in der Themenblock Kistenge-
                                        schäft dann weiterbearbeitet werden.


                                         So erfassen Sie eine Lagerbestellung mit Kisten
                                        1 Erfassen Sie das Dokument, wie im Abschnitt Unabhängige Bestellung be-
                                          schrieben.
                                            “So erfassen Sie eine unabhängige Bestellung” auf Seite D-81
                                        2 Wählen Sie im Feld Typ den Eintrag Lagerbestellung.




                                           Wenn Sie den Typ auf <k.A.> einstellen, können Sie den Wareneingang
                                           nicht automatisch auf das Lager buchen.
                                        3 Wechseln Sie zum Register Positionen.
                                        4 Geben Sie die Produktnummer ein, z. B. 1005.
                                           Die Anzahl können Sie nach der Auswahl des Lagerartikels angeben.
                                           Maße brauchen Sie nicht einzutragen, diese werden aus dem Lagerartikel
                                           übernommen.
                                        5 Wählen Sie im Menü Start > Lagersuche, um den Dialog Lagerinfo zu öff-
                                          nen.
                                           Sie können den Dialog auch über die Taste <F3> öffnen.
3.30 / 04-2020




                 A+W Business Einkauf                                                                             D-83
                 Bestellungen                                                                                 Tutorial




                    A




                    B




                   A Produktnummer der Glasart                          B Kiste (ohne ID)
                   Abb. D-45    Lagerinfo – Lagersuche

                                              Verkauf, “Lagerinfo” auf Seite C-741
                                             Der Dialog Lagerinfo wird mit einer Liste aller Lagermaße und Kisten an-
                                             gezeigt. Für Kisten ist in der Spalte Inh. der Wert größer als 1.
                                         6 Suchen Sie die gewünschte Kiste ohne Kisten-ID aus und übernehmen Sie
                                           sie mit einem Doppelklick.
                                             Der Dialog wird geschlossen und die Positionserfassung wird wieder ange-
                                             zeigt. In der Erfassungszeile werden für Kisten alle Felder ab Menge ge-
                                             sperrt. Die Preisfelder werden aktualisiert.
3.30 / 04-2020




                 D-84                                                                         A+W Business Einkauf
                 Tutorial                                                                                   Bestellungen




                                        A              B
                    A Stückzahl                                              B Menge
                    Abb. D-46     Kiste in der Positionserfassung


                                            7 Geben Sie die gewünschte Stückzahl ein.
                                                Die Anzeige der Details wird aktualisiert.
                                            8 Wiederholen Sie die Schritte 4 bis 7, um alle Bestellpositionen zu erfassen.
                                            9 Wählen Sie im Menü Start > Speichern, um die Daten zu speichern.
                                                Die Daten werden gespeichert.
                                            10 Drucken und versenden Sie die Bestellung.
3.30 / 04-2020




                 A+W Business Einkauf                                                                               D-85
                 Bestellungen                                                                               Tutorial




                                Auftragsbestätigung des Lieferanten
                                Lernziele

                                •   Auftragsbestätigung (AB) eines Lieferanten erfassen.
                                •   AB pro Position erfassen.
                                •   Preise in der AB prüfen.
                                •   Ausstehende Auftragsbestätigungen anmahnen.


                                Nutzen

                                • Die Auftragsbestätigung des Lieferanten wird der Bestellung zugeordnet. Dabei
                                  wird der Liefertermin bestätigt oder angepasst, ohne die Bestellung selbst öffnen
                                  zu müssen. Die Terminänderungen werden in die referenzierten Dokumente
                                  übernommen.
                                • Der Status von referenzierten Aufträgen wird automatisch zusammen mit dem
                                  Status der Bestellung umgesetzt.
                                • AB für Bestätigungen Teilmengen können erfasst werden, ohne die Daten neu
                                  einzugeben.
                                • Überfällige Bestellungen können aus einem Nummernverwalter herausgefiltert
                                  werden, um den jeweiligen Lieferanten anzumahnen.


                                Merke

                                Teilweise Bestätigung        Wenn Ihr Lieferant die bestellte Menge in verschiedenen
                                                             Untermengen bestätigt, können Sie die
                                                             Auftragsbestätigung (AB) zu einzelnen Positionen oder
                                                             Teilmengen erfassen.

                                Status                       Der Status der referenzierten Dokumente wird
                                                             hochgesetzt, wenn Sie in einem der Dokumente die
                                                             Auftragsbestätigung des Lieferanten erfassen.

                                Dokumentensperre             Während der Preis- und Rechnungsprüfung sind die
                                                             referenzierten Dokumente für den Zugriff durch andere
                                                             Mitarbeiter gesperrt.

                                Mahnung senden               Die Mahnung wird auf demselben Kommunikationsweg
                                                             an einen Lieferanten gesendet, wie die Bestellung.

                                Voreinstellungen             Lieferantenstammdaten
                                                             • Fax- und E-Mail-Versand
3.30 / 04-2020




                 D-86                                                                      A+W Business Einkauf
                 Tutorial                                                                                Bestellungen




                                        Lieferanten-AB
                                        Ihr Lieferant bestätigt die eingegangene Bestellung durch eine Auftragsbestä-
                                        tigung (AB). Die Nummer dieser Auftragsbestätigung können Sie erfassen
                                        und der entsprechenden Bestellung zuordnen. Gleichzeitig können Sie die
                                        Termine und Preise prüfen und ggf. in Ihren Dokumenten anpassen.
                                        Beim Erfassen einer Auftragsbestätigung haben Sie die Möglichkeit, die Be-
                                        stellung und/oder den zugehörigen Kundenauftrag zur weiteren Bearbeitung
                                        in einen Ziel-Nummernverwalter zu verschieben.

                                        Teillieferungen
                                        Bei größeren Bestellungen kann es vorkommen, dass Ihr Lieferant nicht alle
                                        Positionen oder die gesamte Stückzahl zum gewünschten Termin bestätigt,
                                        sondern in mehreren Teillieferungen ankündigt. Sie können dann auch eine
                                        Teilmenge der Bestellung bestätigen, ohne ein neues Dokument erfassen zu
                                        müssen.

                                        Status
                                        Der Status aller referenzierten Dokumente wird umgesetzt, sobald die AB-
                                        Nummer bestätigt wurde. Die referenzierten Dokumente werden angezeigt,
                                        sobald die Auftrags- oder der Bestellnummer eingegeben wurde. Bei unab-
                                        hängigen Bestellungen bleiben die entsprechenden Felder gesperrt.

                                        Auftragsbestätigung und Liefertermin
                                        Die AB des Lieferanten kann auf unterschiedliche Weise erfasst werden:
                                        •   Auftragsbestätigung mit oder ohne Wareneingang. Dabei können Sie die
                                            Termine für die Lieferung prüfen und ggf. den Kunden über eine Verschie-
                                            bung benachrichtigen.
                                        •   Bestätigung einzelner Positionen einer Bestellung.
                                        •   Auftragsbestätigung und Preiskontrolle. Dabei können Sie die Einkaufs-
                                            preise und den Liefertermin prüfen und korrigieren und ggf. eine Teilliefe-
                                            rung zur bestellten Menge erfassen. Die Beschreibung dieser Variante
                                            finden Sie unter.
                                             “Preis- und Rechnungskontrolle” auf Seite D-143
                                        Aus einem Kundenauftrag können mehrere Bestellungen an unterschiedliche
                                        Lieferanten erzeugt werden. Die verschiedenen AB-Nummern werden für die
                                        entsprechenden Auftragspositionen gespeichert.
3.30 / 04-2020




                 A+W Business Einkauf                                                                            D-87
                 Bestellungen                                                                       Tutorial




                                Überfällige Lieferungen
                                Sie können überfällige Auftragsbestätigungen oder Lieferungen anmahnen.
                                Die Suche nach offenen Bestellungen kann durch ein Datum, auf bestimmte
                                Lieferanten und/oder Nummernverwalter eingeschränkt werden.
                                Für die Mahnung müssen Sie denselben Kommunikationsweg wählen, über
                                den Sie auch die Bestellungen an den jeweiligen Lieferanten übermitteln. Da-
                                bei gilt:
                                •   Faxversand:
                                    Die Bestellungen werden aus A+W Business direkt auf ein Faxgerät ge-
                                    sendet und an den Lieferanten übermittelt.
                                •   Postversand:
                                    Die Bestellungen werden aus A+W Business direkt auf einen Drucker ge-
                                    sendet.
                                Die Mahnung wird immer für alle Bestellungen erstellt, die anhand der Such-
                                kriterien ausgewählt wurde. Dabei werden die Bestellungen pro Lieferant zu
                                einer Mahnung zusammengefasst.
3.30 / 04-2020




                 D-88                                                               A+W Business Einkauf
                 Tutorial                                                                               Bestellungen




                                        Auftragsbestätigung erfassen
                                        Zu einer Bestellung erfassen Sie die Auftragsbestätigung (AB) Ihres Lieferan-
                                        ten und setzen damit den Status der Bestellung hoch.
                                        Zu dieser Lerneinheit gibt es folgende Handlungsanleitungen:
                                        •   “So erfassen Sie die Auftragsbestätigung für eine Bestellung insgesamt”
                                            auf Seite D-89
                                        •   “So erfassen Sie die Auftragsbestätigung für eine Bestellposition” auf
                                            Seite D-91


                                         So erfassen Sie die Auftragsbestätigung für eine Bestellung
                                          insgesamt
                                        1 Wählen Sie Dokumente > Bestellung > AB Lieferant.

                                             A                B




                                            A Modus der Suche                      B Dokumentennummer
                                            Abb. D-47    AB des Lieferanten erfassen


                                             Softwarereferenz, “AB-Lieferant” auf Seite D-197
                                        2 Wählen Sie die Option (A), mit der Sie die Suche nach offenen Bestellun-
                                          gen starten möchten, z. B. Bestellnummer.
                                        3 Tragen Sie die Bestellnummer (B) ein und springen Sie mit <Tab> in das
                                          nächste Feld.
3.30 / 04-2020




                                            Die Daten werden eingelesen und angezeigt.




                 A+W Business Einkauf                                                                          D-89
                 Bestellungen                                                                            Tutorial




                                A

                                B




                                C

                                D




                                A Ziel-Nummernverwalter                    C Anliefertermin aus der AB
                                B Wareneingang komplett buchen             D Nummer der AB
                                    Abb. D-48   AB-Lieferant – Dokumente


                                4 Wählen Sie den Ziel-Nummernverwalter (A) für Aufträge oder für Bestel-
                                  lungen, wenn die entsprechenden Dokumente in andere Nummernverwal-
                                  ter gestellt werden sollen.
                                5 Markieren Sie die Checkbox Wareneingang buchen (B) nur, wenn Sie
                                  gleichzeitig den gesamten Wareneingang dieser Bestellung verbuchen
                                  möchten.
                                    Mit dieser Einstellung können Sie keinen teilweisen Wareneingang erfas-
                                    sen. Der Wareneingang ist in einer separaten Einheit beschrieben.
                                6 Prüfen Sie die Termine (C) in den Bereichen Bestelldaten und Auftragsda-
                                  ten und korrigieren Sie diese ggf.
                                7 Tragen Sie die Nummer der Auftragsbestätigung (D) ein, die der Lieferant
                                  Ihnen geschickt hat.
                                8 Wählen Sie im Menü Start > Ausführen, um die Daten zu speichern.
                                    Die Daten werden gespeichert. Die AB-Nummer wird in der Übersicht an-
                                    gezeigt.
                                    Wenn Sie gleichzeitig einen Wareneingang gebucht haben, wird der Status
                                    der Bestellung entsprechend umgesetzt.
3.30 / 04-2020




                 D-90                                                                   A+W Business Einkauf
                 Tutorial                                                                                   Bestellungen




                                         So erfassen Sie die Auftragsbestätigung für eine Bestellposition
                                        1 Füllen Sie die Felder wie in Schritt 2 bis 6 der vorigen Handlungssequenz
                                          beschrieben.
                                        2 Wechseln Sie zum Register Positionen.




                                        A




                                        B




                                        A Positionsnummern                         B Termin der Teillieferung
                                        Abb. D-49     AB-Lieferant – Positionen


                                        3 Tragen Sie die Nummer(n) der Positionen (A) ein, für die Sie die AB erhal-
                                          ten habe.
                                            Wenn Sie keine lückenlose Folge von Nummern haben, müssen Sie die
                                            Schritte für jede Position einzeln wiederholen, z. B. für Position 1, 3 und 7.
                                        4 Tragen Sie im Feld Teilliefertermin das Datum für die Lieferung der Positi-
                                          onen ein.
                                        5 Wählen Sie im Menü Start > Ausführen, um die Daten zu speichern.
3.30 / 04-2020




                 A+W Business Einkauf                                                                               D-91
                 Bestellungen                                                                       Tutorial




                                                                                A        B
                                A AB-Nummer                                B Bestätigter Termin
                                Abb. D-50   AB-Lieferant – Teillieferung


                                Die Daten werden gespeichert. Die Nummer der AB und der Teilliefer-
                                termin werden in der Übersicht angezeigt.
3.30 / 04-2020




                 D-92                                                                 A+W Business Einkauf
                 Tutorial                                                                                    Bestellungen




                                          AB erfassen und Preise prüfen
                                          Die Preise können sowohl auf Basis der Auftragsbestätigung des Lieferanten
                                          als auch auf Basis der Lieferantenrechnung geprüft werden. Die Dialoge
                                          Preiskontrolle und Rechnungskontrolle sind identisch aufgebaut.
                                          Ihr Lieferant kann in einer AB mehrere Bestellungen bestätigt haben. Diese
                                          können Sie im Dialog Preiskontrolle sammeln und gemeinsam kontrollieren.
                                          Zu dieser Lerneinheit gibt es folgende Handlungsanleitungen:
                                          •   “So erfassen Sie eine Lieferanten-AB und prüfen die Preise” auf Seite D-93
                                          •   “So erfassen Sie eine Sammel-AB Ihres Lieferanten” auf Seite D-95
                                          Die Preis- und Rechnungskontrolle ist ausführlich in einer separaten Einheit
                                          beschrieben.
                                           “Rechnung kontrollieren” auf Seite D-146


                                           So erfassen Sie eine Lieferanten-AB und prüfen die Preise
                                          1 Wählen Sie Dokumente > Bestellungen > Auftragsbestätigung > Preiskon-
                                            trolle.




                    A                                                                                                      D



                    B
                    C




                    A Daten aus der Auftragsbestätigung                C Anzeigemodus für Preise
                    B Bestätigte Summe                                 D Bestellung(en) suchen
                    Abb. D-51   AB-Nummer des Lieferanten erfassen und Preise prüfen


                                               Softwarereferenz, “Rechnungskontrolle – Bestellungen” auf Seite D-248
3.30 / 04-2020




                                          2 Geben Sie die Nummer der Auftragsbestätigung (A) Ihres Lieferanten und
                                            den bestätigten Anliefertermin ein.



                 A+W Business Einkauf                                                                                   D-93
                 Bestellungen                                                                                  Tutorial




                                         3 Geben Sie die Bestellnummer (D) ein und springen Sie mit <Tab> in das
                                           nächste Feld.
                                             In der Übersicht Bestellungen wird die Bestellung angezeigt.
                                             Wenn in der AB mehrere Bestellungen zusammengefasst sind, können Sie
                                             nacheinander alle Bestellnummern angeben. Dies ist in der nachfolgenden
                                             Handlungssequenz beschrieben.
                                         4 Geben Sie im Feld AB-Summe (B) den Betrag ein, den Ihr Lieferant bestä-
                                           tigt hat.
                                             Der Betrag muss identisch mit dem aus der Bestellung angezeigten Betrag
                                             sein. Wenn der Lieferant einen anderen Betrag angegeben hat, den Sie ak-
                                             zeptieren wollen, müssen Sie die Preise in der Bestellung ändern. Sie kön-
                                             nen diese Änderung im Register Positionen erfassen.
                                             Achten Sie darauf, dass der Modus (C) für die Anzeige der Beträge richtig
                                             eingestellt ist.

                                             Währung
                                             Wenn Sie nur mit einer Währung (EUR) arbeiten, muss im Feld Kurs 1 ein-
                                             getragen sein.


                                            A               B




                   A AB-Summe                                        B Betrag aus der Bestellung
                   Abb. D-52    AB-Nummer des Lieferanten erfassen und Preise prüfen
3.30 / 04-2020




                                         5 Wählen Sie im Menü Start > Ausführen, um die Eingabe zu bestätigen.
                                             Der Betrag wird geprüft und das Register Positionen wird angezeigt.



                 D-94                                                                          A+W Business Einkauf
                 Tutorial                                                                                   Bestellungen




                                                              A




                                                                                                                   B


                    A Positionspreis                                  B Differenz über alle Positionen
                    Abb. D-53   Preise der Bestellpositionen prüfen


                                              Wenn Sie einen Positionspreis ändern müssen, überschreiben Sie den Be-
                                              trag in der entsprechenden Position (A). Diese Änderung wird in die Bestel-
                                              lung zurückgeschrieben.
                                          6 Wählen Sie im Menü Start > Ausführen, wenn keine Differenz (mehr) an-
                                            gezeigt wird (B).
                                              Die Daten werden gespeichert und der Status der Bestellung wird umge-
                                              setzt. Anschließend wird das Register Bestellungen wieder angezeigt und
                                              Sie können die nächste AB erfassen. Die Preiskontrolle für diese Bestel-
                                              lung kann nicht nochmals durchgeführt werden.


                                           So erfassen Sie eine Sammel-AB Ihres Lieferanten

                                              Bestellungen sammeln
                                              Sie können die Bestellungen, die in der AB des Lieferanten aufgeführt sind,
                                              in einem Nummernverwalter sammeln und diesen im Bereich Bestelldaten
                                              auswählen.
                                              Alternativ dazu können Sie die Bestellungen im Dialog Preiskontrolle sam-
                                              meln. Dieses Vorgehen ist in den nachfolgenden Handlungsschritten be-
                                              schrieben.
3.30 / 04-2020




                                          1 Geben Sie im Dialog Preiskontrolle die Nummer der Auftragsbestätigung
                                            Ihres Lieferanten und den Anliefertermin ein, wie oben beschrieben.



                 A+W Business Einkauf                                                                              D-95
                 Bestellungen                                                                                   Tutorial




                                             Wenn Sie die Bestellungen in einem Nummernverwalter gesammelt ha-
                                             ben, so wählen Sie diesen aus und fahren mit Schritt 5 fort.
                                         2 Geben Sie die Nummer der ersten Bestellung ein und warten Sie, bis diese
                                           eingelesen wurde.
                                         3 Geben Sie nun die Nummer der nächsten Bestellung ein, die auf der AB
                                           aufgeführt ist.
                                             Die Bestellung wird in der Übersicht der Bestellungen hinzugefügt. Sie kön-
                                             nen jedoch nur Bestellungen mit identischem Steuersatz zusammenfas-
                                             sen.
                                         4 Wiederholen Sie diesen Schritt, bis alle Bestellungen in der Übersicht auf-
                                           geführt sind.
                                             Sie können eine Bestellung aus der Übersicht wieder entfernen, indem Sie
                                             den Eintrag markieren und auf <Entf> drücken.




                   Abb. D-54    AB-Nummer des Lieferanten erfassen und Preise prüfen


                                         5 Geben Sie den Betrag ein, den Ihr Lieferant bestätigt hat.
                                             Der Betrag muss identisch mit der Summe der aufgeführten Bestellungen
                                             sein.
                                         6 Wählen Sie im Menü Start > Ausführen, um die Eingabe zu bestätigen.
                                             Der Betrag wird geprüft und das Register Positionen wird angezeigt. Wenn
                                             Sie einen Positionspreis ändern müssen, überschreiben Sie den Betrag in
3.30 / 04-2020




                                             der entsprechenden Position. Diese Änderung wird in die Bestellung zu-
                                             rückgeschrieben.




                 D-96                                                                           A+W Business Einkauf
                 Tutorial                                                                                Bestellungen




                                        7 Wählen Sie im Menü Start > Ausführen, wenn keine Differenzen (mehr) an-
                                          gezeigt werden.
                                           Die Daten werden gespeichert und der Status der Bestellungen wird um-
                                           gesetzt.


                                        Lieferanten anmahnen
                                        Für die korrekte Verarbeitung Ihrer Bestellungen werden Auftragsbestätigun-
                                        gen und Lieferungen erfasst. Säumige Lieferanten können Sie anmahnen.

                                           Bestellungen sammeln
                                           Sie können die Bestellungen, die in der AB des Lieferanten aufgeführt sind,
                                           in einem Nummernverwalter sammeln.


                                         So mahnen Sie einen Lieferanten an
                                        1 Wählen Sie Dokumente > Bestellungen > Auftragsbestätigung > Mahnung.

                                                         A        B      C         D




                                                                                                                      E

                                                                                                                      F




                                        A Lieferant                             D Lieferanten (nicht) erneut mahnen
                                        B Nummernverwalter mit den überfälligen E Erfassungsdatum der Bestellung
                                          Bestellungen                          F Versandwege der Bestellung
                                        C Eingrenzung der Auswahl auf einen
                                          Statusbereich
                                        Abb. D-55   Lieferanten mahnen
3.30 / 04-2020




                                            Softwarereferenz, “Mahnung” auf Seite D-225




                 A+W Business Einkauf                                                                           D-97
                 Bestellungen                                                                         Tutorial




                                2 Filtern Sie die Anzeige:
                                   •   nach Lieferanten (A)
                                   •   nach einem Nummernverwalter (B)
                                3 Wählen Sie in den Feldern Mindeststatus und Status kleiner (C) einen Sta-
                                  tusbereich für die Bestellungen aus, deren Lieferung Sie anmahnen wol-
                                  len.
                                   Ein Kriterium für den Mindeststatus könnte sein, dass die Bestellung ge-
                                   druckt wurde oder dass die AB erfasst wurde.
                                   Ein Kriterium für den anderen Status sollte vor dem Status Wareneingang
                                   erfasst liegen.
                                4 Grenzen Sie die Auswahl der Bestellungen auf ein Datum (E) ein.
                                   Standardmäßig wird das aktuelle Tagesdatum angezeigt.
                                5 Wenn Sie die bereits gemahnten Lieferanten nicht nochmals mahnen wol-
                                  len, deaktivieren Sie die Checkbox (C) für dieses Kriterium.
                                   Die bereits gemahnten Lieferanten werden dann in der Trefferliste nicht an-
                                   gezeigt. Wenn die Checkbox markiert ist, werden diese Lieferanten in roter
                                   Schrift angezeigt. Die ausstehenden Lieferungen werden dann nochmals
                                   angemahnt.
                                6 Wählen Sie die Option (F) aus, mit der Sie Bestellungen gesendet haben.
                                   Wenn Sie die Bestellungen an Ihre Lieferanten auf unterschiedliche Weise
                                   senden, beachten Sie den Kommunikationsweg für den ausgewählten Lie-
                                   feranten.
                                   Die Option Alle ist dann sinnvoll, wenn Sie die Bestellungen auf unter-
                                   schiedliche Arten an die Lieferanten senden und die Auswahl auf keinen
                                   bestimmten Lieferanten eingeschränkt haben.
                                7 Wählen Sie im Menü Start > Suchen, um in die Suche zu starten.
3.30 / 04-2020




                                   Abb. D-56    Lieferanten zur Mahnung ausgewählt


                 D-98                                                                 A+W Business Einkauf
                 Tutorial                                                                              Bestellungen




                                          Die offenen Bestellungen werden in der Übersicht aufgelistet.
                                        8 Wählen Sie im Menü Drucken die gewünschte Ausgabeform.
                                          Die Mahnung wird erstellt.




                                          Abb. D-57   Mahnungen erstellt


                                          Anschließend werden alle Einträge in der Übersicht in roter Schrift darge-
                                          stellt.
3.30 / 04-2020




                 A+W Business Einkauf                                                                         D-99
                 Bestellungen                                                                             Tutorial




                                Lieferterminkontrolle
                                Lernziele

                                • Liefertermine zu referenzierten Dokumenten prüfen.
                                • Termine ändern.
                                • Kunde über die Änderung benachrichtigen.


                                Nutzen

                                • In referenzierten Dokumenten brauchen Termine nur in einem Dokument geändert
                                  zu werden.
                                • Liefertermine können in verschiedenen Dialogen geändert werden. Bestellungen
                                  oder Aufträge, die in einem eigenen Nummernverwalter gesammelt sind, können
                                  geändert werden, ohne die Dokumente selbst zu öffnen.


                                Merke

                                Terminänderungen in       Alle Änderungen in Bestellungen werden in die
                                referenzierten Dokumenten referenzierten Aufträge zurückgeschrieben. Dies gilt
                                                          auch in der entgegengesetzten Richtung.

                                Dialog                     In diesem Dialog können Sie den Anliefertermin ändern
                                Kundenbenachrichtigung     und den Kunden benachrichtigen.

                                Dialog Dokumentendaten     In diesem Dialog können Sie alle Termine in den
                                                           Aufträgen und referenzierten Bestellungen anpassen.
                                                           Zusätzlich können Sie die Tour in Aufträgen und mehrere
                                                           Dokumente gemeinsam ändern.

                                Voreinstellungen           Kundenstammdaten (Fax- oder Mail-Versand)
3.30 / 04-2020




                 D-100                                                                   A+W Business Einkauf
                 Tutorial                                                                                Bestellungen




                                        Prüfung und Korrektur von Lieferterminen
                                        Ihr Lieferant wird die Termine aus Ihren Bestellungen bestätigen oder korrigie-
                                        ren. Die vom Lieferanten erhaltenen Auftragsbestätigungen und Liefertermine
                                        ordnen Sie den Bestellungen zu, indem Sie die Lieferanten-AB erfassen. Da-
                                        bei werden die geänderten Termine automatisch in die referenzierten Doku-
                                        mente übernommen.
                                        Für die Benachrichtigung des Kunden können Sie den Dialog Kundenbenach-
                                        richtigung oder die Möglichkeiten im Menü Kommunikation nutzen – oder ein-
                                        fach anrufen.
                                        Den Liefertermin selbst können Sie in verschiedenen Dialogen ändern:
                                        •   Dokumentenverwaltung (Auftrag, Bestellung)
                                        •   Dokumentendaten
                                        •   Kundenbenachrichtigung (Lieferterminkontrolle)
                                        •   AB Lieferant
                                        •   Eingangskontrolle
                                        Sie korrigieren die Termine in aller Regel in den Bestellungen, wodurch sie in
                                        die referenzierten Aufträge zurückgeschrieben werden.

                                        Kundenbenachrichtigung
                                        Sie können den Kunden aus dem Dialog Kundenbenachrichtigung (Lieferter-
                                        minkontrolle) heraus über die Terminverschiebung informieren. Dazu muss in
                                        den Stammdaten des Kunden eine E-Mail-Adresse hinterlegt sein. Im Auftrag
                                        muss im Bereich Anschrift die Checkbox Mail aktiviert sein.
3.30 / 04-2020




                 A+W Business Einkauf                                                                           D-101
                 Bestellungen                                                                                      Tutorial




                                         Liefertermine ändern und Kunden benachrichtigen
                                         Zu den Bestellungen und referenzierten Aufträgen müssen Sie Liefertermine
                                         prüfen, korrigieren und den ggf. den Kunden benachrichtigen, wenn die Ter-
                                         mine nicht eingehalten werden können. Diese Schritte sind über den Dialog
                                         Kundenbenachrichtigung möglich.
                                         Sie können ihn auf folgende Weise öffnen:
                                         •   Auftrag oder Bestellung > Funktionen > Gruppe Dokument > Liefertermin-
                                             kontrolle
                                         •   Dokumente > Kundenbenachrichtigung
                                         Wenn Sie auch die Termine für die Produktion prüfen und korrigieren wollen,
                                         können Sie den Dialog Dokumentendaten nutzen.
                                          “So prüfen und ändern Sie die Dokumentendaten” auf Seite D-105


                                          So ändern Sie den Liefertermin
                                         1 Öffnen Sie ggf. den Auftrag, dessen Termine Sie prüfen wollen oder geän-
                                           dert haben.
                                         2 Wählen Sie Dokumente > Kundenbenachrichtigung.




                                                                                                                           B
                    A




                   A Modus der Suche                                  B Geplantes Lieferdatum
                   Abb. D-58    Liefertermin beim Kunden ändern


                                              Verkauf, “Kundenbenachrichtigung (Lieferterminkontrolle)” auf Seite C-565
3.30 / 04-2020




                 D-102                                                                            A+W Business Einkauf
                 Tutorial                                                                                 Bestellungen




                                          3 Wählen Sie die Option (A) Aufträge oder Bestellungen und ggf. den Num-
                                            mernverwalter.
                                              Wenn in dem Nummernverwalter sehr viele Dokumente aufgelistet sind,
                                              können Sie die Anzeige auf das ursprünglich geplante Lieferdatum (B) ein-
                                              schränken.
                                          4 Wählen Sie im Menü Start > Suchen, um die Daten einzulesen.




                    A




                                                                                  B               C
                    A Kunde wurde noch nicht über den neuen Termin   B Geplanter Liefertermin aus dem Auftrag
                      informiert                                     C Neuer Liefertermin
                    Abb. D-59   Liefertermine prüfen


                                          5 Markieren Sie den Auftrag, zu dem Sie den Liefertermin beim Kunden än-
                                            dern müssen, und wechseln Sie zum Register Terminverschiebung.
3.30 / 04-2020




                 A+W Business Einkauf                                                                           D-103
                 Bestellungen                                                                                Tutorial




                    A




                    B




                   A Neuer Termin beim Kunden                        B Auftrag, für den die Änderung gilt
                   Abb. D-60    Liefertermin beim Kunden ändern


                                         6 Markieren Sie den Auftrag (B), zu dem der Kundentermin verschoben wer-
                                           den muss.
                                             Sie können mehrere Aufträge markieren, wenn diese alle denselben Lie-
                                             fertermin und dieselbe Tour haben.
                                         7 Tragen Sie den neuen Termin (A) ein und ändern Sie ggf. die Tour.
                                         8 Wählen Sie im Menü Start > Speichern, um die Änderung zu speichern.
                                             Sie können die Terminänderung für den Kunden drucken und auf dem üb-
                                             lichen Kommunikationsweg versenden.
                                         9 Wählen Sie über das Menü Druck den Drucker aus.
                                             Die Benachrichtigung wird erzeugt und kann versendet werden. Wenn Sie
                                             mehrere Termine geändert haben, wird pro Kunde eine Benachrichtigung
                                             erstellt.
3.30 / 04-2020




                 D-104                                                                         A+W Business Einkauf
                 Tutorial                                                                                    Bestellungen




                                          Alle Termine prüfen und ändern
                                          Im Dialog Dokumentendaten können Sie sich alle Bestellungen und Aufträge
                                          anzeigen lassen, um neben den Lieferterminen auch die Produktionstermine
                                          zu prüfen und ggf. zu ändern. Wenn Sie in mehreren Aufträgen gemeinsam
                                          z. B. die Termine ändern wollen, können Sie die Aufträge sammeln.
                                          Zu dieser Lerneinheit gibt es folgende Handlungsanleitungen:
                                          •   “So prüfen und ändern Sie die Dokumentendaten” auf Seite D-105
                                          •   “So sammeln Sie Dokumente für gemeinsame Änderungen” auf
                                              Seite D-108


                                           So prüfen und ändern Sie die Dokumentendaten
                                          1 Wählen Sie Dokumente > Dokumentendaten.
                                               Verkauf, “Dokumentendaten” auf Seite C-738


                                  A                                   B




                    A Dokumententyp                                       B Nummer des gesuchten Dokuments
                    Abb. D-61   Termine für Auftrag mit Bestellpositionen prüfen
3.30 / 04-2020




                 A+W Business Einkauf                                                                             D-105
                 Bestellungen                                                                                    Tutorial




                                          2 Wählen Sie den Dokumententyp, z. B. Auftrag oder Bestellung.
                                              Sie können sich auch alle Aufträge in einem Nummernverwalter anzeigen
                                              lassen. In diesem Beispiel soll ein einzelner Auftrag geprüft werden.
                                              Sie können die Termine für mehrere Aufträge und/oder Bestellungen än-
                                              dern, die nicht in einem gemeinsamen Nummernverwalter stehen.
                                               “So sammeln Sie Dokumente für gemeinsame Änderungen” auf Seite D-108
                                          3 Geben Sie die Auftragsnummer ein und übernehmen Sie die Daten mit
                                            <Enter>.




                    A




                    B




                   A Kundentermine                                       B Neuer Termin des Lieferanten
                   Abb. D-62    Termine für Auftrag mit Bestellpositionen prüfen


                                              In den Feldern im Bereich Auftrag werden die Daten aus dem Auftragskopf
                                              angezeigt. In den Feldern im Bereich Bestellung werden die Daten aus der
                                              Bestellung angezeigt.
                                          4 Passen Sie den Lieferantentermin (B) und die Kundentermine (A) an.
                                              Wenn Sie die Termine über den Kalender auswählen, können Sie die Tou-
                                              rentage für den Kunden berücksichtigen.
                                          5 Wählen Sie im Menü Start > Speichern, um die Daten zu speichern.
3.30 / 04-2020




                                              Die neuen Termine werden gespeichert und in die zugehörigen Dokumente
                                              übernommen.




                 D-106                                                                             A+W Business Einkauf
                 Tutorial                                                                            Bestellungen




                    Abb. D-63   Geänderte Termine


                                            Sie können jetzt den Kunden über den geänderten Termin informieren.
3.30 / 04-2020




                 A+W Business Einkauf                                                                      D-107
                 Bestellungen                                                                                    Tutorial




                                           So sammeln Sie Dokumente für gemeinsame Änderungen
                                          1 Wählen Sie Dokumente > Dokumentendaten.


                                  A                                   B            C




                   A Dokumententyp                                        C Nummernverwalter nicht markieren
                   B Nummer des gesuchten Dokuments
                   Abb. D-64    Termine für Auftrag mit Bestellpositionen prüfen


                                          2 Wählen Sie den Dokumententyp aus, z. B. Auftrag (A).
                                          3 Stellen Sie sicher, dass die Checkbox (C) Nummernverwalter nicht markiert
                                            ist.
                                          4 Geben Sie die Auftragsnummer (B) ein und übernehmen Sie die Daten mit
                                            <Enter>.
                                              In der Übersicht werden die Daten des Auftrags angezeigt. Im Bereich Be-
                                              stellung werden die referenzierten Bestellungen aufgelistet.
                                          5 Wiederholen Sie diesen Schritt, bis Sie alle Aufträge zusammengestellt ha-
                                            ben, die Sie gemeinsam ändern wollen.
                                              Achten Sie darauf, dass alle Aufträge mit derselben Tour geliefert werden
                                              können und dasselbe Lieferdatum haben.
3.30 / 04-2020




                 D-108                                                                             A+W Business Einkauf
                 Tutorial                                                                                   Bestellungen




                    A




                    B




                    A Termine der Aufträge                              B Termin der Bestellung
                    Abb. D-65   Aufträge für gemeinsame Terminänderung


                                                In der Übersicht werden alle Aufträge aufgelistet.
                                             6 Markieren Sie alle aufgelisteten Aufträge, indem Sie die <Strg>-Taste ge-
                                               drückt halten.
                                             7 Ändern Sie die Termine (A, B).
                                             8 Prüfen Sie die Tour und ändern Sie diese ggf.
                                             9 Wählen Sie im Menü Start > Speichern, um die Daten zu speichern.
                                                Die neuen Termine werden in alle aufgelisteten Aufträge und referenzierten
                                                Bestellungen übernommen. Sie können jetzt die Kunden benachrichtigen.
3.30 / 04-2020




                 A+W Business Einkauf                                                                              D-109
                 Bestellungen                                                                            Tutorial




                                Anfrage
                                Lernziele

                                • Anfragen beim Lieferanten einholen.
                                • Aus einer Anfrage eine Bestellung erzeugen.
                                • Anfragen zu einer Bestellposition einholen.


                                Nutzen

                                • Anfragen können zur Abstimmung von Terminen und Kapazitäten über den
                                  Bestellpool erzeugt werden.
                                • Aus einer Anfrage kann eine Bestellung erzeugt werden, ohne die Daten neu zu
                                  erfassen.


                                Merke

                                Anfragen                  Wie bei den Bestellungen können Anfragen manuell
                                                          erfasst oder über den Bestellpool aus einem
                                                          Kundenauftrag heraus erzeugt werden.

                                Bestellung                Aus jeder Anfrage kann eine Bestellung erzeugt werden.

                                Referenzen                Die Referenz auf eine Auftragsposition bleibt in der
                                                          Anfrage und in der Bestellung erhalten, wenn sie über
                                                          den Bestellpool erzeugt werden.
                                                          Wenn die Bestellung durch Kopieren aus einer Anfrage
                                                          erzeugt wird, besteht die Referenz nur zwischen diesen
                                                          beiden Dokumenten.

                                Voreinstellungen          Stammdaten:
                                                          • Lieferant > Register Auftrag
3.30 / 04-2020




                 D-110                                                                     A+W Business Einkauf
                 Tutorial                                                                                Bestellungen




                                           Anfrage zu Bestellpositionen oder Bestellungen
                                           Anfragen erstellen Sie genau wie eine Bestellung und senden Sie an den Lie-
                                           feranten. Wenn das Angebot zurückkommt und angenommen werden soll,
                                           können Sie aus der Anfrage eine Bestellung erzeugen, ohne die Daten erneut
                                           eingeben zu müssen. Dazu nutzen Sie die Funktion Dokument kopieren.
                                           Anfragen können Sie auch zu den Bestellpositionen aus einem Kundenauftrag
                                           erstellen.



                   Auftrag        Bestellübergabe     Anfrage        Kopieren in   Bestellung   keine Referenz
                   Nr. 1167        Sofort anfragen                                              auf Auftrag 1167




                                     Bestellpool      Anfrage      Referenz auf
                   Auftrag                                         Auftrag 1167
                   Nr. 1167                                                        Bestellung   Referenz auf
                                                                                                Auftrag 1167




                                     Unabhängige Anfrage             Kopieren in       Unabhängige Bestellung




                 Abb. D-66    Anfrage – Bestellung


                                           Wenn bei der Bestellübergabe die Option Sofort Anfragen gewählt wurde,
                                           werden auch aus einem Kundenauftrag Anfragen erzeugt. Wenn Sie dabei
                                           über den Bestellpool gehen, könne Sie auch zu einzelnen Auftragspositionen
                                           eine Anfrage erstellen und einen bestimmten Lieferanten auswählen.
                                           Aus so erstellen Anfragen können natürlich auch Bestellungen erzeugt wer-
                                           den. Die Referenz zum Auftrag bleibt jedoch nur erhalten, wenn entsprechen-
                                           den Bestellungen wieder über den Bestellpool erzeugt werden.
                                           Unabhängige Anfragen werden analog zu Aufträgen und Bestellungen er-
                                           zeugt. Dazu steht im Modul Dokumente das Menü Anfragen zur Verfügung.
3.30 / 04-2020




                 A+W Business Einkauf                                                                              D-111
                 Bestellungen                                                                                   Tutorial




                                         Anfrage zu einer Bestellposition erzeugen
                                         Sie können zu einer Bestellposition zunächst eine Anfrage erzeugen, z. B.,
                                         um festzustellen, ob der Lieferant die Kapazitäten frei hat. Aus jeder Anfrage
                                         kann über den Bestellpool auch eine Bestellung erzeugt werden.
                                         Zu dieser Lerneinheit gibt es folgende Handlungsanleitungen:
                                         •   “So erzeugen Sie eine Anfrage zu einem Kundenauftrag” auf Seite D-112
                                         •   “So erstellen Sie zu einer referenzierten Anfrage eine Bestellung” auf
                                             Seite D-113


                                          So erzeugen Sie eine Anfrage zu einem Kundenauftrag
                                         1 Wählen Sie Dokumente > Auftrag > Bestellübergabe.


                                                          A                                    B




                    C

                   A Modus der Übergabe                              C Ziel-Nummernverwalter
                   B Nummernverwalter mit Aufträgen für die Übergabe
                   Abb. D-67    Aufträge aus dem Nummernverwalter übergeben


                                         2 Wählen Sie die den Modus Sofort anfragen (A) und den Nummernverwal-
                                           ter (B), in dem Sie die Aufträge mit Bestellpositionen gesammelt haben.
3.30 / 04-2020




                 D-112                                                                         A+W Business Einkauf
                 Tutorial                                                                                Bestellungen




                                          3 Wählen Sie den Ziel-Nummernverwalter (C) aus, in den die Anfragen ge-
                                            stellt werden.
                                             Sie können einen neuen Namen eingeben und so einen neuen Nummern-
                                             verwalter anlegen. Wenn Sie dazu einen anderen Mitarbeiter auswählen,
                                             wird der Nummernverwalter diesem zugeordnet.
                                          4 Wählen Sie ggf. im Bereich Ziel-Nummernkreis den Mandanten und den
                                            AV-Bereich aus.
                                          5 Wählen Sie im Menü Start > Ausführen, um die Positionen zu übergeben.
                                             Bestätigen Sie die Erfolgsmeldung.
                                             Für jede Bestellposition wurde eine Anfrage erzeugt. Die erzeugten Anfra-
                                             gen können Sie unter Dokumente > Anfrage öffnen, drucken und an den
                                             Lieferanten senden.


                                           So erstellen Sie zu einer referenzierten Anfrage eine Bestellung
                                          1 Öffnen Sie den Dialog Bestellübergabe.


                            A                                                                   B




                    C

                    A Modus der Übergabe                              C Ziel-Nummernverwalter
                    B Nummernverwalter mit Aufträgen für die Übergabe
3.30 / 04-2020




                    Abb. D-68   Aufträge aus dem Nummernverwalter übergeben




                 A+W Business Einkauf                                                                          D-113
                 Bestellungen                                                                                   Tutorial




                                          2 Wählen Sie den Nummernverwalter (B), in dem die Aufträge stehen, zu de-
                                            nen Sie Anfragen erzeugt haben.
                                          3 Wählen Sie die Option Pool füllen (A).
                                          4 Wählen Sie im Menü Start > Ausführen, um die Aufträge in den Bestellpool
                                            zu stellen.
                                             Die Bestellpositionen werden eingelesen und die Anzeige wechselt zum
                                             Register Bestellpool.


                                                                         A                      B




                    C

                   A Modus Bestellung                                C Ziel-Nummernverwalter
                   B Anfragen, die zum angezeigten Auftrag erzeugt
                     wurden
                   Abb. D-69    Bestellungen zu Aufträgen erzeugen


                                             Zu den Anfragepositionen aus dem Auftrag werden die Dokumenten-
                                             Nummern der Anfragen angezeigt.
                                          5 Markieren Sie die Option Bestellung (A) und wählen Sie den Ziel-Num-
                                            mernverwalter (C) für Bestellungen aus.
                                          6 Markieren Sie die Positionen, für die eine Bestellung erstellt werden soll.
3.30 / 04-2020




                                             Klicken Sie dazu doppelt in den jeweiligen Zeilenkopf. Nur die Positionen
                                             sind markiert, die mit einem X gekennzeichnet sind.




                 D-114                                                                          A+W Business Einkauf
                 Tutorial                                                                                   Bestellungen




                                          7 Wählen Sie im Menü Start > Ausführen, um die Bestellungen zu erzeugen.
                                             Die Bestellungen wurden erzeugt. Die übergebenen Positionen werden
                                             aus dem Bestellpool gelöscht.
                                             Die erzeugten Bestellungen können Sie unter Dokumente > Bestellung öff-
                                             nen, drucken und an den Lieferanten senden.


                                          Bestellung aus unabhängiger Anfrage erstellen
                                          Sie können aus jeder Anfrage durch Kopieren eine Bestellung erzeugen, un-
                                          abhängig davon, ob die Anfrage referenziert ist oder nicht. Die Referenz auf
                                          einen Kundenauftrag wird dabei jedoch nicht übernommen.
                                          Die Kopierfunktion ist ausführlich im Part Verkauf beschrieben.


                                           So erfassen Sie eine Bestellung zu einer Anfrage
                                          1 Öffnen Sie die Anfrage, zu der Sie eine Bestellung erfassen möchten.
                                          2 Wählen Sie im Menü Funktionen > Gruppe Dokument > Dokument kopie-
                                            ren.


                                                             B                                          C




                    A




                    A Ziel-Dokumententyp                               C Ziel-Nummernverwalter
3.30 / 04-2020




                    B Kopier-Modus
                    Abb. D-70   Bestellung aus einer Anfrage erstellen




                 A+W Business Einkauf                                                                            D-115
                 Bestellungen                                                                         Tutorial




                                3 Wählen Sie den Dokumententyp Bestellung (A) aus.
                                   Im Bereich Ziel wird automatisch der erste Nummernverwalter für Bestel-
                                   lungen angezeigt.
                                4 Wählen Sie ggf. einen anderen Ziel-Nummernverwalter (C) aus.
                                5 Prüfen Sie die weiteren Einstellungen.
                                6 Wählen Sie im Menü Start > Ausführen, um die Bestellung zu erzeugen.
                                   Die Positionen werden geprüft und kopiert. Die Bestellung wird gespei-
                                   chert.
                                7 Schließen Sie den Dialog.
                                   Der Dialog Dokumente kopieren wird geschlossen und der Dialog Doku-
                                   mentenverwaltung wird wieder angezeigt.
                                   In der Historie der Anfrage und der Bestellung wird die Referenz angezeigt.
                                   Die erzeugte Bestellung können Sie unter Dokumente > Bestellung öffnen,
                                   drucken und an den Lieferanten senden.
3.30 / 04-2020




                 D-116                                                                A+W Business Einkauf
                 Tutorial                                                                               Bestellungen




                                        Übungen
                                        Die Übungen sind so konzipiert, dass Sie den gesamten Einkauf trainieren.
                                        Das bedeutet, dass Sie die Bestellungen, die Sie mit den Aufgaben erstellen,
                                        im nächsten Themenblock weiterbearbeiten.

                                            Vorbedingungen und Stammdaten prüfen
                                            Wenn Sie in Ihrer eigenen Anwendung arbeiten, stellen Sie bitte sicher,
                                            dass die Voreinstellungen in den Stammdaten den Bedingungen für einen
                                            reibungslosen Ablauf der Erfassung von Dokumenten und Wareneingän-
                                            gen genügen.
                                            Achten Sie auch darauf, dass der Status der Dokumente richtig umgesetzt
                                            ist, wenn sie weiterverarbeitet werden sollen, z. B. im Bestellpool.

                                        Bestellposition im Auftrag erfassen
                                        Erfassen Sie einen Kundenauftrag mit folgenden Positionen:
                                        •   Positionen mit unterschiedlichen Bestellkennzeichen.
                                        •   Positionen, die von unterschiedlichen Lieferanten geliefert werden können.
                                        •   Positionen, die nicht bestellt werden müssen.

                                            Tipp
                                            Stellen Sie 2 bis 3 Kopien der Aufträge und der manuellen Bestellungen
                                            her, damit Sie die unterschiedlichen Auswirkungen von Änderungen prüfen
                                            können, z. B. die Änderung des Lieferanten auf unterschiedlichen Ebenen.

                                        Manuelle Bestellung erfassen
                                        Erfassen Sie eine Bestellung mit folgenden Positionen:
                                        •   Positionen mit Lagerartikeln und Produkten, die nicht im Lager gepflegt
                                            werden.
                                        •   Positionen mit unterschiedlichen Kisten.
                                        •   Mindestens 5 Kisten pro Position.

                                        Auftrag an den Einkauf übergeben
                                        Übergeben Sie Aufträge an den Einkauf:
                                        •   Mindestens einen Auftrag direkt (ohne Bestellpool).
                                        •   Mindestens einen Auftrag über den Bestellpool.
                                        •   Prüfen Sie anschließend die neuen Bestellungen auf Unterschiede.

                                        Auftragsbestätigung erfassen und Preise prüfen
                                        Erfassen Sie eine AB zu mindestens je einer referenzierten und einer manu-
                                        ellen Bestellung.
3.30 / 04-2020




                 A+W Business Einkauf                                                                          D-117
                 Bestellungen                                                                          Tutorial




                                Liefertermine prüfen, ändern und Kunden benachrichtigen
                                Tragen Sie folgende Änderungen ein:
                                •   Tragen Sie in einer referenzierten Bestellung eine größere Stückzahl in ei-
                                    ner Position ein und übergeben Sie Position erneut.
                                •   Wählen Sie einen anderen Lieferanten, weil der ursprüngliche die Termine
                                    nicht einhalten wird.
                                •   Ändern den Liefertermin in einer Bestellung und benachrichtigen Sie an-
                                    schließend den Kunden über die Verzögerung.

                                Lieferanten mahnen
                                Suchen Sie nach Bestellungen, zu denen Sie noch keine AB erfasst haben,
                                und mahnen Sie den Lieferanten.


                                Ergänzende Informationen
                                 “Lieferantenkartei” auf Seite D-31
                                 “Lieferungen im Wareneingang” auf Seite D-119
                                 “Kistengeschäft” auf Seite D-136
                                 “Wareneingang von Kisten” auf Seite D-135
                                 “Elektronischer Dokumentenaustausch” auf Seite D-150

                                Part Verkauf
                                 Verkauf, “Dokumente kopieren” auf Seite C-244
                                 Verkauf, “Dokumente kopieren” auf Seite C-532
                                 Verkauf, “Auftrags-/Bestell-Info” auf Seite C-562
                                 Verkauf, “Dokumentendaten” auf Seite C-737

                                Part Stammdaten
                                 Stammdaten, “Produkt” auf Seite B-139
                                 Stammdaten, “Währungen” auf Seite B-457
                                 Stammdaten, “Lagermaße” auf Seite B-637
                                 Stammdaten, “Preise” auf Seite B-714
                                 Stammdaten, “Partnerverwaltung” auf Seite B-759
                                 Stammdaten, “Firmendaten” auf Seite B-918
                                 Stammdaten, “Pos. ohne Lagerkennz. im WE anzeigen bei Lagerbestell.” auf
                                  Seite B-959

                                Part Lagerwirtschaft
                                 Lagerwirtschaft, “Lagerverwaltung” auf Seite G-68
                                 Lagerwirtschaft, “Lagerbestellung (automatisch)” auf Seite G-107
                                 Lagerwirtschaft, “Lagerverwaltung – Lagerartikel” auf Seite G-186
                                 Lagerwirtschaft, “Lagerbewegung – Abgang, Zugang” auf Seite G-196
3.30 / 04-2020




                 D-118                                                                 A+W Business Einkauf
                 Tutorial                                                            Lieferungen im Wareneingang




                                        Lieferungen im Wareneingang
                                        In diesem Themenblock lernen Sie, wie Sie die Preise und Rechnungen kon-
                                        trollieren und den Wareneingang erfassen.
                                        Dazu gehören folgende Lerneinheiten:
                                        •   “Wareneingang” auf Seite D-120
                                        •   “Wareneingang von Kisten” auf Seite D-135
                                        •   “Preis- und Rechnungskontrolle” auf Seite D-143
                                        Üblicherweise gehören zum Wareneingang folgende Schritte:
                                        •   Lieferung als Wareneingang erfassen.
                                        •   Wareneingang auf ausstehende oder unvollständige Lieferungen prüfen.
                                        •   Rechnung prüfen.
                                        •   Übergabe der Dokumente an Archiv und Statistik.
                                        •   Dokument aus der Hauptdatenbank löschen.
                                        Diese Reihenfolge entspricht im Wesentlichen auch der Reihenfolge der Dia-
                                        loganordnung in A+W Business. Einige der Schritte können jedoch in ver-
                                        schiedenen Dialogen ausgeführt werden. Sie sind daher in einer Lerneinheit
                                        zusammengefasst.
                                        Die Preise auf der Auftragsbestätigung werden logischerweise vor dem Wa-
                                        reneingang geprüft. In diesem Tutorial wird die Preiskontrolle zusammen mit
                                        der Rechnungskontrolle beschrieben, da diese Dialoge gleich aufgebaut sind.
                                        Die Archivierung der Dokumente ist bereits aus dem Part Verkauf bekannt und
                                        wird hier daher nicht mehr behandelt.
3.30 / 04-2020




                 A+W Business Einkauf                                                                       D-119
                 Lieferungen im Wareneingang                                                                     Tutorial




                                       Wareneingang
                                       Lernziele

                                       • Dialog Wareneingang kennenlernen.
                                       • Unterscheidung von Wareneingängen aus Lagerbestellungen und aus
                                         referenzierten Bestellungen kennenlernen.
                                       • Wareneingänge auf Vollständigkeit prüfen.
                                       • Vergessene Eingangsbuchungen nachholen.


                                       Nutzen

                                       • Lieferungen müssen erfasst werden, damit die Kundenaufträge fertiggestellt und
                                         ausgeliefert werden können.
                                       • Beim Erfassen von Wareneingängen aus Lagerbestellungen wird der
                                         Lagerbestand aktualisiert, so dass Sie sich immer über den aktuellen Bestand
                                         informieren können.
                                       • Wareneingänge können trotz Differenzen zwischen den bestellten und den
                                         gelieferten Mengen erfasst werden.


                                       Merke

                                       Unvollständige Lieferung   Der Wareneingang kann teilweise erfasst werden, wenn
                                                                  die gelieferte Menge nicht der bestellten Menge
                                                                  entspricht.

                                       Überzählige Stückzahlen    Wenn die Liefermenge von Lagerartikeln (mit einer
                                                                  Lager-ID) die bestellte Menge einer Lagerbestellung
                                                                  überschreitet, wird diese Menge in den Lagerbestand
                                                                  gebucht.
                                                                  Der Wareneingang von Übermengen wird nur dann
                                                                  verbucht, wenn Sie die Checkbox akzeptieren markiert
                                                                  haben.
                                                                  Übermengen bei Kundenaufträgen müssen in den
                                                                  Stammdaten zugelassen und eingegrenzt werden.

                                       Voreinstellungen           Firmendaten:
                                                                  • Register Parameter
                                                                  • Register Lager/EK/EDI
                                                                  Stammdaten (Übermengen):
                                                                  • Kunde, Lieferant
                                                                  • Produkt
3.30 / 04-2020




                 D-120                                                                          A+W Business Einkauf
                 Tutorial                                                                   Lieferungen im Wareneingang




                                              Lieferungen
                                              Bei der Erfassung von Wareneingängen wird zwischen Kisten, Lagerbestel-
                                              lungen, unabhängigen und referenzierten Bestellungen unterschieden.


                   Wareneingang                                                 Buchung, Status



                   Lagerbestellung                                              Buchung in Bestand

                                                       Vergabe von IDs
                   Kiste                                                        Buchung in Bestand
                                                                                Status in ref. Dokumenten


                   Referenzierte Bestellung                                     Buchung in Bestand nur für Lagerartikel
                                                                                Status in ref. Dokumenten

                   Unabhängige Bestellung                                       Keine Buchung in Bestand



                 Abb. D-71    Wareneingang und Lagerbuchungen


                                              Diese Unterscheidung dient in der Lagerverwaltung zur Pflege der Bestands-
                                              daten.
                                              Nach der Buchung des Wareneingangs werden sämtliche automatischen Zu-
                                              schläge für die Bestellung überrechnet und gespeichert.

                                              Wareneingang von Lagerbestellungen
                                              Mit der Buchung des Wareneingangs von Lagerbestellungen werden die
                                              Stückzahlen im Lager aktualisiert. Im Dialog Lagerinfo werden neben den La-
                                              gerbeständen auch die reservierten Stückzahlen angezeigt. Damit haben Sie
                                              schon in der Positionserfassung einen Überblick über aktuelle und zukünftige
                                              Lagerbestände.
                                              Auch Positionen einer Lagerbestellung mit Artikeln ohne Lagerkennzeichen
                                              werden im Wareneingang angezeigt und können verbucht werden. Diese Bu-
                                              chungen ändern jedoch nicht den Lagerbestand.
3.30 / 04-2020




                 A+W Business Einkauf                                                                                D-121
                 Lieferungen im Wareneingang                                                                         Tutorial




                 A




                 B



                 C




                 D




                 A Liefertermin der markierten Bestellung               C Hinweis auf Sperrstatus
                 B Vollständig gebuchter Wareneingang in blauer Schrift D Referenzierter Auftrag zur markierten Bestellung
                 Abb. D-72    Wareneingang – Bestellungen im Nummernverwalter


                                            Bestellposition für die Produktion
                                            Wenn Sie in einem Kundenauftrag eine Bestellposition erfasst haben, die für
                                            die Produktion des Auftrags benötigt wird, kann dieser erst nach dem Waren-
                                            eingang weiterbearbeitet werden. Wenn Sie den Wareneingang erfassen,
                                            muss daher eine Meldung an die Produktion gesendet werden, damit der Auf-
                                            trag produziert wird.
                                            Im Wareneingang können Sie dazu eine Option aktivieren, mit der die Über-
                                            gabe automatisch angestoßen wird, sobald der Eingang dieser Position er-
                                            fasst wurde.
                                            Für Auftragspositionen mit dem Kennzeichen Bestellung (komplett) wird der
                                            Status umgesetzt und an den Auftrag weitergegeben, damit der Auftrag ggf.
                                            ausgeliefert werden kann.
3.30 / 04-2020




                 D-122                                                                              A+W Business Einkauf
                 Tutorial                                                              Lieferungen im Wareneingang




                                        Positionen ohne Lagerkennzeichen
                                        Wenn Sie Lagerbestellungen mit Positionen erfassen, die nicht als Lagerarti-
                                        kel geführt werden, werden diese im Wareneingang nicht angezeigt. Sie kön-
                                        nen in den Firmendaten jedoch die entsprechende Option aktivieren.




                                        A


                                        A Anzeige im Wareneingang aktivieren
                                        Abb. D-73    Firmendaten – Register Lager/EK/EDI


                                        Teilweiser Wareneingang
                                        Der Wareneingang kann vollständig oder auch teilweise gebucht werden. Der
                                        teilweise Wareneingang kann sowohl einzelne Positionen insgesamt betreffen
                                        als auch Teillieferungen zu einzelnen Positionen, z. B. die Positionen 5 und 7
                                        einer Bestellung oder 15 Stück einer Position mit bestellten 30 Stück. Der Sta-
                                        tus der Bestellung und/oder des Auftrags wird danach entsprechend gesetzt.

                                        Wareneingang von Stücklisten-Komponenten
                                        Stücklisten-Komponenten werden nicht einzeln im Wareneingang aufgeführt,
                                        sondern gehören zu ihrem jeweiligen Hauptprodukt. In der Artikelbezeichnung
                                        werden die Stücklisten-Komponenten mit "/" getrennt aufgeführt.
3.30 / 04-2020




                 A+W Business Einkauf                                                                           D-123
                 Lieferungen im Wareneingang                                                               Tutorial




                                       Lieferung mit Übermengen
                                       Wenn ein Lieferant eine größere Stückzahl (Übermenge) zu einer bestellten
                                       Position liefert, können Sie diese Lieferung im Wareneingang erfassen. Wenn
                                       es sich dabei um Lagerartikel (mit einer Lager-ID) aus einem Dokument vom
                                       Typ Lagerbestellung handelt, werden die gelieferten Stückzahlen in den La-
                                       gerbestand gebucht. In der Bestellung selbst werden die Stückzahlen dabei
                                       entsprechend geändert.
                                       Dies gilt entsprechend auch für Untermengen, die jedoch in der Praxis eher
                                       selten vorkommen.
                                       Die Über- und Untermengen werden in folgenden Dialogen festgelegt:
                                       •   Pro Kunde und pro Produkt: prozentuale Höhe der Abweichung.




                                       •   Pro Produkt: prozentuale Höhe der Abweichung.




                                       •   Pro Auftragsposition: zusätzlich abweichende Menge.
3.30 / 04-2020




                 D-124                                                                     A+W Business Einkauf
                 Tutorial                                                              Lieferungen im Wareneingang




                                        Eingangskontrolle
                                        Einen schnellen Überblick über offene oder unvollständige Lieferungen kön-
                                        nen Sie sich über den Dialog Eingangskontrolle anzeigen lassen.

                                                A                         B       C    D




                                        A Bestellnummer                           C Gelieferte Menge
                                        B Bestellte Menge                         D Wareneingang komplett
                                        Abb. D-74   Kontrolle des Wareneingangs


                                        Sie können die Buchung für Bestellungen oder Bestellpositionen nachholen,
                                        für die der Wareneingang noch nicht erfasst wurde, obwohl die Lieferung ein-
                                        getroffen ist.
3.30 / 04-2020




                 A+W Business Einkauf                                                                        D-125
                 Lieferungen im Wareneingang                                                                   Tutorial




                                           Voreinstellungen für Wareneingang prüfen
                                           In den Firmendaten müssen die Voreinstellungen festgelegt werden, die sich
                                           auf den Wareneingang beziehen. Die entsprechenden Parameter und Optio-
                                           nen finden Sie in folgenden Registern:
                                           •   Parameter
                                           •   Lager/EK/EDI




                                                                                                               A




                 A Virtuelle Positionsnummern für den Wareneingang von Kisten
                 Abb. D-75    Firmendaten – Register Parameter


                                           Die virtuellen Positionsnummern werden erzeugt, damit der Wareneingang
                                           von Kisten korrekt verbucht werden kann. Diese Funktion wird in der Lernein-
                                           heit für den Wareneingang von Kisten beschrieben.
                                            “Wareneingang von Kisten” auf Seite D-135
3.30 / 04-2020




                 D-126                                                                         A+W Business Einkauf
                 Tutorial                                                               Lieferungen im Wareneingang




                                        Lagerbestand
                                        Um den Lagerbestand mit den Eingangsbuchungen aktualisieren zu können,
                                        müssen in den Firmendaten die Reservierungsoption und die Lagerführung
                                        auf Stücklistenebene aktiviert werden.


                                                                                            A
                                        B




                                        A Reservierung mit                     B Lagerführung auf Stücklistenebene
                                          Bestandsaktualisierung
                                        Abb. D-76    Firmendaten – Register Lager/EK/EDI


                                        Wareneingang erfassen
                                        Mit dem Wareneingang können Sie auch die Nummer der Auftragsbestätigung
                                        (AB) des Lieferanten erfassen und den Liefertermin ändern. Teillieferungen er-
                                        fassen Sie, indem Sie die gelieferte Stückzahl einer Position angeben oder nur
                                        einzelne Positionen als vollständig geliefert kennzeichnen.

                                            Erfassung im Wareneingang
                                            In der Regel werden die Dokumentennummern über den Barcode-Scanner
                                            erfasst. Bei den folgenden Beispielen werden sie manuell erfasst. Alle wei-
                                            teren Handlungsschritte sind für die beiden Varianten identisch.

                                        Zu dieser Lerneinheit gibt es folgende Handlungsanleitungen:
                                        •   “So erfassen Sie einen Wareneingang ganz” auf Seite D-128
                                        •   “So erfassen Sie einen Wareneingang teilweise” auf Seite D-130
3.30 / 04-2020




                 A+W Business Einkauf                                                                           D-127
                 Lieferungen im Wareneingang                                                                  Tutorial




                                          So erfassen Sie einen Wareneingang ganz
                                         1 Wählen Sie Dokumente > Bestellung > Wareneingang > Wareneingang.




                 A




                                                        B
                 A Auswahl nach Nummernverwalter                   B Auswahl des Nummernverwalters
                 Abb. D-77   Wareneingang – Auswahl nach Nummernverwalter

                                             Softwarereferenz, “Wareneingang (Dialog)” auf Seite D-227
                                         2 Wählen Sie im Bereich Auswahl die Option nach Nummernverwalter.
                                         3 Wählen Sie im Menü Start > Ausführen, um die Daten einzulesen.
                                            Die Anzeige wechselt zum Register Komplett, in dem die Bestellungen an-
                                            gezeigt werden, die im Nummernverwalter stehen.
3.30 / 04-2020




                 D-128                                                                          A+W Business Einkauf
                 Tutorial                                                                  Lieferungen im Wareneingang




                 A




                 B




                                  C                                                                    D
                 A Anliefertermin und AB der markierten Bestellung   C Checkbox für vollständigen Wareneingang
                 B Hinweis auf Sperrstatus                           D Anzeige für Kisten in der Bestellung
                 Abb. D-78    Wareneingang – Bestellungen


                                               Die Felder im Bereich Liefertermin (A) sind gesperrt, wenn zu der markier-
                                               ten Bestellung eine Auftragsbestätigung des Lieferanten erfasst wurde.
                                           4 Markieren Sie die Bestellung, zu der Sie den Wareneingang erfassen
                                             möchten.
                                               Die Felder im Bereich Liefertermin (A) werden freigeschaltet. In der Regel
                                               sind der Anliefertermin und die AB-Nummer des Lieferanten bereits er-
                                               fasst. Sie können diese Daten jedoch nachtragen, falls sie noch fehlen.
                                           5 Markieren Sie die Checkbox komplett buchen (C).
3.30 / 04-2020




                 Abb. D-79    Wareneingang – Bestellung komplett melden




                 A+W Business Einkauf                                                                             D-129
                 Lieferungen im Wareneingang                                                                     Tutorial




                                         6 Wählen Sie im Menü Start > Ausführen, um den Wareneingang zu erfas-
                                           sen.
                                            Die Daten werden gespeichert und der Status der Bestellung wird umge-
                                            setzt. Bei Lagerartikeln wird der Lagerbestand aktualisiert. Bei referenzier-
                                            ten Bestellungen wird der Wareneingang an die Produktion und/oder den
                                            Verkauf übergeben, um den zugehörigen Kundenauftrag weiterzubearbei-
                                            ten oder abzuschließen.


                                          So erfassen Sie einen Wareneingang teilweise
                                         1 Wählen Sie Dokumente > Bestellung > Wareneingang > Wareneingang.
                                         2 Wählen Sie im Bereich Auswahl die Option nach Bestellnummer (A) und
                                           geben Sie die Bestellnummer (B) ein.


                                                        B




                 A




                 A Auswahl nach Bestellnummer                      B Nummer der Bestellung
                 Abb. D-80   Wareneingang – Auswahl


                                         3 Wählen Sie im Menü Start > Ausführen, um die Daten einzulesen.
                                            Die Daten werden eingelesen und die Anzeige wechselt zum Register
                                            Komplett.
                                            Wenn Sie öfter nur über die Bestell- oder Auftragsnummer gehen, können
                                            Sie im Menü Optionen einstellen, dass die Anzeige nach dem Einlesen des
3.30 / 04-2020




                                            Dokuments zum Register Positionsweise wechselt.
                                         4 Wechsel Sie ggf. zum Register Positionsweise.




                 D-130                                                                          A+W Business Einkauf
                 Tutorial                                                                  Lieferungen im Wareneingang




                                        C                      D   E                                     F




                 B




                 A




                 A Position komplett buchen                            D Bereits gelieferte Menge
                 B Lagerort für Lagerartikel                           E Über- oder Untermengen akzeptieren
                 C Teilmenge als Wareneingang erfassen                 F Nummer der Auftragsbestätigung
                 Abb. D-81   Wareneingang – Teilmenge der Bestellung melden


                                               Alle Positionen der Bestellung werden angezeigt. Sie haben folgende Mög-
                                               lichkeiten, einen teilweisen Wareneingang zu erfassen:
                                               •   Eine der Bestellpositionen komplett buchen (A).
                                               •   Zu einer Position eine Teilmenge (C) der bestellten Stückzahl erfassen.
                                               Wenn die Lieferung z. B. bei einer Lagerbestellung nicht exakt der Bestell-
                                               menge entspricht, können Sie die Über- oder Untermenge akzeptieren (E),
                                               und so den Wareneingang einer Position komplett buchen.
                                            5 Markieren Sie die Position, zu der Sie den Wareneingang erfassen wollen.
                                            6 Tragen Sie im Feld Menge Eingang (C) die Stückzahl der gelieferten Posi-
                                              tion ein oder markieren Sie die Checkbox komplett buchen (A), um die ge-
                                              samte Position als geliefert zu melden.
                                            7 Tragen Sie ggf. AB-Nummer des Lieferanten (F) ein.
                                            8 Wählen Sie bei Lagerartikeln den Lagerort (B) aus.
3.30 / 04-2020




                 A+W Business Einkauf                                                                              D-131
                 Lieferungen im Wareneingang                                                                    Tutorial




                                       C                    D    E                                     F




                 B




                 A




                 A Position komplett buchen                          D Bereits gelieferte Menge
                 B Lagerort für Lagerartikel                         E Über- oder Untermengen akzeptieren
                 C Teilmenge als Wareneingang erfassen               F Nummer der Auftragsbestätigung
                 Abb. D-82   Wareneingang – Teilmenge der Bestellung melden


                                           9 Wählen Sie im Menü Start > Ausführen, um die Daten zu speichern.
                                             Der teilweise Wareneingang wird verbucht.
                                             Die Bestellpositionen werden in blauer Schrift angezeigt, wenn die Bestel-
                                             lung/Position komplett geliefert ist.
                                             Änderungen werden in die Bestellung und ggf. in den referenzierten Kun-
                                             denauftrag übernommen.
                                             Eine Übermenge wird in die Bestellung zurückgeschrieben, ein referen-
                                             zierter Auftrag bleibt davon unberührt. Im Lager wird die Übermenge nur
                                             bei Lagerartikeln aus einer Lagerbestellung automatisch verbucht. Dies gilt
                                             ebenso für Untermengen, jedoch wird dann in der Praxis eher eine Teillie-
                                             ferung erstellt und die fehlende Menge beanstandet.
3.30 / 04-2020




                 D-132                                                                          A+W Business Einkauf
                 Tutorial                                                                 Lieferungen im Wareneingang




                                        Wareneingang kontrollieren
                                        Sie müssen die Vollständigkeit der Lieferungen prüfen, um festzustellen, wel-
                                        che Bestellungen weiterverarbeitet werden können. Wenn Sie wissen, dass
                                        die Lieferung tatsächlich gekommen ist, können Sie den Wareneingang nach-
                                        träglich erfassen. Sie können folgende Sachverhalte prüfen:
                                        •   Komplette Bestellungen pro Nummernverwalter
                                        •   Mengendiskrepanzen pro Bestellposition


                                         So kontrollieren Sie den Wareneingang
                                        1 Wählen Sie Dokumente > Bestellung > Wareneingang > Eingangskontrol-
                                          le.




                                            Abb. D-83    Eingangskontrolle – Komplette Bestellung


                                             Softwarereferenz, “Eingangskontrolle” auf Seite D-241
                                        2 Wählen Sie im Register Komplette Bestellungen den Nummernverwalter
                                          für die Bestellungen aus.
                                            In der Übersicht Wareneingang komplett werden alle Bestellungen aufge-
                                            listet, deren Bestellungen vollständig erfasst sind.
                                        3 Wechseln Sie zum Register Mengendiskrepanzen, um sich die unvollstän-
                                          digen Positionen anzeigen zu lassen.
3.30 / 04-2020




                 A+W Business Einkauf                                                                         D-133
                 Lieferungen im Wareneingang                                                                  Tutorial




                                                                                        A B
                                          A Teilgelieferte Menge                B Wareneingang komplett buchen
                                          Abb. D-84    Eingangskontrolle – Mengendiskrepanzen


                                          In der Übersicht werden alle Bestellungen aufgelistet, zu denen noch kein
                                          oder ein unvollständiger Wareneingang gebucht wurde.
                                          Wenn Sie die Bestellungen beim Buchen des kompletten Wareneingangs
                                          in einen Ziel-Nummernverwalter geschoben haben, sollten hier keine Dis-
                                          krepanzen angezeigt werden.
                                       4 Holen Sie ggf. versäumte Buchungen nach, indem Sie die Checkbox
                                         OK (B) markieren.
                                          Beachten Sie dabei, dass Sie nur komplette Wareneingänge nachholen
                                          können. Um Teilmengen zu erfassen, wechseln Sie zum Dialog Warenein-
                                          gang.
                                       5 Wählen Sie im Menü Start > Ausführen, um den Wareneingang zu buchen.
                                          Der Wareneingang wird verbucht. Die vollständig verbuchten Bestellungen
                                          werden aus der Liste entfernt.


                                       Ergänzende Informationen
                                        Stammdaten, “Pos. ohne Lagerkennz. im WE anzeigen bei Lagerbestell.” auf
                                         Seite B-959
                                        Stammdaten, “Lagerführungsmodus” auf Seite B-960
                                        Verkauf, “Lagerinfo” auf Seite C-741
                                        Softwarereferenz, “Wareneingang” auf Seite D-227
3.30 / 04-2020




                 D-134                                                                        A+W Business Einkauf
                 Tutorial                                                                  Lieferungen im Wareneingang




                                        Wareneingang von Kisten
                                        Lernziele

                                        • Sinn der Dummy-Kiste kennenlernen.
                                        • Vergabe von Identnummern (IDs) kennenlernen.
                                        • Einstellungen für automatische Vergabe der Kisten-ID kennenlernen.


                                        Nutzen

                                        • Jede Kiste erhält im Wareneingang eine ID, damit sie im Lagerbestand eindeutig
                                          identifiziert und für einen Auftrag reserviert werden kann.
                                        • Die IDs können manuell oder automatisch vergeben werden. Sie können dabei
                                          auch die Kisten-ID des Lieferanten übernehmen.


                                        Merke

                                        Virtuelle Positionsnummern Wenn die Stückzahl einer Kistenposition größer als 1 ist,
                                                                   wird für jede Kiste eine Unterposition erzeugt. Diese
                                                                   Unterpositionen erhalten virtuelle Positionsnummern, die
                                                                   sich aus der Positionsnummer und der Anzahl der Kisten
                                                                   zusammensetzt, z B. 1.1, 1.2 oder 3.1, 3.2 usw.

                                        ID                          Bei der Erfassung des Wareneingangs wird für die Kiste
                                                                    jeder Unterposition eine eigene Identnummer (ID)
                                                                    vergeben.

                                        Kisten identifizieren       Nur eine Kiste mit einer ID kann als Lagerbestand
                                                                    gebucht und/oder einer Auftragsposition zugeordnet
                                                                    werden.

                                        Voreinstellungen            Stammdaten:
                                                                    • Produktverwaltung
                                                                    Firmendaten:
                                                                    • Register Parameter
                                                                    • Register Lager/EK/EDI
3.30 / 04-2020




                 A+W Business Einkauf                                                                                D-135
                 Lieferungen im Wareneingang                                                                  Tutorial




                                       Kistengeschäft
                                       Für Kisten werden in der Regel Identnummern (ID) vergeben, die entweder
                                       vom Lieferanten stammen können oder im eigenen System gepflegt werden.
                                       Diese IDs werden beim Wareneingang von Kisten erfasst. Jede Kiste wird mit
                                       einer eigenen Kisten-ID verbucht und im Lager geführt.
                                       Auch wenn die Anzahl von Kisten in einer Bestellposition größer als 1 ist, wird
                                       jede Kiste als ein eigener Wareneingang verbucht. Dazu legt das System au-
                                       tomatisch Unterpositionen (virtuelle Positionen) zu der ursprünglichen Positi-
                                       on an und ordnet jeder dieser Positionen genau eine Kiste zu. Diese Funktion
                                       muss in den Firmendaten aktiviert werden.
                                       Zu jeder Unterposition muss eine eigene Kisten-ID angegeben werden, damit
                                       der Lagerbestand der Kisten gepflegt werden kann. Diese Kisten-IDs können
                                       nach selbst definierten Vorgaben automatisch eingefügt werden. Eine ID kann
                                       jedoch auch manuell eingegeben werden, z. B. um die Kisten-ID aus dem Lie-
                                       ferschein des Lieferanten zu übernehmen.
                                       Im Rahmen des Wareneingangs kann im Dialog zur automatischen Kisten-ID
                                       auch ein Produktionsdatum angegeben werden. Für beschichtetes Glas wird
                                       dieses zur Berechnung des Verfallsdatums herangezogen, damit nach dem
                                       FiFo-Prinzip gearbeitet werden kann (FiFo = First in - First out).
                                       Nach der Vergabe der IDs können über die Druckfunktion die Kistenetiketten
                                       mit den IDs als Barcode gedruckt und an den entsprechenden Kisten ange-
                                       bracht werden.
                                       In der Regel werden die Barcodes von Kisten beim Warenausgang oder bei
                                       der Auflösung von Kisten gescannt. Damit ist der Bestand von Kisten nicht nur
                                       mengenmäßig aktuell, sondern die Kisten sind eindeutig identifiziert.


                                       Firmendaten prüfen
                                       Im Part Stammdaten ist ausführlich beschrieben, wie Sie die Stammdaten zu
                                       Ihrer Firma einrichten. In der folgenden Beschreibung wird daher nur auf die
                                       Besonderheiten eingegangen, die Sie für den Wareneingang von Kisten be-
                                       achten müssen.

                                          A+W Business neu starten
                                          Nach Änderungen der Firmendaten sollten Sie A+W Business neu starten.


                                        So prüfen Sie die Firmendaten
                                       1 Wählen Sie Stammdaten > Firma > Firmendaten und prüfen Sie im Regis-
                                         ter Parameter die Einstellung für die Checkbox Virtuelle Positionsnummern
                                         verwenden.
                                          Diese Einstellung ist bereits in der Lerneinheit Wareneingang dargestellt.
                                           “Firmendaten – Register Parameter” auf Seite D-126
                                       2 Wählen Sie im Menü Start > Speichern, um Änderungen zu speichern.
3.30 / 04-2020




                                          Die Daten werden gespeichert.




                 D-136                                                                       A+W Business Einkauf
                 Tutorial                                                                Lieferungen im Wareneingang




                                        Einstellungen für Identnummern prüfen
                                        Wenn Sie die Kisten mit einer eigenen Kisten-ID erfassen wollen, können Sie
                                        diese ID automatisch vergeben lassen. Dazu müssen Sie die Einstellungen
                                        festlegen. Diese Einstellungen können vor jedem Wareneingang für Kisten an-
                                        gepasst werden, z.B. um die ID um ein Kennzeichen für den Lieferanten zu
                                        ergänzen.
                                        Sie können maximal 20 Zeichen verwenden, die automatisch durch eine 5-stel-
                                        lige Zahl ergänzt werden. Die eingegebene Zeichenfolge bleibt so lange be-
                                        stehen, bis sie manuell geändert wird. Wenn Sie also die Kisten-ID mit einem
                                        Kennzeichen für den Lieferanten versehen, müssen Sie darauf achten, die ID
                                        zu ändern, wenn Sie den Wareneingang von Kisten eines anderen Lieferanten
                                        erfassen.


                                         So prüfen Sie die Einstellungen für die automatische Vergabe von
                                          Identnummern
                                        1 Wählen Sie Dokumente > Bestellung > Wareneingang > Wareneingang.
                                           Der Dialog Wareneingang wird geöffnet.
                                        2 Wählen Sie im Menü Optionen > Gruppe Identnummernvergabe > Einstel-
                                          lungen.




                                            Softwarereferenz, “Einstellungen (ID)” auf Seite D-240
                                        3 Tragen Sie das Kennzeichen ein.
                                           Achten Sie darauf, dass Sie die Platzhalter (X) für die Ziffern nicht über-
                                           schreiben.
                                        4 Klicken Sie auf [OK], um die Änderung zu speichern.
                                           Der Dialog wird geschlossen. Die Einstellungen werden gespeichert und
                                           bleiben erhalten, bis sie erneut manuell geändert werden.
                                        5 Wählen Sie im Menü Optionen > Gruppe Identnummernvergabe > Auto-
                                          matische Vergabe.
                                           Damit ist die automatische Vergabe der ID für Kisten eingerichtet.
3.30 / 04-2020




                 A+W Business Einkauf                                                                            D-137
                 Lieferungen im Wareneingang                                                                    Tutorial




                                         Wareneingang von Kisten erfassen
                                         Bei der Erfassung des Wareneingangs von Kisten, wird pro Kiste eine Kisten-
                                         ID vergeben. Anschließend werden die zugehörigen Etiketten gedruckt.
                                         Zu dieser Lerneinheit gibt es folgende Handlungsanleitungen:
                                         •   “So erfassen Sie den Wareneingang einer Kiste mit einer automatischen
                                             ID” auf Seite D-138
                                         •   “So vergeben Sie Kisten-IDs manuell” auf Seite D-141
                                         •   “So drucken Sie Kistenetiketten” auf Seite D-142


                                          So erfassen Sie den Wareneingang einer Kiste mit einer
                                           automatischen ID
                                         1 Wählen Sie Dokumente > Bestellung > Wareneingang > Wareneingang.


                                                         B




                 A




                 A Suchoption                                       B Bestellnummer
                 Abb. D-85   Wareneingang für Kisten – nach Nummernverwalter


                                              Softwarereferenz, “Wareneingang (Dialog)” auf Seite D-227
                                             Stellen Sie sicher, dass die automatische Vergabe für Kisten-IDs aktiviert
                                             ist.
                                         2 Wählen Sie die Option (A), mit der Sie die Suche nach offenen Bestellun-
3.30 / 04-2020




                                           gen starten möchten, z. B. nach Bestellnummer.
                                         3 Geben Sie die Bestellnummer (B) ein.
                                         4 Wählen Sie im Menü Start > Ausführen, um die Daten einzulesen.


                 D-138                                                                           A+W Business Einkauf
                 Tutorial                                                                    Lieferungen im Wareneingang




                                              Die Anzeige wechselt zum Register Komplett. Sie können die Daten noch-
                                              mals prüfen.
                                           5 Wechseln Sie zum Register Identnummern.


                 A



                 B

                 C




                 D




                 A Ausgewählte Bestellung                             C Lagerort
                 B Eingabe der Kisten-ID des Lieferanten              D Pro Kiste eine Zeile (Unterposition)
                 Abb. D-86    Wareneingang für Kisten – Eingang erfassen


                                              Wenn die Stückzahl der bestellten Position größer als 1 ist, wird in der
                                              Übersicht Kistenpositionen für jede Kiste eine Zeile angezeigt.
                                              Sie können mehrere Kisten auf einmal auswählen, um diese in einem
                                              Schritt zu buchen.
                                           6 Markieren Sie eine Zeile, in der noch keine virtuelle Positionsnummer an-
                                             gezeigt ist.
                                           7 Geben Sie im Feld Lieferanten-Identnummer (B) die Kisten-ID des Liefe-
                                             ranten ein oder scannen Sie die Kisten-ID und springen Sie mit <Tab> in
                                             das nächste Feld.
                                              Wenn mehr als eine Kiste ausgewählt ist und die Lieferanten-Identnummer
                                              eingegeben ist, berechnet das System die Kisten-Identnummern für alle
                                              markierte Einträge.
3.30 / 04-2020




                                           8 Wählen Sie den Lagerort aus und prüfen und korrigieren ggf. den Inhalt
                                             und den Preis.




                 A+W Business Einkauf                                                                             D-139
                 Lieferungen im Wareneingang                                                                      Tutorial




                 A




                 B




                 A Kisten-ID des Lieferanten                             B Wareneingang für diese Kiste buchen
                 Abb. D-87    Wareneingang für Kisten – Daten für markierte Zeile


                                               Die Eingaben werden in die markierte Zeile übernommen.
                                            9 Wählen Sie im Menü Start > Ausführen, um die Eingaben zu bestätigen
                                              und den Wareneingang zu buchen.




                 A

                                                                               B
                 A Virtuelle Positionsnummer (verbuchte Unterposition)         B (Automatische) Kisten-ID
                 Abb. D-88    Wareneingang für Kisten – neue virtuelle Positionsnummer erzeugt


                                               Die Kiste wird verbucht und mit der nächsten virtuellen Positionsunternum-
                                               mer an das Ende der Liste Kistenpositionen verschoben.
                                            10 Wiederholen Sie die Schritte 7 bis 9, bis Sie den gesamten Wareneingang
                                               erfasst haben.
3.30 / 04-2020




                                               Wenn Sie alle Kisten erfasst haben, können Sie den Druck der Kisten-
                                               etiketten und des Protokolls starten.
                                                “So drucken Sie Kistenetiketten” auf Seite D-142


                 D-140                                                                              A+W Business Einkauf
                 Tutorial                                                                    Lieferungen im Wareneingang




                                            So vergeben Sie Kisten-IDs manuell
                                           1 Wählen Sie Dokumente > Bestellung > Wareneingang > Wareneingang.
                                           2 Deaktivieren Sie im Menü Optionen > Gruppe Identnummernvergabe > Au-
                                             tomatische Vergabe.
                                           3 Bereiten Sie die Erfassung des Wareneingangs vor, wie in den Schritten 2
                                             bis 7 der vorhergehenden Handlungssequenz gezeigt.


                 A



                 B
                 C




                 D




                 A Ausgewählte Bestellung                             C Manuelle Kisten-ID
                 B Kisten-ID des Lieferanten                          D Pro Kiste eine Zeile (Unterposition)
                 Abb. D-89    Wareneingang für Kisten – Eingang erfassen


                                               Wenn die Stückzahl der bestellten Position größer als 1 ist, wird in der
                                               Übersicht Kistenpositionen für jede Kiste eine Zeile angezeigt.
                                           4 Geben Sie die Kisten-ID (C) ein, mit der die Kiste in Ihrem Lager verbucht
                                             werden soll.
                                               Sie können die ID des Lieferanten übernehmen, indem Sie den Cursor in
                                               das Feld stellen und Lieferanten-ID erneut scannen.
                                           5 Wählen Sie den Lagerort aus und prüfen und korrigieren ggf. den Inhalt
                                             und den Preis.
3.30 / 04-2020




                                               Diese Eingaben gelten nur für die Kistenposition, die in der Übersicht mar-
                                               kiert ist.




                 A+W Business Einkauf                                                                              D-141
                 Lieferungen im Wareneingang                                                                  Tutorial




                                       6 Wählen Sie im Menü Start > Ausführen, um die Eingaben zu bestätigen.
                                          Die Kiste wird verbucht und mit der nächsten virtuellen Positionsunternum-
                                          mer an das Ende der Liste Kistenpositionen verschoben.
                                       7 Wiederholen Sie die Schritte 4 bis 6, bis Sie den gesamten Wareneingang
                                         erfasst haben.
                                          Wenn Sie alle Kisten erfasst haben, können Sie den Druck der Kisteneti-
                                          ketten starten, um die Etiketten mit den manuell vergebenen IDs zu dru-
                                          cken.


                                        So drucken Sie Kistenetiketten
                                       1 Nachdem Sie die Kisten einer Lieferung erfasst haben, wählen Sie im
                                         Menü Druck > Gruppe Drucker > Etiketten.
                                          Wenn Sie den Eintrag Etiketten und Protokoll wählen, wird zusätzlich das
                                          Protokoll gedruckt, das Sie sich auch im Register Protokoll (Identnum-
                                          mern) anzeigen lassen können.




                                                                                        A

                                                                                        B




                                          A Anzahl                               B Drucker
                                          Abb. D-90    Kistenetiketten drucken


                                       2 Wählen Sie den Drucker (B) und die Anzahl (A) der erforderlichen Kopien.
                                       3 Klicken Sie auf [OK], um den Druck zu starten.
                                          Der Dialog wird geschlossen und die Etiketten werden gedruckt. Im Proto-
                                          koll werden alle verbuchten Kisten mit den Kisten-IDs aufgeführt.


                                       Ergänzende Informationen
                                        Stammdaten, “Virtuelle Positionsnummern verwenden” auf Seite B-943
                                        Softwarereferenz, “Einstellungen (ID)” auf Seite D-240
3.30 / 04-2020




                 D-142                                                                       A+W Business Einkauf
                 Tutorial                                                                Lieferungen im Wareneingang




                                        Preis- und Rechnungskontrolle
                                        Lernziele

                                        • Auftragsbestätigung des Lieferanten erfassen.
                                        • Preise prüfen.
                                        • Gesammelte Auftragsbestätigung zu mehreren Bestellungen erfassen.


                                        Nutzen

                                        • Zusammen mit der Auftragsbestätigung können die Preise geprüft werden.
                                        • Preise mehrerer Bestellungen können in einer gemeinsamen Auftragsbestätigung
                                          geprüft werden.


                                        Merke

                                        Status                    Nach der Preis- und nach der Rechnungskontrolle wird
                                                                  der Status der Dokumente hochgesetzt. In Verbindung
                                                                  mit einem Sperrstatus ist eine erneute Preis- und/oder
                                                                  Rechnungskontrolle daher nicht möglich.

                                        Differenzen               Sie können die Preis- oder Rechnungskontrolle nur dann
                                                                  abschließen, wenn keine Differenz zwischen dem
                                                                  eingegebenen Gesamtbetrag und der Summe der
                                                                  angezeigten Bestellungen besteht.

                                        Schnellerfassung          Wenn Sie im Menü Optionen > Schnellerfassung
                                                                  aktivieren, springt der Cursor nach der Eingabe der
                                                                  Bestellnummer direkt in das Feld Rechnungssumme
                                                                  bzw. AB-Summe. Sie können diese Option dann nutzen,
                                                                  wenn Sie in der Regel nur eine Bestellnummer
                                                                  eintragen.

                                        Dokumentensperre          Während der Preis- und Rechnungsprüfung sind die
                                                                  referenzierten Dokumente für den Zugriff durch andere
                                                                  Mitarbeiter gesperrt.

                                        Voreinstellungen          Firmendaten:
                                                                  •   Register Steuer
                                                                  •   Register Preisberechnung
                                                                  •   Register Druck
                                                                  •   Register Lager/EK/EDI
3.30 / 04-2020




                 A+W Business Einkauf                                                                             D-143
                 Lieferungen im Wareneingang                                                                Tutorial




                                       Eingangsrechnung
                                       Die Preise können sowohl auf Basis der Auftragsbestätigung des Lieferanten
                                       als auch auf Basis der Lieferantenrechnung geprüft werden. Die Dialoge
                                       Preiskontrolle und Rechnungskontrolle sind identisch aufgebaut. In beiden Di-
                                       alogen können Sie die Preise korrigieren und Ihre Einkaufspreise (EK) in den
                                       Dokumenten aktualisieren.
                                       Während der Preis-/Rechnungskontrolle ist die zugehörige Bestellung für den
                                       Zugriff durch andere Benutzer gesperrt. Um die Bestellung während der Preis-
                                       bzw. Rechnungskontrolle anpassen zu können, kann das Dokument direkt ge-
                                       öffnet werden. So können Sie z. B. fehlende Zuschläge erfassen, ohne die
                                       Preis- und Rechnungskontrolle zu verlassen.
                                       Die Prüfungen von Preisen und Rechnungen können auch in elektronisch
                                       ausgetauschten Dokumenten durchgeführt werden. Diese Funktionalität ist im
                                       Themenblock Elektronischer Dokumentenaustausch beschrieben:
                                        “Export/Import (openTRANS)” auf Seite D-151

                                       Preiskorrekturen
                                       Sie können die Preis- oder Rechnungskontrolle nur dann abschließen, wenn
                                       keine Differenz zwischen dem eingegebenen Gesamtbetrag und der Summe
                                       der angezeigten Bestellungen besteht. Eine solche Differenz kann z. B. durch
                                       unterschiedliche Preise, nicht erfasste Zuschläge oder durch Fehleingaben
                                       entstehen.
                                       Wenn der eingegebene Betrag nicht mit der Bestellung oder der Summe der
                                       Bestellungen übereinstimmt, müssen Sie die Preise in den Positionen oder in
                                       den Stücklisten korrigieren – oder die AB/Rechnung zur Korrektur zurückschi-
                                       cken.
                                       Nach der Rechnungskontrolle werden die Bestellungen mit dem entsprechen-
                                       den Status versehen und sind damit zur Anweisung und zur Übergabe an die
                                       FiBu bereit.
                                       Nach der Prüfung, Korrektur und Bestätigung der Preise wird der Status der
                                       Bestellung umgesetzt.
                                        “Dokumentenstatus” auf Seite D-40

                                       EK-Preise im Auftrag
                                       Der EK eines referenzierten Auftrags kann nur so lange aktualisiert werden,
                                       wie der Sperrstatus dies zulässt. Nach der Rechnungskontrolle wird der Status
                                       der Bestellung hochgesetzt. Die Preis- oder Rechnungskontrolle kann dann
                                       nicht nochmals durchgeführt werden.
3.30 / 04-2020




                 D-144                                                                      A+W Business Einkauf
                 Tutorial                                                              Lieferungen im Wareneingang




                                        Fußzuschläge und Fußrabatte
                                        Die Fußzuschläge/-rabatte einer Bestellung, z. B. ein Energiezuschlag,
                                        werden in die Kosten des Auftrags zurückgeschrieben. Die Fußzuschläge/-ra-
                                        batte werden positionsgenau zurückgerechnet und in der Dokumentenverwal-
                                        tung angezeigt. Damit ist auch bei bestellten Produkten der Deckungsbeitrag
                                        immer aktuell, der in der Positionserfassung angezeigt wird.
                                        Optional kann bei der Rechnungskontrolle automatisch die Position Anliefer-
                                        pauschale pro Bestellung angefügt werden. Damit entfällt die manuelle Nach-
                                        erfassung in der Bestellung.

                                        Fremdwährung
                                        Wenn Sie mit mehreren Währungen arbeiten, können Sie die Preise und
                                        Rechnungen in einer Fremdwährung bestätigen. Die Preise der Bestellpositi-
                                        onen werden in der Landeswährung gespeichert. Die Einkaufspreise werden
                                        unter Berücksichtigung der Währungsumrechnung aktualisiert.

                                        Sammel-AB und Sammelrechnung
                                        Wenn Ihr Lieferant mehrere Bestellungen gesammelt in einer AB oder Rech-
                                        nung aufgeführt hat, kann diese nur geprüft und akzeptiert werden, wenn in
                                        allen Bestellungen derselbe MwSt-Satz und dieselbe Währung angegeben
                                        sind.
                                        Wenn einer Ihrer Lieferanten in der Regel Sammelrechnungen erstellt, kann
                                        es sinnvoll sein, für diesen Lieferanten einen eigenen Nummernverwalter für
                                        die Bestellungen einzurichten.

                                        EK-Rückschreibung
                                        Der EK wird in die referenzierten Aufträge zurückgeschrieben, wenn er bei der
                                        Preis- oder Rechnungskontrolle und/oder beim Buchen des Wareneingangs
                                        geändert wurde. Diese angepassten Einkaufspreise werden zur Kalkulation
                                        des Deckungsbeitrags und bei der Lagerbewertung oder bei Lagerbestellun-
                                        gen herangezogen.
                                        Dazu müssen in den Firmendaten die Option zur Ermittlung der Einkaufs-
                                        preise aktiviert und die Preistabellen für den Einkauf gepflegt sein.




                                        Abb. D-91   Firmendaten – Register Lager/EK/EDI
3.30 / 04-2020




                 A+W Business Einkauf                                                                         D-145
                 Lieferungen im Wareneingang                                                                        Tutorial




                                           Rechnung kontrollieren
                                           Sie können die Preise sowohl in der Auftragsbestätigung als auch in der Rech-
                                           nung des Lieferanten prüfen. Dazu stehen zwei Dialoge zur Verfügung, die im
                                           Aufbau und in den Funktionen identisch sind:
                                           •   Preiskontrolle
                                           •   Rechnungskontrolle
                                           Die Preiskontrolle haben Sie bereits in der Einheit AB erfassen und Preise prü-
                                           fen kennengelernt. Analog zur Preiskontrolle können Sie die Lieferantenrech-
                                           nung prüfen und damit zur Anweisung freigeben.

                                               Cursorposition bestimmen
                                               Wenn Sie im Menü Optionen > Schnellerfassung aktivieren, springt der
                                               Cursor nach der Eingabe der Bestellnummer direkt in das Feld Rech-
                                               nungssumme bzw. AB-Summe. Sie können diese Option dann nutzen,
                                               wenn Sie in der Regel nur eine Bestellnummer eintragen.


                                            So prüfen Sie eine eingegangene Lieferantenrechnung
                                           1 Wählen Sie Dokumente > Bestellungen > Rechnung > Rechnungskontrol-
                                             le.




                 A                                                                                                       D
                 B

                 C

                                                                                                                         E




                 A Rechnungsnummer                                      D Bestellnummer(n)
                 B Rechnungsdatum                                       E Kurs
                 C Betrag der Rechnung (netto/brutto)
3.30 / 04-2020




                 Abb. D-92    Rechnungskontrolle


                                                Softwarereferenz, “Rechnungskontrolle – Bestellungen” auf Seite D-248



                 D-146                                                                             A+W Business Einkauf
                 Tutorial                                                                Lieferungen im Wareneingang




                                          2 Geben Sie die Rechnungsnummer (A), das Datum (B) und die Bestellnum-
                                            mer (D) ein und springen Sie mit <Tab> in das nächste Feld.
                                             In der Übersicht Bestellungen wird die Bestellung angezeigt.
                                             Wenn in der Rechnung mehrere Bestellungen zusammengefasst sind,
                                             können Sie nacheinander alle Bestellnummern angeben. Die Bestellungen
                                             werden dann jeweils in der Übersicht hinzugefügt. Sie können jedoch nur
                                             Bestellungen mit identischem Steuersatz zusammenfassen. Geben Sie
                                             einfach die nächste Bestellnummer ein und drücken Sie die <Tab>-Taste.
                                             Sie können eine Bestellung aus der Übersicht wieder entfernen, indem Sie
                                             den Eintrag markieren und auf <Entf> drücken.
                                          3 Geben Sie die Rechnungssumme (C) ein.

                                             Währung
                                             Wenn Sie nur mit einer Währung (EUR) arbeiten, muss im Feld Kurs (E) 1
                                             eingetragen sein.

                                          4 Wählen Sie im Menü Start > Ausführen, um die Eingabe zu bestätigen.
                                             Der Betrag wird geprüft und das Register Positionen wird angezeigt.




                                                                                                            A




                                                                                                            B


                 A Positionspreis                                    B Differenz über alle Positionen
                 Abb. D-93   Rechnungskontrolle – Positionen


                                             Sie können Preisdifferenzen ausgleichen, indem Sie einen Positionspreis
                                             überschreiben. Geänderte Beträge werden in die referenzierten Dokumen-
3.30 / 04-2020




                                             te zurückgeschrieben.




                 A+W Business Einkauf                                                                           D-147
                 Lieferungen im Wareneingang                                                                     Tutorial




                                       5 Wählen Sie im Menü Start > Ausführen, wenn keine Differenz (mehr) an-
                                         gezeigt wird.
                                          Die Daten werden gespeichert und der Status der Bestellung(en) wird um-
                                          gesetzt. Die Rechnungskontrolle für diese Dokumente kann danach nicht
                                          nochmals durchgeführt werden.
                                          Die Berechnung der EK-Preise wird in den zugehörigen Bestellungen und
                                          Aufträgen korrigiert, sofern diese Option im Menü Optionen > Gruppe Ein-
                                          stellungen aktiviert ist.


                                       Ergänzende Informationen
                                        Softwarereferenz, “Preiskontrolle” auf Seite D-205
                                        Softwarereferenz, “Rechnungskontrolle – Bestellungen” auf Seite D-248
3.30 / 04-2020




                 D-148                                                                        A+W Business Einkauf
                 Tutorial                                                              Lieferungen im Wareneingang




                                        Übungen
                                        Die Übungen sind so konzipiert, dass Sie den gesamten Einkauf trainieren.
                                        Das bedeutet, dass Sie die Bestellungen aus dem vorigen Themenblock jetzt
                                        weiterbearbeiten.

                                        Wareneingang erfassen
                                        Erfassen Sie den Wareneingang zu einer referenzierten Bestellung vollstän-
                                        dig und prüfen Sie die Statusumsetzung im Auftrag.

                                        Wareneingang teilweise erfassen
                                        Erfassen Sie eine Teillieferung zu einer referenzierten und zu einer manuellen
                                        Bestellung.
                                        Erfassen Sie den Wareneingang einer Lagerbestellung und einer Position mit
                                        Produkten, die nicht als Lagerartikel geführt werden (ganz oder teilweise).

                                        Wareneingang von Kisten erfassen
                                        Erfassen Sie den Wareneingang von Kisten ganz oder teilweise.

                                        Vollständigkeit der Lieferungen prüfen
                                        Suchen Sie nach Bestellungen, zu denen Positionen oder Teilpositionen nicht
                                        geliefert wurden.
                                        Holen Sie ggf. die Erfassung des Wareneingangs durch eine komplett-Bu-
                                        chung nach.

                                        Rechnung prüfen
                                        Erfassen Sie die Rechnung zu einem Wareneingang.
3.30 / 04-2020




                 A+W Business Einkauf                                                                          D-149
                 Elektronischer Dokumentenaustausch                                                               Tutorial




                                           Elektronischer Dokumenten-
                                           austausch
                                           In diesem Themenblock lernen Sie, wie Sie A+W Business für elektronischen
                                           Dokumentenaustausch anpassen und Dokumente exportieren und importie-
                                           ren.
                                           Dazu gehören folgende Lerneinheiten:
                                           •   “Export/Import (openTRANS)” auf Seite D-151
                                           •   “Datenexport/-import (EDI)” auf Seite D-177
                                           Sie können Dokumente mit Ihren Lieferanten/Kunden elektronisch austau-
                                           schen.
                                           Für den Austausch von Bestellungen werden die Daten in eine ASC-Datei ge-
                                           schrieben. Für den Austausch von Rechnungen oder Auftragsbestätigungen
                                           müssen die Daten im openTRANS-Format (XML-Format) vorliegen.



                                                                   EDI
                             Kundenauftrag = Bestellung                           Bestellung




                             Kunde                           A+W Business                             Lieferant

                         A+W Business                                                              A+W Business


                             Auftragsbestätigung (AB)                              Auftragsbestätigung (AB)
                             Rechnung                          openTRANS           Rechnung


                 Abb. D-94   Daten Ex- und Import


                                           Per EDI können Bestellungen ausgetauscht werden. Ein Kundenauftrag ist
                                           dabei aus Sicht des Kunden eine Bestellung, aus Sicht von A+W Business ein
                                           Auftrag.
                                           Im Format openTRANS können Auftragsbestätigungen (ABs) und Rechnun-
                                           gen ausgetauscht werden. Dazu müssen alle Beteiligten mit A+W Business
                                           arbeiten. Diese Funktion ist in den folgenden Kapiteln ausführlich dargestellt.
3.30 / 04-2020




                 D-150                                                                            A+W Business Einkauf
                 Tutorial                                                        Elektronischer Dokumentenaustausch




                                        Export/Import (openTRANS)
                                        Lernziele

                                        •   Funktionsweise des elektronischen Dokumentenaustauschs kennenlernen.
                                        •   Voreinstellungen kennenlernen und anpassen.
                                        •   Pflichtfelder in Dokumenten kennenlernen.
                                        •   Elektronische Dokumente senden und einlesen.


                                        Nutzen

                                        • Mit dem elektronischen Dokumentenaustausch können Sie Dokumente Ihrer
                                          Kunden und Lieferanten einlesen, ohne die Daten einzeln erfassen zu müssen.
                                        • Mit dem Einlesen von Daten vermindern sich Fehler bei der Erfassung.


                                        Merke

                                        Voraussetzung              Beim Lieferanten/Kunden und Ihnen muss die gleiche
                                                                   Version von A+W Business installiert sein, mindestens
                                                                   A+W Business 5.
                                                                   Die notwendigen Dienste müssen installiert und
                                                                   gestartet sein.

                                        Datenformat                Elektronische Dokumente können in den Formaten
                                                                   openTRANS und XML ausgetauscht werden.

                                        Datenimport                Die Daten können als Datei per E-Mail gesendet oder
                                                                   auf einem gemeinsamen freigegebenen Laufwerk auf
                                                                   einem Server gespeichert werden.

                                        Datenexport                Bei jedem Drucklauf von Auftragsbestätigungen oder
                                                                   Rechnungen wird geprüft, ob Dokumente mit dem
                                                                   Kennzeichen für den Export vorhanden sind. Diese
                                                                   Dokumente werden dann automatisch an die hinterlegte
                                                                   E-Mail-Adresse gesendet.

                                        Referenzen                 Dokumentenreferenzen werden aus folgenden Feldern
                                                                   gebildet:
                                                                   • Im Auftragskopf Feld Bestelltext1
                                                                   • In der Positionserfassung Feld Kundenposition.
                                                                   Diese Felder müssen daher immer gefüllt sein.
                                                                   Wenn diese Referenzen in eingelesenen Dokumenten
                                                                   nicht hergestellt werden können, muss die Zuordnung
                                                                   beim Prüfen des elektronischen Dokuments manuell
                                                                   nachgeholt werden.

                                        Teillieferungen            Aus einer elektronischen AB können Teillieferungen
                                                                   erstellt werden.

                                        Rundungsdifferenzen        Bei der Preis- und Rechnungskontrolle können
                                                                   Rundungsdifferenzen im Cent-Bereich akzeptiert
3.30 / 04-2020




                                                                   werden, wenn in der Produktverwaltung ein
                                                                   Ausgleichsprodukt angelegt ist, dem diese Differenzen
                                                                   zugeordnet werden können.



                 A+W Business Einkauf                                                                               D-151
                 Elektronischer Dokumentenaustausch                                                       Tutorial




                                       Merke

                                       Sammelrechnungen   Bei Sammelrechnungen des Lieferanten kann ein einmal
                                                          aufgeführter Zuschlag auf alle Positionen der
                                                          zugehörigen Bestellungen oder Bestellpositionen verteilt
                                                          werden.

                                       Dokumentensperre   Während der Preis- und Rechnungsprüfung sind die
                                                          referenzierten Dokumente für den Zugriff durch andere
                                                          Mitarbeiter gesperrt.

                                       Voreinstellungen   Stammdaten:
                                                          •   Produktdaten
                                                          •   Kunden-/Lieferantendaten
                                                          •   Statusdefinition
                                                          •   Statuszuordnung
                                                          •   Währungen
                                                          Firmendaten:
                                                          • Register Parameter
                                                          Stammdaten:
                                                          • B2B Kunde/Lieferant
3.30 / 04-2020




                 D-152                                                                   A+W Business Einkauf
                 Tutorial                                                      Elektronischer Dokumentenaustausch




                                        Dokumentenaustausch
                                        Auftragsbestätigungen und Rechnungen können im openTRANS-Format ex-
                                        portiert und importiert werden. Dieses Format wurde für A+W Business erwei-
                                        tert. Es können jedoch auch Dokumente im Standard-Format und XML-
                                        Dateien eingelesen werden.
                                        Der Datenaustausch über das openTRANS-Format setzt voraus, dass beim
                                        Lieferanten/Kunden und Ihnen die gleichen Versionen von A+W Business in-
                                        stalliert sind, mindestens A+W Business 5. Außerdem müssen in der Schnitt-
                                        stellenverwaltung die Parameter beim Lieferanten/Kunden genauso
                                        festgelegt werden wie in Ihrem A+W Business.

                                        Dokumenten-Export
                                        Der Export von Auftragsbestätigungen und Rechnungen wird pro Kunde/Lie-
                                        ferant im Modul Stammdaten > B2B konfiguriert. Dazu wird festgelegt, ob und
                                        welche Dokumente exportiert werden sollen und welcher Modus dazu verwen-
                                        det wird.

                                                                                 C




                                        B
                                        A




                                                                                         D
                                        A Export-Modus                         C Auswahl der Dokumente
                                        B Export-Format                        D Einstellungen für E-Mail-Modus
                                        Abb. D-95   Einstellungen für den elektronischen Datenaustausch


                                        Export-Modus (A):
                                        •   Automatischer Versand per E-Mail:
3.30 / 04-2020




                                            Dazu muss im Netzwerk ein E-Mail-Server zur Verfügung stehen. Stan-
                                            dardmäßig wird die E-Mail-Adresse aus den Stammdaten des Kunden/Lie-
                                            feranten verwendet. Für Auftragsbestätigungen und für Rechnungen
                                            können aber auch abweichende E-Mail-Adressen hinterlegt werden.


                 A+W Business Einkauf                                                                             D-153
                 Elektronischer Dokumentenaustausch                                                                Tutorial




                                       •   Ablage in einem bestimmten Verzeichnis (auf dem Server):
                                           Diese Dateien können anschließend manuell übermittelt werden.
                                       Bei jedem Drucklauf von Auftragsbestätigungen oder Rechnungen wird ge-
                                       prüft, ob Dokumente mit dem Kennzeichen für den Export vorhanden sind. Der
                                       eigentliche Export wird über einen Dienst zyklisch im Hintergrund durchge-
                                       führt. Zur Kontrolle werden die entsprechenden Dokumente im Dialog Export
                                       angezeigt. Durch den Export werden folgende Dateien erzeugt:
                                       •   RESPONSExxxx.awotres für Auftragsbestätigungen.
                                       •   DISPATCHxxxx.awotdis für ein Liefer-Avis.
                                       •   INVOICExxxx.awotinv für Rechnungen.
                                       Bei den Dateinamen wird zwischen Groß- und Kleinschreibung unterschie-
                                       den.

                                       Dokumentenreferenzen
                                       Die Dokumentenreferenzen auf Positionsebene werden benötigt, um Auf-
                                       tragspositionen automatisch ihren jeweiligen Bestellpositionen zuzuordnen
                                       (Referenzierung). Bei der manuellen Erfassung eines Auftrags werden diese
                                       Dokumentenreferenzen automatisch aus den Feldern Bestelltext1 im Auf-
                                       tragskopf und Kundenposition in der Positionserfassung gebildet.




                                                        A          B


                                       A Kopfdaten – Dokument                   B Positionen – Register Position
                                       Abb. D-96      Referenzen für den Datenaustausch


                                       Außerdem muss in den Firmendaten im Register Parameter die Option
                                       Bestelltext1 und Kundenposition in Dokumentenreferenzen übernehmen akti-
                                       viert sein.




                                       Abb. D-97      Firmendaten – Parameter
3.30 / 04-2020




                 D-154                                                                         A+W Business Einkauf
                 Tutorial                                                     Elektronischer Dokumentenaustausch




                                        Dokumenten-Import
                                        Auftragsbestätigungen und Rechnungen im openTRANS-Format werden
                                        über das A+W openTRANS ImportTool importiert. Es wird standardmäßig auf
                                        dem A+W Business-Client installiert.
                                        Zum Einlesen stehen damit unterschiedliche Möglichkeiten zur Verfügung:
                                        •   Doppelklick auf die gespeicherte Datei.
                                        •   Doppelklick auf die als E-Mail-Anhang gesendete Datei.
                                        Durch den Doppelklick werden die Daten in die Datenbank importiert und kön-
                                        nen in den Import-Dialogen von A+W Business angezeigt werden.
                                        Wenn die Dateien auf der Festplatte abgelegt sind, so kann über das Kontext-
                                        menü die Option Anzeigen gestartet und eine generische Ansicht des Doku-
                                        ments angezeigt werden.

                                        XML-Dateien
                                        XML-Dateien können nicht direkt aus dem E-Mail-Client heraus eingelesen
                                        werden. Diese Dateien müssen zunächst gespeichert werden. Danach kön-
                                        nen sie über das Kontextmenü eingelesen oder als generische Ansicht ange-
                                        zeigt werden.
                                        Nachdem ein Dokument erfolgreich eingelesen wurde, steht es im jeweiligen
                                        Dialog Elektr. Preiskontrolle oder Elektr. Rechnungskontrolle zur Verfügung.
3.30 / 04-2020




                 A+W Business Einkauf                                                                        D-155
                 Elektronischer Dokumentenaustausch                                                                Tutorial




                                            Dokumentenkontrolle
                                            Die Dialoge Elektr. Preiskontrolle und Elektr. Rechnungskontrolle sind iden-
                                            tisch aufgebaut.




                 A




                 B



                 C




                                                                              D
                 A Eingelesenes Dokument                              C Status
                 B Anzeige- und Filtereinstellungen                   D Referenzierte Dokumente
                 Abb. D-98    Elektronische Rechnungskontrolle


                                            In beiden Dialogen werden alle Dokumente (D) einschließlich möglicher Teil-
                                            lieferungen angezeigt, die mit dem importierten Dokument (A) verknüpft sind.
                                            Zu jeder Bestellung wird optisch signalisiert (C), ob die Verknüpfungen zwi-
                                            schen Bestellung und importiertem Dokument vollständig sind. Nur vollständig
                                            referenzierte Dokumente können akzeptiert werden.
                                            Wenn das importierte Dokument akzeptiert wurde, wird der Status der referen-
                                            zierten Bestellungen entsprechend umgesetzt. Die Preis- oder Rechnungs-
                                            kontrolle kann dann nicht nochmals durchgeführt werden.

                                            Buchungsarten
                                            Bei der Kontrolle der importierten Dokumente werden je nach Status die Op-
                                            tionen Akzeptieren, Teillieferung erstellen und Ablehnen angeboten.
                                            Die Buchungsart Akzeptieren ist nur dann freigeschaltet, wenn ein importier-
                                            tes Dokument vollständig und fehlerfrei referenziert ist. Wenn nur die Bestell-
3.30 / 04-2020




                                            mengen nicht vollständig referenziert sind, das Dokument jedoch ansonsten
                                            vollständig ist, so kann über die Buchungsart automatisch eine Teillieferung
                                            erzeugt werden.


                 D-156                                                                            A+W Business Einkauf
                 Tutorial                                                       Elektronischer Dokumentenaustausch




                                        Positionszuordnung
                                        Sind in einem openTRANS-Dokument die Bestellreferenzen fehlerhaft oder
                                        gar nicht vorhanden, kann das System Dokumenten- und Bestellpositionen
                                        nicht automatisch miteinander verknüpfen. Diese (nicht verknüpften) Positio-
                                        nen werden in der Positionsübersicht gekennzeichnet und müssen manuell
                                        verknüpft werden.
                                        In der Rechnung kann z. B. die Referenz zu einer Position fehlen oder fehler-
                                        haft aufgeführt sein. Anhand der Produktbezeichnungen können Sie diese Re-
                                        ferenzen im Dialog Positionen manuell zuordnen herstellen.

                                        Fußzuschläge/-rabatte
                                        Fußzuschläge oder -rabatte werden im Normalfall nicht in der Bestellung
                                        erfasst. In der Auftragsbestätigung oder Rechnung sind sie jedoch aufgeführt.
                                        Um eine Rechnungskontrolle durchführen zu können, müssen diese Positio-
                                        nen in den Bestellungen nachträglich erfasst werden. Dazu kann die Bestell-
                                        erfassung aus dem Dialog Rechnungskontrolle heraus geöffnet werden.
                                        Nachdem der Zuschlag in der Bestellung eingefügt ist, muss er in der Rech-
                                        nung zugeordnet werden.
                                        Wenn mehrere Bestellungen vom Lieferanten in einer Rechnung zusammen-
                                        gefasst sind, in der ein Fußzuschlag/-rabatt nur einmal aufgeführt ist, so kann
                                        diese Position auf alle verknüpften Bestellungen verteilt werden. Das Pro-
                                        gramm versucht, für die anteiligen Beträge anhand der Zuschlagsbasis sinn-
                                        volle Vorschlagswerte zu finden und bietet diese an. Diese Werte können
                                        überschrieben werden.
                                        Außerdem können die Fußzuschläge/-rabatte anhand der Produktnummer für
                                        diesen Lieferanten automatisch zugeordnet werden. Dabei wird die Zuord-
                                        nung der Produktnummer des Lieferanten zur eigenen Produktnummer ge-
                                        speichert.

                                        Sammelrechnungen in A+W Business
                                        Wenn in A+W Business Sammelrechnungen erstellt werden, so werden für je-
                                        den Auftrag die Fußzuschläge/-rabatte als eigene Position aufgeführt. Da eine
                                        direkte manuelle Zuordnung oft schwer ist, können in diesem Fall mehrere Do-
                                        kumentenpositionen zusammengefasst und den Bestellpositionen zugeordnet
                                        werden. In der Positionsübersicht ist anschließend nur noch die zusammen-
                                        gefasste Dokumentenposition aufgeführt.
3.30 / 04-2020




                 A+W Business Einkauf                                                                           D-157
                 Elektronischer Dokumentenaustausch                                                           Tutorial




                                       Betragsdifferenzen
                                       Üblicherweise können Sie eine Rechnung nur akzeptieren, wenn keine Diffe-
                                       renzen auftreten. Wenn Sie bei einem Lieferanten mit Betragsdifferenzen
                                       rechnen (müssen), können Sie diese auf unterschiedliche Weise behandeln:
                                       •   Sie können die Rechnung ablehnen und den Lieferanten über die Unstim-
                                           migkeiten (telefonisch) informieren.
                                       •   Betragsdifferenzen können auch durch unterschiedliche Rundungen ent-
                                           stehen. Mit der Option Betragsdifferenzen akzeptieren können Sie die
                                           Rechnungskontrolle trotz solcher Differenzen durchführen. Die Differenz
                                           darf sich nur im Cent-Bereich bewegen. Sie sollten sich mit der Option Hin-
                                           weis auf Betragsdifferenz/Ausgleichsposition darauf aufmerksam machen
                                           lassen.
                                           Die Rundungsdifferenzen im Cent-Bereich können automatisch akzeptiert
                                           werden. Dazu muss ein sogenanntes Ausgleichsprodukt angelegt sein, auf
                                           das der Differenzbetrag gebucht werden kann.
                                       •   Mit der Funktion Prod.Nr. für Ausgleichspos. können Sie ein Produkt aus-
                                           wählen, auf das Rundungsdifferenzen (im Cent-Bereich) verbucht werden
                                           sollen.
3.30 / 04-2020




                 D-158                                                                        A+W Business Einkauf
                 Tutorial                                                       Elektronischer Dokumentenaustausch




                                         Dienste prüfen
                                         Folgende Dienste müssen installiert und gestartet sein:
                                         •   A+W Business 6 Interface Service
                                             Dieser Dienst wird in aller Regel auf einem separaten Rechner installiert.
                                             Bei der Installation durch einen Service-Mitarbeiter der A+W Software
                                             GmbH muss die Funktion Interface Service handles B2B documents akti-
                                             viert werden.
                                         •   AWProtocol:
                                             Diesen Dienst finden Sie unter Systemsteuerung > Verwaltung > Dienste.
                                         •   ERP-WebService:
                                             Diesen Service finden Sie unter Systemsteuerung > Computerverwaltung
                                             > Dienste und Anwendungen > Sites > Default Web Site.




                    Abb. D-99   ERP-Service prüfen


                                         Die Dienste werden in der Regel mit A+W Business zusammen installiert. Sie
                                         sind auf den Starttyp Automatisch eingestellt. Dadurch sollten sie beim Start
                                         des Rechners automatisch gestartet werden.
                                         Wenn der Datenaustausch nicht funktioniert, sollten Sie die Dienste prüfen
                                         und ggf. manuell starten. Eine Anleitung dazu finden Sie in der Online-Hilfe
                                         des Betriebssystems.
                                         Außerdem benötigen Sie das A+W openTRANS ImportTool, das vom
                                         A+W Business-Setup automatisch installiert wird.
3.30 / 04-2020




                 A+W Business Einkauf                                                                           D-159
                 Elektronischer Dokumentenaustausch                                                              Tutorial




                                       Statusvergabe
                                       Der Status der Dokumente wird auch beim Im- und Export umgesetzt. Dazu
                                       müssen folgende Statuspunkte zugeordnet sein.

                                          Statuspunkte

                                          für Import                          für Export

                                          61 - Auftragsbestätigung nicht      830 - Rechnungsexport
                                          akzeptieren

                                          64 - Rechnung nicht akzeptieren     840 - Auftragsbestätigungsexport


                                       Beim Import wird der Status manuell umgesetzt, beim Export automatisch.
                                       Im Part Stammdaten sind die Statuspunkte und Statuszuordnungen ausführ-
                                       lich beschrieben. In dieser Einheit wird daher nur auf die Besonderheiten ein-
                                       gegangen, die Sie für den Austausch von elektronischen Dokumenten
                                       beachten müssen.
3.30 / 04-2020




                 D-160                                                                       A+W Business Einkauf
                 Tutorial                                                         Elektronischer Dokumentenaustausch




                                            Voreinstellungen für Datenaustausch prüfen
                                            In den Firmendaten müssen die Einstellungen für den Austausch von Pro-
                                            duktdaten korrekt eingestellt sein. Nur wenn die entsprechenden Produkt-
                                            daten hinterlegt und zugeordnet sind, können die Dokumente korrekt
                                            eingelesen werden.

                                               A+W Business neu starten
                                               Nach Änderungen der Firmendaten sollten Sie A+W Business neu starten.


                                             So prüfen Sie die Firmendaten
                                            1 Wählen Sie Stammdaten > Firma > Firmendaten und wechseln Sie zum
                                              Register Parameter.




                                                                                                              A




                 A Bestelltext übernehmen
                 Abb. D-100   Firmendaten – Parameter


                                                Stammdaten, “Firmendaten – Parameter” auf Seite B-936
                                            2 Aktivieren Sie die Checkbox Bestelltext1 und Kundenposition in Dokumen-
                                              tenreferenzen übernehmen.
3.30 / 04-2020




                                            3 Wählen Sie im Menü Start > Speichern, um Änderungen zu speichern.
                                               Die Daten werden gespeichert.


                 A+W Business Einkauf                                                                             D-161
                 Elektronischer Dokumentenaustausch                                                        Tutorial




                                       Währungseinstellungen prüfen
                                       Für die Währungen, die in den Aufträgen und Bestellungen verwendet wer-
                                       den, muss das internationale Währungskennzeichen hinterlegt sein. Die Ein-
                                       stellungen müssen Sie prüfen, wenn Sie mit mehreren Währungen arbeiten.


                                        So prüfen Sie die Währungseinstellungen
                                       1 Wählen Sie Stammdaten > Finanzen > Währung.

                                                                A                            B




                                          A Wechselkurs für Umrechnung von     B Internationales
                                            Preisen                              Währungskennzeichen
                                          Abb. D-101   Internationales Währungskennzeichen


                                           Stammdaten, “Währung” auf Seite B-909
                                          Jeder Währung muss das internationale Kennzeichen (B) zugewiesen
                                          sein.
                                       2 Markieren Sie die Zeile der Währung, der Sie das Kennzeichen zuweisen
                                         wollen.
                                       3 Öffnen Sie in der Spalte Internat. Kennzeichen die Kombobox und wählen
                                         Sie aus der Liste das entsprechende Kennzeichen aus.
                                       4 Prüfen Sie die jeweils eingetragenen Wechselkurse (A) und aktualisieren
                                         Sie diese ggf.
                                       5 Wählen Sie im Menü Start > Speichern, um Änderungen zu speichern.
                                          Die Daten werden gespeichert.
3.30 / 04-2020




                 D-162                                                                       A+W Business Einkauf
                 Tutorial                                                       Elektronischer Dokumentenaustausch




                                        Statusdefinitionen prüfen
                                        Damit die elektronischen Dokumente verarbeitet werden können, müssen die
                                        Statuspunkte 61, 64, 830, 840 definiert und zugeordnet sein. Diese Status-
                                        punkte werden für folgende Aktionen benötigt:
                                        •   Dokumente ex- und importieren.
                                        •   Importiertes Dokument ablehnen oder akzeptieren.
                                        Zu diesem Thema gibt es folgende Handlungsanleitungen:
                                        •   “So prüfen Sie die Statuspunkte” auf Seite D-163
                                        •   “So prüfen Sie die Statusverwaltung” auf Seite D-164
                                        •   “So prüfen Sie die Statuszuordnung” auf Seite D-165


                                         So prüfen Sie die Statuspunkte
                                        1 Wählen Sie Stammdaten > Auftrag > Statuspunkte.




                                            Abb. D-102   Statuspunkte


                                             Stammdaten, “Statuspunkte” auf Seite B-886
                                        2 Prüfen Sie, ob die Statuspunkte 61, 64, 830 und 840 vorhanden sind.
                                            Die Nummern der Statuspunkte sind in der Spalte Kennz. angegeben.
                                            In der Regel werden die Statuspunkte mit der Installation zusammen er-
                                            stellt. Sie müssen immer manuell zugeordnet werden.
                                        3 Wenn diese Statuspunkte nicht vollständig vorhanden sind, legen Sie die
                                          fehlenden an.
                                        4 Wählen Sie im Menü Start > Speichern, um Änderungen zu speichern.
                                            Die Daten werden gespeichert. Diese Statuspunkte müssen einem ent-
3.30 / 04-2020




                                            sprechenden Anwenderstatus zugeordnet sein.




                 A+W Business Einkauf                                                                        D-163
                 Elektronischer Dokumentenaustausch                                                        Tutorial




                                        So prüfen Sie die Statusverwaltung
                                       1 Wählen Sie Stammdaten > Auftrag > Statusverwaltung.




                                          Abb. D-103   Statusverwaltung


                                           Stammdaten, “Statusverwaltung” auf Seite B-885
                                          Wenn die Anwenderstatus 61/64 und 830/840 nicht vollständig vorhanden
                                          sind, legen Sie die fehlenden an.
                                       2 Wählen Sie im Menü Start > Speichern, um Änderungen zu speichern.
                                          Prüfen Sie als Nächstes, ob alle Zuordnungen vorhanden und vollständig
                                          sind.
3.30 / 04-2020




                 D-164                                                                       A+W Business Einkauf
                 Tutorial                                                     Elektronischer Dokumentenaustausch




                                         So prüfen Sie die Statuszuordnung
                                        1 Wählen Sie Stammdaten > Auftrag > Statuszuordnung.




                                                                                                                 A

                                                                                                                 B

                                                                                                                 C




                                        A Statuspunkt                         C Zugeordneter Anwenderstatus
                                        B Dokumententyp
                                        Abb. D-104   Statuszuordnung


                                            Stammdaten, “Statuszuordnung” auf Seite B-887
                                        2 Prüfen Sie, ob die Statuspunkte 61, 64, 830 und 840 zugeordnet sind.
                                           Wenn Sie in der Tabelle Statuszuordnung einen Statuspunkt markieren,
                                           muss mindestens der Anwenderstatus (C) angezeigt werden.
                                           Wenn diese Statuspunkte nicht vollständig zugeordnet sind, holen Sie die
                                           Zuordnung nach.
                                        3 Wählen Sie im Menü Start > Neu, um in den Erfassungs-Modus zu wech-
                                          seln.
                                        4 Wählen Sie in den Feldern Statuspunkt, Dokumententyp und Anwender-
                                          status die entsprechenden Einträge aus.
                                        5 Wählen Sie im Menü Start > Speichern, um Änderungen zu speichern.
                                           Die Daten werden gespeichert.
3.30 / 04-2020




                 A+W Business Einkauf                                                                         D-165
                 Elektronischer Dokumentenaustausch                                                            Tutorial




                                       Datenexport per openTRANS einstellen
                                       Im Modul Stammdaten > B2B müssen Sie festlegen, wie die Daten ausge-
                                       tauscht werden sollen.


                                        So legen Sie die Exportart für openTRANS fest
                                       1 Wählen Sie Stammdaten > B2B > Kunde > Dokumentenexport.
                                            Der Dialog openTRANS-Dokumentenexport wird mit dem Register Aus-
                                            wahl angezeigt.
                                       2 Wählen Sie im Menü Start > Suchen, um in die Kunden einzulesen.
                                            Die Kunden werden im Register Tabelle aufgelistet.
                                       3 Markieren Sie den Kunden (C), mit dem Dokumente über das open-
                                         TRANS-Format ausgetauscht werden sollen.
                                       4 Wechseln Sie zum Register Auswahl.
                                            •   Wenn die Angaben für den Kunden korrekt sind, können Sie den nächs-
                                                ten Kunden prüfen.
                                            •   Wenn keine Angaben vorhanden sind, müssen Sie diese einpflegen.

                                                                                 D                     E




                                        C


                                        B
                                        A




                                       A Exportart per Datei oder per E-Mail   D Auswahl der Dokumentenart
                                       B Übertragungstyp                       E E-Mail-Adressen für unterschiedliche
                                       C Kundennummer                            Dokumentenarten

                                       Abb. D-105     openTRANS-Dokumentenexport
3.30 / 04-2020




                 D-166                                                                        A+W Business Einkauf
                 Tutorial                                                      Elektronischer Dokumentenaustausch




                                        5 Wählen Sie im Feld Typ (B) den Eintrag Standard (openTRANS basierend)
                                          aus.
                                           Mit dieser Einstellung erhalten die Dokumente für diesen Kunden automa-
                                           tisch das Kennzeichen für den openTRANS-Austausch.
                                        6 Wählen Sie im Feld Exportart (A) aus, wie die Dateien ausgetauscht wer-
                                          den sollen.
                                           •   Export in eine Datei:
                                               Mit dieser Einstellung werden die Daten in eine Datei geschrieben. Die
                                               Felder für den Zielpfad werden freigeschaltet. Sie können ein Verzeich-
                                               nis auswählen oder den Pfad manuell eintragen.
                                           •   Export per E-Mail:
                                               Mit dieser Einstellung werden die Daten als Anhang einer E-Mail gesen-
                                               det. Dazu müssen Sie prüfen, ob in den Stammdaten des Kunden die
                                               E-Mail-Adresse korrekt eingetragen ist.
                                                “Partnerstammdaten prüfen” auf Seite D-168
                                        7 Wählen Sie aus, ob Auftragsbestätigungen und/oder Rechnungen (D) ex-
                                          portiert werden sollen.
                                        8 Wenn Sie die Daten per E-Mail senden, können Sie abweichende E-Mail-
                                          Adressen (E) für Auftragsbestätigungen, Rechnungen und/oder Lieferavis
                                          eintragen.
                                        9 Wählen Sie im Menü Start > Speichern, um Änderungen zu speichern.
                                           Die Daten werden gespeichert.
                                        10 Wiederholen Sie die Schritte 3 bis 9 für alle Kunden, mit denen Sie Daten
                                           austauschen.
                                           Um Auftragsbestätigungen und Rechnungen Ihrer Lieferanten importieren
                                           zu können, brauchen Sie keine weiteren Einstellungen festzulegen.
3.30 / 04-2020




                 A+W Business Einkauf                                                                          D-167
                 Elektronischer Dokumentenaustausch                                                            Tutorial




                                          Partnerstammdaten prüfen
                                          In den Stammdaten der Lieferanten/Kunden müssen die Daten für die Kom-
                                          munikation korrekt hinterlegt sein, damit Dokumente direkt aus A+W Business
                                          heraus versendet werden können.


                                           So prüfen Sie die Lieferanten-/Kundendaten
                                          1 Wählen Sie Stammdaten > Marktpartner > Lieferant, Kunde > Lieferanten,
                                            Kunden.




                    A




                   A E-Mail-Adresse für den Dokumentenaustausch
                   Abb. D-106   Partnerdaten – Adresse


                                              Stammdaten, “Partnerverwaltung” auf Seite B-759
                                          2 Prüfen Sie, ob die E-Mail-Adresse des Lieferanten, Kunden korrekt ist.
                                             Wenn Ihr Lieferanten oder Kunden mehrere E-Mail-Adressen haben, kön-
                                             nen Sie in den Einstellungen für den Dokumentenaustausch auch alterna-
                                             tive E-Mail-Adressen eingeben.
                                              “Datenexport per openTRANS einstellen” auf Seite D-166
                                          3 Wechseln Sie zum Register Auftrag und prüfen Sie, ob die externe Num-
                                            mer eingetragen ist.




                                                                                                                 A


                   A Externe Nummer angeben
                   Abb. D-107   Partnerdaten – Auftrag
3.30 / 04-2020




                 D-168                                                                           A+W Business Einkauf
                 Tutorial                                                     Elektronischer Dokumentenaustausch




                                           In den Kunden- und Lieferantendaten hat diese Nummer folgende Bedeu-
                                           tung:
                                           •   Lieferantendaten:
                                               Die externe Kundennummer erhalten Sie von Ihrem Lieferanten. Sie
                                               muss auch dann eingetragen werden, wenn Sie mit Ihrer internen Num-
                                               mer identisch ist.
                                           •   Kundendaten:
                                               In den Stammdaten zu Ihren Kunden muss in diesem Feld die Nummer
                                               stehen, die Sie bei Ihrem Kunden als Lieferant kennzeichnet.
                                        4 Wählen Sie im Menü Start > Speichern, um Änderungen zu speichern.


                                        Elektronisches Dokument einlesen
                                        Elektronische Dokumente können Sie in zwei Formaten erhalten haben: als
                                        openTRANS-Datei oder als XML-Datei. Je nach den Einstellungen in Ihrem
                                        Betrieb sind diese Dateien in einem bestimmten Verzeichnis auf dem Server
                                        abgelegt oder als Anhang einer E-Mail verfügbar.


                                         So lesen Sie ein openTRANS-Dokument ein
                                        1 Öffnen Sie das Verzeichnis mit den gesendeten Dateien oder die E-Mail,
                                          mit der die Datei gesendet wurde.
                                           Die openTRANS-Datei hat die Dateiendung *.awotdis, *.awotres oder
                                           *.awotinv.
                                        2 Starten Sie den Import mit einem Doppelklick auf die Datei.
                                           Die Daten werden eingelesen und in den Dialogen für die elektronische
                                           Preis- oder Rechnungskontrolle angezeigt.


                                         So lesen Sie ein XML-Dokument ein
                                        1 Öffnen Sie das Verzeichnis mit den gesendeten Dateien oder die E-Mail,
                                          mit der die Datei gesendet wurde.
                                        2 Speichern Sie die XML-Datei auf Ihren Rechner.
                                        3 Wählen Sie die Datei im Explorer aus und öffnen Sie das Kontext-Menü.
                                        4 Wählen Sie die Option Als openTRANS-Dokument einlesen.
                                           Die Daten werden eingelesen und in den Dialogen für die elektronische
                                           Preis- oder Rechnungskontrolle angezeigt.
3.30 / 04-2020




                 A+W Business Einkauf                                                                      D-169
                 Elektronischer Dokumentenaustausch                                                                 Tutorial




                                           Elektronisches Dokument prüfen
                                           Sie können in importierten Dokumenten Ihrer Lieferanten die Preise sowohl in
                                           der Auftragsbestätigung als auch in der Rechnung prüfen. Dazu stehen zwei
                                           Dialoge zur Verfügung, die im Aufbau und den Funktionen identisch sind:
                                           •   Elektronische Preiskontrolle
                                           •   Elektronische Rechnungskontrolle
                                           Die Handlungsschritte werden im Folgenden am Beispiel der elektronischen
                                           Rechnungskontrolle beschrieben.


                                            So prüfen und akzeptieren Sie eine importierte Lieferantenrechnung
                                           1 Wählen Sie Dokumente > Bestellungen > Rechnung > Elektr. Rechnungs-
                                             kontrolle.




                 A




                 B




                 C




                                                       D    E                    F
                 A Optionen für die Buchungsart                           D Hinweis zu Diskrepanzen
                 B Einschränkung der Anzeige                              E Filterung der angezeigten Dokumente
                 C Status des markierten Dokuments                        F Referenzierte Dokumente
                 Abb. D-108   Elektronische Rechnungskontrolle – Dokumentenimport


                                           2 Schränken Sie die Anzeige ein, wenn zu viele Dokumente angezeigt wer-
                                             den:
                                               •   Wählen Sie für die Anzeige (B) den Eintrag Nur offene Dokumente.
                                               •   Klicken Sie auf die Schaltfläche (E) und stellen Sie die gewünschten Fil-
3.30 / 04-2020




                                                   ter ein. Im Dialog Filtereinstellungen können Sie mehrere Lieferanten
                                                   auswählen und mit [OK] übernehmen.
                                                    Softwarereferenz, “Filtereinstellungen” auf Seite D-223



                 D-170                                                                                A+W Business Einkauf
                 Tutorial                                                            Elektronischer Dokumentenaustausch




                                           3 Markieren Sie eine der angezeigten Rechnungen.
                                              In der Übersicht Bestellungen/Teillieferungen (F) werden alle Bestellungen
                                              aufgelistet, die zu dieser Rechnung gehören.
                                              Im Bereich Dokumentenstatus (C) können Sie sehen, ob Referenzen feh-
                                              len und/oder Differenzen in Preisen oder Mengen auftreten.
                                              •   Wenn Sie Preisdifferenzen nicht akzeptieren wollen, wählen Sie die Op-
                                                  tion Ablehnen (A) und schicken Sie die Rechnung zurück.
                                                  Das Dokument wird als abgelehnt gekennzeichnet und kann archiviert
                                                  werden.
                                              •   Korrigieren Sie die Differenzen wie in den folgenden Handlungsschrit-
                                                  ten erläutert wird.
                                              •   Stellen Sie die fehlenden Referenzen her.
                                                   “So ordnen Sie Positionen in einer importierten Rechnung zu” auf
                                                    Seite D-173
                                           4 Wechseln Sie ggf. zum Register Positionsübersicht, um die Differenzen
                                             der Einkaufspreise einzelner Positionen zu prüfen.
                                              Wenn Betragsdifferenzen durch unterschiedliche Rundungen aufgetreten
                                              sind, können Sie diese über Menü Optionen > Betragsdifferenzen akzep-
                                              tieren generell zulassen. In diesem Fall können Sie eine der Buchungsar-
                                              ten Ablehnen oder Akzeptieren wählen.




                    Abb. D-109   Elektronische Rechnungskontrolle – Positionsübersicht
3.30 / 04-2020




                                              Sie können die Positionspreise und -mengen nicht direkt korrigieren.
                                           5 Markieren Sie die Position, die Sie korrigieren möchten.



                 A+W Business Einkauf                                                                                  D-171
                 Elektronischer Dokumentenaustausch                                                             Tutorial




                                       6 Wählen Sie im Menü Funktionen > Bestellerfassung öffnen und korrigieren
                                         Sie die Menge.
                                          Wenn Sie die Differenzen korrigiert und gespeichert haben und die Bestel-
                                          lerfassung wieder schließen, werden die neuen Werte in der elektroni-
                                          schen Rechnungskontrolle angezeigt.
                                          Preisdifferenzen brauchen Sie nicht manuell zu korrigieren. Es genügt,
                                          wenn Sie das Dokument trotz dieser Differenzen akzeptieren. Die Korrek-
                                          tur führt das Programm automatisch aus.
                                       7 Wenn alle Fehler behoben sind, wählen Sie die Option Akzeptieren.
                                       8 Wählen Sie im Menü Start > Speichern, um die Rechnungskontrolle abzu-
                                         schließen.
                                          Die Daten werden gespeichert und der Status der Bestellung(en) wird um-
                                          gesetzt. Die Rechnungskontrolle für diese Dokumente kann danach nicht
                                          nochmals durchgeführt werden.


                                       Teillieferung aus elektronischem Dokument erstel-
                                       len
                                       Wenn in dem eingelesenen Dokument nur ein Teil der Bestellpositionen oder
                                       bestellten Mengen aufgeführt ist, können Sie eine Teillieferung erstellen.


                                        So erstellen Sie eine Teillieferung zu einer importierten
                                         Lieferantenrechnung
                                       1 Wählen Sie Dokumente > Bestellungen > Rechnung > Elektr. Rechnungs-
                                         kontrolle.
                                           Softwarereferenz, “Elektronische Rechnungskontrolle” auf Seite D-256
                                       2 Markieren Sie die Rechnung, zu der Sie eine Teillieferung erfassen möch-
                                         ten.
                                          Wenn der Dokumentenstatus außer Mengendifferenzen keine weiteren
                                          Fehler anzeigt, können Sie eine Teillieferung erzeugen. Nur dann ist die
                                          Option Teillieferung erstellen freigeschaltet.
                                          Wie Sie fehlende Referenzen herstellen, finden Sie unter:
                                           “So ordnen Sie Positionen in einer importierten Rechnung zu” auf Seite D-173
                                       3 Wählen Sie die Option Teillieferung erstellen.
                                       4 Wählen Sie im Menü Start > Ausführen, um die Teillieferung zu erzeugen.
                                          Damit wird eine Teillieferung mit der Rechnungsnummer, der gelieferten
                                          Menge und den Preisen aus dem importierten Dokument erzeugt.
                                          Der Status der Original-Bestellung wird entsprechend umgesetzt.
                                          Die Original-Bestellung kann so lange wieder zugeordnet werden, bis alle
                                          Positionen vollständig geliefert und referenziert sind.
3.30 / 04-2020




                 D-172                                                                         A+W Business Einkauf
                 Tutorial                                                             Elektronischer Dokumentenaustausch




                                           Positionen im elektronischen Dokument zuordnen
                                           Wenn die Referenzen im elektronischen Dokument nicht eindeutig sind, kann
                                           die Position nicht zugeordnet werden. Diese Zuordnung können Sie bei der
                                           Prüfung des Dokuments nachholen.
                                           Wenn eine Position in der Bestellung vollständig fehlt, z. B. ein Energiezu-
                                           schlag, müssen Sie diese Position in der entsprechenden Bestellung zunächst
                                           erfassen. Sie können dazu die Bestellung aus der Preis-/Rechnungskontrolle
                                           heraus öffnen. Wenn Sie die Position erfasst und gespeichert haben, fahren
                                           Sie in der Rechnungskontrolle fort.


                                            So ordnen Sie Positionen in einer importierten Rechnung zu
                                           1 Wählen Sie Dokumente > Bestellungen > Rechnung > Elektr. Rechnungs-
                                             kontrolle.
                                               Der Dialog (elektronische) Rechnungskontrolle wird geöffnet und die im-
                                               portierten Rechnungen werden angezeigt.
                                                Softwarereferenz, “Elektronische Rechnungskontrolle” auf Seite D-256
                                           2 Markieren Sie die Rechnung, deren Positionen Sie zuordnen möchten.
                                           3 Wechseln Sie zum Register Positionsübersicht.
                                               Sie können eine Position in der Bestellung nachträglich erfassen, indem
                                               Sie über das Menü Funktionen > Bestellerfassung öffnen zum Dokument
                                               wechseln. Wenn Sie die Position erfasst und gespeichert haben, fahren
                                               Sie in der Rechnungskontrolle mit Schritt 4 fort.
3.30 / 04-2020




                 Abb. D-110   Elektronische Rechnungskontrolle – Positionsübersicht



                 A+W Business Einkauf                                                                                   D-173
                 Elektronischer Dokumentenaustausch                                                                 Tutorial




                                           4 Markieren Sie die Position, die nicht zugeordnet werden konnte, und wäh-
                                             len Sie im Menü Funktionen > Positionen manuell zuordnen.




                 A                                                                                            D




                 B
                 C

                 A Position aus der Rechnung                             C  Zuordnung des Fußzuschlags für alle künftigen
                 B Zuordnung des Fußzuschlags für die aktuelle Sitzung     Importe speichern
                   beibehalten                                           D Position in der Bestellung
                 Abb. D-111   Elektronische Rechnungskontrolle – Positionen zuordnen

                                               Softwarereferenz, “Positionen manuell zuordnen” auf Seite D-221
                                           5 Markieren Sie in der linken und der rechten Übersicht jeweils die Positio-
                                             nen (A, D), die Sie einander zuordnen möchten.
                                           6 Klicken Sie auf [OK], um die Zuordnung zu speichern.
                                           7 Wiederholen Sie den Vorgang, bis alle Positionen zugeordnet sind.
                                              Wenn Sie Fußzuschläge/-rabatte zugeordnet haben, können Sie über die
                                              beiden Checkboxen (B, C) festlegen, ob die Zuordnung für diese Rech-
                                              nung und/oder diesen Lieferanten beibehalten werden soll.
                                              Wie Sie einen Fußzuschlag/-rabatt auf mehrere Bestellungen verteilen, fin-
                                              den Sie unter:
                                               “Zuschläge/Rabatte manuell zuordnen” auf Seite D-175
                                           8 Klicken Sie auf [Ende], wenn alle Zuordnungen korrekt sind.
                                              Im Dialog Elektr. Rechnungskontrolle sind alle Buchungsarten freigeschal-
                                              tet.
                                           9 Wählen Sie die gewünschte Buchungsart, z. B. Akzeptieren.
                                           10 Wählen Sie im Menü Start > Ausführen, um die Aktion zu starten.


                                           11 Wählen Sie im Menü Start > Speichern, um die Daten zu speichern.
                                              Die Daten werden gespeichert und der Status der Bestellung(en) wird um-
3.30 / 04-2020




                                              gesetzt.




                 D-174                                                                             A+W Business Einkauf
                 Tutorial                                                        Elektronischer Dokumentenaustausch




                                        Zuschläge/Rabatte manuell zuordnen
                                        Wenn in einer Rechnung zu mehreren Bestellungen nur ein Fußzuschlag/-ra-
                                        batt aufgeführt ist, können Sie diesen manuell auf die einzelnen Bestellungen
                                        und/oder Bestellpositionen verteilen. Der Zuschlag/Rabatt wird dann anteilig
                                        berechnet und in die Bestellungen zurückgeschrieben.


                                         So verteilen Sie den Fußzuschlag/-rabatt auf Bestellungen
                                        1 Wählen Sie Dokumente > Bestellungen > Rechnung > Elektr. Rechnungs-
                                          kontrolle.
                                           Der Dialog Elektr. Rechnungskontrolle wird geöffnet und die importierten
                                           Rechnungen werden angezeigt.
                                        2 Markieren Sie die Rechnung, aus der Sie den Fußzuschlag/-rabatt vertei-
                                          len möchten.




                                            Softwarereferenz, “Fußzuschläge/-rabatte verteilen” auf Seite D-222
                                           In der Übersicht Bestellungen/Teillieferungen werden alle referenzierten
                                           Dokumente angezeigt.
                                        3 Wählen Sie im Menü Funktionen > Fußzuschläge/-rabatte auf Bestellun-
                                          gen verteilen.
                                        4 Halten Sie die Taste <Strg> gedrückt und markieren Sie alle Position, auf
                                          die der Zuschlag/Rabatt verteilt werden soll.
                                        5 Klicken Sie auf [OK], um die Verteilung zu speichern.
                                           Die Daten werden in die betreffenden Bestellungen zurückgeschrieben.
                                           Die Einkaufspreise in den Bestellungen werden aktualisiert.
                                        6 Schließen Sie den Dialog mit [Ende] und fahren Sie mit der Rechnungs-
                                          kontrolle fort.
                                            “So prüfen und akzeptieren Sie eine importierte Lieferantenrechnung” auf
                                             Seite D-170
3.30 / 04-2020




                 A+W Business Einkauf                                                                              D-175
                 Elektronischer Dokumentenaustausch                                                             Tutorial




                                       Ergänzende Informationen
                                        Softwarereferenz, “Elektronische Preiskontrolle” auf Seite D-213
                                        Softwarereferenz, “Elektronische Rechnungskontrolle” auf Seite D-256
                                        Softwarereferenz, “Positionen manuell zuordnen” auf Seite D-221
                                        Stammdaten, “Geschäftsabläufe abbilden” auf Seite B-420
                                        Stammdaten, “Firmendaten – Parameter” auf Seite B-936
3.30 / 04-2020




                 D-176                                                                         A+W Business Einkauf
                 Tutorial                                                         Elektronischer Dokumentenaustausch




                                        Datenexport/-import (EDI)
                                        Lernziele

                                        • Funktion der Fremdschnittstelle kennenlernen.
                                        • Voreinstellungen für den Datenaustausch per EDI-Schnittstelle kennenlernen.


                                        Nutzen

                                        • Durch den Datenaustausch über EDI-Schnittstellen müssen Dokumente nicht
                                          manuell erfasst werden.


                                        Merke

                                        EDI                        EDI = Electronic Data Interchange, Elektronischer
                                                                   Datenaustausch per ASCII-Datei

                                        Schnittstellen             Die Schnittstellen müssen für Kunden und Lieferanten
                                                                   eingerichtet werden.

                                        Voreinstellungen           Firmendaten:
                                                                   • Register Lager/EK/EDI
                                                                   B2B:
                                                                   • Kunde, Lieferant
3.30 / 04-2020




                 A+W Business Einkauf                                                                              D-177
                 Elektronischer Dokumentenaustausch                                                         Tutorial




                                       Datenaustausch im ASC-Format
                                       Über eine EDI-Schnittstelle können Angebote, Aufträge, Bestellungen und
                                       Gutschriften ausgetauscht werden. Dabei werden die Daten in eine ASC-Datei
                                       (ascii) geschrieben. Den Pfad für diese Datei legen Sie für jeden Kunden und
                                       jeden Lieferanten fest.
                                       Standardmäßig werden die Daten der zu transferierenden Datei automatisch
                                       im ANSI-Format konvertiert, z. B. ä in ae.


                                       Firmendaten prüfen
                                       In den Firmendaten müssen Sie im Register Lager/EK/EDI die Voreinstellun-
                                       gen prüfen, die sich auf die Konvertierung beziehen.




                                       Abb. D-112     Firmendaten – Register Lager/EK/EDI


                                       In der Regel sollte die OEM/ANSI-Konvertierung nur deaktiviert werden, wenn
                                       die verwendete Schnittstelle dies explizit fordert.


                                       Einstellungen prüfen
                                       Wenn Sie mit Ihren Lieferanten/Kunden Aufträge und Bestellungen im ASC-
                                       Format austauschen, müssen Sie die Parameter für jeden einzelnen Lieferan-
                                       ten/Kunden einstellen.


                                        So prüfen Sie die Einstellungen für den Datenexport per EDI
                                       1 Wählen Sie Stammdaten > B2B > Lieferant > Lieferant.
                                          Für den Datenimport per EDI wählen Sie Stammdaten > B2B > Kunde >
                                          Kunde. Die nachfolgenden Handlungsschritte gelten analog.
                                       2 Wählen Sie im Menü Start > Suchen, um in die Suche zu starten.
                                          Die Trefferliste wird im Register Tabelle angezeigt.
                                       3 Markieren Sie den Lieferanten, an den Bestellungen über die EDI-Schnitt-
                                         stelle gesendet werden sollen.
3.30 / 04-2020




                 D-178                                                                       A+W Business Einkauf
                 Tutorial                                                          Elektronischer Dokumentenaustausch




                                            4 Wechseln Sie zum Register Auswahl.




                                                                                                        B




                                                                                                        C
                                                                                                        D

                 A




                 A Typ der Schnittstelle                             C Angaben für die Protokolldatei
                 B Angaben für die Zieldatei                         D Pfad für die Sicherungsdatei
                 Abb. D-113   Schnittstellenverwaltung


                                            5 Geben Sie die Verzeichnisse und Dateinamen (B) für die Export- und die
                                              Sicherungsdatei an (D).
                                            6 Wählen Sie die Schnittstellenversion (A) aus, mit der Ihr System arbeitet.
                                               Wenn Sie Auftragsbestätigungen und Rechnungen ebenfalls elektronisch
                                               austauschen (openTRANS-Format), müssen Sie die Version wählen, mit
                                               der Sie die Daten bisher übertragen haben. Die Version wird bei der Instal-
                                               lation von A+W Business festgelegt.
3.30 / 04-2020




                 A+W Business Einkauf                                                                              D-179
                 Elektronischer Dokumentenaustausch                                                          Tutorial




                                       Abb. D-114     Einstellungen für EDI-Dokumentenexport


                                       7 Wählen Sie im Menü Start > Speichern, um die Daten zu speichern.
                                          Die Daten werden gespeichert.
                                       8 Wechseln Sie zum Register Parameter.
3.30 / 04-2020




                 D-180                                                                         A+W Business Einkauf
                 Tutorial                                                            Elektronischer Dokumentenaustausch




                                                                                                       A
                                                                                                       B




                                                                                                                         A
                                                                                                                         B




                                                                                                                         C



                 A Zwangsreferenzierung                                C Parameter für den EDI-Import von Aufträgen
                 B Sperre für den Zugriff und Zeit der Sperre            (nur bei Kunden)

                 Abb. D-115   Parameter für den EDI-Austausch


                                            9 Markieren Sie die Checkboxen für Export:
                                                •   Zwangsreferenzierung (A):
                                                    Wenn eine Position ohne Referenz auf ein (externes) Produkt gesendet
                                                    wird, kann diese Position ignoriert werden. In diesem Fall wird eine Feh-
                                                    lermeldung im Logbuch eingetragen.
                                                    Wenn die Checkbox nicht markiert ist, wird die Produktnummer aus den
                                                    Stammdaten in die Schnittstellendatei geschrieben. Das ist z. B. dann
                                                    sinnvoll, wenn das sendende und das empfangende System die glei-
                                                    chen Produktstammdaten benutzen. In dem Fall ist es nicht nötig, Da-
                                                    ten in die Referenztabellen einzutragen.
                                                •   Locking aktiv und Maximale Lock-Zeit (B):
                                                    Mit dieser Einstellung verhindern Sie, dass für den eingegebenen Zeit-
                                                    raum nur ein Programm auf dieselbe Schnittstellendatei zugreifen kann.
                                                •   Import von Kundenaufträgen (C):
3.30 / 04-2020




                                                    Wenn Sie die Daten für Kunden einrichten, können Sie zusätzlich Ein-
                                                    stellungen für den Import festlegen.




                 A+W Business Einkauf                                                                                 D-181
                 Elektronischer Dokumentenaustausch                                                           Tutorial




                                       10 Wiederholen Sie die Schritte für alle Lieferanten, mit denen Sie Daten per
                                          EDI austauschen.
                                       11 Wechseln Sie zu Stammdaten > B2B > Kunde > Kunde und wiederholen
                                          Sie die Schritte für alle Kunden, mit denen Sie Daten per EDI austauschen.


                                       Bestellung exportieren
                                       Wenn Sie Bestellungen exportieren, werden die Daten in eine ASC-Datei ge-
                                       schrieben. Diese wird im festgelegten Verzeichnis abgelegt. Die Datei wird da-
                                       nach über die EDI-Schnittstelle zum Lieferanten übertragen.


                                        So exportieren Sie eine Bestellung
                                       1 Wählen Sie Dokumente > Bestellungen > Export.
                                          Der Dialog Export wird geöffnet und die Bestellungen im aktuellen Num-
                                          mernverwalter werden angezeigt.




                                          Abb. D-116   Export von Bestellungen


                                       2 Wählen Sie im Menü Start > Ausführen, um den Export zu starten.
                                          Der Export wird gestartet. Eine Verlaufsmeldung zeigt an, welche Bestel-
                                          lung aktuell übertragen wird.
                                       3 Wechseln Sie zum Register Pool, um den Status des Exports zu prüfen.
                                          Sie können die Anzeige mit [Abfragen] aktualisieren.


                                       Ergänzende Informationen
3.30 / 04-2020




                                        Verkauf, “Import von Dokumenten” auf Seite C-377
                                        Stammdaten, “Schnittstellen-Dienst” auf Seite B-1032




                 D-182                                                                          A+W Business Einkauf
Einkauf                D

          Softwarereferenz




          A+W Business
                 Softwarereferenz                                                                             Übersicht




                                        Übersicht
                                        In der Dokumentenverwaltung können Sie alle Dokumente erfassen und be-
                                        arbeiten, die im Rahmen des Einkaufs benötigt werden, z. B. Anfragen zu Lie-
                                        ferungen und Bestellungen. Außerdem können Sie Wareneingänge erfassen,
                                        Liefertermine prüfen und korrigieren und die Lieferanten-Rechnungen kontrol-
                                        lieren.
                                        In der Softwarereferenz finden Sie Informationen zu folgenden Themen:
                                        •   Anfrage (Menü)
                                        •   Bestellung (Menü)
                                        •   Auftragsbestätigung
                                        •   Wareneingang
                                        •   Rechnung
                                        •   Basisglasverrechnung
                                        Folgende Dialoge sind für alle Dokumentenarten gleich und sind daher nur
                                        einmal im Part Verkauf erklärt:
                                        •   FiBu-Übergabe
                                        •   Übergabe Archiv
                                        •   Suche

                                            Dialoge können von unterschiedlichen Stellen aus geöffnet werden
                                            Bitte beachten Sie, dass viele Übersichten und Funktionen zum Thema
                                            Einkauf in A+W Business aus unterschiedlichen Dialogen heraus gestartet
                                            werden können. In dieser Anleitung werden die entsprechenden Dialoge
                                            nur einmal beschrieben.

                                            Dialoge, die auch für den Verkauf benötigt werden, sind ausführlich im Part
                                            Verkauf beschrieben.


                                        Dialogbeschreibungen im Part Verkauf
                                         Softwarereferenz, “Dokumentenverwaltung” auf Seite C-409
                                         Softwarereferenz, “Übersichten und Referenzen zu Kopfdaten” auf Seite C-522
                                         Softwarereferenz, “Positionsdaten” auf Seite C-440
                                         Softwarereferenz, “Übersichten und Referenzen zu Positionen” auf Seite C-582
                                         Softwarereferenz, “Nummernverwalter” auf Seite C-629
                                         Softwarereferenz, “Druck” auf Seite C-637
                                         Softwarereferenz, “Übergabe Archiv” auf Seite C-686
3.30 / 04-2020




                 A+W Business Einkauf                                                                            D-185
                 Anfrage (Menü)                                                                Softwarereferenz




                                  Anfrage (Menü)
                                  Dokumente > Anfrage
                                  Über das Menü Anfrage erreichen Sie folgende Programmpunkte:
                                  •   NV Anfrage:
                                      Die Funktion des Nummernverwalters ist für alle Dokumente gleich. Sie
                                      wird ausführlich zu den Aufträgen erklärt.
                                       Verkauf, “Nummernverwalter” auf Seite C-629
                                  •   Anfrage:
                                      Die Erfassung von Dokumenten ist für alle Dokumentenarten gleich. Sie
                                      wird ausführlich zu den Aufträgen erklärt.
                                       Verkauf, “Dokumentenverwaltung” auf Seite C-409
                                       Verkauf, “Positionsdaten” auf Seite C-440
                                  •   Druck Anfrage:
                                      Der Formular- und Etikettendruck ist für alle Dokumente gleich. Er wird
                                      ausführlich zu den Aufträgen erklärt.
                                       Verkauf, “Druck” auf Seite C-637
                                  •   Journal:
                                      Der Journaldruck ist für alle Dokumente gleich. Er wird ausführlich zu den
                                      Aufträgen erklärt.
                                       Verkauf, “Journal” auf Seite C-725
                                  •   Übergabe Archiv:
                                      Die Archivübergabe ist für alle Dokumente gleich. Sie wird ausführlich zu
                                      den Aufträgen erklärt.
                                       Verkauf, “Übergabe Archiv” auf Seite C-686
                                  •   Suche:
                                      Die Suche ist für alle Dokumente gleich. Sie wird ausführlich zu den Auf-
                                      trägen erklärt.
                                       Verkauf, “Dokument suchen” auf Seite C-523
3.30 / 04-2020




                 D-186                                                                    A+W Business Einkauf
                 Softwarereferenz                                                                         Anfrage (Menü)




                                          Anfrage (Dokumentenverwaltung)
                                          Dokumente > Anfrage > Anfrage




                 Abb. D-117   Dokumentenverwaltung – Anfrage


                                          In diesem Dialog erfassen und bearbeiten Sie Anfragen an Ihren Lieferanten.
                                          Anfragen können entweder manuell erfasst werden oder sie werden bei der
                                          Bestellübergabe erzeugt, wenn im Bestellpool die Option Sofort anfragen ge-
                                          wählt ist.
                                           Tutorial, “Anfrage” auf Seite D-110
                                           Verkauf, “Bestellübergabe – Bestellnummern” auf Seite C-657
                                          Die Felder im Dialog Dokumentenverwaltung und in der Positionserfassung
                                          sind für alle Dokumententypen gleich. Sie sind ausführlich zu den Aufträgen
                                          erklärt:
                                           Verkauf, “Dokument – Kopfdaten” auf Seite C-417
                                           Verkauf, “Dokument – Positionen” auf Seite C-451
3.30 / 04-2020




                 A+W Business Einkauf                                                                            D-187
                 Bestellung (Menü)                                                                 Softwarereferenz




                                     Bestellung (Menü)
                                     Dokumente > Bestellung
                                     Über das Menü Bestellung erreichen Sie folgende Programmpunkte:
                                     •   NV Bestellung:
                                         Die Funktion des Nummernverwalters ist für alle Dokumente gleich. Sie
                                         wird ausführlich zu den Aufträgen erklärt.
                                          Verkauf, “Nummernverwalter” auf Seite C-629
                                     •   Bestellung:
                                         Die Erfassung von Dokumenten ist für alle Dokumentenarten gleich. Sie
                                         wird ausführlich zu den Aufträgen erklärt.
                                          Verkauf, “Dokumentenverwaltung” auf Seite C-409
                                          Verkauf, “Positionsdaten” auf Seite C-440
                                     •   Teillieferung:
                                         Die Erstellung von Teillieferungen ist für alle Dokumentenarten gleich. Sie
                                         wird ausführlich zu den Aufträgen erklärt.
                                          Verkauf, “Teillieferungen” auf Seite C-616
                                     •   Nachbestellung:
                                         In diesem Dialog können Sie Bestellteile, die als Bruch gemeldet sind,
                                         nachbestellen, reklamieren, verrechnen oder die Auftragsmenge reduzie-
                                         ren.
                                          “Nachbestellung” auf Seite D-191
                                     •   Druck Bestellung:
                                         Der Formular- und Etikettendruck ist für alle Dokumente gleich. Er wird
                                         ausführlich zu den Aufträgen erklärt.
                                          Verkauf, “Druck” auf Seite C-637
                                     •   Export (EDI):
                                         In diesem Dialog exportieren Sie Bestellungen über die EDI-Schnittstelle.
                                          “Export (EDI)” auf Seite D-193
                                     •   Journal:
                                         Der Journaldruck ist für alle Dokumente gleich. Er wird ausführlich zu den
                                         Aufträgen erklärt.
                                          Verkauf, “Journal” auf Seite C-725
                                     •   AB Lieferant:
                                         In diesem Dialog erfassen und prüfen Sie die Auftragsbestätigungen (AB)
                                         Ihrer Lieferanten.
                                          “AB-Lieferant” auf Seite D-197
3.30 / 04-2020




                 D-188                                                                       A+W Business Einkauf
                 Softwarereferenz                                                                      Bestellung (Menü)




                                        •   Auftragsbestätigung:
                                            – Preiskontrolle:
                                               In diesem Dialog prüfen Sie die Auftragsbestätigungen Ihrer Lieferan-
                                               ten und korrigieren ggf. Preise.
                                                “Auftragsbestätigung” auf Seite D-204
                                            – Elektr. Preiskontrolle:
                                              In diesem Dialog prüfen Sie die Preise und Referenzen in elektronisch
                                              übermittelten Auftragsbestätigungen.
                                                “Auftragsbestätigung” auf Seite D-204
                                            – Mahnung:
                                              In diesem Dialog erfassen Sie Mahnungen für ausstehende Lieferun-
                                              gen.
                                                “Mahnung” auf Seite D-225
                                        •   Wareneingang
                                            – Wareneingang:
                                              In diesem Dialog erfassen Sie Wareneingänge zu Bestellungen und La-
                                              gerbestellungen.
                                                “Wareneingang” auf Seite D-227
                                            – Eingangskontrolle:
                                              In diesem Dialog prüfen Sie die Vollständigkeit der Wareneingänge.
                                                “Eingangskontrolle” auf Seite D-241
                                        •   Rechnung:
                                            – Rechnungskontrolle:
                                              In diesem Dialog prüfen Sie die Rechnungen Ihrer Lieferanten und kor-
                                              rigieren ggf. die Preise.
                                                “Rechnungskontrolle – Bestellungen” auf Seite D-248
                                            – Elektr. Rechnungskontrolle:
                                              In diesem Dialog prüfen Sie die Preise und die Referenzen in elektro-
                                              nisch übermittelten Rechnungen.
                                                “Elektronische Rechnungskontrolle” auf Seite D-256
                                        •   FiBu-Übergabe:
                                            Die FiBu-Übergabe ist für alle Dokumente gleich. Sie wird am Beispiel Auf-
                                            trag erklärt.
                                             Verkauf, “FiBu-Übergabe” auf Seite C-679
                                        •   Übergabe Archiv:
                                            Die Archivübergabe ist für alle Dokumente gleich. Sie wird ausführlich zu
                                            den Aufträgen erklärt.
                                             Verkauf, “Übergabe Archiv” auf Seite C-686
                                        •   Suche:
                                            Die Suche ist für alle Dokumente gleich. Sie wird ausführlich zu den Auf-
                                            trägen erklärt.
                                             Verkauf, “Dokument suchen” auf Seite C-523
                                        •   Basisglasverrechnung:
                                            Hier werden interne Verrechnungen von Profit Centern verwaltet. Die Ba-
                                            sisglasverrechnung ist nur kundenspezifisch freigeschaltet.
3.30 / 04-2020




                 A+W Business Einkauf                                                                            D-189
                 Bestellung (Menü)                                                                   Softwarereferenz




                                          Bestellung (Dokumentenverwaltung)
                                          Dokumente > Bestellung > Bestellung




                 Abb. D-118   Dokumentenverwaltung – Bestellung


                                          In diesem Dialog erfassen und bearbeiten Sie Bestellungen.
                                           Tutorial, “Manuelle Bestellung” auf Seite D-79
                                          Der Dialog Dokumentenverwaltung und die zugehörigen Menüs sind für alle
                                          Dokumentenarten gleich. Er wird am Beispiel Auftrag beschrieben.
                                           Verkauf, “Dokument – Kopfdaten” auf Seite C-417
                                           Verkauf, “Dokument – Positionen” auf Seite C-451

                                             Bestellung erfassen
                                             Die Bestellungen erfassen Sie auf die gleiche Weise wie einen Auftrag.
                                             Achten Sie dabei darauf, dass Sie den richtigen Dokumententyp auswäh-
                                             len:

                                             •   Lagerbestellung:
3.30 / 04-2020




                                                 Mit dieser Einstellung bestellen Sie Lagerprodukte. Mit dem Warenein-
                                                 gang werden die gelieferten Positionen automatisch auf Lager ver-
                                                 bucht.
                                                 In dieser Bestellung müssen Sie den Lagerartikel über die Lagersuche


                 D-190                                                                         A+W Business Einkauf
                 Softwarereferenz                                                                        Bestellung (Menü)




                                                   <F3> auswählen.
                                                   Der Typ Lagerbestellung wird im Feld Typ angezeigt.
                                               •   <k.A>:
                                                   Mit dieser Einstellung bestellen Sie alle Produkte, die nicht über das La-
                                                   ger verbucht werden.
                                                Verkauf, “Typ” auf Seite C-422
                                                Tutorial, “Unabhängige Bestellung erfassen” auf Seite D-81
                                               Wenn Sie eine Lagerbestellung mit Produkten erfassen, die nicht als La-
                                               gerartikel geführt werden, kann der Wareneingang für diese Produkte nicht
                                               automatisch ins Lager verbucht werden. Eine entsprechende Meldung
                                               weist Sie beim Erfassen der Bestellung darauf hin.

                                               Positionen ohne Lagerkennzeichen
                                               Wenn Sie Lagerbestellungen mit Positionen erfassen, die nicht als Lager-
                                               artikel geführt werden, werden diese im Wareneingang nicht angezeigt. Sie
                                               können in den Firmendaten die entsprechende Option aktivieren.

                                                Stammdaten, “Pos. ohne Lagerkennz. im WE anzeigen bei Lagerbestell.” auf
                                                 Seite B-959



                                          Nachbestellung
                                          Dokumente > Bestellung > Nachbestellung




                 Abb. D-119   Nachbestellung
3.30 / 04-2020




                                          In diesem Dialog verwalten Sie Aufträge mit Bestellteilen, die aus der Produk-
                                          tion als Bruch gemeldet sind. Sie können die Bestellteile nachbestellen, rekla-
                                          mieren, verrechnen oder die Auftragsmenge reduzieren.


                 A+W Business Einkauf                                                                                D-191
                 Bestellung (Menü)                                                               Softwarereferenz




                                     Selektion

                                     Auftrag von, bis Einschränkung der Suche auf einen Auftrag oder eine Fol-
                                     ge von Aufträgen.

                                     Liefertermin von, bis Einschränkung der Suche auf einen bestimmten Lie-
                                     fertermin oder eine Reihe von Lieferterminen.

                                     Dokumente
                                     In der Übersicht werden alle Aufträge mit Bruchscheiben angezeigt, die den
                                     Suchkriterien entsprechen.
                                     •   Auftrag:
                                         Auftragsnummer.
                                     •   Auftragsposition:
                                         Positionsnummer aus dem Auftrag.
                                     •   Lieferdatum:
                                         Lieferdatum aus dem Auftragskopf.
                                     •   Bestellung:
                                         Bestellnummer.
                                     •   Bestellposition:
                                         Positionsnummer aus der Bestellung.
                                     •   Lieferant:
                                         Name des Lieferanten aus der Bestellung.
                                     •   Produkt:
                                         Nummer und Bezeichnung des Produkts.
                                     •   Auftragsmenge:
                                         Menge aus dem Auftrag.
                                     •   Bestellmenge:
                                         Menge, die bestellt ist.
                                     •   Bruchmenge:
                                         Menge, die als Bruch gemeldet ist.
                                     •   Rückmeldedatum:
                                         Datum der Bruchmeldung.
                                     •   Aktion:
                                         Auswahl der Aktion:
                                         – Nachbestellung:
                                            Die Bestellung wird erstellt und in den ausgewählten Nummernverwal-
                                            ter gestellt.
                                         – Reklamation:
                                            Für die Bestellteile wird eine Reklamation erstellt. Wenn diese Option
                                            gewählt wird, können Reklamationsgrund und -verursacher angegeben
                                            werden.
                                         – wertmäßige Buchung:
                                            Die Bestellung wird mit einer negativen Positionsmenge erstellt. Damit
                                            wird die Bruchmenge ausgebucht und der Wert der Bruchmenge mit
                                            dem Wert des Auftrags verrechnet.
3.30 / 04-2020




                                         – Auftragsmenge reduzieren:
                                            Der Ursprungsauftrag wird um die Bruchmenge reduziert. Damit wird
                                            eine Nachbestellung ausgeschlossen.


                 D-192                                                                    A+W Business Einkauf
                 Softwarereferenz                                                                   Bestellung (Menü)




                                        •   Reklamationsgrund:
                                            Der Reklamationsgrund wird nur angegeben, wenn als Aktion Reklamation
                                            gewählt ist.
                                        •   Reklamationsverursacher:
                                            Der Reklamationsverursacher wird nur angegeben, wenn als Aktion Rekla-
                                            mation gewählt ist.
                                        •   Bemerkung:
                                            Sie können eine Bemerkung eintragen, z. B. Absprachen, die mit dieser
                                            Nachbestellung oder Reklamation verbunden sind.
                                        •   Etikett:
                                            Nummer des Etiketts aus der Produktion. Die Nummer kann nicht geändert
                                            werden.

                                        Ziel

                                        Nummernverwalter Nummernverwalter, in den die Nachbestellungen ge-
                                        stellt werden sollen.


                                        Export (EDI)
                                        Dokumente > Bestellung > Export
                                        In diesem Dialog können Sie Bestellungen exportieren, um Sie über die EDI-
                                        Schnittstelle an den betreffenden Lieferanten zu übertragen.
                                         Tutorial, “Datenexport/-import (EDI)” auf Seite D-177

                                            Voraussetzung
                                            Die Parameter für die Schnittstelle müssen für jeden einzelnen Lieferanten/
                                            Kunden festgelegt werden, mit dem Dokumente über die Fremdschnittstel-
                                            le ausgetauscht werden sollen. Diese Parameter werden im Menü Stamm-
                                            daten > B2B eingestellt.

                                        In diesem Kapitel finden Sie Informationen zu folgenden Themen:
                                        •   “Menü Funktionen” auf Seite D-194
                                        •   “Export – Export” auf Seite D-195
                                        •   “Export – Pool” auf Seite D-196
3.30 / 04-2020




                 A+W Business Einkauf                                                                           D-193
                 Bestellung (Menü)                                                                Softwarereferenz




                                     Menü Funktionen
                                     Dokumente > Bestellung > Export > Menü Funktionen
                                     Über dieses Menü können Sie andere Dialoge öffnen, ohne den Dialog Export
                                     zu schließen.

                                     Gruppe Bearbeiten
                                     •   Kopieren:
                                         Öffnet den Dialog Nummernverwalter kopieren, um einen neuen Num-
                                         mernverwalter zu erstellen.
                                          Verkauf, “Nummernverwalter kopieren” auf Seite C-634
                                     •   Statusänderung:
                                         Öffnet den Dialog Statusänderung, um den Status manuell umzusetzen
                                         und den Nummernverwalter zu ändern.
                                          Verkauf, “Statusänderung” auf Seite C-554

                                     Gruppe Dokument
                                     •   Dokument anzeigen:
                                         Öffnet den Dialog Dokumentenansicht zu einer Vorschau auf den Druck.
                                          Verkauf, “Reklamationen” auf Seite C-591
                                     •   Historie:
                                         Öffnet eine Übersicht über die Statusänderungen des markierten Doku-
                                         ments.
                                          Verkauf, “Historie” auf Seite C-552
                                     •   Dokumentendaten:
                                         Öffnet den Dialog Dokumentendaten, um ggf. die Termine und den Status
                                         zu korrigieren.
                                          Verkauf, “Dokumentendaten” auf Seite C-738
                                     •   Dokumentenerfassung:
                                         Öffnet den Dialog Dokumentenverwaltung, in dem Sie Dokumente anlegen
                                         oder ändern können.
                                          Verkauf, “Dokumentenverwaltung” auf Seite C-409

                                     Gruppe Dokumentenkopie
                                     •   Dokumente kopieren:
                                         Öffnet den Dialog Dokumente kopieren, um ein Dokument in den gleichen
                                         oder einen anderen Dokumententyp zu kopieren.
                                          Verkauf, “Dokumente kopieren” auf Seite C-532
                                     •   Teillieferung:
                                         Öffnet den Dialog Dokumente kopieren, um eine Teillieferung zu erfassen.
                                          Verkauf, “Dokumente kopieren” auf Seite C-532
3.30 / 04-2020




                 D-194                                                                       A+W Business Einkauf
                 Softwarereferenz                                                                 Bestellung (Menü)




                                        Export – Export
                                        Dokumente > Bestellung > Export > Register Export




                                        Abb. D-120    Export – Export


                                        In diesem Register exportieren Sie die Bestellungen. Die Daten werden in eine
                                        ASC-Datei geschrieben. Diese wird im festgelegten Verzeichnis abgelegt. Die
                                        Datei wird danach über die EDI-Schnittstelle zum Lieferanten übertragen.
                                        Die Einstellungen für den Export werden pro Lieferant im Modul Stammdaten
                                        > B2B festgelegt.
                                         Tutorial, “Datenexport/-import (EDI)” auf Seite D-177

                                        Selektion nach

                                        Mitarbeiter Name des Mitarbeiters, der sich in A+W Business angemeldet
                                        hat.

                                        Nummernverwalter Auswahl des Nummernverwalters, auf den der Dialog
                                        Export zugreifen soll.

                                        [Logbuch] Schaltfläche zum Öffnen des Systemlogbuchs.

                                        Dokumente
                                        Liste aller Dokumente, die im gewählten Nummernverwalter stehen. Sie sollen
                                        über die Schnittstellen an den Lieferanten gesendet werden.
                                        •   Nummer:
3.30 / 04-2020




                                            Nummer des Dokuments.
                                        •   Nummer Kunde/Lief.:
                                            Nummer des Kunden oder Lieferanten.



                 A+W Business Einkauf                                                                         D-195
                 Bestellung (Menü)                                                                Softwarereferenz




                                     •   Kunde/Lieferant:
                                         Name des Kunden oder Lieferanten.
                                     •   Status:
                                         Status des Dokuments:
                                     •   Datum Erfassung:
                                         Datum, an dem das Dokument erfasst wurde.
                                     •   Datum Lieferung:
                                         Lieferdatum
                                     •   Datum AB:
                                         Datum der Auftragsbestätigung
                                     •   Sperr-KZ:
                                         Kennzeichen, ob das Dokument gesperrt ist. Das Sperrkennzeichen wird
                                         bei Bestellungen selten gesetzt.


                                     Export – Pool
                                     Dokumente > Bestellung > Export > Register Pool




                                     Abb. D-121   Export – Pool


                                     In diesem Register können Sie die aufgelisteten Bestellungen elektronisch
                                     über die EDI-Schnittstelle übergeben.

                                     Übertragungs-Pool
                                     In der Übersicht werden alle Bestellungen aufgelistet, die elektronisch überge-
                                     ben werden sollen.

                                     [Löschen] Die Schaltfläche ist nur freigeschaltet, wenn ein Fehler bei der
3.30 / 04-2020




                                     Übertragung festgestellt wurde. Sie können dann einen Eintrag aus dem
                                     Übertragungspool löschen.




                 D-196                                                                     A+W Business Einkauf
                 Softwarereferenz                                                                   Bestellung (Menü)




                                        [Aktivieren] Die Schaltfläche ist nur freigeschaltet, wenn ein Fehler bei der
                                        Übertragung festgestellt wurde. Wenn ein Fehler festgestellt wurde, können
                                        Sie die Daten korrigieren und erneut zur Übertragung übergeben. Sie lösen
                                        die Übertragung mit [Aktivieren] aus.

                                        [Abfragen] Mit dieser Schaltfläche aktualisieren Sie die Anzeige, um den
                                        Übertragungsstatus zu prüfen.


                                        AB-Lieferant
                                        Dokumente > Bestellung > AB Lieferant
                                        In diesem Dialog können Sie die Auftragsbestätigung erfassen, die Ihr Liefe-
                                        rant zu einer Bestellung gesendet hat. Außerdem können Sie den zugehöri-
                                        gen Wareneingang erfassen und/oder die Termine für Bestellungen und
                                        Lieferungen prüfen und ggf. korrigieren.
                                        In diesem Kapitel finden Sie Informationen zu folgenden Themen:
                                        •   “Menü Optionen” auf Seite D-197
                                        •   “AB-Lieferant – Dokumente” auf Seite D-198
                                        •   “AB-Lieferant – Positionen” auf Seite D-202
                                        •   “AB-Lieferant – Liefertermine ändern” auf Seite D-203


                                        Menü Optionen
                                        Dokumente > Bestellung > AB Lieferant > Menü Optionen
                                        Über dieses Menü können Sie die Standardeinstellung des Dialoges bestim-
                                        men. Sie können die Optionen aktivieren oder deaktivieren. Die Einstellung
                                        wird nicht zurückgesetzt, wenn Sie den Dialog schließen.
                                        Folgende Einträge werden angezeigt:
                                        •   Lagerbuchungsdatum = Lieferdatum:
                                            Als Buchungsdatum wird automatisch das Lieferdatum aus der Bestellung
                                            übernommen. Wenn die Option deaktiviert ist, wird standardmäßig das Ta-
                                            gesdatum übernommen.
                                        •   AB-Nummer prüfen:
                                            Mit dieser Einstellung wird eine Meldung angezeigt, wenn die Nummer der
                                            Auftragsbestätigung durch den Lieferanten nicht eingegeben ist.
                                        •   Identnummernvergabe:
                                            Diese Einstellung wird für den Wareneingang von Kisten und Lagerplatten
                                            benötigt.
                                            – Manuell:
                                               Mit dieser Option müssen Sie die ID manuell vergeben. Die Checkbox
                                               Identnummer(n) vergeben im Bereich Optionen wird freigeschaltet.
                                                “Optionen” auf Seite D-199
                                            – Automatisch:
                                              Mit dieser Option wird die ID automatisch vergeben. Dazu kann eine
3.30 / 04-2020




                                              Vorgabe festgelegt werden. Wenn die Option nicht aktiviert ist, müssen
                                              Sie die ID manuell eingeben.



                 A+W Business Einkauf                                                                         D-197
                 Bestellung (Menü)                                                                      Softwarereferenz




                                              – Einstellungen:
                                                Öffnet den Dialog Einstellungen, in dem Sie die Vorgabe für die auto-
                                                matische Vergabe von IDs festlegen.
                                                  “Einstellungen (ID)” auf Seite D-240


                                          AB-Lieferant – Dokumente
                                          Dokumente > Bestellung > AB Lieferant > Register Dokumente




                 Abb. D-122   AB-Lieferant – Dokumente


                                          In diesem Register können Sie eine Auftragsbestätigung des Lieferanten und/
                                          oder den zugehörigen Wareneingang erfassen. Außerdem können Sie die
                                          Termine für Bestellungen und Lieferungen prüfen und ggf. korrigieren.
                                          Alle Daten, die Sie in diesem Register eintragen, gelten jeweils für alle Positi-
                                          onen, die in der Bestellübersicht aufgeführt sind. Wenn Sie die Daten zu ein-
                                          zelnen Positionen erfassen möchten, müssen Sie zum Register Positionen
                                          wechseln.
                                           Tutorial, “Lieferanten-AB” auf Seite D-87

                                          Dokumente
                                          Mit der Wahl der Option legen Sie fest, zu welcher Dokumentenart Sie die Auf-
                                          tragsbestätigung erfassen möchten. Mit der Lupe können Sie nach der Bestel-
                                          lung oder dem Auftrag suchen.
                                          •   Bestellnummer:
3.30 / 04-2020




                                              Auswahl einer Bestellung. Das Eingabefeld für die Bestellnummer ist frei-
                                              geschaltet.




                 D-198                                                                            A+W Business Einkauf
                 Softwarereferenz                                                                Bestellung (Menü)




                                        •   Auftragsnummer:
                                            Auswahl eines Kundenauftrags, aus dem eine Bestellung erzeugt wurde.
                                            Das Eingabefeld für die Auftragsnummer ist freigeschaltet.

                                        Optionen

                                        Auftrags-NV füllen Wenn Sie eine Auftragsbestätigung Ihres Lieferanten
                                        und ggf. auch den zugehörigen Wareneingang buchen, kann der zugehörige
                                        (Kunden-) Auftrag automatisch in einen anderen Nummernverwalter gestellt
                                        werden.
                                        ☐ Der referenzierte (Kunden-) Auftrag wird nicht in einen anderen Nummern-
                                        verwalter gestellt.
                                        ☑ Der referenzierte (Kunden-) Auftrag wird in den ausgewählten Nummern-
                                        verwalter gestellt.

                                        Bestell-NV füllen Wenn Sie eine Auftragsbestätigung Ihres Lieferanten und
                                        ggf. auch den zugehörigen Wareneingang buchen, kann die zugehörige Be-
                                        stellung automatisch in einen anderen Nummernverwalter gestellt werden.
                                        ☐ Die Bestellung wird nicht in einen anderen Nummernverwalter gestellt.
                                        ☑ Die Bestellung wird in den ausgewählten Nummernverwalter gestellt.

                                        Wareneingang buchen Sie können den kompletten Wareneingang erfas-
                                        sen, wenn Ihr Lieferant die Ware zusammen mit der AB geliefert hat.
                                        ☐ Der Wareneingang wird nicht erfasst.
                                        ☑ Der Wareneingang wird als komplett verbucht. Wenn in der Lieferung Kis-
                                        ten enthalten sind, müssen Sie die Einstellungen für die Kisten-ID prüfen.

                                            Wareneingang teilweise erfassen
                                            Den vollständigen Wareneingang für einzelne Positionen können Sie im
                                            Register Positionen erfassen.
                                            Wenn Sie den teilweisen Wareneingang einer Position erfassen möchten,
                                            müssen Sie zum Dialog Wareneingang wechseln.

                                             “Wareneingang (Dialog)” auf Seite D-227

                                        Identnummer(n) vergeben Die Checkbox wird über die Einstellung zur
                                        Identnummernvergabe aktiviert oder deaktiviert. Identnummern (IDs) werden
                                        in der Regel für Kisten vergeben. Sie können eine Vorgabe für die ID festle-
                                        gen, mit der der Wareneingang im Lager verbucht werden soll.
                                        Die Checkbox ist nur freigeschaltet, wenn Sie im Menü Optionen die Einstel-
                                        lung Manuell gewählt haben.
                                        ☐ Die Checkbox ist deaktiviert, wenn Sie im Menü Optionen die Einstellung
                                        Manuell gewählt haben. Die ID muss manuell eingegeben werden.
                                        ☑ Die Checkbox ist aktiviert, wenn Sie im Menü Optionen die Einstellung Au-
                                        tomatisch gewählt haben.
                                         “Einstellungen (ID)” auf Seite D-240

                                        Bestelldaten
3.30 / 04-2020




                                        Lieferant Name des Lieferanten aus der Bestellung oder dem Kundenauf-
                                        trag.


                 A+W Business Einkauf                                                                        D-199
                 Bestellung (Menü)                                                                  Softwarereferenz




                                     Status Status des ausgewählten Dokuments.

                                     Gesamtstückzahl Stückzahl aller Positionen insgesamt im ausgewählten
                                     Dokument.

                                     Bestätigter Anliefertermin Termin der Lieferung durch den Lieferanten.
                                     Das Datum ist aus der Bestellung übernommen. Sie können es ggf. ändern.
                                     Ein geänderter Termin wird in die Bestellung und ggf. in den referenzierten
                                     Auftrag zurückgeschrieben.
                                      “AB-Lieferant – Liefertermine ändern” auf Seite D-203

                                     Teilliefertermin Liefertermin, der in der Auftragsbestätigung durch den Lie-
                                     feranten gemeldet wird.

                                     AB-Nummer Nummer der Auftragsbestätigung, die der Lieferant gesendet
                                     hat. Diese Nummer wird in alle Positionen eingetragen, die in der Bestellüber-
                                     sicht angezeigt werden.
                                     Wenn die AB-Nummer nur für eine Position gelten soll, müssen Sie zum Re-
                                     gister Positionen wechseln.
                                      “AB-Lieferant – Positionen” auf Seite D-202

                                     Auftragsdaten
                                     Die Daten in diesem Bereich werden nur angezeigt, wenn ein Auftrag oder
                                     eine Bestellung zu einem Auftrag ausgewählt ist. Bei einer Lagerbestellung
                                     (ohne Auftrag) bleiben die Felder leer.

                                     Kunde Name des Kunden, für den die Bestellung erzeugt wurde.

                                     Status Status des Kundenauftrags.

                                     Gesamtstückzahl Stückzahl aller Positionen insgesamt im Kundenauftrag.

                                     Anliefertermin bei Kunden Termin der Anlieferung beim Kunden. Das Da-
                                     tum wird aus dem Auftrag übernommen. Sie können es ggf. ändern. Ein ge-
                                     änderter Termin wird in die Bestellung und ggf. in den referenzierten Auftrag
                                     zurückgeschrieben.
                                      Verkauf, “Kundenbenachrichtigung (Lieferterminkontrolle)” auf Seite C-565
                                      Tutorial, “Liefertermine ändern und Kunden benachrichtigen” auf Seite D-102
                                      “AB-Lieferant – Liefertermine ändern” auf Seite D-203

                                     Geplant Ursprünglich geplanter Anliefertermin beim Kunden.

                                     Versandtag Termin, an dem die Lieferung an den Kunden gesendet wird. In
                                     der Regel ist dieser Termin mit dem Termin der Anlieferung identisch. Nur
                                     wenn die Lieferung länger als einen Tag benötigt, muss der Versandtag vor
                                     dem Anliefertermin liegen.

                                     Tour Auswahl der Tour, mit der die Lieferung an den Kunden geht.
3.30 / 04-2020




                 D-200                                                                         A+W Business Einkauf
                 Softwarereferenz                                                                   Bestellung (Menü)




                                        Bestellpositionen
                                        Übersicht über alle Positionen der Bestellung. Wenn die Bestellung aus einem
                                        Kundenauftrag erzeugt wurde, können die Bestellpositionen zugleich die Po-
                                        sitionen des referenzierten Auftrags sein.
                                        •   Pos. Nr.:
                                            Nummer der Bestellposition. Bei einer Kundenbestellung kann dies auch
                                            die Positionsnummer aus dem Auftrag sein.
                                        •   Artikelbezeichnung:
                                            Nummer und Bezeichnung der bestellten Position.
                                        •   Menge:
                                            Menge der bestellten Position.
                                        •   Breite / Höhe:
                                            Maße der bestellten Position.
                                        •   Lieferanten-AB:
                                            Nummer der Auftragsbestätigung des Lieferanten. Wenn Sie die AB-Num-
                                            mer für die gesamte Bestellung erfasst haben, wird für alle Positionen die-
                                            selbe Nummer angezeigt.
                                        •   Teilliefertermin:
                                            Liefertermin für die Teillieferung.
                                        •   Pr./PE:
                                            EK-Preis pro Preiseinheit der bestellten Position.
                                        •   Pr./PE Gesamt:
                                            Gesamtpreis pro Preiseinheit der bestellten Position.
                                        •   Liste/Schlüssel:
                                            Preisliste und Preisschlüssel, die für den zugrundegelegten Einkaufspreis
                                            (EK) gelten.
                                        •   Rabatt:
                                            Rabatt, der auf den EK gewährt wird.
                                        •   Netto/Pos:
                                            Betrag der Position ohne Rabatt und/oder Zuschläge.
                                        •   Netto/Pos Gesamt:
                                            Betrag aller Positionen der Bestellung ohne Rabatt und/oder Zuschläge.
                                        •   Preiseinheit Anzahl:
                                            Menge in der angezeigten Preiseinheit.
                                        •   Preiseinheit:
                                            Preiseinheit für den angezeigten Preis.
                                        •   Stückpreis:
                                            Stückpreis der markierten Position inklusive aller Komponenten. Er wird
                                            über die Preiseinheit, die Zuschläge und Rabatte errechnet.
                                        •   Auftrag:
                                            Auftragsnummer.
                                        •   Bezeichnung:
                                            Produktbezeichnung aus dem referenzierten Auftrag. Sie können in der
                                            Bestellung eine abweichende Lieferantenbezeichnung angeben.
3.30 / 04-2020




                 A+W Business Einkauf                                                                           D-201
                 Bestellung (Menü)                                                                     Softwarereferenz




                                           AB-Lieferant – Positionen
                                           Dokumente > Bestellung > AB Lieferant > Register Positionen




                 Abb. D-123   AB-Lieferant – Positionen


                                           In diesem Register können Sie die gleichen Daten erfassen wie im Register
                                           Dokumente. Die erfassten Daten beziehen sich jeweils nur auf die angegebe-
                                           nen Positionen.
                                           Die Felder in diesem Register sind ausführlich zum Register Dokumente be-
                                           schrieben.
                                            “AB-Lieferant – Dokumente” auf Seite D-198

                                           Positionen von – bis Positionsnummern, zu denen Sie eine AB-Nummer
                                           und/oder einen Wareneingang verbuchen. Dabei gelten die Positionen als
                                           vollständig geliefert. Die Auftragsnummer wird in der Bestellübersicht nur für
                                           die eingetragenen Positionen angezeigt.
                                           Wenn Sie zu einzelnen Positionen Teillieferungen/-wareneingänge verbuchen
                                           wollen, müssen Sie zum Dialog Wareneingang wechseln.
                                            Tutorial, “Wareneingang erfassen” auf Seite D-127
                                            “Wareneingang (Dialog)” auf Seite D-227
3.30 / 04-2020




                 D-202                                                                           A+W Business Einkauf
                 Softwarereferenz                                                                   Bestellung (Menü)




                                           AB-Lieferant – Liefertermine ändern
                                           Dokumente > Bestellung > AB Lieferant > Register Liefertermine ändern




                 Abb. D-124   AB-Lieferant – Liefertermine ändern


                                           In diesem Register können Sie die Termine für die Lieferung durch den Liefe-
                                           ranten anpassen.
                                           Die Felder in diesem Register sind ausführlich zum Register Dokumente be-
                                           schrieben.
                                            “AB-Lieferant – Dokumente” auf Seite D-198
3.30 / 04-2020




                 A+W Business Einkauf                                                                           D-203
                 Auftragsbestätigung                                                                  Softwarereferenz




                                       Auftragsbestätigung
                                       Dokumente > Bestellung > Auftragsbestätigung > Preiskontrolle
                                       Sie können die Preise Ihrer Lieferanten prüfen, bevor Sie eine Auftragsbestä-
                                       tigung akzeptieren. Wenn ein Lieferant die vereinbarten Termine nicht einhält,
                                       können Sie eine Mahnung an ihn senden.
                                       In diesem Kapitel finden Sie Informationen zu folgenden Themen:
                                       •   “Preiskontrolle” auf Seite D-205
                                       •   “Elektronische Preiskontrolle” auf Seite D-213
                                       •   “Auswahl (Prod. Nr. für Ausgleichspos.)” auf Seite D-220
                                       •   “Einstellungen für Xternal” auf Seite D-221
                                       •   “Positionen manuell zuordnen” auf Seite D-221
                                       •   “Fußzuschläge/-rabatte verteilen” auf Seite D-222
                                       •   “Filtereinstellungen” auf Seite D-223
                                       •   “Mahnung” auf Seite D-225
3.30 / 04-2020




                 D-204                                                                       A+W Business Einkauf
                 Softwarereferenz                                                                    Auftragsbestätigung




                                        Preiskontrolle
                                        Dokumente > Bestellung > Auftragsbestätigung > Preiskontrolle
                                        Sie können die von Ihren Lieferanten bestätigten Preise prüfen und ggf. korri-
                                        gieren.
                                         Tutorial, “AB erfassen und Preise prüfen” auf Seite D-93

                                            Sammelrechnung
                                            Wenn Ihr Lieferant mehrere Bestellungen in einer Sammelbestätigung zu-
                                            sammengefasst hat, kann diese nur geprüft und akzeptiert werden, wenn
                                            in allen Bestellungen derselbe MwSt.-Satz und dieselbe Währung angege-
                                            ben sind.

                                        In diesem Kapitel finden Sie Informationen zu folgenden Themen:
                                        •   “Menü Funktionen” auf Seite D-205
                                        •   “Menü Optionen” auf Seite D-206
                                        •   “Preiskontrolle – Bestellungen” auf Seite D-207
                                        •   “Preiskontrolle – Position” auf Seite D-210
                                        •   “Preiskontrolle – Stückliste” auf Seite D-212


                                        Menü Funktionen
                                        Dokumente > Bestellung > Auftragsbestätigung > Preiskontrolle > Menü Funk-
                                        tionen
                                        Über dieses Menü können Sie andere Dialoge öffnen, ohne die Preiskontrolle
                                        zu schließen.
                                        Folgende Einträge werden angezeigt:
                                        •   Teillieferungen erstellen:
                                            Öffnet den Dialog Dokumente kopieren, um eine Teillieferung zu erfassen.
                                             Verkauf, “Dokumente kopieren” auf Seite C-532
                                        •   Anlieferpauschale einfügen:
                                            Die Lieferpauschale wird automatisch als Position im Register Positionen
                                            eingefügt. Wenn in der Bestellung bereits eine Lieferpauschale enthalten
                                            ist, wird die Option nicht ausgeführt.
                                        •   Bestellerfassung öffnen:
                                            Während der Preiskontrolle sind alle aufgelisteten Bestellungen für die Be-
                                            arbeitung (durch andere Mitarbeiter) gesperrt. Mit dieser Funktion öffnen
                                            Sie den Dialog Dokumentenverwaltung, um eine der angezeigten Bestel-
                                            lungen zu bearbeiten. Geänderte Werte werden in die Preiskontrolle über-
                                            nommen.
                                             Verkauf, “Dokument – Kopfdaten” auf Seite C-417
                                        •   Bestelldaten aktualisieren:
                                            Mit dieser Funktion werden die geänderte Werte sofort in die Bestellung
                                            zurückgeschrieben.
3.30 / 04-2020




                 A+W Business Einkauf                                                                            D-205
                 Auftragsbestätigung                                                                Softwarereferenz




                                       Menü Optionen
                                       Dokumente > Bestellung > Auftragsbestätigung > Preiskontrolle > Menü Opti-
                                       onen
                                       Über dieses Menü können Sie die Standardeinstellung des Dialoges bestim-
                                       men. Sie können die Optionen aktivieren oder deaktivieren. Die Einstellung
                                       wird nicht zurückgesetzt, wenn Sie den Dialog schließen.

                                       Gruppe Standard
                                       •   NettoMwst.:
                                           Nettobeträge werden inkl. Mwst. angezeigt.
                                       •   BruttoMwst.:
                                           Bruttobeträge werden inkl. Mwst. angezeigt.
                                       •   Netto:
                                           Nettobeträge werden ohne Mwst. angezeigt.

                                       Gruppe Verhalten
                                       •   Schnellerfassung:
                                           Mit dieser Option springt der Cursor nach der Eingabe einer Bestellnum-
                                           mer in das Feld Auftragssumme. Diese Einstellung wird benutzerbezogen
                                           gespeichert.
                                       •   Einschränkung bei Rech.dat.:
                                           Öffnet den Dialog Rechnungsdatum, um eine Abweichung in Tagen festzu-
                                           legen.
                                            “Rechnungsdatum” auf Seite D-255
                                       •   Ziel-NV füllen:
                                           Schaltet die Felder im Bereich Ziel-Nummernverwalter frei, um einen Mit-
                                           arbeiter und den zugehörigen Nummernverwalter auszuwählen.

                                       Gruppe Einstellungen
                                       •   Rabatt einfrieren:
                                           Der Rabatt wird fixiert. Diese Option sollten Sie aktivieren, wenn Sie neue
                                           Rabatte festgelegt haben, in den alten Bestellungen aber die alten Rabatte
                                           angewendet werden sollen. Die Preise werden dann nach der Preiskon-
                                           trolle nicht neu errechnet.
                                       •   Auftragskosten nicht in Statistik korrigieren:
                                           Die EK-Preise im referenzierten Auftrag werden nur korrigiert, solange der
                                           Auftrag noch in der Hauptdatenbank vorhanden ist und nicht an die Statistik
                                           übergeben wurde.
                                       •   Hinweis auf Lieferterminüberschreitung:
                                           Wenn der bestätigte Liefertermin später als der gewünschte Liefertermin
                                           der Bestellung ist, wird eine Meldung angezeigt.
3.30 / 04-2020




                 D-206                                                                        A+W Business Einkauf
                 Softwarereferenz                                                                        Auftragsbestätigung




                                            Gruppe Xternal
                                            •   Xternal-XML-Datei erstellen:
                                                Diese Option ist nur kundenspezifisch aktiviert.
                                            •   Einstellungen für Xternal:
                                                Öffnet den Dialog Einstellungen, um Vorgaben für den XML-Export festzu-
                                                legen. Diese Funktion ist nur freigeschaltet, wenn die Option Xternal-XML-
                                                Datei erstellen aktiviert ist.


                                            Preiskontrolle – Bestellungen
                                            Dokumente > Bestellung > Auftragsbestätigung > Preiskontrolle > Register
                                            Bestellungen




                 Abb. D-125   Preiskontrolle – Bestellungen


                                            In diesem Register wählen Sie eine Bestellung aus, um die Preise der Auf-
                                            tragsbestätigung zu prüfen. Die Daten werden erst angezeigt, wenn die Felder
                                            zur Bestellnummer oder zum Nummernverwalter im Bereich Bestelldaten ge-
                                            füllt sind und der Cursor in einem anderen Feld steht.
                                             Tutorial, “AB erfassen und Preise prüfen” auf Seite D-93

                                            AB-Daten

                                            AB-Nummer Pflichtfeld. Sie müssen die Nummer der Auftragsbestätigung
                                            des Lieferanten eingeben.
3.30 / 04-2020




                 A+W Business Einkauf                                                                                D-207
                 Auftragsbestätigung                                                              Softwarereferenz




                                       Bestätigter Anliefertermin Pflichtfeld. Termin, der auf der Auftragsbestäti-
                                       gung angegeben ist. Sie können das Datum über den Kalender auswählen
                                       oder manuell eingeben.

                                       Bestelldaten
                                       Mit der Wahl der Option werden die zugehörigen Felder freigeschaltet, um die
                                       Bestellung(en) auszuwählen, zu denen die Preise geprüft werden sollen.
                                       •   Bestellnummer, bis:
                                           Wenn Sie in beiden Feldern dieselbe Nummer eintragen, wird nur diese
                                           eine Bestellung eingelesen. Wenn zu einer Auftragsbestätigung mehrere
                                           Bestellungen gehören, können Sie nacheinander mehrere Bestellnum-
                                           mern eingeben und in die Übersicht übernehmen. Dazu müssen alle Be-
                                           stellungen zum selben Lieferanten gehören und denselben MwSt.-Satz
                                           haben.
                                       •   Nummernverwalter:
                                           Wenn Sie einen Nummernverwalter ausgewählt haben, werden im Bereich
                                           Bestellungen alle Bestellungen aufgelistet, die in diesem Nummernverwal-
                                           ter stehen.

                                       Summen
                                       Erst wenn Sie den Betrag aus der Auftragsbestätigung des Lieferanten einge-
                                       geben und mit [Ausführen] bestätigt haben, können Sie zu einem der anderen
                                       Register wechseln.

                                       AB-Summe/Mwst. Pflichtfeld. Gesamtbetrag der bestätigten Lieferung und
                                       der Mehrwertsteuer. Der Betrag der Mehrwertsteuer wird nicht angezeigt,
                                       wenn der Modus Netto ausgewählt ist.

                                       Modus Mit der Wahl des Modus wird die Mehrwertsteuer angezeigt oder
                                       ausgeblendet. Den Standard-Modus können Sie im Menü Optionen > Gruppe
                                       Standard festlegen.
                                       • Netto mit Mwst.:
                                          Der Gesamtbetrag wird als Nettobetrag gewertet, der Betrag der Mehrwert-
                                          steuer wird angezeigt.
                                       • Brutto mit Mwst.:
                                          Der Gesamtbetrag wird als Bruttobetrag gewertet, der Betrag der Mehr-
                                          wertsteuer wird angezeigt.
                                       • Netto:
                                          Der Gesamtbetrag wird als Nettobetrag gewertet, der Betrag der Mehrwert-
                                          steuer wird nicht angezeigt.

                                       Währung Auswahl der Währung, wenn Sie mit mehreren Währungen arbei-
                                       ten.
                                       In der Kombobox werden alle Währungen zur Auswahl angeboten, die in den
                                       Stammdaten hinterlegt sind. Mit der Auswahl einer anderen Währung als Euro
                                       werden in der Übersicht die Beträge für die Aufträge und die Mehrwertsteuer
                                       zusätzlich in der gewählten Währung angezeigt.
3.30 / 04-2020




                                        Stammdaten, “Währungen” auf Seite B-457




                 D-208                                                                      A+W Business Einkauf
                 Softwarereferenz                                                                   Auftragsbestätigung




                                        Kurs Wenn Sie mit mehreren Währungen arbeiten, wird der Wechselkurs
                                        angezeigt, der in den Stammdaten hinterlegt ist. Er kann überschrieben wer-
                                        den. Wenn Sie nur mit Euro arbeiten, muss in diesem Feld 1 stehen.

                                           Wechselkurs fixieren
                                           Sie können pro Bestellung einen abweichenden Wechselkurs vereinbaren.
                                           Dieser wird automatisch zur Berechnung in der Preiskontrolle herangezo-
                                           gen. Sie können ihn nur überschreiben, wenn er in der Bestellung nicht fi-
                                           xiert ist.

                                            Verkauf, “Kurs fixiert für Rechnungsdruck” auf Seite C-432

                                        Ziel-Nummernverwalter
                                        Diese beiden Felder sind nur freigeschaltet, wenn die Option Ziel-NV füllen ak-
                                        tiviert ist.
                                         “Menü Optionen” auf Seite D-206

                                        Mitarbeiter Name des Mitarbeiters, dem der Ziel-Nummernverwalter zuge-
                                        ordnet ist.

                                        Nummernverwalter Nummernverwalter, in den die Bestellungen nach der
                                        Prüfung gestellt werden sollen.

                                        Bestellungen
                                        In der Übersicht werden alle Bestellungen angezeigt, die sich im Nummern-
                                        verwalter befinden. Wenn Sie im Bereich Bestelldaten über die Bestellnum-
                                        mern gefiltert haben, werden nur die entsprechenden Bestellungen angezeigt.
                                        Die Spalten mit den Beträgen der Mehrwertsteuer und der Fremdwährung
                                        werden nur angezeigt, wenn ein Modus mit Mehrwertsteuer und/oder eine
                                        Fremdwährung ausgewählt ist.

                                        Summe Anzeige der Gesamtsumme und der Mehrwertsteuer der aufgeliste-
                                        ten Bestellungen.

                                        Zugrundeliegender Mwst-Satz Anzeige des Mehrwertsteuersatzes aus der
                                        Bestellung.
                                         Verkauf, “Steuersatz” auf Seite C-521
3.30 / 04-2020




                 A+W Business Einkauf                                                                           D-209
                 Auftragsbestätigung                                                                      Softwarereferenz




                                            Preiskontrolle – Position
                                            Dokumente > Bestellung > Auftragsbestätigung > Preiskontrolle > Register
                                            Position




                 Abb. D-126   Preiskontrolle – Position


                                            In diesem Register werden die Preise der Bestellpositionen angezeigt.
                                            Das Register wird nur angezeigt, wenn im Register Bestellungen die Pflichtfel-
                                            der gefüllt sind und mit [Ausführen] bestätigt wurden.
                                             Tutorial, “AB erfassen und Preise prüfen” auf Seite D-93

                                            Bestellpositionen
                                            In der Übersicht werden alle Positionen der Bestellung aufgeführt, zu der Sie
                                            die Preise und die Rechnungssumme kontrollieren.
                                            •   Bestell-Nr.:
                                                Nummer, mit der die Bestellung in der Datenbank gespeichert ist.
                                            •   Pos:
                                                Nummer der Bestellposition
                                            •   Artikel:
                                                Bezeichnung der bestellten Position
                                            •   Breite / Höhe:
                                                Maße der bestellten Position
3.30 / 04-2020




                 D-210                                                                               A+W Business Einkauf
                 Softwarereferenz                                                                 Auftragsbestätigung




                                        •   Euro-Netto:
                                            Preis der Position in der Landeswährung (hier Euro).
                                            Wenn Sie mit einer anderen Währung arbeiten, ändert sich die Bezeich-
                                            nung entsprechend. Wenn Sie mit zwei Währungen arbeiten, wird für die
                                            zweite Währung eine weitere Spalte mit dem entsprechenden Betrag an-
                                            gezeigt.
                                        •   Mwst.-Euro:
                                            Betrag der Mehrwertsteuer in der Landeswährung (hier Euro). Die Spalte
                                            wird nicht angezeigt, wenn im Register Bestellungen die Option Netto ge-
                                            wählt ist.
                                            Für die Anzeige der Mehrwert-Steuer im Mehrwährungssystem gilt das
                                            gleiche wie für die Anzeige des Betrags.
                                        •   Stückl.genaue Eingabe:
                                            In dieser Spalte wird angezeigt, ob Sie Preisdifferenzen auf der Ebene der
                                            Stücklisten-Komponenten oder der Positionen korrigiert haben.
                                            – Deaktiv:
                                                Der Preis wurde nicht geändert oder der Preis der gesamten Position
                                                wurde geändert.
                                            – Aktiv:
                                                Der Preis wurde an einer Stücklisten-Komponente geändert.
                                        •   Lieferant:
                                            Nummer und Name des Lieferanten.
                                        •   Menge:
                                            Bestellte Menge
                                        •   Kundenliefertermin:
                                            Datum der Anlieferung beim Kunden.
                                        •   Auftr.Nr.:
                                            Nummer des referenzierten Auftrags.

                                        Gesamtbetrag Anzeige der Summe der (eingegebenen) Positionsbeträge.

                                        Gesamtmenge Summe der Positionsmengen.

                                        Differenz Anzeige der Differenz zwischen der Rechnungssumme im Regis-
                                        ter Bestellungen und der Summe der (eingegebenen) Positionsbeträge. In
                                        diesem Fall kann der Preis nicht bestätigt werden, bevor Sie die Preise der Po-
                                        sitionen oder der Stücklisten geändert haben.

                                            Differenz
                                            Eine Differenz wird auch angezeigt, wenn Sie im Register Bestellungen
                                            versehentlich eine falsche AB-Summe eingetragen haben oder der Wech-
                                            selkurs nicht korrekt ist.
3.30 / 04-2020




                 A+W Business Einkauf                                                                           D-211
                 Auftragsbestätigung                                                                      Softwarereferenz




                                            Preiskontrolle – Stückliste
                                            Dokumente > Bestellung > Auftragsbestätigung > Preiskontrolle > Register
                                            Stückliste




                 Abb. D-127   Preiskontrolle – Stückliste


                                            In diesem Register können Sie sich den Preis einer Position auf der Ebene der
                                            Stückliste und der Stücklisten-Komponenten anzeigen lassen. Das Register
                                            ist nur aktiv, wenn im Register Positionen eine Position mit Stückliste markiert
                                            ist.
                                             Tutorial, “AB erfassen und Preise prüfen” auf Seite D-93

                                            Stücklistenaufbau
                                            In diesem Feld wird die Stückliste der Position angezeigt, die im Register Po-
                                            sitionen markiert ist.

                                            Preise
                                            Die Anzeige der Felder hängt davon ab, welche Stücklisten-Komponente mar-
                                            kiert ist.
                                            Sie können die Preise auf der Hauptebene oder an den Stücklisten-Kompo-
                                            nenten korrigieren.
                                            Sie können die Austauschzuschläge und Preise der einzelnen Komponenten
                                            ändern.
3.30 / 04-2020




                                            Preis / PE Anzeige des Preises und der Preiseinheit aus der Bestellung.




                 D-212                                                                               A+W Business Einkauf
                 Softwarereferenz                                                                Auftragsbestätigung




                                        Rabatt Anzeige des Rabattes aus der Bestellung. Der Wert kann nicht geän-
                                        dert werden.

                                        Netto / Positionsmenge Anzeige des Preises und der Menge aus der Be-
                                        stellung, wenn die Hauptposition markiert ist. Der Wert kann nicht geändert
                                        werden.

                                        Netto / Stücklistenmenge Anzeige des Preises und der Menge aus der Be-
                                        stellung, wenn eine Komponente markiert ist. Der Wert kann nicht geändert
                                        werden.

                                        Netto ges. Anzeige des Positions-Preises aus der Bestellung, wenn die
                                        Hauptposition markiert ist. Der Wert kann geändert werden.

                                        Netto ges. / Pos. Menge Anzeige des Komponenten-Preises und der Men-
                                        ge, wenn eine Komponente markiert ist. Der Wert kann geändert werden.

                                        Gesamtsumme Anzeige des Komponenten-Preises pro Position, wenn eine
                                        Komponente markiert ist. Der Wert kann geändert werden.


                                        Elektronische Preiskontrolle
                                        Dokumente > Bestellung > Auftragsbestätigung > Elektr. Preiskontrolle
                                        Wenn Sie Auftragsbestätigungen Ihrer Lieferanten elektronisch (openTRANS-
                                        Format) erhalten, können Sie die Zuordnung der Positionen zu Ihren Bestel-
                                        lungen, die Preise und Termine prüfen. Dazu steht Ihnen der Dialog Auftrags-
                                        bestätigung - Elektr. Preiskontrolle zur Verfügung.
                                        In diesem Kapitel finden Sie Informationen zu folgenden Themen:
                                        •   “Menü Funktionen” auf Seite D-214
                                        •   “Menü Optionen” auf Seite D-214
                                        •   “Elektronische Preiskontrolle – Dokumentenimport” auf Seite D-216
                                        •   “Elektronische Preiskontrolle – Positionsübersicht” auf Seite D-219
3.30 / 04-2020




                 A+W Business Einkauf                                                                         D-213
                 Auftragsbestätigung                                                                  Softwarereferenz




                                       Menü Funktionen
                                       Dokumente > Bestellung > Auftragsbestätigung > Elektr. Preiskontrolle >
                                       Menü Funktionen
                                       Über dieses Menü können Sie andere Dialoge öffnen, ohne die elektronische
                                       Preiskontrolle zu schließen.
                                       Folgende Einträge werden angezeigt:
                                       •   Anlieferpauschale einfügen:
                                           Die Lieferpauschale wird automatisch als Position im Register Positionen
                                           eingefügt. Wenn in der Bestellung bereits eine Lieferpauschale enthalten
                                           ist, wird die Option nicht ausgeführt.
                                       •   Bestellerfassung öffnen:
                                           Während der Preiskontrolle sind alle aufgelisteten Bestellungen für die Be-
                                           arbeitung (durch andere Mitarbeiter) gesperrt. Mit dieser Funktion können
                                           Sie den Dialog Dokumentenverwaltung öffnen, um eine der angezeigten
                                           Bestellungen zu bearbeiten. Geänderte Werte werden in die Preiskontrolle
                                           übernommen.
                                            Verkauf, “Dokument – Kopfdaten” auf Seite C-417
                                       •   Positionen manuell zuordnen:
                                           Öffnet den Dialog Positionen manuell zuordnen, um Positionen des elektr.
                                           Dokuments den entsprechenden Positionen der Bestellung(en) zuzuord-
                                           nen.
                                            “Positionen manuell zuordnen” auf Seite D-221
                                       •   Fußzuschläge/-rabatte auf Bestellungen verteilen:
                                           Öffnet den Dialog Fußzuschläge/-rabatte auf Bestellungen verteilen, um
                                           den Zuschlag/Rabatt aus dem elektr. Dokument auf die zugeordneten Be-
                                           stellungen zu verteilen.
                                            “Fußzuschläge/-rabatte verteilen” auf Seite D-222
                                       •   Manuelle Positionszuordnung aufheben:
                                           Hebt die manuelle Zuordnung der markierten Rechnungs-/Bestellpositio-
                                           nen wieder auf.
                                       •   Alle Positionszuordnungen aufheben:
                                           Hebt alle manuellen Zuordnungen von Rechnungs- und Bestellpositionen
                                           wieder auf.


                                       Menü Optionen
                                       Dokumente > Bestellung > Auftragsbestätigung > Elektr. Preiskontrolle >
                                       Menü Optionen
                                       Über dieses Menü können Sie die Standardeinstellung des Dialoges bestim-
                                       men. Sie können die Optionen aktivieren oder deaktivieren. Die Einstellung
                                       wird nicht zurückgesetzt, wenn Sie den Dialog schließen.
3.30 / 04-2020




                 D-214                                                                           A+W Business Einkauf
                 Softwarereferenz                                                                    Auftragsbestätigung




                                        Gruppe Allgemein
                                        •   Betragsdifferenzen akzeptieren:
                                            Bei der elektronischen Preiskontrolle können Betragsdifferenzen, die
                                            durch Rundungen auftreten können, generell akzeptiert werden.
                                        •   Hinweis auf Betragsdiff./Ausgl.pos.:
                                            Wenn Rundungsdifferenzen automatisch einer Ausgleichsposition zuge-
                                            ordnet wurden, wird ein Hinweis angezeigt.
                                        •   Rabatt einfrieren:
                                            Mit dieser Option wird der Rabatt fixiert. Diese Option sollten Sie aktivieren,
                                            wenn Sie neue Rabatte festgelegt haben, in den alten Bestellungen aber
                                            die alten Rabatte angewendet werden sollen. Die Preise werden dann
                                            nach der Preiskontrolle nicht neu errechnet.
                                        •   Auftr.-EK nur korrigieren bis in Statistik:
                                            Die Korrekturen des EK-Preises im referenzierten Auftrag werden nur
                                            durchgeführt, solange der Auftrag noch in der Hauptdatenbank vorhanden
                                            ist und nicht an die Statistik übergeben wurde.
                                        •   Prod.Nr. für Ausgleichspos.:
                                            Öffnet den Dialog Auswahl, um eine Ausgleichposition für Rundungsdiffe-
                                            renzen auszuwählen.
                                             “Auswahl (Prod. Nr. für Ausgleichspos.)” auf Seite D-220

                                        Gruppe Einstellungen
                                        •   Hinweis auf Lieferterminüberschreitung:
                                            Bei Überschreitung des geplanten Liefertermins wird eine Meldung ange-
                                            zeigt.
                                        •   Automatische Zuordnung unterdrücken:
                                            Im Dialog Positionen manuell zuordnen können Sie die Checkbox für die
                                            automatische Zuordnung aktivieren, damit die Fußzuschläge-/rabatte der
                                            Auftragsbestätigung automatisch einem A+W Business-Produkt zugeord-
                                            net werden. Diese automatische Zuordnung können Sie unterdrücken.
                                             “Zuordnung des Fußzuschlags/-rabatts zukünftig automatisch auflösen” auf
                                              Seite D-222
                                            Wenn diese Option geändert wurde, muss das aktuell eingelesene Doku-
                                            ment nochmals eingelesen werden.
                                             Tutorial, “So lesen Sie ein openTRANS-Dokument ein” auf Seite D-169
                                        •   Referenzierenden Produktnummern des Lieferanten vertrauen:
                                            Wenn im importierten Dokument eine A+W Business-Produktnummer als
                                            Referenz angegeben ist, kann die Zuordnung automatisch durchgeführt
                                            werden.

                                        Gruppe Xternal
                                        •   Xternal-XML-Datei erstellen:
                                            Diese Option ist nur kundenspezifisch aktiviert.
                                        •   Einstellungen für Xternal:
                                            Öffnet den Dialog Einstellungen, um Vorgaben für den XML-Export festzu-
3.30 / 04-2020




                                            legen. Diese Funktion ist nur freigeschaltet, wenn die Option Xternal-XML-
                                            Datei erstellen aktiviert ist.




                 A+W Business Einkauf                                                                               D-215
                 Auftragsbestätigung                                                                      Softwarereferenz




                                           Elektronische Preiskontrolle – Dokumentenimport
                                           Dokumente > Bestellung > Auftragsbestätigung > Elektr. Preiskontrolle >
                                           Register Dokumentenimport




                 Abb. D-128   Elektronische Preiskontrolle – Dokumentenimport


                                           In diesem Register prüfen Sie die importierten Auftragsbestätigungen. Nur
                                           wenn der Dokumentenstatus fehlerfrei ist, kann die Preiskontrolle erfolgreich
                                           abgeschlossen werden.
                                            Tutorial, “Elektronisches Dokument prüfen” auf Seite D-170

                                           Buchungsart
                                           Mit der Wahl der Option legen Sie fest, wie das elektronische Dokument ver-
                                           arbeitet werden soll. Die Optionen sind dem Dokumentenstatus entsprechend
                                           freigeschaltet.
                                           •   Ablehnen:
                                               Mit dieser Option werden die Dokumente nicht übernommen. Die Preiskon-
                                               trolle wird nicht durchgeführt.
                                           •   Akzeptieren:
                                               Mit dieser Option wird die Preiskontrolle bestätigt. Die AB-Nummer, Preise
                                               und Liefertermine aus dem importierten Dokument werden in die Bestellun-
                                               gen zurückgeschrieben.
                                               Die Dokumentenhistorie wird aktualisiert.
3.30 / 04-2020




                 D-216                                                                             A+W Business Einkauf
                 Softwarereferenz                                                                  Auftragsbestätigung




                                        •   Teillieferung erstellen:
                                            Zu den im Dokument enthaltenen Positionen wird eine (neue) Teillieferung
                                            erstellt und wie bei Akzeptieren verbucht. Die restlichen Positionen bleiben
                                            in der ursprünglichen Bestellung erhalten. Der Status dieser Bestellung
                                            wird entsprechend angepasst.
                                            Bei einem Lieferavis wird mit dieser Buchungsart eine Teilbestellung er-
                                            zeugt.

                                        Auftragsbestätigungen
                                        In der Übersicht sind alle importierten Auftragsbestätigungen aufgelistet. Die-
                                        se können von unterschiedlichen Lieferanten stammen.
                                        Wenn Sie einen Eintrag markieren, werden die referenzierten Dokumente in
                                        der Übersicht Bestellungen / Teillieferungen angezeigt.
                                        •   AB-Nummer:
                                            AB-Nummer, die der Lieferant angegeben hat.
                                        •   Lieferant:
                                            Name des Lieferanten.
                                        •   Lieferdatum bestätigt:
                                            Lieferdatum, das der Lieferant in der AB angegeben hat.
                                        •   Netto:
                                            Gesamtbetrag der Lieferung.
                                        •   Währung:
                                            Währung, in der der Betrag in der AB angegeben ist. Diese Anzeige ist nur
                                            dann von Bedeutung, wenn Sie mit einem Mehrwährungssystem arbeiten.

                                        Anzeige Sie können die Anzeige der Dokumente einschränken.

                                        Filtereinstellungen Sie können Filter für die Anzeige der importierten Doku-
                                        mente festlegen.
                                         “Filtereinstellungen” auf Seite D-223

                                        Dokumentenstatus
                                        Die rote oder grüne Markierung gibt an, ob Unstimmigkeiten festgestellt wur-
                                        den oder nicht. Die Optionen im Bereich Buchungsart sind entsprechend ge-
                                        sperrt oder freigeschaltet.
                                        •   Kein Dokument ausgewählt:
                                            Die Anzeige des Dokumentenstatus kann nicht aktualisiert werden, da kein
                                            Dokument in der Übersicht markiert ist. Dieser Eintrag wird nicht angezeigt,
                                            wenn eine AB markiert ist.
                                        •   Mindestens ein Fußzuschlag/-rabatt einer Bestellung konnte dem Doku-
                                            ment nicht zugeordnet werden:
                                            Dieser Eintrag wird nur angezeigt, wenn eine AB mit einem entsprechen-
                                            den Fehler markiert ist.
                                        •   Bestellungen vollständig referenziert:
                                            Bei einer roten Anzeige stimmt mindestens eine der referenzierten Positi-
3.30 / 04-2020




                                            onen nicht vollständig mit der importierten AB überein. Die unvollständig
                                            referenzierten Bestellungen werden in der Übersicht gekennzeichnet.




                 A+W Business Einkauf                                                                            D-217
                 Auftragsbestätigung                                                                  Softwarereferenz




                                       •   Fehlende Artikelpositionen in Bestellungen:
                                           In der Auftragsbestätigung sind Positionen enthalten, die in der Bestellung
                                           nicht aufgeführt sind.
                                       •   Fehlende Fußzuschläge/-rabatte in Bestellungen:
                                           Fußzuschläge/-rabatte werden nicht mitbestellt. Da sie aber in der AB auf-
                                           geführt sind, müssen sie für die Preiskontrolle als Positionen in den Bestel-
                                           lungen vorhanden sein. Die fehlenden Fußzuschläge/-rabatte müssen in
                                           der Bestellung manuell erfasst werden.
                                       •   Preisdifferenz:
                                           Die Gesamtpreise von Bestellung und AB sind unterschiedlich. In den zu-
                                           gehörigen Feldern wird die Abweichung als Betrag und prozentual ange-
                                           zeigt.
                                       •   Mengendifferenzen:
                                           Die Positionsmengen von Bestellung und AB sind unterschiedlich.

                                       [Dokument anzeigen] Öffnet die Dokumentenansicht des markierten Doku-
                                       ments.

                                       Bestellungen / Teillieferungen
                                       In der Übersicht werden die referenzierten Dokumente angezeigt, wenn Sie
                                       einen Eintrag im Bereich Auftragsbestätigungen markiert haben. Teillieferun-
                                       gen werden in blauer Schrift angezeigt.
                                       •   Bestellnummer:
                                           Nummer der Bestellung, die von A+W Business erzeugt wurde.
                                       •   Lieferdatum gewünscht:
                                           Datum aus der Lagerbestellung oder dem Kundenauftrag.
                                       •   Netto:
                                           Gesamtbetrag der Bestellung oder des Auftrags.
                                       •   Währung:
                                           Währung, in der der Betrag in der Bestellung angegeben ist. Diese Anzeige
                                           ist nur dann von Bedeutung, wenn Sie mit einem Mehrwährungssystem ar-
                                           beiten.
                                       •   Auftr.Nr.:
                                           Auftragsnummer.
                                       •   Kundenliefertermin:
                                           Datum der Anlieferung beim Kunden.
                                       •   Bemerkung:
                                           Wenn die Verknüpfung zwischen der Bestellung und dem importierten Do-
                                           kument nicht vollständig ist, wird ggf. ein Hinweis auf den Fehler angezeigt.
3.30 / 04-2020




                 D-218                                                                         A+W Business Einkauf
                 Softwarereferenz                                                                      Auftragsbestätigung




                                            Elektronische Preiskontrolle – Positionsübersicht
                                            Dokumente > Bestellung > Auftragsbestätigung > Elektr. Preiskontrolle > Re-
                                            gister Positionsübersicht




                 Abb. D-129   Elektronische Preiskontrolle – Positionsübersicht


                                            In diesem Register können Sie die Positionen der Auftragsbestätigung (AB)
                                            prüfen, die Ihr Lieferant gesendet hat. Sie können die Preise der Positionen
                                            korrigieren. Die Korrekturen werden in die referenzierten Bestellungen zurück-
                                            geschrieben.
                                            Die Optionen im Bereich Buchungsart sind zu Register Dokumentenimport er-
                                            klärt.
                                             “Elektronische Preiskontrolle – Dokumentenimport” auf Seite D-216

                                            Positionsübersicht
                                            In der Übersicht sind alle Positionen der Auftragsbestätigung aufgeführt.
                                            Wenn Sie eine Position markieren, werden die Details in den Bereichen Doku-
                                            mentenposition und Bestellposition angezeigt.
                                            •   Pos-Nr.:
                                                Positionsnummer aus der AB.
                                            •   Bestell-Nummer:
                                                Nummer der referenzierten Bestellung.
3.30 / 04-2020




                                            •   Bestell-Position:
                                                Positionsnummer aus der Bestellung.
                                            •   Netto Dokument/Netto 1 Bestellung:
                                                Positionspreis aus der importierten AB und aus der Bestellung.


                 A+W Business Einkauf                                                                              D-219
                 Auftragsbestätigung                                                                  Softwarereferenz




                                       •   Menge Dokument/Menge 1 Bestellung:
                                           Positionsmenge aus der importierten AB und aus der Bestellung.
                                       •   Abmessung Dokument/Abmessung 1 Bestellung:
                                           Positionsmaße aus der importierten AB und aus der Bestellung.
                                       •   Differenz Preis:
                                           Differenz aus Spalte Netto Dokumente und Netto Bestellung.
                                       •   Differenz 1 Preis %:
                                           Preisdifferenz in Prozent.
                                       •   Differenz 2 Menge:
                                           Differenz aus Spalte Menge Dokumente und Menge Bestellung.
                                       •   Auftr.Nr.:
                                           Auftragsnummer.
                                       •   Kundenliefertermin:
                                           Datum der Anlieferung beim Kunden.

                                       Dokumentenposition, Bestellposition
                                       In diesen beiden Bereichen werden Details zu der Position angezeigt, die in
                                       der Positionsübersicht markiert ist.


                                       Auswahl (Prod. Nr. für Ausgleichspos.)
                                       Dokumente > Bestellung > Auftragsbestätigung > Elektr. Preiskontrolle >
                                       Menü Optionen > Prod.Nr. für Ausgleichspos.
                                       Dokumente > Bestellung > Rechnung > Elektr. Rechnungskontrolle > Menü
                                       Optionen > Prod.Nr. für Ausgleichspos.




                                       Abb. D-130   Auswahl


                                       In diesem Dialog können Sie die Produktnummer eintragen, mit der Run-
                                       dungsdifferenzen verbucht werden.
                                       Der Dialog kann nur bei der elektronischen Preis-/Rechnungskontrolle geöff-
                                       net werden.
                                        Tutorial, “Betragsdifferenzen” auf Seite D-158
                                        Tutorial, “Elektronisches Dokument prüfen” auf Seite D-170

                                           Voraussetzung
                                           In der Produktverwaltung muss ein Produkt angelegt sein, auf das die Run-
3.30 / 04-2020




                                           dungsdifferenzen verbucht werden können.

                                       Artikelnummer Nummer des Produktes, auf das die Preisdifferenz verbucht
                                       werden soll.


                 D-220                                                                         A+W Business Einkauf
                 Softwarereferenz                                                                         Auftragsbestätigung




                                           Einstellungen für Xternal
                                           Diese Funktion und der Dialog sind nur kundenspezifisch freigeschaltet.
                                           Während der Rechnungskontrolle kann eine XML-Datei zur Schnittstelle Xter-
                                           nal gesendet werden. Darin enthalten ist ein Auszug aus den Kopf- und Posi-
                                           tionsdaten der vorliegenden Bestellungen.


                                           Positionen manuell zuordnen
                                           Dokumente > Bestellung > Auftragsbestätigung > Elektr. Preiskontrolle >
                                           Menü Funktionen > Positionen manuell zuordnen
                                           Dokumente > Bestellung > Rechnung > Elektr. Rechnungskontrolle > Menü
                                           Funktionen > Positionen manuell zuordnen




                 Abb. D-131   Positionen in der elektr. Preis- oder Rechnungskontrolle manuell zuordnen


                                           In diesem Dialog ordnen Sie die Positionen des importierten Dokuments den
                                           Positionen der Bestellung(en) zu. Diesen Dialog können Sie nur öffnen, wenn
                                           Sie die automatische Zuordnung im Menü Funktionen deaktiviert haben.
                                            “Menü Funktionen” auf Seite D-214
                                            Tutorial, “Positionen im elektronischen Dokument zuordnen” auf Seite D-173

                                           Dokumenten-Positionen, Bestell-Positionen
                                           In diesen beiden Bereichen werden die Positionen aus dem importierten Do-
                                           kument und der zugehörigen Bestellung aufgelistet. Um die Positionen einan-
                                           der zuzuordnen, markieren Sie jeweils die entsprechenden Einträge und
                                           bestätigen die Zuordnung mit [OK]. Die zugeordneten Positionen werden da-
                                           nach nicht mehr angezeigt.
3.30 / 04-2020




                                           Die Zuordnungen können Sie aufheben, wenn Sie im Menü Funktionen den
                                           Eintrag Alle Positionszuordnungen aufheben wählen.
                                            “Menü Funktionen” auf Seite D-214



                 A+W Business Einkauf                                                                                 D-221
                 Auftragsbestätigung                                                                 Softwarereferenz




                                       Produktzuordnung des Fußzuschlages/-rabatts merken Die Checkbox
                                       ist nur freigeschaltet, wenn Sie einen Fußzuschlag/-rabatt zugeordnet haben.
                                       Sie können diese Zuordnung für die aktuelle Sitzung speichern. Die Speiche-
                                       rung gilt nicht, wenn Sie den Dokumentenimport erneut starten.
                                       ☐ Die Zuordnung gilt nur für dieses eine Dokument und die zugehörigen Be-
                                       stellungen.
                                       ☑ Die Zuordnung gilt für alle weiteren Dokumente, die der Importfilter ausge-
                                       wählt hat.

                                       Zuordnung des Fußzuschlags/-rabatts zukünftig automatisch auflösen
                                       Die Checkbox ist nur freigeschaltet, wenn die Checkbox Produktzuordnung
                                       des Fußzuschlages/-rabatts merken markiert ist.
                                       Wenn Sie einen Fußzuschlag/-rabatt zugeordnet haben, können Sie diese Zu-
                                       ordnung für alle künftigen Importe speichern.
                                       ☐ Die Zuordnung gilt nur für dieses eine Dokument und die zugehörigen Be-
                                       stellungen.
                                       ☑ Die Zuordnung wird für alle weiteren importierten Dokumente des Lieferan-
                                       ten automatisch durchgeführt.


                                       Fußzuschläge/-rabatte verteilen
                                       Dokumente > Bestellung > Auftragsbestätigung > Elektr. Preiskontrolle >
                                       Menü Funktionen > Fußzuschläge/-rabatte auf Bestellungen verteilen
                                       Dokumente > Bestellung > Rechnung > Elektr. Rechnungskontrolle > Menü
                                       Funktionen > Fußzuschläge/-rabatte auf Bestellungen verteilen




                                       Abb. D-132   Fußzuschläge/-rabatte auf Bestellungen verteilen


                                       In diesem Dialog können Sie den Fußzuschlag/-rabatt in einem elektronischen
                                       Dokument mehreren Bestellungen zuordnen.
                                       In der Übersicht werden alle Bestellpositionen aufgelistet, die zu dem impor-
                                       tierten Dokument gehören.
3.30 / 04-2020




                                        Tutorial, “Fußzuschläge/-rabatte” auf Seite D-157
                                        Tutorial, “Zuschläge/Rabatte manuell zuordnen” auf Seite D-175




                 D-222                                                                         A+W Business Einkauf
                 Softwarereferenz                                                                   Auftragsbestätigung




                                        Sie können die Zuordnung über das Menü Optionen wieder auflösen.
                                         “Menü Optionen” auf Seite D-257



                                        Filtereinstellungen
                                        Dokumente > Bestellung > Auftragsbestätigung > Elektr. Preiskontrolle >
                                        Schaltfläche Filtereinstellungen
                                        Dokumente > Bestellung > Rechnung > Elektr. Rechnungskontrolle > Menü
                                        Funktionen > Schaltfläche Filtereinstellungen




                                        Abb. D-133   Filtereinstellungen für die Anzeige von importierten Dokumenten


                                        In diesem Dialog können Sie festlegen, welche Bestellungen zu importierten
                                        Dokumenten angezeigt werden sollen. Die Filter können sich auf den Erfasser
                                        und/oder auf den Lieferanten beziehen.

                                        Nach Erfasser
                                        Sie können festlegen, wessen Bestellungen zum importierten Dokument an-
                                        gezeigt werden können.

                                        Alle Sie können sich alle Bestellungen zu den importieren Dokumenten an-
                                        zeigen lassen.
                                        ☐ Die Anzeige der Bestellungen soll über die weiteren Filter eingeschränkt
                                        werden. Die Checkboxen Nur eigene und Festlegen sind freigeschaltet.
                                        ☑ Die Anzeige der Bestellungen wird nicht auf Erfasser oder Nummernverwal-
                                        ter eingeschränkt. Die Checkboxen Nur eigene und Festlegen sind gesperrt.

                                        Nur eigene Die Checkbox ist gesperrt, wenn die Checkbox Alle markiert ist.
                                        ☐ Die Anzeige wird nicht auf die eigenen Bestellungen eingeschränkt.
3.30 / 04-2020




                                        ☑ Die Anzeige wird auf die Bestellungen eingeschränkt, die Sie selbst erfasst
                                        haben. Wenn Sie zusätzlich einen Nummernverwalter auswählen, werden Ih-
                                        nen nur Ihre Bestellungen aus dem gewählten Nummernverwalter angezeigt.


                 A+W Business Einkauf                                                                              D-223
                 Auftragsbestätigung                                                                     Softwarereferenz




                                       Festlegen Die Checkbox ist gesperrt, wenn die Checkbox Alle markiert ist.
                                       ☐ Die Anzeige der Bestellungen wird nicht auf einen Nummernverwalter ein-
                                       geschränkt.
                                       ☑ Nur die Bestellungen aus dem angezeigten Nummernverwalter werden an-
                                       gezeigt. Wenn Sie zusätzlich die Checkbox Nur eigene markiert haben, wer-
                                       den Ihnen nur Ihre Bestellungen aus dem gewählten Nummernverwalter
                                       angezeigt.

                                       Nach Lieferanten
                                       Sie können die Anzeige der Bestellungen auf einen oder mehrere Lieferanten
                                       einschränken.

                                       Lieferant Sie können einen oder mehrere Lieferanten auswählen.

                                       Schaltflächen Mit den Schaltflächen übernehmen Sie den gewählten Liefe-
                                       ranten in die Übersicht oder entfernen einen Eintrag aus ihr.
                                        Tutorial, “Schaltflächen in Suchdialogen” auf Seite C-42

                                       Übersicht
                                       In der Übersicht werden alle Lieferanten angezeigt, die als Filter für die Anzei-
                                       ge von Bestellungen gelten.

                                          Einstellungen speichern
                                          Beim Verlassen werden die Einstellungen gespeichert und gelten so lange,
                                          bis sie geändert oder zurückgesetzt werden.
3.30 / 04-2020




                 D-224                                                                              A+W Business Einkauf
                 Softwarereferenz                                                               Auftragsbestätigung




                                        Mahnung
                                        Dokumente > Bestellung > Auftragsbestätigung > Mahnung




                                        Abb. D-134   Lieferanten mahnen


                                        In diesem Dialog können Sie nach offenen Bestellungen suchen, deren Liefe-
                                        rung überfällig ist. Die Suche kann durch ein Datum, auf bestimmte Lieferan-
                                        ten und/oder Nummernverwalter eingeschränkt werden.
                                         Tutorial, “Lieferanten anmahnen” auf Seite D-97

                                        Menü Funktionen
                                        •   Mahnkennzeichen löschen:
                                            Löscht das Mahnkennzeichen aus den angezeigten Bestellungen.

                                        Auswahl

                                        Lieferant von, bis Einschränkung der Suche auf einen Lieferanten oder
                                        eine Folge von Lieferanten.

                                        Nummernverwalter Anzeige der Bestellungen in einem Nummernverwalter.

                                        Mindeststatus, Status kleiner Einschränkung der Suche auf Bestellungen,
                                        die in einem bestimmten Statusbereich liegen.

                                        Optionen

                                        Bis Erfassungsdatum Angabe des Erfassungsdatums, zu dem nach offe-
3.30 / 04-2020




                                        nen Bestellungen gesucht werden soll. Standardmäßig ist das aktuelle Tages-
                                        datum ausgewählt. Mit dieser Einstellung werden ggf. auch Bestellungen
                                        angezeigt, die noch gar nicht geliefert sein können.



                 A+W Business Einkauf                                                                        D-225
                 Auftragsbestätigung                                                                 Softwarereferenz




                                       Bereits gemahnte Lieferanten nochmals mahnen Wenn Sie eine Liefe-
                                       rung angemahnt haben, wird an der betreffenden Bestellung ein Mahnkenn-
                                       zeichen gesetzt.
                                       ☐ Bereits angemahnte Bestellungen werden nicht angezeigt.
                                       ☑ Offene Bestellungen werden auch dann angezeigt, wenn sie bereits ange-
                                       mahnt wurden. Sie können erneut angemahnt werden.

                                       Faxversand/Postversand/Alle Die Suche kann zusätzlich auf Bestellungen
                                       eingeschränkt werden, die als Fax oder als Post versendet wurde. Als Post-
                                       versand gilt auch, wenn Sie eine PDF-Datei als Anhang einer E-Mail gesendet
                                       haben.
                                       Wenn Sie die Suche nicht einschränken wollen, wählen Sie die Option Alle.
                                       Die Mahnungen werden auf dem Weg versendet, der für den entsprechenden
                                       Lieferanten als Standard für Bestellungen festgelegt ist.

                                       Tabelle
                                       In der Übersicht werden alle Lieferanten aufgeführt, zu denen offene Bestel-
                                       lungen vorliegen, die den Filterkriterien entsprechen. In roter Schrift sind die
                                       Lieferanten angezeigt, an die bereits eine Mahnung geschickt wurde.
                                       •   Bestellnummer:
                                           Nummer der offenen Bestellung.
                                       •   Stat.:
                                           Status der offenen Bestellung.
                                       •   Lieferant:
                                           Lieferant, an den die Bestellung gesendet wurde.
                                       •   Erfassungsdatum:
                                           Erfassungsdatum der Bestellung.
                                       •   Liefertermin:
                                           Geplanter und/oder bestätigter Liefertermin aus der Bestellung.
3.30 / 04-2020




                 D-226                                                                         A+W Business Einkauf
                 Softwarereferenz                                                                       Wareneingang




                                        Wareneingang
                                        Dokumente > Bestellung > Wareneingang > Wareneingang
                                        Sie können den Wareneingang und die Auftragsbestätigung vom Lieferanten
                                        erfassen sowie die gelieferten Positionen prüfen und ggf. korrigieren.
                                        In diesem Kapitel finden Sie Informationen zu folgenden Themen:
                                        •   “Wareneingang (Dialog)” auf Seite D-227
                                        •   “Eingangskontrolle” auf Seite D-241


                                        Wareneingang (Dialog)
                                        Dokumente > Bestellung > Wareneingang > Wareneingang
                                        In diesem Dialog können Sie den Wareneingang zu einzelnen Bestellungen
                                        oder zu den Bestellungen in einem Nummernverwalter erfassen.
                                        Für die jeweilige Bestandsbuchung können Sie Vorgaben für die Identifikati-
                                        onsnummern (ID) festlegen, die automatisch vergeben wird, wenn in der La-
                                        gerbestellung Positionen mit einer Menge größer als 1 erfasst sind. Die
                                        Identnummern werden für Kisten und Gläser (Lagerplatten) vergeben.

                                            Voraussetzung
                                            In den Firmendaten muss die Checkbox für die virtuelle Vergabe von Posi-
                                            tionsnummern markiert sein.

                                             Stammdaten, “Virtuelle Positionsnummern verwenden” auf Seite B-943
                                        In diesem Kapitel finden Sie Informationen zu folgenden Themen:
                                        •   “Menü Funktionen” auf Seite D-228
                                        •   “Menü Optionen” auf Seite D-228
                                        •   “Menü Druck” auf Seite D-229
                                        •   “Wareneingang – Auswahl” auf Seite D-230
                                        •   “Wareneingang – Komplett” auf Seite D-232
                                        •   “Wareneingang – Positionsweise” auf Seite D-234
                                        •   “Wareneingang – Identnummer” auf Seite D-237
                                        •   “Wareneingang – Protokoll (Identnummern)” auf Seite D-239
3.30 / 04-2020




                 A+W Business Einkauf                                                                              D-227
                 Wareneingang                                                                 Softwarereferenz




                                Menü Funktionen
                                Dokumente > Bestellung > Wareneingang > Wareneingang > Menü Funktio-
                                nen
                                Über dieses Menü können Sie andere Dialoge öffnen, ohne den Warenein-
                                gang zu schließen.
                                Folgende Einträge werden angezeigt:
                                •   Dokument anzeigen:
                                    Öffnet den Dialog Dokumentenansicht zu einer Vorschau auf den Druck.
                                     Verkauf, “Reklamationen” auf Seite C-591
                                •   Dokumentendaten:
                                    Öffnet den Dialog Dokumentendaten, um ggf. die Termine und den Status
                                    zu korrigieren.
                                     Verkauf, “Dokumentendaten” auf Seite C-738
                                •   Lagersuche:
                                    Öffnet den Dialog Lagerinfo, um die aktuellen Lagerbestände anzuzeigen.
                                     Verkauf, “Lagerinfo” auf Seite C-741
                                •   Artikel Info:
                                    Öffnet einen Dialog Artikelinfo, um Detailinformationen zum aktuellen Pro-
                                    dukt zu erhalten.
                                     Verkauf, “Artikel-Informationen” auf Seite C-602


                                Menü Optionen
                                Dokumente > Bestellung > Wareneingang > Wareneingang > Menü Optionen
                                Über dieses Menü können Sie die Standardeinstellung des Dialoges bestim-
                                men. Sie können die Optionen aktivieren oder deaktivieren. Die Einstellung
                                wird nicht zurückgesetzt, wenn Sie den Dialog schließen.
                                Folgende Einträge werden angezeigt:
                                •   Positionsansicht bei Auswahl von einzelnem Dokument:
                                    Mit dieser Option wechselt die Ansicht zum Register Positionsweise, wenn
                                    Sie sich ein einzelnes Dokument anzeigen lassen.
                                •   Identnummernvergabe:
                                    Diese Einstellung wird für den Wareneingang von Kisten und Lagerplatten
                                    benötigt.
                                    – Automatische Vergabe:
                                       Mit dieser Option wird die ID automatisch vergeben. Dazu kann eine
                                       Vorgabe festgelegt werden. Wenn die Option nicht aktiviert ist, müssen
                                       Sie die ID manuell eingeben.
                                    – Einstellungen:
                                       Öffnet den Dialog Einstellungen, in dem Sie die Vorgabe für die auto-
                                       matische Vergabe von IDs festlegen.
                                        “Einstellungen (ID)” auf Seite D-240
                                •   Lagerort für Identnummern aus Position vorblenden:
3.30 / 04-2020




                                    Mit dieser Option wird der Lagerort vorgeschlagen, der in der zuvor ver-
                                    buchten Position angegeben war.




                 D-228                                                                   A+W Business Einkauf
                 Softwarereferenz                                                                       Wareneingang




                                        •   Lagerbuchungsdatum = Lieferdatum:
                                            Als Buchungsdatum wird automatisch das Lieferdatum aus der Bestellung
                                            übernommen. Wenn die Option deaktiviert ist, wird standardmäßig das Ta-
                                            gesdatum übernommen.
                                        •   AB-Nummer prüfen:
                                            Mit dieser Einstellung wird eine Meldung angezeigt, wenn die Nummer der
                                            Auftragsbestätigung durch den Lieferanten nicht eingegeben ist.


                                        Menü Druck
                                        Dokumente > Bestellung > Wareneingang > Wareneingang > Menü Druck
                                        Über dieses Menü können Sie die Druckfunktionen starten.
                                        Folgende Einträge werden angezeigt:
                                        •   Wareneingang:
                                            Startet den Druck einer Liste mit allen Bestellungen und referenzierten Auf-
                                            trägen, die im Dialog aufgeführt sind.
                                        •   Etiketten:
                                            Startet den Druck von Kistenetiketten.
                                        •   Protokoll:
                                            Startet den Druck eines Protokolls mit allen Kistenpositionen und den ver-
                                            gebenen Kisten-IDs.
                                        •   Etiketten und Protokoll (nur Gruppe Drucker):
                                            Startet den Druck der Kistenetiketten und eines Protokolls mit den verge-
                                            benen Kisten-IDs.
                                        •   Einstellungen:
                                            Öffnet die Druckereinstellungen.
3.30 / 04-2020




                 A+W Business Einkauf                                                                           D-229
                 Wareneingang                                                                         Softwarereferenz




                                          Wareneingang – Auswahl
                                          Dokumente > Bestellung > Wareneingang > Wareneingang > Register Aus-
                                          wahl




                 Abb. D-135   Wareneingang – Auswahl


                                          In diesem Register können Sie die Auswahl und Anzeige der Dokumente fil-
                                          tern, zu denen Sie Wareneingänge prüfen und/oder erfassen möchten.
                                           Tutorial, “Wareneingang” auf Seite D-120

                                          Auswahl
                                          Mit der Wahl der Option legen Sie fest, wie die Bestellungen gefiltert werden.
                                          Die offenen Bestellungen werden nach der Suche im Register Komplett ange-
                                          zeigt, damit die Wareneingänge verbucht werden können.
                                          •   Nach Bestellnummer:
                                              Das Eingabefeld für die Bestellnummer wird freigeschaltet. Im Register
                                              Komplett werden die gesuchte Bestellung und alle referenzierten Aufträge
                                              angezeigt.
                                          •   Nach Auftragsnummer:
                                              Das Eingabefeld für die Auftragsnummer wird freigeschaltet. Im Register
                                              Komplett werden alle Bestellungen angezeigt, die zur eingetragenen Auf-
                                              tragsnummer erzeugt wurden.
3.30 / 04-2020




                 D-230                                                                          A+W Business Einkauf
                 Softwarereferenz                                                                      Wareneingang




                                        •   Nach Lieferanten:
                                            Das Eingabefeld für die Lieferantennummer wird freigeschaltet. Im Regis-
                                            ter Komplett werden alle Bestellungen beim gewählten Lieferanten ange-
                                            zeigt.
                                        •   Nach Lieferscheinnummer / Lieferavis, Gesamtliefermenge:
                                            Das Eingabefeld für die Nummer des Lieferscheins oder des Lieferavis und
                                            das Feld für die Gesamtmenge werden freigeschaltet. Wurde ein Lieferavis
                                            importiert, müssen die tatsächlich gelieferten Mengen eingetragen werden.
                                        •   Nach Anliefertermin des Lieferanten:
                                            Das Eingabefeld für den Liefertermin wird freigeschaltet. Im Register Kom-
                                            plett werden alle Bestellungen angezeigt, die zum gewählten Termin ange-
                                            liefert werden sollen.
                                        •   Nach Nummernverwalter:
                                            Die Kombobox zur Auswahl des Nummernverwalters wird freigeschaltet.
                                            Im Register Komplett werden alle Bestellungen im gewählten Nummern-
                                            verwalter angezeigt.
                                        •   Nach Scanner / Dokument:
                                            Die Felder für den Barcode der Bestellnummer oder einer Bestellposition
                                            werden freigeschaltet.

                                        Ziel-Nummernverwalter

                                        Ziel-Nummernverwalter Die Lagerbestellungen können nach dem Buchen
                                        des Wareneingangs automatisch in einen anderen Nummernverwalter gestellt
                                        werden.
                                        ☐ Die Lagerbestellungen werden nicht in einen anderen Nummernverwalter
                                        gestellt.
                                        ☑ Die Felder im Bereich Ziel-Nummernverwalter werden freigeschaltet. Die
                                        Lagerbestellungen werden in den gewählten Nummernverwalter gestellt.

                                        Mitarbeiter Name des Mitarbeiters, dem der Ziel-Nummernverwalter zuge-
                                        ordnet ist.

                                        Nummernverwalter Nummernverwalter, in den die Lagerbestellungen mit
                                        (vollständigen) Wareneingängen gestellt werden sollen.
3.30 / 04-2020




                 A+W Business Einkauf                                                                          D-231
                 Wareneingang                                                                        Softwarereferenz




                                          Wareneingang – Komplett
                                          Dokumente > Bestellung > Wareneingang > Wareneingang > Register Kom-
                                          plett




                 Abb. D-136   Wareneingang – Komplett


                                          In diesem Register werden alle Bestellungen angezeigt, die den Suchkriterien
                                          entsprechen. Wenn Sie eine Bestellung markieren, werden die referenzierten
                                          Aufträge aufgelistet.
                                           Tutorial, “Wareneingang erfassen” auf Seite D-127

                                          Liefertermin

                                          Anliefertermin des Lieferanten Anzeige des aktuellen Tagesdatums. Sie
                                          können es überschreiben, wenn Sie eine Lieferung erfassen wollen, die vor
                                          diesem Datum eingetroffen ist. Das Datum wird nur für die Dokumente über-
                                          nommen, die in der Übersicht markiert sind.

                                          AB-Lieferant Sie können zu einem Wareneingang auch die Nummer der
                                          Auftragsbestätigung durch den Lieferanten erfassen.
3.30 / 04-2020




                 D-232                                                                          A+W Business Einkauf
                 Softwarereferenz                                                                     Wareneingang




                                        Dokumente
                                        Mit den Schaltflächen können Sie alle oder einige Dokumente markieren oder
                                        die Markierung entfernen.
                                        In der Übersicht werden alle Bestellungen angezeigt, die den Suchkriterien im
                                        Register Auswahl entsprechen. Der vollständige Wareneingang wird für die
                                        Dokumente erfasst, bei denen die Checkbox Komplett buchen markiert ist.
                                        •   Bestell-Nr.:
                                            Nummer der Bestellung.
                                        •   Komplett buchen:
                                            Eine Bestellung kann als komplett gebucht werden, wenn alle Positionen
                                            vollständig geliefert wurden.
                                            ☐ Der Wareneingang ist nicht vollständig. Es stehen noch Lieferungen
                                            aus.
                                            ☑ Der Wareneingang ist vollständig und die Bestellung soll als komplett
                                            verbucht werden.
                                        •   Status:
                                            Aktueller Status. Der Status wird nach der Erfassung des Wareneingangs
                                            umgesetzt.
                                        •   Lieferant:
                                            Nummer und Name des Lieferanten.
                                        •   Anlief.-Term. d. Lieferant:
                                            Anliefertermin des Lieferanten. Der Termin wird aus der Bestellung oder
                                            der AB übernommen. Wenn Sie den Wareneingang erfasst haben, wird der
                                            Termin auf das aktuelle Tagesdatum oder das von Ihnen gewählte Datum
                                            umgesetzt.
                                        •   Enthält Kisten:
                                            Anzeige der Bestellungen, in denen Kisten enthalten sind. Die Markierung
                                            der Checkbox kann nicht geändert werden.

                                        Zugehörige Aufträge
                                        In der Übersicht werden nur die referenzierten Aufträge angezeigt, die zu der
                                        ausgewählten Bestellung gehören. Wenn mehrere Bestellungen ausgewählt
                                        sind, bleibt die Liste leer.

                                        Anliefertermin bei Kunde Das Datum wird aus dem referenzierten Auftrag
                                        übernommen. Sie können es überschreiben, wenn der ursprüngliche Termin
                                        nicht eingehalten werden kann.
3.30 / 04-2020




                 A+W Business Einkauf                                                                         D-233
                 Wareneingang                                                                        Softwarereferenz




                                          Wareneingang – Positionsweise
                                          Dokumente > Bestellung > Wareneingang > Wareneingang Kiste > Register
                                          Positionsweise




                 Abb. D-137   Wareneingang – Positionsweise


                                          In diesem Register können Sie Wareneingänge positionsweise für eine Be-
                                          stellung erfassen, die im Register Komplett ausgewählt wurde.

                                          Warenein-/ausgang

                                          Menge Eingang Menge, die für die markierte Position geliefert wurde.

                                          Menge bestellt, Bereits geliefert, Menge avisiert In diesen Feldern wer-
                                          den die entsprechenden Mengen für die markierte Position angezeigt. Die Fel-
                                          der werden nach der Erfassung aktualisiert.

                                          Lagerort Zur markierten Position können Sie einen Lagerort auswählen, an
                                          dem der Lagerartikel verbucht werden soll. Beachten Sie dabei, dass Lager-
                                          artikel auch auf den Lagerort <k.A.> gebucht werden können. Der Lagerort
                                          aus der Bestellung kann über das Menü Optionen vorgeblendet werden.
                                           “Menü Optionen” auf Seite D-228
3.30 / 04-2020




                 D-234                                                                        A+W Business Einkauf
                 Softwarereferenz                                                                        Wareneingang




                                        Über-/Unterlieferung akzeptieren Die Stückzahl der Lieferung kann sich
                                        von der Bestellung unterscheiden. Sie können die abweichenden Stückzahlen
                                        akzeptieren und damit die Lieferung für die Position als komplett erfassen.
                                        ☐ Über- oder Untermengen werden nicht akzeptiert.
                                        ☑ Die eingegebene Stückzahl wird akzeptiert und die Position wird als kom-
                                        plett gebucht.
                                        • Wenn ein Lagerartikel geliefert wurde, wird der Lagerbestand der geliefer-
                                           ten Menge entsprechend aktualisiert. Die geänderte Menge wird in die Be-
                                           stellung zurückgeschrieben.
                                        • Wenn die Lieferung zu einem Auftrag bestellt wurde, wird die neuen Men-
                                           gen in den Auftrag als Über- oder Untermenge eingetragen.
                                           – Ist der Auftrag bereits in der Produktion, wird die Mengenänderung an
                                               das Produktionssystem übergeben.
                                           – Ist der Auftrag noch nicht in der Produktion, wird die Über-/Untermenge
                                               mit der Produktionsübergabe an das Produktionssystem gemeldet.
                                            Dazu muss in den Firmendaten die Checkbox Bestellung und Auftrag än-
                                            dern, wenn Über/-Unterlieferung akzeptiert aktiviert werden.
                                             Stammdaten, “Firmendaten – Lager/EK/EDI” auf Seite B-957

                                        Bestätigung

                                        AB-Lieferant Nummer der Auftragsbestätigung des Lieferanten für die mar-
                                        kierte Position.

                                        AB-Liefertermin Liefertermin für die Position.

                                        Positionen
                                        In der Übersicht werden die Positionen der gewählten Bestellung angezeigt.
                                        •   Pos:
                                            Nummer der Bestellposition.
                                        •   Komplett buchen:
                                            Eine Position kann als komplett gebucht werden, wenn die gesamte Stück-
                                            zahl geliefert wurde.
                                            ☐ Der Wareneingang ist nicht vollständig.
                                            ☑ Die Position soll als komplett verbucht werden.
                                        •   Auftr.Nr.:
                                            Auftragsnummer.
                                        •   Artikel:
                                            Bezeichnung des bestellten Produkts.
                                        •   Farbe:
                                            (Farb-) Varianten, die zu dem bestellten Produkt erfasst sind.
                                        •   Breite/Höhe:
                                            Maße der bestellten Position.
                                        •   Bestellt:
                                            Stückzahl der Bestellung für diese Position.
3.30 / 04-2020




                                        •   Avisiert:
                                            Avisierte Stückzahl der Position.



                 A+W Business Einkauf                                                                          D-235
                 Wareneingang                                                                  Softwarereferenz




                                •   Geliefert:
                                    Menge, die für diese Position bereits geliefert wurde. Bei Teillieferungen ist
                                    dies die Summe der Stückzahlen, die bisher zu dieser Bestellung geliefert
                                    wurden.
                                •   Eingang:
                                    Menge, die für die markierte Position geliefert wurde.
                                •   Akzeptieren:
                                    Wenn die Stückzahl der Lieferung höher oder niedriger ist als die der Be-
                                    stellung, kann diese Stückzahl übernommen werden. Die nicht bestellten
                                    Scheiben werden im Lager nur verbucht, wenn es Lagerartikel sind, die in
                                    einer Lagerbestellung bestellt wurden. Wenn die Bestellung aus einem
                                    Auftrag erzeugt worden ist, werden die Lagerbestände nicht aktualisiert.
                                    ☐ Die Liefermenge entspricht der Bestellung und braucht nicht gesondert
                                    gekennzeichnet zu werden.
                                    ☑ Die Lieferung ist größer oder kleiner als die Bestellung und wird akzep-
                                    tiert. Die gelieferte Stückzahl wird in die Bestellung zurückgeschrieben.
                                    Der referenzierte Auftrag wird nicht geändert. Die überzähligen Scheiben
                                    können ggf. als Bestand verbucht werden.
                                •   Enthält Kisten:
                                    Anzeige der Bestellungen, in denen Kisten enthalten sind. Die Markierung
                                    der Checkbox kann nicht geändert werden.
                                •   AB-Lieferant:
                                    Nummer der Auftragsbestätigung des Lieferanten.
                                •   AB-Liefertermin:
                                    Liefertermin aus der Auftragsbestätigung des Lieferanten.
                                •   Lagerort:
                                    Standard-Lagerort des Lagerartikels. Beachten Sie dabei, dass Lager-
                                    artikel auch auf den Lagerort <k.A.> gebucht werden können.
                                •   Artikelbezeichnung 2 + 3:
                                    Bezeichnungen des bestellten Produkts, die in den Stammdaten hinterlegt
                                    sind. Bei Float-Glas ist in der Regel nur die Bezeichnung 1 hinterlegt, die
                                    in der Spalte Artikel angezeigt wird.

                                Zugehörige Aufträge
                                In der Übersicht werden die referenzierten Aufträge zu den Positionen ange-
                                zeigt. Die Felder sind zum Register Komplett beschrieben.
                                 “Wareneingang – Komplett” auf Seite D-232
3.30 / 04-2020




                 D-236                                                                   A+W Business Einkauf
                 Softwarereferenz                                                                          Wareneingang




                                          Wareneingang – Identnummer
                                          Dokumente > Bestellung > Wareneingang > Wareneingang > Register Ident-
                                          nummer




                 Abb. D-138   Wareneingang – Identnummer


                                          In diesem Register werden die Positionen einer Bestellung mit Kisten ange-
                                          zeigt. Dabei wird für jede Kiste einer Bestellposition eine Unterposition (virtu-
                                          elle Positionsnummer) erzeugt, der eine Kiste mit einer eigenen Identnummer
                                          (Identifikationsnummer, ID) zugewiesen werden kann. Die Vorgabe für die ID
                                          können Sie festlegen.
                                           “Einstellungen (ID)” auf Seite D-240

                                             Voraussetzung
                                             In den Firmendaten muss die Checkbox für die Vergabe von virtuellen Po-
                                             sitionsnummern markiert sein.

                                              Stammdaten, “Virtuelle Positionsnummern verwenden” auf Seite B-943

                                          Kistendaten

                                          Lieferanten-Identnummer Die Kisten-ID, die der Lieferant für diese Position
                                          der Lieferung vergeben hat. Wenn die Nummer eingegeben ist, wird im Feld
                                          Identnummer die automatische Kisten-ID angezeigt.
3.30 / 04-2020




                 A+W Business Einkauf                                                                               D-237
                 Wareneingang                                                                Softwarereferenz




                                Identnummer Die automatische Kisten-ID wird angezeigt, sobald Sie die
                                Lieferanten-ID eingetragen haben. Für jede Kiste einer Bestellposition wird
                                beim Erfassen des Wareneingangs eine eigene Kisten-ID erzeugt. Wenn z. B.
                                5 Kisten mit Float 5 à 1200 x 800 mm bestellt und geliefert wurden, werden
                                die IDs XXXX00001, XXXX00002, …, XXXX00005 vergeben. Die Vorgabe für
                                XXXX können Sie selbst bestimmen.
                                 “Einstellungen (ID)” auf Seite D-240

                                Lagerort Sie können jeder Position einen eigenen Lagerort zuweisen. Be-
                                achten Sie dabei, dass Sie auch den Lagerort <k.A.> zuweisen können.

                                Bemerkung Bei Besonderheiten, z. B. in der Zuweisung des Lagerortes
                                oder bei Reservierungen, können Sie eine Anmerkung eintragen.

                                Inhalt Inhalt der Kiste, die in der Übersicht markiert ist. Der Wert kann ggf.
                                geändert werden.

                                Prod. Datum Datum, bis zu dem die Produktion mit der bestellten Lieferung
                                abgeschlossen sein sollte. Dieses Datum ist für die Lagerentnahme nach dem
                                FiFo-Prinzip wichtig, z. B. für beschichtetes Glas.

                                EK / ME Einkaufspreis und Preiseinheit der bestellten Position. Wenn Sie
                                den Preis ändern, wird die Änderung in die Bestellung zurückgeschrieben.

                                Kistenpositionen
                                Sie können mehrere Kisten auf einmal auswählen, um diese in einem Schritt
                                zu buchen. Wenn mehr als eine Kiste ausgewählt ist und die Lieferanten-
                                Identnummer eingegeben ist, berechnet das System die Kisten-Identnum-
                                mern für alle markierte Einträge.
                                •   Pos:
                                    Positionsnummer aus der Bestellung. Eine Positionsunternummer wird
                                    beim Buchen automatisch dann vergeben, wenn die Stückzahl der Bestell-
                                    position größer als 1 ist, z. B. 1.1, 1.2 usw.
                                •   Bezeichnung:
                                    Bezeichnung aus der Bestellung.
                                •   Breite / Höhe:
                                    Lagermaße der Scheiben in der Kiste.
                                •   Lieferanten-Identnummer:
                                    Kisten-ID des Lieferanten wie im Bereich Kistendaten eingetragen.
                                •   Inhalt:
                                    Kisteninhalten wie im Bereich Kistendaten eingetragen.
                                •   Identnummer:
                                    (Automatische) ID wie im Bereich Kistendaten eingetragen.
                                •   Lagerort:
                                    Lagerort wie im Bereich Kistendaten eingetragen.
                                •   Prod. Datum:
                                    Produktionsdatum wie im Bereich Kistendaten eingetragen.
3.30 / 04-2020




                                •   Pr./ME:
                                    EK-Preis pro Mengeneinheit wie im Bereich Kistendaten eingetragen.




                 D-238                                                                 A+W Business Einkauf
                 Softwarereferenz                                                                      Wareneingang




                                           •   Pr. Einh.:
                                               Preiseinheit für den angezeigten Preis.


                                           Wareneingang – Protokoll (Identnummern)
                                           Dokumente > Bestellung > Wareneingang > Wareneingang > Register Proto-
                                           koll (Identnummern)




                 Abb. D-139   Wareneingang – Protokoll (Identnummern)


                                           In diesem Register können Sie sich einen Überblick über die vergebenen Kis-
                                           ten-IDs verschaffen.
3.30 / 04-2020




                 A+W Business Einkauf                                                                          D-239
                 Wareneingang                                                                Softwarereferenz




                                Einstellungen (ID)
                                Dokumente > Bestellung > Wareneingang > Wareneingang > Menü Optionen
                                > Gruppe Identnummernvergabe > Einstellungen




                                Abb. D-140   Einstellungen


                                In diesem Dialog legen Sie die Vorgabe für die Identifikationsnummern (ID) für
                                Kisten fest. Diese Einstellung ist notwendig, um eigene Kisten-IDs automa-
                                tisch zu vergeben.
                                Wenn in einer Lieferung z. B. eine Position mit 5 Kisten aufgeführt ist, werden
                                beim Erfassen des Wareneingangs 5 (virtuelle) Unternummern vergeben. Die-
                                se Nummern müssen Sie mit einem Kennzeichen versehen, so dass z. B. statt
                                der gescannten Kistennummer 12345 die Unternummern LieferantA00001,
                                LieferantA00002, ..., LieferantA00005 vergeben werden.
                                 Tutorial, “Kistengeschäft” auf Seite D-136

                                   Voraussetzung
                                   In den Firmendaten muss die Checkbox für die virtuelle Vergabe von Posi-
                                   tionsnummern markiert sein.

                                    Stammdaten, “Virtuelle Positionsnummern verwenden” auf Seite B-943

                                Lageridentnummer

                                Vorgabe Sie können einen Text (oder Zahlen) mit max. 15 Zeichen eingeben,
                                der durch XXXXX ergänzt wird. XXXXX steht für die automatisch vergebene
                                Nummer. Der Text wird so lange beibehalten, bis Sie ihn ändern.
                                Wenn Sie von unterschiedlichen Lieferanten Kisten beziehen und diese ge-
                                trennt kennzeichnen möchten, müssen Sie vor dem Erfassen des Warenein-
                                gangs die Vorgabe jeweils entsprechend anpassen.
3.30 / 04-2020




                 D-240                                                                A+W Business Einkauf
                 Softwarereferenz                                                                     Wareneingang




                                        Eingangskontrolle
                                        Dokumente > Bestellung > Wareneingang > Eingangskontrolle
                                        Im Dialog Wareneingangskontrolle können Sie für Bestellungen prüfen, wel-
                                        che Bestellungen komplett und welche unvollständig geliefert sind.
                                        Wenn Sie beim Buchen von Wareneingängen einen Ziel-Nummernverwalter
                                        angegeben haben, werden die Bestellungen automatisch in diesen verscho-
                                        ben.
                                         “Ziel-Nummernverwalter” auf Seite D-231
                                        In diesem Dialog finden Sie folgende Register:
                                        •   “Eingangskontrolle – Komplette Bestellungen” auf Seite D-241
                                        •   “Eingangskontrolle – Mengendiskrepanzen” auf Seite D-243


                                        Eingangskontrolle – Komplette Bestellungen
                                        Dokumente > Bestellung > Wareneingang > Eingangskontrolle > Register
                                        Komplette Bestellungen




                                        Abb. D-141   Eingangskontrolle – Komplette Bestellungen


                                        In diesem Register können Sie sich alle Bestellungen eines bestimmten Num-
                                        mernverwalters anzeigen lassen und prüfen, ob sie vollständig geliefert sind.
                                         Tutorial, “Wareneingang kontrollieren” auf Seite D-133
3.30 / 04-2020




                 A+W Business Einkauf                                                                         D-241
                 Wareneingang                                                                 Softwarereferenz




                                Nummernverwalter

                                Bestell-Nummernverwalter Nummernverwalter, in dem die Bestellungen
                                (mit Wareneingängen) verwaltet werden. Zur Auswahl werden nur die Num-
                                mernverwalter angeboten, die im Menü Bestellung > NV Bestellung angelegt
                                wurden.

                                Wareneingang komplett
                                In der Übersicht werden alle Bestellungen aus dem gewählten Nummernver-
                                walter angezeigt.
                                •   Nr.:
                                    Nummer der Bestellung.
                                •   Lieferant:
                                    Name des Lieferanten, an den die Bestellung geschickt wurde.
                                •   Status:
                                    Status der Bestellung. Der Status wird umgesetzt, wenn die Bestellung voll-
                                    ständig erfasst ist.

                                    Alte Bestellungen im Nummernverwalter
                                    In der Regel werden Bestellungen nach der Archivierung aus der Hauptda-
                                    tenbank gelöscht. Die Einstellungen dazu finden Sie in den Firmendaten.

                                     Stammdaten, “Firmendaten – Archiv” auf Seite B-965
                                    Wenn der Nummernverwalter für Bestellungen mit Wareneingängen zu voll
                                    wird, sollten Sie ihn gelegentlich leeren bzw. einen neuen anlegen.
                                     Verkauf, “So leeren Sie einen Nummernverwalter” auf Seite C-187
3.30 / 04-2020




                 D-242                                                                 A+W Business Einkauf
                 Softwarereferenz                                                                      Wareneingang




                                        Eingangskontrolle – Mengendiskrepanzen
                                        Dokumente > Bestellung > Wareneingang > Eingangskontrolle > Register
                                        Mengendiskrepanzen




                                        Abb. D-142   Eingangskontrolle – Mengendiskrepanzen


                                        In diesem Register können Sie sich alle Positionen von Bestellungen anzei-
                                        gen lassen, deren Wareneingang noch nicht vollständig verbucht ist.
                                        Sie können Bestellungen als komplett buchen. Teillieferungen können Sie je-
                                        doch nur über den Dialog Wareneingang erfassen.
                                         “Wareneingang (Dialog)” auf Seite D-227

                                        Mengendiskrepanzen
                                        In der Übersicht sind alle Bestellungen mit den Positionen angezeigt, deren
                                        Wareneingang noch nicht vollständig ist.
                                        •   Nr.:
                                            Nummer der Bestellung.
                                        •   Pos.:
                                            Nummer der Bestellposition, zu der ein Wareneingang offen ist.
                                        •   Artikel:
                                            Bezeichnung der Position.
                                        •   Best. Menge:
                                            Stückzahl der Position, die bestellt wurde.
                                        •   Gel. Menge:
3.30 / 04-2020




                                            Stückzahl der Lieferung dieser Position. Bei Teillieferungen kann dieser
                                            Wert sich von der bestellten Menge unterscheiden.




                 A+W Business Einkauf                                                                          D-243
                 Wareneingang                                                             Softwarereferenz




                                •   OK:
                                    Wenn die Restlieferung inzwischen eingetroffen ist, können Sie die kom-
                                    plett-Buchung nachholen, indem Sie die Checkbox markieren.
                                •   Lief.Datum:
                                    Das Lieferdatum wird aus der Bestellung übernommen. Wenn es bei teil-
                                    weisen Wareneingängen geändert wurde, wird auch hier das neue Datum
                                    angezeigt.
                                •   Lieferant:
                                    Name des Lieferanten, an den die Bestellung geschickt wurde.
3.30 / 04-2020




                 D-244                                                              A+W Business Einkauf
                 Softwarereferenz                                                                         Rechnung




                                        Rechnung
                                        Dokumente > Bestellung > Rechnung > Rechnungskontrolle
                                        Sie können die Rechnungen Ihrer Lieferanten in A+W Business erfassen und
                                        prüfen, bevor Sie diese an Ihre Buchhaltung und/oder Finanzbuchhaltung (Fi-
                                        Bu) übergeben. Dazu steht Ihnen der Dialog Rechnungskontrolle zur Verfü-
                                        gung.
                                        In diesem Kapitel finden Sie Informationen zu folgenden Themen:
                                        •   “Rechnungskontrolle – Bestellungen” auf Seite D-248
                                        •   “Rechnungsdatum” auf Seite D-255


                                        Rechnungskontrolle
                                        Dokumente > Bestellung > Rechnung > Rechnungskontrolle
                                        In diesem Dialog können Sie die Lieferantenrechnungen erfassen und kontrol-
                                        lieren und zur Übergabe an die FiBu in einen entsprechenden Nummernver-
                                        walter stellen.
                                        Angezeigt werden nur die Bestellungen, die den definierten Mindeststatus er-
                                        reicht haben, z. B. Wareneingang komplett.
                                         Tutorial, “Preis- und Rechnungskontrolle” auf Seite D-143

                                            Sammelrechnung
                                            Wenn Ihr Lieferant mehrere Bestellungen in einer Sammelrechnung zu-
                                            sammengefasst hat, kann diese nur geprüft und akzeptiert werden, wenn
                                            in allen Bestellungen derselbe MwSt.-Satz und dieselbe Währung angege-
                                            ben sind.

                                        In diesem Kapitel finden Sie Informationen zu folgenden Themen:
                                        •   “Menü Funktionen” auf Seite D-246
                                        •   “Menü Optionen” auf Seite D-246
                                        •   “Rechnungskontrolle – Bestellungen” auf Seite D-248
                                        •   “Rechnungskontrolle – Positionen” auf Seite D-251
                                        •   “Rechnungskontrolle – Stückliste” auf Seite D-253
3.30 / 04-2020




                 A+W Business Einkauf                                                                        D-245
                 Rechnung                                                                Softwarereferenz




                            Menü Funktionen
                            Dokumente > Bestellung > Rechnung > Rechnungskontrolle > Menü Funktio-
                            nen
                            Über dieses Menü können Sie andere Dialoge öffnen, ohne die Rechnungs-
                            kontrolle zu schließen.
                            Folgende Einträge werden angezeigt:
                            •   Teillieferung erstellen:
                                Öffnet den Dialog Dokumente kopieren, um eine Teillieferung zu erfassen.
                                 Verkauf, “Dokumente kopieren” auf Seite C-532
                            •   Anlieferpauschale einfügen:
                                Die Lieferpauschale wird automatisch als Position im Register Positionen
                                eingefügt. Wenn in der Bestellung bereits eine Lieferpauschale enthalten
                                ist, wird die Option nicht ausgeführt.
                            •   Bestellerfassung öffnen:
                                Während der Preiskontrolle sind alle aufgelisteten Bestellungen für die Be-
                                arbeitung (durch andere Mitarbeiter) gesperrt. Mit dieser Funktion öffnen
                                Sie den Dialog Dokumentenverwaltung, um eine der angezeigten Bestel-
                                lungen zu bearbeiten. Geänderte Werte werden in die Preiskontrolle über-
                                nommen.
                                 Verkauf, “Dokument – Kopfdaten” auf Seite C-417
                            •   Bestelldaten aktualisieren:
                                Mit dieser Funktion werden die geänderten Werte sofort in die Bestellung
                                zurückgeschrieben.


                            Menü Optionen
                            Dokumente > Bestellung > Rechnung > Rechnungskontrolle > Menü Optionen
                            Über dieses Menü können Sie die Standardeinstellung des Dialoges bestim-
                            men. Sie können die Optionen aktivieren oder deaktivieren. Die Einstellung
                            wird nicht zurückgesetzt, wenn Sie den Dialog schließen.

                            Gruppe Standard
                            •   NettoMwst.:
                                Nettobeträge werden inkl. Mwst. angezeigt.
                            •   BruttoMwst.:
                                Bruttobeträge werden inkl. Mwst. angezeigt.
                            •   Netto:
                                Nettobeträge werden ohne Mwst. angezeigt.

                            Gruppe Verhalten
                            •   Schnellerfassung:
                                Mit dieser Option springt der Cursor nach der Eingabe einer Bestellnum-
                                mer in das Feld Auftragssumme. Diese Einstellung wird benutzerbezogen
                                gespeichert.
3.30 / 04-2020




                 D-246                                                              A+W Business Einkauf
                 Softwarereferenz                                                                           Rechnung




                                        •   Einschränkung bei Rech.dat.:
                                            Öffnet den Dialog Rechnungsdatum, um eine Abweichung in Tagen festzu-
                                            legen.
                                             “Rechnungsdatum” auf Seite D-255
                                        •   Ziel-NV füllen:
                                            Schaltet die Felder im Bereich Ziel-Nummernverwalter frei, um einen Mit-
                                            arbeiter und den zugehörigen Nummernverwalter auszuwählen.

                                        Gruppe Einstellungen
                                        •   Rabatt einfrieren:
                                            Der Rabatt wird fixiert. Diese Option sollten Sie aktivieren, wenn Sie neue
                                            Rabatte festgelegt haben, in den alten Bestellungen aber die alten Rabatte
                                            angewendet werden sollen. Die Preise werden dann nach der Preiskon-
                                            trolle nicht neu errechnet.
                                        •   Auftragskosten nicht in Statistik korrigieren:
                                            Die EK-Preise im referenzierten Auftrag werden nur korrigiert, solange der
                                            Auftrag noch in der Hauptdatenbank vorhanden ist und nicht an die Statistik
                                            übergeben wurde.
                                        •   Hinweis auf Lieferterminüberschreitung:
                                            Wenn der Liefertermin beim Kunden nicht eingehalten werden kann, wird
                                            eine Meldung angezeigt.

                                        Gruppe Xternal
                                        •   Xternal-XML-Datei erstellen:
                                            Diese Option ist nur kundenspezifisch aktiviert.
                                        •   Einstellungen für Xternal:
                                            Öffnet den Dialog Einstellungen, um Vorgaben für den XML-Export festzu-
                                            legen. Diese Funktion ist nur freigeschaltet, wenn die Option Xternal-XML-
                                            Datei erstellen aktiviert ist.
3.30 / 04-2020




                 A+W Business Einkauf                                                                           D-247
                 Rechnung                                                                              Softwarereferenz




                                           Rechnungskontrolle – Bestellungen
                                           Dokumente > Bestellung > Rechnung > Rechnungskontrolle > Register Be-
                                           stellungen




                 Abb. D-143   Rechnungskontrolle – Bestellungen


                                           In diesem Register können Sie Lieferantenrechnungen erfassen und zur
                                           Übergabe an die FiBu in einen anderen Nummernverwalter weiterleiten.
                                            Tutorial, “Rechnung kontrollieren” auf Seite D-146

                                           Rechnungsdaten

                                           Rechnungsnummer Pflichtfeld. Sie müssen die Nummer der Lieferanten-
                                           rechnung eingeben.

                                           Rechnungsdatum Pflichtfeld. Datum, das auf der Rechnung angegeben ist.
                                           Standardmäßig wird immer das zuletzt vergebene Rechnungsdatum vorge-
                                           schlagen. Sie können das Datum über den Kalender auswählen oder manuell
                                           eingeben, z. B. als 16052013.
3.30 / 04-2020




                 D-248                                                                            A+W Business Einkauf
                 Softwarereferenz                                                                        Rechnung




                                        Bestelldaten
                                        Mit der Wahl einer der beiden Optionen werden die zugehörigen Felder freige-
                                        schaltet, um die Bestellung(en) auszuwählen, zu denen die Rechnungen ge-
                                        prüft werden sollen.
                                        •   Bestellnummer, bis:
                                            Wenn Sie in beiden Feldern dieselbe Nummer eintragen, wird nur diese
                                            eine Bestellung im Bereich Bestellungen angezeigt. Wenn zu einer Rech-
                                            nung mehrere Bestellungen gehören, können Sie nacheinander mehrere
                                            Bestellnummern eingeben und in die Übersicht übernehmen. Dazu müs-
                                            sen alle Bestellungen zum selben Lieferanten gehören und denselben
                                            MwSt.-Satz haben.
                                        •   Nummernverwalter:
                                            Wenn Sie einen Nummernverwalter ausgewählt haben, werden im Bereich
                                            Bestellungen alle Bestellungen aufgelistet, die in diesem Nummernverwal-
                                            ter stehen.

                                        Summen
                                        Erst wenn Sie den Betrag aus der Rechnung des Lieferanten eingegeben und
                                        mit [Ausführen] bestätigt haben, können Sie zu einem der anderen Register
                                        wechseln.

                                        Rechnungssumme, Mwst. Pflichtfeld. Gesamtbetrag der Rechnung und
                                        der Mehrwertsteuer. Der Betrag der Mehrwertsteuer wird nicht angezeigt,
                                        wenn der Modus Netto ausgewählt ist.

                                        Modus Mit der Wahl des Modus wird die Mehrwertsteuer angezeigt oder
                                        ausgeblendet. Den Standard-Modus können Sie im Menü Optionen > Gruppe
                                        Standard festlegen.
                                        • Netto mit Mwst.:
                                           Der Gesamtbetrag wird als Nettobetrag gewertet, der Betrag der Mehrwert-
                                           steuer wird angezeigt.
                                        • Brutto mit Mwst.:
                                           Der Gesamtbetrag wird als Bruttobetrag gewertet, der Betrag der Mehr-
                                           wertsteuer wird angezeigt.
                                        • Netto:
                                           Der Gesamtbetrag wird als Nettobetrag gewertet, der Betrag der Mehrwert-
                                           steuer wird nicht kontrolliert.

                                        Währung Sie können nur dann eine andere Währung auswählen, wenn Sie
                                        mit mehreren Währungen arbeiten.
                                        In der Kombobox werden alle Währungen zur Auswahl angeboten, die in den
                                        Stammdaten hinterlegt sind. Mit der Auswahl einer anderen Währung als Euro
                                        werden in der Übersicht die Beträge der Bestellungen und die Mehrwertsteuer
                                        zusätzlich in der gewählten Währung angezeigt.
                                         Stammdaten, “Währungen” auf Seite B-457
3.30 / 04-2020




                 A+W Business Einkauf                                                                        D-249
                 Rechnung                                                                     Softwarereferenz




                            Kurs Wenn Sie mit mehreren Währungen arbeiten, wird der Wechselkurs
                            angezeigt, der in den Stammdaten hinterlegt ist. Er kann überschrieben wer-
                            den. Wenn Sie nur mit Euro arbeiten, muss in diesem Feld 1 stehen.

                               Wechselkurs fixieren
                               Sie können pro Bestellung einen abweichenden Wechselkurs vereinbaren.
                               Dieser wird automatisch zur Berechnung in der Rechnungskontrolle heran-
                               gezogen. Sie können ihn nur überschreiben, wenn er in der Bestellung
                               nicht fixiert ist.

                                Verkauf, “Kurs fixiert für Rechnungsdruck” auf Seite C-432

                            Ziel-Nummernverwalter
                            Diese beiden Felder sind nur freigeschaltet, wenn die Option Ziel-NV füllen ak-
                            tiviert ist. Die Rechnungen werden dann nach der Rechnungskontrolle in den
                            angegebenen Nummernverwalter verschoben, z. B. um sie dann anzuweisen.
                             “Menü Optionen” auf Seite D-206

                            Mitarbeiter Name des Mitarbeiters, dem der Ziel-Nummernverwalter zuge-
                            ordnet ist.

                            Nummernverwalter Nummernverwalter, in den die Rechnungen nach der
                            Prüfung gestellt werden sollen.

                            Bestellungen
                            In der Übersicht werden alle Bestellungen angezeigt, die sich im Nummern-
                            verwalter befinden. Wenn Sie im Bereich Bestelldaten über die Bestellnum-
                            mern gefiltert haben, werden nur die entsprechenden Bestellungen angezeigt.
                            Die Spalten mit den Beträgen der Mehrwertsteuer und der Fremdwährung
                            werden nur angezeigt, wenn ein Modus mit Mehrwertsteuer und/oder eine
                            Fremdwährung ausgewählt ist.

                            Summe In diesen Feldern werden die Gesamtsumme der aufgelisteten Be-
                            stellungen und der Gesamtbetrag der Mehrwertsteuer angezeigt.

                            Zugrundeliegender Mwst-Satz In diesem Feld wird der Prozentsatz zur Be-
                            rechnung der Mehrwertsteuer angezeigt, der in der Bestellung angegeben ist,
                            die zu dieser Rechnung gehört.
                             Verkauf, “Steuersatz” auf Seite C-521
3.30 / 04-2020




                 D-250                                                               A+W Business Einkauf
                 Softwarereferenz                                                                             Rechnung




                                           Rechnungskontrolle – Positionen
                                           Dokumente > Bestellung > Rechnung > Rechnungskontrolle > Register Posi-
                                           tionen




                 Abb. D-144   Rechnungskontrolle – Positionen


                                           In diesem Register können Sie die Positionen aller Bestellungen prüfen, zu
                                           der Sie eine Lieferantenrechnung erfasst haben.
                                           Das Register wird nur angezeigt, wenn im Register Bestellungen die Pflichtfel-
                                           der gefüllt sind und mit [Ausführen] bestätigt wurden.
                                            Tutorial, “Rechnung kontrollieren” auf Seite D-146

                                           Bestellpositionen
                                           In der Übersicht werden alle Positionen der Bestellungen aufgeführt, auf die
                                           sich die Rechnung bezieht.
                                           •   Bestell-Nr.:
                                               Nummer, mit der die Bestellung in der Datenbank gespeichert ist.
                                           •   Pos:
                                               Nummer der Bestellposition.
                                           •   Artikel:
                                               Bezeichnung der bestellten Position.
                                           •   Breite / Höhe:
                                               Maße der bestellten Position.
3.30 / 04-2020




                 A+W Business Einkauf                                                                             D-251
                 Rechnung                                                                Softwarereferenz




                            •   Euro-Netto:
                                Preis der Position in der Landeswährung (hier Euro).
                                Wenn Sie mit einer anderen Währung arbeiten, ändert sich die Bezeich-
                                nung entsprechend. Wenn Sie mit zwei Währungen arbeiten, wird für die
                                zweite Währung eine weitere Spalte mit dem entsprechenden Betrag an-
                                gezeigt.
                            •   Mwst.-Euro:
                                Betrag der Mehrwertsteuer in der Landeswährung (hier Euro). Die Spalte
                                wird nicht angezeigt, wenn im Register Bestellungen die Option Netto ge-
                                wählt ist.
                                Für die Anzeige der Mehrwert-Steuer im Mehrwährungssystem gilt das
                                gleiche, wie für die Anzeige des Betrags.
                            •   Stückl.genaue Eingabe:
                                In dieser Spalte wird angezeigt, ob Sie Preisdifferenzen auf der Ebene der
                                Stücklisten-Komponenten oder der Positionen korrigiert haben.
                                – Deaktiv:
                                    Der Preis wurde nicht geändert oder der Preis der gesamten Position
                                    wurde geändert.
                                – Aktiv:
                                    Der Preis wurde in der Stückliste geändert.
                            •   Menge:
                                Gelieferte Menge.
                            •   Lieferant:
                                Nummer und Name des Lieferanten.

                            Gesamtbetrag Anzeige der Summe der (eingegebenen) Positionsbeträge.

                            Gesamtmenge Summe der Positionsmengen.

                            Differenz Anzeige der Differenz zwischen der Rechnungssumme im Regis-
                            ter Bestellungen und der Summe der (eingegebenen) Positionsbeträge. In
                            diesem Fall kann der Preis nicht bestätigt werden, bevor Sie die Preise der Po-
                            sitionen oder der Stücklisten geändert haben.

                                Differenz
                                Eine Differenz wird auch angezeigt, wenn Sie im Register Bestellungen
                                versehentlich eine falsche Rechnungssumme eingetragen haben oder der
                                Wechselkurs nicht korrekt ist.
3.30 / 04-2020




                 D-252                                                            A+W Business Einkauf
                 Softwarereferenz                                                                               Rechnung




                                           Rechnungskontrolle – Stückliste
                                           Dokumente > Bestellung > Rechnung > Rechnungskontrolle > Register Stück-
                                           liste




                 Abb. D-145   Rechnungskontrolle – Stückliste


                                           In diesem Register können Sie sich den Preis einer Position auf der Ebene der
                                           Stückliste und der Stücklisten-Komponenten anzeigen lassen. Das Register
                                           ist nur aktiv, wenn im Register Positionen eine Position mit Stückliste markiert
                                           ist.
                                            Tutorial, “Rechnung kontrollieren” auf Seite D-146

                                           Stücklistenaufbau
                                           In diesem Feld wird die Stückliste der Position angezeigt, die im Register Po-
                                           sitionen markiert ist.

                                           Preise
                                           Die Anzeige der Felder hängt davon ab, welche Stücklisten-Komponente mar-
                                           kiert ist.
                                           Sie können die Preise auf der Hauptebene oder an den Stücklisten-Kompo-
                                           nenten korrigieren. Sie können die Austauschzuschläge und Preise der ein-
                                           zelnen Komponenten ändern.
3.30 / 04-2020




                                           Preis / PE Anzeige des Preises und der Preiseinheit aus der Bestellung.

                                           Rabatt Anzeige des Rabattes aus der Bestellung. Der Wert kann nicht geän-
                                           dert werden.


                 A+W Business Einkauf                                                                               D-253
                 Rechnung                                                              Softwarereferenz




                            Netto / Positionsmenge Anzeige des Preises und der Menge aus der Be-
                            stellung, wenn die Hauptposition markiert ist. Der Wert kann nicht geändert
                            werden.

                            Netto / Stücklistenmenge Anzeige des Preises und der Menge aus der Be-
                            stellung, wenn eine Komponente markiert ist. Der Wert kann nicht geändert
                            werden.

                            Netto ges. Anzeige des Positions-Preises aus der Bestellung, wenn die
                            Hauptposition markiert ist. Der Wert kann geändert werden.

                            Netto ges. / Pos. Menge Anzeige des Komponenten-Preises und der Men-
                            ge, wenn eine Komponente markiert ist. Der Wert kann geändert werden.

                            Gesamtsumme Anzeige des Komponenten-Preises pro Position, wenn eine
                            Komponente markiert ist. Der Wert kann geändert werden.
3.30 / 04-2020




                 D-254                                                           A+W Business Einkauf
                 Softwarereferenz                                                                          Rechnung




                                        Rechnungsdatum
                                        Dokumente > Bestellung > Auftragsbestätigung > Preiskontrolle > Menü Opti-
                                        onen > Gruppe Verhalten > Einschränkung bei Rech.dat.
                                        Dokumente > Bestellung > Rechnung > Rechnungskontrolle > Menü Optionen
                                        > Gruppe Verhalten > Einschränkung bei Rech.dat.




                                        Abb. D-146    Einschränkungen für Rechnungsdatum


                                        In diesem Dialog können Sie angeben, um wie viele Tage das Rechnungs-
                                        datum vom aktuellen Tagesdatum höchstens abweichen darf. Damit können
                                        fehlerhafte Eingaben des Datums verhindert werden.
                                        Die Einstellung ist nur für die Rechnungskontrolle sinnvoll.

                                        Abweichung

                                        In Tagen Der Wert gibt die Anzahl der Tage an, um die das Rechnungs-
                                        datum vom aktuellen Tagesdatum abweichen darf. Wenn der erlaubte Zeit-
                                        raum durch eine fehlerhafte Eingabe des Datums überschritten wird, wird
                                        automatisch das maximal erlaubte Datum eingesetzt.

                                           Beispiel

                                           Angezeigt: 24.08. - erlaubt sind 10 Tage
                                           Eingabe 13.08. - Korrektur auf 14.08.


                                        Wenn Sie eine 0 (Null) eintragen, ist die Funktion abgeschaltet.
3.30 / 04-2020




                 A+W Business Einkauf                                                                        D-255
                 Rechnung                                                                  Softwarereferenz




                            Elektronische Rechnungskontrolle
                            Dokumente > Bestellung > Rechnung > Elektr. Rechnungskontrolle
                            Wenn Sie Rechnungen Ihrer Lieferanten elektronisch erhalten, können Sie die
                            Zuordnung der Positionen zu Ihren Bestellungen, die Preise und Termine prü-
                            fen. Dazu steht Ihnen die elektronische Rechnungskontrolle zur Verfügung.
                             Tutorial, “Export/Import (openTRANS)” auf Seite D-151
                             Tutorial, “Elektronisches Dokument prüfen” auf Seite D-170
                            In diesem Kapitel finden Sie Informationen zu folgenden Themen:
                            •   “Menü Funktionen” auf Seite D-256
                            •   “Menü Optionen” auf Seite D-257
                            •   “Elektronische Rechnungskontrolle – Dokumentenimport” auf Seite D-259
                            •   “Elektronische Rechnungskontrolle – Positionsübersicht” auf Seite D-262


                            Menü Funktionen
                            Dokumente > Bestellung > Rechnung > Elektr. Rechnungskontrolle > Menü
                            Funktionen
                            Über dieses Menü können Sie andere Dialoge öffnen, ohne die elektronische
                            Rechnungskontrolle zu schließen.
                            Folgende Einträge werden angezeigt:
                            •   Anlieferpauschale einfügen:
                                Die Lieferpauschale wird automatisch als Position im Register Positionen
                                eingefügt. Wenn in der Bestellung bereits eine Lieferpauschale enthalten
                                ist, wird die Option nicht ausgeführt.
                            •   Bestellerfassung öffnen:
                                Während der Rechnungskontrolle sind alle aufgelisteten Bestellungen für
                                die Bearbeitung (durch andere Mitarbeiter) gesperrt. Mit dieser Funktion
                                können Sie den Dialog Dokumentenverwaltung öffnen, um eine der ange-
                                zeigten Bestellungen zu bearbeiten. Geänderte Werte werden in die Rech-
                                nungskontrolle übernommen.
                                 Verkauf, “Dokument – Kopfdaten” auf Seite C-417
                            •   Positionen manuell zuordnen:
                                Öffnet den Dialog Positionen manuell zuordnen, um die Positionen des
                                elektr. Dokuments den Positionen der Bestellung(en) zuzuordnen.
                                 “Positionen manuell zuordnen” auf Seite D-221
                            •   Fußzuschläge/-rabatte auf Bestellungen verteilen:
                                Öffnet den Dialog Fußzuschläge/-rabatte auf Bestellungen verteilen, um
                                den Zuschlag/Rabatt aus dem elektr. Dokument auf die zugeordneten Be-
                                stellungen zu verteilen.
                                 “Fußzuschläge/-rabatte verteilen” auf Seite D-222
                            •   Manuelle Positionszuordnung aufheben:
                                Hebt die manuelle Zuordnung der markierten Rechnungs-/Bestellpositio-
                                nen wieder auf.
3.30 / 04-2020




                            •   Alle Positionszuordnungen aufheben:
                                Hebt alle manuellen Zuordnungen von Rechnungs- und Bestellpositionen
                                wieder auf.


                 D-256                                                                A+W Business Einkauf
                 Softwarereferenz                                                                               Rechnung




                                        Menü Optionen
                                        Dokumente > Bestellung > Rechnung > Elektr. Rechnungskontrolle > Menü
                                        Optionen
                                        Über dieses Menü können Sie die Standardeinstellung des Dialoges bestim-
                                        men. Sie können die Optionen aktivieren oder deaktivieren. Die Einstellung
                                        wird nicht zurückgesetzt, wenn Sie den Dialog schließen.

                                        Gruppe Allgemein
                                        •   Betragsdifferenzen akzeptieren:
                                            Bei der elektronischen Rechnungskontrolle können Betragsdifferenzen,
                                            die durch Rundungen auftreten können, generell akzeptiert werden.
                                        •   Hinweis auf Betragsdiff./Ausgl.pos.:
                                            Wenn Rundungsdifferenzen automatisch einer Ausgleichsposition zuge-
                                            ordnet wurden, wird ein Hinweis angezeigt.
                                        •   Rabatt einfrieren:
                                            Mit dieser Option wird der Rabatt fixiert. Diese Option sollten Sie aktivieren,
                                            wenn Sie neue Rabatte festgelegt haben, in den alten Bestellungen aber
                                            die alten Rabatte angewendet werden sollen. Die Preise werden dann
                                            nach der Rechnungskontrolle nicht neu errechnet.
                                        •   Auftr.-EK nur korrigieren bis in Statistik:
                                            Die Korrekturen des EK-Preises im referenzierten Auftrag werden nur
                                            durchgeführt, solange der Auftrag noch in der Hauptdatenbank vorhanden
                                            ist und nicht an die Statistik übergeben wurde.
                                        •   Prod.Nr. für Ausgleichspos.:
                                            Öffnet den Dialog Auswahl, um eine Ausgleichposition für Rundungsdiffe-
                                            renzen zuzuordnen.
                                             “Auswahl (Prod. Nr. für Ausgleichspos.)” auf Seite D-220
3.30 / 04-2020




                 A+W Business Einkauf                                                                               D-257
                 Rechnung                                                                  Softwarereferenz




                            Gruppe Einstellungen
                            •   Hinweis auf Lieferterminüberschreitung:
                                Bei Überschreitung des geplanten Liefertermins wird eine Meldung ange-
                                zeigt.
                            •   Automatische Zuordnung unterdrücken:
                                Im Dialog Positionen manuell zuordnen können Sie die Checkbox für die
                                automatische Zuordnung aktivieren, damit die Fußzuschläge/-rabatte der
                                Auftragsbestätigung automatisch einem A+W Business-Produkt zugeord-
                                net werden. Diese automatische Zuordnung können Sie unterdrücken.
                                 “Zuordnung des Fußzuschlags/-rabatts zukünftig automatisch auflösen” auf
                                  Seite D-222
                                Wenn diese Option geändert wurde, muss das aktuell eingelesene Doku-
                                ment nochmals eingelesen werden.
                                 Tutorial, “So lesen Sie ein XML-Dokument ein” auf Seite D-169
                            •   Referenzierenden Produktnummern des Lieferanten vertrauen:
                                Wenn im importierten Dokument eine A+W Business-Produktnummer als
                                Referenz angegeben ist, kann die Zuordnung automatisch durchgeführt
                                werden.

                            Gruppe Xternal
                            •   Xternal-XML-Datei erstellen:
                                Für den elektronischen Datenaustausch wird eine XML-Datei erzeugt.
                            •   Einstellungen für Xternal:
                                Öffnet den Dialog Einstellungen, um Vorgaben für den XML-Export festzu-
                                legen. Diese Funktion ist nur freigeschaltet, wenn die Option Xternal-XML-
                                Datei erstellen aktiviert ist.
3.30 / 04-2020




                 D-258                                                              A+W Business Einkauf
                 Softwarereferenz                                                                           Rechnung




                                           Elektronische Rechnungskontrolle – Dokumenten-
                                           import
                                           Dokumente > Bestellung > Rechnung > Elektr. Rechnungskontrolle > Register
                                           Dokumentenimport




                 Abb. D-147   Elektronische Rechnungskontrolle – Dokumentenimport


                                           In diesem Register prüfen Sie die importieren Rechnungen. Nur wenn der Do-
                                           kumentenstatus fehlerfrei ist, kann die Rechnungskontrolle erfolgreich abge-
                                           schlossen werden.
                                            Tutorial, “Export/Import (openTRANS)” auf Seite D-151
                                            Tutorial, “Elektronisches Dokument prüfen” auf Seite D-170

                                           Buchungsart
                                           Mit der Wahl der Option legen Sie fest, wie das elektronische Dokument ver-
                                           arbeitet werden soll. Die Optionen sind dem Dokumentenstatus entsprechend
                                           freigeschaltet.
                                           •   Ablehnen:
                                               Mit dieser Option werden die Dokumente nicht übernommen. Die Rech-
                                               nungskontrolle wird nicht durchgeführt.
                                           •   Akzeptieren:
                                               Mit dieser Option wird die Rechnungskontrolle bestätigt. Die AB-Nummer,
                                               Preise und Liefertermine aus dem importierten Dokument werden in die
3.30 / 04-2020




                                               Bestellungen zurückgeschrieben.
                                               Die Dokumentenhistorie wird aktualisiert.



                 A+W Business Einkauf                                                                           D-259
                 Rechnung                                                                  Softwarereferenz




                            •   Teillieferung erstellen:
                                Zu den im Dokument (Teilrechnung) enthaltenen Positionen wird eine
                                (neue) Teillieferung erstellt und wie bei Akzeptieren verbucht. Die restli-
                                chen Positionen bleiben in der ursprünglichen Bestellung erhalten. Der
                                Status dieser Bestellung wird entsprechend angepasst.
                                Bei einem Lieferavis wird mit dieser Buchungsart eine Teilbestellung er-
                                zeugt.

                            Rechnungen
                            In der Übersicht sind alle importierten Rechnungen aufgelistet. Diese können
                            auch von unterschiedlichen Lieferanten stammen.
                            Wenn Sie einen Eintrag markieren, werden die referenzierten Dokumente in
                            der Übersicht Bestellungen / Teillieferungen angezeigt.
                            •   Rechnungsnummer:
                                Rechnungsnummer, die der Lieferant angegeben hat.
                            •   Lieferant:
                                Name des Lieferanten.
                            •   Netto:
                                Gesamtbetrag der Lieferung.
                            •   Mwst:
                                Betrag der Mehrwertsteuer dieser Rechnung.
                            •   Währung:
                                Währung, in der der Betrag in der Rechnung angegeben ist. Diese Anzeige
                                ist nur dann von Bedeutung, wenn Sie mit einem Mehrwährungssystem ar-
                                beiten.

                            Anzeige Sie können die Anzeige der Dokumente einschränken.

                            Filtereinstellungen Sie können Filter für die Anzeige der importierten Doku-
                            mente festlegen.
                             “Filtereinstellungen” auf Seite D-223

                            Dokumentenstatus
                            Die rote oder grüne Markierung gibt an, ob Unstimmigkeiten festgestellt wur-
                            den oder nicht. Die Optionen im Bereich Buchungsart sind entsprechend ge-
                            sperrt oder freigeschaltet.
                            •   Kein Dokument ausgewählt:
                                Die Anzeige des Dokumentenstatus kann nicht aktualisiert werden, da kein
                                Dokument in der Übersicht markiert ist. Dieser Eintrag wird nicht angezeigt,
                                wenn eine Rechnung markiert ist.
                            •   Mindestens ein Fußzuschlag/-rabatt einer Bestellung konnte dem Doku-
                                ment nicht zugeordnet werden:
                                Dieser Eintrag wird nur angezeigt, wenn eine Rechnung mit einem entspre-
                                chenden Fehler markiert ist.
                            •   Bestellungen vollständig referenziert:
3.30 / 04-2020




                                Bei einer roten Anzeige stimmt mindestens eine der referenzierten Positi-
                                onen nicht vollständig mit der importierten Rechnung überein. Die unvoll-
                                ständig referenzierten Bestellungen werden in der Übersicht
                                gekennzeichnet.


                 D-260                                                              A+W Business Einkauf
                 Softwarereferenz                                                                             Rechnung




                                        •   Fehlende Artikelpositionen in Bestellungen:
                                            In der Rechnung sind Positionen enthalten, die in der Bestellung nicht auf-
                                            geführt sind.
                                        •   Fehlende Fußzuschläge/-rabatte in Bestellungen:
                                            Fußzuschläge/-rabatte werden nicht mitbestellt. Da sie aber in der Rech-
                                            nung aufgeführt sind, müssen sie für die Rechnungskontrolle als Positio-
                                            nen in den Bestellungen vorhanden sein. Die fehlenden Fußzuschläge/-
                                            rabatte müssen in der Bestellung manuell erfasst werden.
                                        •   Preisdifferenz:
                                            Die Gesamtpreise von Bestellung und Rechnung sind unterschiedlich. In
                                            zugehörigen Feldern wird die Abweichung als Betrag und prozentual ange-
                                            zeigt.
                                        •   Mengendifferenz:
                                            Die Positionsmengen von Bestellung und Rechnung sind unterschiedlich.

                                        [Dokument anzeigen] Öffnet die Dokumentenansicht des markierten Doku-
                                        ments.

                                        Bestellungen / Teillieferungen
                                        In der Übersicht werden die referenzierten Dokumente angezeigt, wenn Sie
                                        einen Eintrag im Bereich Rechnungen markiert haben. Teillieferungen werden
                                        in blauer Schrift angezeigt.
                                        •   Bestellnummer:
                                            Nummer der Bestellung, die von A+W Business erzeugt wurde.
                                        •   Netto:
                                            Gesamtbetrag der Bestellung.
                                        •   Mwst:
                                            Betrag der Mehrwertsteuer dieser Bestellung.
                                        •   Währung:
                                            Währung, in der der Betrag in der Bestellung angegeben ist. Diese Anzeige
                                            ist nur dann von Bedeutung, wenn Sie mit einem Mehrwährungssystem ar-
                                            beiten.
                                        •   Auftr.Nr.:
                                            Nummer des referenzierten Auftrags.
                                        •   Kundenliefertermin:
                                            Datum der Anlieferung beim Kunden.
                                        •   Bemerkung:
                                            Wenn die Verknüpfung zwischen der Bestellung und dem importierten Do-
                                            kument nicht vollständig ist, wird ggf. ein Hinweis auf den Fehler angezeigt.
3.30 / 04-2020




                 A+W Business Einkauf                                                                            D-261
                 Rechnung                                                                               Softwarereferenz




                                           Elektronische Rechnungskontrolle – Positions-
                                           übersicht
                                           Dokumente > Bestellung > Rechnung > Elektr. Rechnungskontrolle > Register
                                           Positionsübersicht




                 Abb. D-148   Elektronische Rechnungskontrolle – Positionsübersicht


                                           In diesem Register können Sie die Positionen der Rechnung prüfen, die Ihr
                                           Lieferant gesendet hat.
                                           Die Optionen im Bereich Buchungsart sind zu Register Dokumentenimport er-
                                           klärt.
                                            “Elektronische Rechnungskontrolle – Dokumentenimport” auf Seite D-259

                                           Positionsübersicht
                                           In der Übersicht sind alle Positionen der Rechnung aufgeführt. Wenn Sie eine
                                           Position markieren, werden die Details in den Bereichen Dokumentenposition
                                           und Bestellposition angezeigt.
                                           •   Pos-Nr.:
                                               Positionsnummer aus der AB.
                                           •   Bestell-Nummer:
                                               Nummer der referenzierten Bestellung.
                                           •   Bestell-Position:
3.30 / 04-2020




                                               Positionsnummer aus der Bestellung.
                                           •   Netto Dokument/Netto 1 Bestellung:
                                               Positionspreis aus der importierten AB und aus der Bestellung.


                 D-262                                                                           A+W Business Einkauf
                 Softwarereferenz                                                                         Rechnung




                                        •   Menge Dokument/Menge 1 Bestellung:
                                            Positionsmenge aus der importierten AB und aus der Bestellung.
                                        •   Abmessung Dokument/Abmessung 1 Bestellung:
                                            Positionsmaße aus der importierten AB und aus der Bestellung.
                                        •   Differenz Preis:
                                            Differenz aus Spalte Netto Dokumente und Netto Bestellung.
                                        •   Differenz 1 Preis %:
                                            Preisdifferenz in Prozent.
                                        •   Differenz 2 Menge:
                                            Differenz aus Spalte Menge Dokumente und Menge Bestellung.
                                        •   Auftr.Nr.:
                                            Nummer des referenzierten Auftrags.
                                        •   Kundenliefertermin:
                                            Datum der Anlieferung beim Kunden.

                                        Dokumentenposition, Bestellposition
                                        In diesen beiden Bereichen werden Details zu der Position angezeigt, die in
                                        der Positionsübersicht markiert ist.
3.30 / 04-2020




                 A+W Business Einkauf                                                                        D-263
                 Basisglasverrechnung                                                             Softwarereferenz




                                        Basisglasverrechnung
                                        Dokumente > Bestellung > Basisglasverrechnung
                                        Diese Funktion ist nur kundenspezifisch freigeschaltet.
                                        In der Basisglasverrechnung werden Modellscheiben mit ihrer tatsächlichen
                                        Fläche anstatt der fakturierten Fläche übergeben und verrechnet.
3.30 / 04-2020




                 D-264                                                                       A+W Business Einkauf
Einkauf              D

               Partindex




          A+W Business
                 Partindex                                                                Index Einkauf




                 Index Einkauf
                 A                                         Bestellpool D-62
                 A+W B2B Purchasing Service D-159          – Anfrage erzeugen D-113
                 AB Lieferant D-197                        – Lieferant ändern D-72
                 – Auftragsdaten D-200                     – Preise vergleichen D-74
                 – Bestelldaten D-199                      – Sammelbestellung D-67
                 – Bestellpositionen D-201                 Bestellposition
                 – Liefertermin D-203                      – AB erfassen D-91
                 AB siehe auch Auftragsbestätigung         – im Auftrag erfassen D-54
                 AB-Lieferant                              – Produktion D-122
                 – Wareneingang D-198                      Bestellte Position ändern D-57
                 – Wareneingang pro Position D-202         Bestellung
                 Anfrage                                   – Auftragsbestätigung D-87
                 – Referenz D-111                          – aus Kundenauftrag D-51
                 – über Bestellpool erzeugen D-113         – aus unabhängiger Anfrage erzeugen D-115
                 – unabhängige Bestellung erzeugen D-115   – automatisch D-60
                 – zu Kundenauftrag erzeugen D-112         – Bestellpool D-62
                 – zu Kundenposition D-111                 – bestellte Position ändern D-53, D-57
                 Anfrage (Menü) D-186                      – Eingangskontrolle D-125
                 Anzeige                                   – elektr. Preiskontrolle D-213
                 – im elektr. Dokument filtern D-223       – elektr. Rechnungskontrolle D-256
                 Auftrag                                   – Export (Dokument) D-193
                 – Lieferant pro Position D-52             – Fremdwährung D-145
                 Auftragsbestätigung                       – Kiste erfassen D-83
                 – des Lieferanten erfassen D-89           – Kundenbestellung D-51
                 – Einkauf D-87                            – Lagerbestellung erfassen D-83
                 – elektr. Preiskontrolle D-213            – Lieferanten ändern D-72
                 – für Position erfassen D-91              – Liefertermin D-65
                 – Lieferant D-197                         – Mahnung D-88
                 – Preis pro Position D-210                – manuell D-45
                 – Preise prüfen D-146                     – manuell erfassen D-81
                 – Preiskontrolle D-204                    – Mengendiskrepanzen D-243
                 – Stücklistenpreise D-212                 – Preiskontrolle D-207
                 Auftragsdaten                             – Preisvergleich D-65
                 – AB Lieferant D-200                      – Rechnungskontrolle D-248
                 Ausgleichposition D-220                   – Sammelbestellung D-67
                 AW CommonBase Service D-159               – Teilbestellung D-259
                 AWProtocolService D-159                   – Terminüberwachung D-101
                                                           – übergeben D-68
                                                           – unabhängige Bestellung D-80
                 B
                                                           – unabhängige Bestellung erfassen D-81
                 Bestellanfrage D-186
                                                           – Wareneingang komplett D-241
                 Bestellarten
                                                           Bestellung (Menü) D-188
                 – Lagerbestellung D-80
                                                           Betragsdifferenz
                 – referenzierte Bestellung D-45
                                                           – elektronisches Dokument D-158
                 – unabhängige Bestellung D-80
                                                           – Produktzuordnung D-220
                 Bestelldaten
                                                           Buchen
3.30 / 04-2020




                 – AB Lieferant D-199
                                                           – Teillieferung D-216
                 Bestellkennzeichen
                                                           – Wareneingang D-127
                 – Einkauf D-22



                 A+W Business Einkauf                                                           D-267
                 Index Einkauf                                                                 Partindex




                 Buchungsart                              – Bestellkennzeichen D-22
                 – Dokumentenimport D-156                 – Bestellübergabe aus Auftrag D-60
                 – elektronische Preiskontrolle   D-216   – Bestellung D-190
                 – Preiskontrolle D-216                   – Dokumente D-185
                                                          – Firmendaten für Bestellung prüfen D-47
                 D                                        – Firmendaten prüfen D-161
                 Darstellungskonventionen D-13            – Firmendaten prüfen (Kisten) D-136
                 Datenaustausch D-150                     – Grundgedanken D-17
                 – Dokument D-151                         – Handlungsablauf D-18
                 – Fremdschnittstellenverwaltung D-178    – Liefertermin D-87
                 – openTRANS-Dokument einlesen D-169      – Menü-Übersicht D-14
                 – XML-Datei einlesen D-169               – Nachbestellung D-191
                 Datenexport                              – Preiskontrollen D-143
                 – EDI D-177                              – Preislisten D-37
                 Dienste                                  – Rechnungskontrolle D-144
                 – A+W B2B Purchasing Service D-159       – Schema D-17
                 – AW CommonBase Service D-159            – Schnittstellenverwaltung prüfen D-178
                 – AWProtocolService D-159                – Stammdaten Lieferant prüfen D-32
                 – ERP-WebService D-159                   – Stammdaten Preise prüfen D-38
                 Differenz                                – Stammdaten Produkt prüfen D-25
                 – Rechnungskontrolle D-251               – Stammdaten Währung prüfen D-162
                 Dokument                                 – Status D-41
                 – Bestellung D-45                        – Status für elektr. Dokument prüfen D-163
                 Dokumentation                            – Statuszuordnung D-41
                 – Arten D-12                             Einstellungen
                 Dokumente                                – Kisten-ID D-240
                 – Bestellanfrage D-186                   EK-Rückschreibung
                 – Bestellung D-188                       – Lagerbewertung D-145
                 – Einkauf D-185                          Elektr. Dokument
                 Dokumentenaustausch D-150                – Status D-160
                 – Dienste D-159                          Elektronische Rechnungskontrolle D-256
                 – openTRANS D-151                        Elektronischer Datenaustausch D-150
                 – Referenzen D-154                       – Anzeige D-223
                 – XML-Datei D-151                        – Dokumentenstatus D-217
                 Dokumentenimport D-155                   – EDI-Schnittstelle (Einstellungen) D-178
                 – Buchungsart D-156                      – Filtereinstellungen D-223
                 – Fußzuschläge/-rabatte D-157            – openTRANS-Einstellungen D-166
                 – openTRANS-Datei einlesen D-169         – Preiskontrolle D-213
                 – Positionszuordnung D-157               – Rechnungskontrolle D-256
                 – Rundungsdifferenz D-158                – Referenzen D-161
                 – XML-Datei einlesen D-169               – Schnittstellenverwaltung D-166
                 Dokumentenstatus D-217                   – Währungen D-162
                                                          Elektronischer Dokumentenaustausch
                                                          – Dienste D-159
                 E                                        – Firmendaten D-161
                 EDI                                      – Partnerstammdaten D-168
                 – Einstellungen für Datenexport D-178    – Position zuordnen D-221
                 – Export D-177                           Elektronisches Dokument
                 – Fremdschnittstellenverwaltung D-178    – Betragsdifferenz D-158
                 Eingangskontrolle D-241
3.30 / 04-2020




                                                          – Position zuordnen D-173
                 Einkauf                                  – prüfen D-170
                 – Anfrage D-110, D-186                   – Teillieferung erstellen D-172
                 – Beschaffungsart D-23                   – Zuschlag/Rabatt verteilen D-175


                 D-268                                                            A+W Business Einkauf
                 Partindex                                                                 Index Einkauf




                 Elektronsicher Dokumentenaustausch        K
                 – Statusdefinition D-163                  Kiste
                 ERP-WebService D-159                      – Etikett drucken D-142
                 Etikett                                   – Kisten-ID D-237
                 – für Kiste drucken D-142                 – virtuelle Positionsnummer D-238
                 Export                                    – Wareneingang D-136, D-230
                 – Bestellung D-195                        – Wareneingang erfassen D-138
                 – Datenexport per EDI D-193               Kistenbestellung
                 – Dokument (openTRANS) D-153              – virtuelle Positionsnummer D-47, D-136
                 – EDI-Einstellungen D-178                 Kisten-ID D-136
                 – Übertragungspool D-196                  – Einstellungen D-240
                 Externe Kundennummer D-168                Kontrolle
                                                           – elektronisches Dokument prüfen D-170
                 F                                         – Lieferantenpreise prüfen D-146
                 Firmendaten                               – Lieferantenrechnung D-245
                 – Einstellungen für Wareneingang D-126    – Mengendiskrepanzen D-243
                 – Referenzen D-161                        – unvollständige Lieferungen D-243
                 – virtuelle Positionsnummer D-47, D-136   – vollständige Lieferungen D-241
                 Fremdschnittstelle                        – Wareneingang D-133, D-241
                 – Export (EDI) D-193                      Kunde
                 – Übertragungs-Pool D-196                 – Individualpreis D-37
                 Fußzuschlag/-rabatt                       Kundenauftrag
                 – auf Bestellungen verteilen D-222        – Anfrage erzeugen D-112
                 – Importdokument D-157                    – Bestellposition erfassen D-54
                                                           – Bestellung D-51
                                                           – Bestellung erzeugen D-68
                 H
                                                           – Lieferant ändern D-56
                 Handlungsablauf
                 – Einkauf D-18
                                                           L
                                                           Lagerartikel
                 I
                                                           – Lagermaß D-27
                 Identnummer
                                                           Lagerbestellung
                 – Einstellungen D-240
                                                           – gemischte Bestellung erfassen D-83
                 – Kisten-ID D-237
                                                           – Kiste D-136, D-230
                 Identnummern
                                                           – Wareneingang D-121
                 – im Wareneingang D-137
                                                           Lagermaß
                 Importdokument
                                                           – in Stammdaten anlegen D-27
                 – Bestellungen D-218
                                                           – Lagerartikel D-27
                 – Buchungsart D-216, D-259
                                                           Lieferant
                 – Dokumentenstatus D-217, D-260
                                                           – AB erfassen D-89
                 – Filtereinstellung D-223
                                                           – für Auftragsposition D-52
                 – Positionen D-219
                                                           – im Bestellpool ändern D-72
                 – Positionszuordnung D-221
                                                           – in Bestellposition ändern D-56
                 – Preiskontrolle D-213
                                                           – Lieferung anmahnen D-97
                 – prüfen D-170
                                                           – Preis in AB prüfen D-93
                 – Rechnungskontrolle D-259
                                                           – Preise vergleichen D-74
                 Individualpreis D-37
                                                           – Preisvergleich D-65
                                                           – Sammel-AB erfassen D-95
                                                           – Stammdaten D-31
3.30 / 04-2020




                                                           Lieferanten mahnen D-225




                 A+W Business Einkauf                                                                D-269
                 Index Einkauf                                                                       Partindex




                 Lieferantenkartei D-31                          – importiertes Dokument D-216
                 – Standard-Lieferant D-33                       – Position D-210
                 Lieferantenkartei prüfen D-33                   – Positionsübersicht D-219
                 Lieferantenrechnung                             – Rechnungsdatum D-255
                 – importierte Rechnung prüfen D-170             – Stückliste D-212
                 – Kontrolle D-245                               Produktion
                 – prüfen D-146                                  – Meldung bei Wareneingang D-122
                 Liefertermin
                 – AB Lieferant D-203                            R
                 – ändern D-102, D-105                           Rechnung
                 – Bestellung D-87                               – abweichendes Datum D-255
                 – im Bestellpool ändern D-72                    – prüfen D-146
                 – in mehreren Dokumenten ändern D-108           Rechnungskontrolle D-245
                 – Kontrolle und Korrektur D-101                 – Bestellungen D-248
                 – Kunden benachrichtigen D-102                  – Buchungsart D-259
                 – prüfen D-105                                  – Differenz D-251
                 Lieferung                                       – Dokumentenstatus D-260
                 – buchen D-127                                  – Einkauf D-144
                 – Teilmenge D-235                               – elektr. Dokument D-256
                 – Wareneingang D-121                            – Fußzuschläge D-145
                 – Wareneingang mit AB D-199                     – importiertes Dokument D-259
                                                                 – Korrektur D-144
                 M                                               – Positionsübersicht D-251, D-262
                 Mahnung                                         – Stückliste D-253
                 – Lieferung D-97                                – Teilbestellung D-259
                 Mengendiskrepanzen                              – Teilrechnung D-259
                 – prüfen D-133                                  – Währung D-249
                 Modul                                           – Wechselkurs D-249
                 – Funktion D-11                                 Referenzen
                                                                 – beim Dokumentenimport D-154
                 O                                               Referenzierte Bestellung D-45
                 openTRANS D-151                                 Rundungsdifferenz D-158
                 – Dokumentenexport D-153                        – Produktzuordnung D-220
                 – Dokumentenimport D-155
                 – Einstellungen D-166                           S
                 – Preiskontrolle D-156                          Schnittstellenverwaltung
                 – XML-Datei D-155                               – Lieferantendaten prüfen D-178
                                                                 Stammdaten
                 P                                               – Firmendaten prüfen D-47, D-136, D-161
                 Position                                        – Lagermaß anlegen D-27
                 – im elektr. Dokument zuordnen   D-173, D-221   – Lieferantendaten prüfen D-32
                 – Referenzen D-157                              – Preisdaten prüfen D-38
                 Preis                                           – Produktdaten prüfen D-25
                 – in AB prüfen D-93                             – Status für elektr. Dokumente prüfen D-163
                 – Individualpreis D-37                          – Währung prüfen D-162
                 – Rechnung prüfen D-146                         Standard-Lieferant D-33
                 Preiskontrolle                                  Status
                 – Auftragsbestätigung D-204                     – Bestellungen D-41
                                                                 – elektronischer Dokumentenaustausch D-163
3.30 / 04-2020




                 – Bestellungen D-207
                 – EK-Rückschreibung D-145                       – Vergabe beim elektr. Dokumenten D-160
                 – elektr. Datei D-213                           – Vergabe beim Wareneingang D-42
                 – elektr. Dokument D-213                        – Wareneingang D-121


                 D-270                                                                  A+W Business Einkauf
                 Partindex                                                                         Index Einkauf




                 T                                              Z
                 Teillieferung                                  Zuschlag/Rabatt
                 – aus elektr. Dokument erstellen D-172         – auf Bestellungen verteilen   D-175
                 – Wareneingang D-123                           – Zuordnung D-157
                 – Wareneingang erfassen D-130
                 Terminüberwachung D-101

                 U
                 Überblick
                 – offene Lieferungen D-243
                 – Wareneingang D-133
                 Übergabe
                 – Bestellung D-68
                 Übermenge
                 – Wareneingang D-124
                 Unterposition
                 – Wareneingang Kiste D-237

                 V
                 Virtuelle Positionsnummer D-136, D-238
                 – Firmendaten D-47, D-136

                 W
                 Währung
                 – elektronischer Datenaustausch D-162
                 Wareneingang D-227
                 – Eingangskontrolle D-125
                 – Einstellung für ID D-137
                 – erfassen D-127
                 – ID für Kiste D-237
                 – Kiste D-136, D-230
                 – Kisten erfassen D-138
                 – komplett erfassen D-128
                 – komplette Bestellungen D-241
                 – kontrollieren D-133
                 – Lagerbestellung D-121
                 – Mengendiskrepanzen D-243
                 – Mengendiskrepanzen prüfen D-133
                 – mit automatischer Kisten-ID erfassen D-138
                 – mit manueller Kisten-ID D-141
                 – offene Bestellung suchen D-128
                 – ohne Lagerkennzeichen D-123
                 – Produktionsdatum D-136
                 – Status D-42, D-121
                 – Teillieferung D-123
                 – Teillieferung erfassen D-130
                 – Teilmenge D-235
                 – Übermenge D-124
3.30 / 04-2020




                 – Unterposition (Kisten) D-237
                 – unvollständige Lieferungen anzeigen D-133
                 – vollständig D-233
                 – Voreinstellungen prüfen D-126


                 A+W Business Einkauf                                                                    D-271
                 Index Einkauf               Partindex
3.30 / 04-2020




                 D-272           A+W Business Einkauf

