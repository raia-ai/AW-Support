---
title: "DE AWBusiness LogisticOptimizer 2.01"
category: "user_manuals"
product: "Unknown"
doc_type: "Unknown"
language: "EN"
tags: ["DE_AWBusiness_LogisticOptimizer_2.01"]
version: "1.0"
last_updated: "2025-12-10"
description: "Logistic Optimizer              I                                   Deutsch                          A+W Business                                                                                                            Vorspann                                             Vorspann                                         In diesem Teil der Dokumentation finden Sie editorische Notizen.                                           Revisionsübersicht                                         Part"
source_file: "DE_AWBusiness_LogisticOptimizer_2.01.pdf"
---


# DE AWBusiness LogisticOptimizer 2.01

Logistic Optimizer              I




                              Deutsch




                     A+W Business
                                                                                                           Vorspann




                                        Vorspann
                                        In diesem Teil der Dokumentation finden Sie editorische Notizen.


                                        Revisionsübersicht
                                        Part              Beschreibung
                                        Version/Datum

                                        1.00/05-2014      Ersterstellung

                                        2.00/10-2015      Komplette Überarbeitung

                                        2.01/01-2017      Produkt- und Firmennamen angepasst.



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
                                        nen Fehler nicht vollständig ausgeschlossen werden. Die A+W Software
                                        GmbH übernimmt keine Haftung für Fehler oder Ungenauigkeiten, es sei
                                        denn, diese beruhen auf vorsätzlichem oder grobfahrlässigem Handeln.
                                        Dieses Dokument beschreibt die volle Ausbaustufe der Stammdaten.

                                        Urheberrechte
                                        © 2017, A+W Software GmbH, alle Rechte, auch des Nachdrucks, der Her-
                                        stellung von Kopien und der Übersetzung, bleiben vorbehalten.
                                        Die Dokumentation darf nur gemäß dem Lizenzvertrag ganz oder in Teilen ko-
                                        piert, in einem Archivierungssystem gespeichert oder in irgendeiner anderen
                                        Form übertragen werden. Ohne die vorherige schriftliche Genehmigung der
2.01 / 01-2017




                                        A+W Software GmbH darf die Dokumentation weder elektronisch, mecha-
                                        nisch, per Aufzeichnung oder in sonstiger Form übertragen werden.




                 A+W Business Logistic Optmizer                                                                 I-3
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
2.01 / 01-2017




                 I-4                                                    A+W Business Logistic Optmizer
                                                                                                                                                             Inhalt




                                        Inhalt
                                        Vorspann ................................................................................................................. I-3
                                         Revisionsübersicht ............................................................................................... I-3
                                         Editorial ................................................................................................................ I-3

                                        Tutorial                                                                                                               I-9
                                        Überblick ................................................................................................................ I-11
                                          Dokumentation ................................................................................................... I-12
                                            Aufbau des Tutorials ....................................................................................... I-12
                                            Darstellungskonventionen ............................................................................... I-13
                                        Grundgedanken zu OTR ........................................................................................ I-14
                                          Datenbankverbindungen .................................................................................... I-15
                                              Verbindung zur OTR-Datenbank ................................................................. I-15
                                              Verbindung zur ERP-Datenbank ................................................................. I-15
                                          Der dynamische Modus ...................................................................................... I-17
                                          Die Oberfläche ................................................................................................... I-18
                                            Die Menü- und Symbolleisten ......................................................................... I-20
                                            Feldhilfe .......................................................................................................... I-27
                                        Administration ........................................................................................................ I-28
                                          Parameter ........................................................................................................... I-29
                                          Stammdaten ....................................................................................................... I-30
                                            Benutzer .......................................................................................................... I-31
                                            Status .............................................................................................................. I-32
                                              Die Status-Typen verwalten ........................................................................ I-33
                                            Kunden ............................................................................................................ I-34
                                              Die Kunden verwalten ................................................................................. I-35
                                            Abteilungen ..................................................................................................... I-37
                                              Die Abteilungen verwalten ........................................................................... I-37
                                            Fahrzeuge ....................................................................................................... I-39
                                              Die Fahrzeuge verwalten ............................................................................. I-40
                                            Fahrer ............................................................................................................. I-43
                                              Die Fahrer verwalten ................................................................................... I-44
                                            Reports ........................................................................................................... I-46
                                              Die Reports verwalten ................................................................................. I-47
                                            Datenimport .................................................................................................... I-49
                                        Planung .................................................................................................................. I-50
                                          Touren und Bestimmungsorte ............................................................................ I-51
                                            Allgemein ........................................................................................................ I-52
                                            Import .............................................................................................................. I-53
                                            Touren ............................................................................................................. I-54
                                              Eine gespeicherte Tour laden ...................................................................... I-54
                                              Eine gespeicherte Tour kopieren ................................................................. I-55
                                            Mit Touren arbeiten ......................................................................................... I-57
                                            Bestimmungsorte ............................................................................................ I-64
                                              Dokumente anzeigen ................................................................................... I-65
                                              Dokumente löschen ..................................................................................... I-65
                                              Positionen anzeigen .................................................................................... I-66
                                              Informationen anzeigen ............................................................................... I-67
                                              Die Detailansicht .......................................................................................... I-68
                                              Kundenadressen bearbeiten ....................................................................... I-70
                                              Mit Bestimmungsorten arbeiten ................................................................... I-71
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                                                                                  I-5
                 Inhalt




                            Kosten ................................................................................................................ I-74
                              Ausgaben ........................................................................................................ I-75
                              Variable Kosten ............................................................................................... I-75
                              Fixkosten ......................................................................................................... I-76
                              Tourkosten ...................................................................................................... I-76
                          Optimierung ........................................................................................................... I-77
                            Überblick ............................................................................................................ I-78
                              Touren optimieren ........................................................................................... I-79
                                Unterschiedliche Kartenmodi ....................................................................... I-82
                              Touren verändern ........................................................................................... I-83
                          Ergebnis ................................................................................................................. I-86
                            Überblick ............................................................................................................ I-87
                              Das Ergebnis der Optimierung ........................................................................ I-88
                                Touren ......................................................................................................... I-88
                                Tourenplan .................................................................................................. I-89
                                Bestimmungsort ........................................................................................... I-89
                              Tourstatus ändern ........................................................................................... I-90
                              Tatsächliche Tourkosten ................................................................................. I-91
                          Abfragen ................................................................................................................ I-93
                            Überblick ............................................................................................................ I-94
                              Unterschiedliche Abfragen .............................................................................. I-95
                              Touren ............................................................................................................. I-95
                                Filtern ........................................................................................................... I-95
                                Ändern und Status ....................................................................................... I-96
                                Löschen ....................................................................................................... I-96
                              Export .............................................................................................................. I-97
                                Export an Navigationssysteme .................................................................... I-97
                                Laden der Daten auf mobile Endgeräte (über die Cloud) ............................ I-99
                              Historie .......................................................................................................... I-104
                              Reports ......................................................................................................... I-105
                                Ausgewählte Tour ...................................................................................... I-105
                                Listen drucken ........................................................................................... I-106
                                Report Launcher ........................................................................................ I-107
                                Statistiken .................................................................................................. I-107
                                Eine Statistik erstellen ............................................................................... I-108
                              Ansicht .......................................................................................................... I-110
                                Tour ........................................................................................................... I-110
                                Bestimmungsort ......................................................................................... I-110
                                Kalender .................................................................................................... I-110
                              Routen Administrator .................................................................................... I-112

                          Softwarereferenz                                                                                                 I-115
                          Konfiguration ........................................................................................................ I-117
                            OTR-Verbindung .............................................................................................. I-118
                            ERP-Verbindung .............................................................................................. I-119
                            Parameter ......................................................................................................... I-120
                          Administration ...................................................................................................... I-129
                            Benutzer ........................................................................................................... I-130
                            Status ............................................................................................................... I-131
                            Kunden ............................................................................................................. I-133
                            Abteilungen ...................................................................................................... I-135
                            Fahrzeuge ........................................................................................................ I-136
                            Fahrer ............................................................................................................... I-139
2.01 / 01-2017




                            Reports ............................................................................................................. I-142
                            Datenimport ...................................................................................................... I-143
                          Planung ................................................................................................................ I-145
                            Eine gespeicherte Tour kopieren ..................................................................... I-147


                 I-6                                                                             A+W Business Logistic Optmizer
                                                                                                                                                              Inhalt




                                          Eine gespeicherte Tour laden .......................................................................... I-150
                                          Bestimmungsorte importieren .......................................................................... I-151
                                          Eine neue Tour zusammenstellen – Allgemein ................................................ I-152
                                          Geolokalisieren ................................................................................................. I-155
                                          Eine neue Tour zusammenstellen – Fahrzeuge ............................................... I-156
                                          Fahrzeug wählen .............................................................................................. I-159
                                          Fahrer hinzufügen ............................................................................................ I-160
                                          Eine neue Tour zusammenstellen – Parameter ............................................... I-162
                                          Tour-Faktoren ................................................................................................... I-166
                                          Eine neue Tour zusammenstellen – Kosten ..................................................... I-168
                                          Bereiche ........................................................................................................... I-170
                                          Fahrzeuge ........................................................................................................ I-171
                                          Bestimmungsort bearbeiten ............................................................................. I-172
                                          Zeitbereich ........................................................................................................ I-175
                                          Dokumente ....................................................................................................... I-176
                                          Positionen anzeigen ......................................................................................... I-177
                                          Informationen anzeigen .................................................................................... I-179
                                          Kunden ............................................................................................................. I-181
                                          Detailansicht ..................................................................................................... I-183
                                        Optimierung ......................................................................................................... I-184
                                          Tour optimieren ................................................................................................ I-185
                                        Ergebnis ............................................................................................................... I-187
                                          Ergebnis der Optimierung ................................................................................ I-188
                                          Tour-Informationen ........................................................................................... I-190
                                        Abfrage ................................................................................................................ I-192
                                          Routen filtern .................................................................................................... I-193
                                          Export ............................................................................................................... I-195
                                          Statusänderung ................................................................................................ I-197
                                          Historie ............................................................................................................. I-198
                                          Bestätigungs- und Lieferliste ............................................................................ I-200
                                          Report Launcher ............................................................................................... I-203
                                          Statistik ............................................................................................................. I-204
                                            Register Allgemein ........................................................................................ I-204
                                            Register Allgemeine Grafik ........................................................................... I-205
                                            Register Fahrzeuge ...................................................................................... I-206
                                            Register Fahrer ............................................................................................. I-207
                                            Register Abteilungen ..................................................................................... I-208
                                            Register Kunden ........................................................................................... I-209
                                          Kalender ........................................................................................................... I-210

                                        Partindex                                                                                                         I-211
                                        Index .................................................................................................................... I-213
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                                                                                   I-7
                 Inhalt
2.01 / 01-2017




                 I-8      A+W Business Logistic Optmizer
Logistic Optimizer               I

                            Tutorial




                     A+W Business
                 Tutorial                                                                                    Überblick




                                        Überblick
                                        Der A+W Logistic Optimizer (auch OTR genannt - Optimizer of Transport Rou-
                                        tes) beschäftigt sich mit den Grundlagen der Touren- und Routenplanung. Das
                                        Tutorial baut auf den Kenntnissen zu den Stammdaten und zum Nummernver-
                                        walter auf.

                                            Funktionen sind von den freigeschalteten Modulen abhängig
                                            Bitte beachten Sie, dass die unterschiedlichen Funktionen nur dann zur
                                            Verfügung stehen, wenn die zugehörigen Module und Schnittstellen instal-
                                            liert und freigeschaltet sind.

                                            Wenn Sie in dieser Beschreibung Funktionen finden, die in Ihrer Installati-
                                            on nicht zugänglich sind, wenden Sie sich bitte an die A+W Software
                                            GmbH.

                                        Themenblöcke
                                        In diesem Tutorial finden Sie folgende Themenblöcke:
                                        •   Grundgedanken zu OTR
                                        •   Administration
                                        •   Touren planen
                                        •   Touren optimieren
                                        •   Ergebnisse prüfen
                                        •   Abfragen

                                        Vorausgesetzte Kenntnisse
                                        Das Tutorial richtet sich an Teilnehmer, die in OTR Aufträge zur Auslieferung
                                        vorbereiten und im Büro die Lieferung mittels verschiedener LKW überwa-
                                        chen. Die Teilnehmer müssen das Konzept der Stammdaten und des Num-
                                        mernverwalters kennen.
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                                   I-11
                 Überblick                                                                              Tutorial




                             Dokumentation
                             Für das Modul OTR stehen folgende Dokumente zur Verfügung:

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
2.01 / 01-2017




                 I-12                                                       A+W Business Logistic Optmizer
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
                                                                 Fertigung > Produktion > Produktionsübergabe.

                                        []                       Eckige Klammern bezeichnen Schaltflächen im Dialog,
                                                                 z. B.: Mit [OK] speichern Sie die Daten.

                                        <>                       Spitze Klammern bezeichnen Tasten oder
                                                                 Tastenkombinationen auf der Tastatur, z. B.: Mit <F1>
                                                                 öffnen Sie die Online-Hilfe.
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                                        I-13
                 Grundgedanken zu OTR                                                                         Tutorial




                                        Grundgedanken zu OTR
                                        Durch eine sinnvolle Routenoptimierung und Tourenplanung im Transportbe-
                                        reich können Fahrtzeiten und Fahrwege verkürzt und damit der Kraftstoffver-
                                        brauch erheblich vermindert werden. In der Folge werden die
                                        Umweltbelastungen reduziert, Fahrzeuge werden weniger abgenutzt und die
                                        Fahrer werden durch weniger überflüssig gefahrene Kilometer entlastet.
                                        Sowohl eine Tourenplanung als auch eine Routenoptimierung spart also Kos-
                                        ten und erhöht die Produktivität.
                                        Der Optimizer for Transport Routes (OTR) bringt Ihre Zielorte, Kundenadres-
                                        sen oder Haltepunkte in eine sinnvolle und effiziente Reihenfolge.
                                        Diese Reihenfolge berücksichtigt neben dem individuellen Fuhrpark auch die
                                        hinterlegten Streckenanforderungen, wie z. B. Tunnel oder Mautstraßen. Die
                                        Technik basiert auf Nokia Maps in Kombination mit einem mathematischen Al-
                                        gorithmus.
                                        Über die mobile App können Lieferungen durch den Fahrer direkt verbucht
                                        und zurückgemeldet werden. Weiterhin erhält der Fahrer alle notwendigen In-
                                        formationen über die Gesamtstrecke und einzelne Ladestationen.
                                        Via GPS können Sie im Büro die Lieferung überwachen.
                                        Der Prozessablauf stellt sich wie folgt dar:


                                            Planung       Optimierung    Ergebnis



                                        Abb. I-1      Standardprozess für die Lieferreihenfolge


                                        Der Prozess gliedert sich in vier Phasen:
                                        •   Planung: In dieser Phase stellen Sie die Tour(en) zusammen. Sie können
                                            neue Touren erstellen, vorhandene Touren bearbeiten oder auch löschen.
                                            Innerhalb der Touren können Sie Bestimmungsorte (Haltepunkte) hinzufü-
                                            gen, bearbeiten oder aber auch einzelne Orte löschen. In dieser Phase ha-
                                            ben Sie ebenfalls Zugriff auf die einzelnen Positionen, um sich einen
                                            Überblick zu verschaffen.
                                        •   Optimierung: In dieser Phase findet die Optimierung der Strecke statt. Auf
                                            der Übersichtskarte sehen Sie die Streckenführung und auf der rechten
                                            Seite die Auflistung der einzelnen Stationen (Wegpunkte). Sie können ein-
                                            zelne Stationen miteinander tauschen und haben Zugriff auf die Optimie-
                                            rungs-Faktoren.
                                            In der Optimierung werden auch Einstellungen und Änderungen aus der
                                            Phase der Planung berücksichtigt - bspw. spezielle Abladezeiten oder Pri-
                                            oritäten von Kunden (Ladestationen).
                                        •   Ergebnis: Diese Phase liefert Ihnen das Gesamtergebnis der Tour geglie-
                                            dert in die einzelnen Touren, den grafischen Tourenplan sowie die Über-
                                            sicht der Bestimmungsorte.
2.01 / 01-2017




                 I-14                                                                  A+W Business Logistic Optmizer
                 Tutorial                                                                      Grundgedanken zu OTR




                                        Datenbankverbindungen
                                        Um mit dem Modul arbeiten zu können, müssen Verbindungen zu den beiden
                                        folgenden Datenbanken bestehen:
                                        •   OTR
                                        •   ERP

                                        Verbindung zur OTR-Datenbank
                                        Die Verbindung zum OTR-Datenbank-Server ist nötig, um die Routen zu pla-
                                        nen.




                                        Abb. I-2      Datenbank-Einstellungen OTR


                                        Beim erstmaligen Aufruf erscheint dieser Dialog automatisch. Geben Sie im
                                        Feld Datenquelle den Pfad zum OTR-Datenbankserver ein. Diese Informatio-
                                        nen erhalten Sie von Ihrem zuständigen Ansprechpartner im A+W Support
                                        oder Qualified Service.
                                        Im Feld Start-Katalog geben Sie die Standard-Datenbank ein. Diese ist OTR.
                                        Die Einträge für Benutzer-ID und Kennwort erhalten Sie ebenfalls von Ihrem
                                        zuständigen Ansprechpartner im A+W Support oder Qualified Service.
                                        Nachdem Sie die Einstellungen vorgenommen haben, können Sie über die
                                        Symbol-Schaltfläche [Test] eine Testverbindung zur Datenbank aufbauen.

                                            Datenbankverbindung
                                            Bitte beachten Sie, dass diese Einstellungen für jeden Benutzer vorgenom-
                                            men werden müssen.


                                        Ergänzende Informationen
                                         Softwarereferenz, “OTR-Verbindung” auf Seite I-134

                                        Verbindung zur ERP-Datenbank
2.01 / 01-2017




                                        Die Verbindung zum ERP-Datenbank-Server ist nötig, damit das Modul auf die
                                        Daten von A+W Business zugreifen kann.



                 A+W Business Logistic Optmizer                                                                 I-15
                 Grundgedanken zu OTR                                                                        Tutorial




                                        Abb. I-3     Datenbank-Einstellungen ERP


                                        Beim erstmaligen Aufruf erscheint dieser Dialog automatisch mit dem Register
                                        OTR-Datenbank. Wechseln Sie in das Register ERP-Verbindung.
                                        Im Feld Start-Katalog geben Sie die Standard-Datenbank ein. Die Einträge für
                                        Benutzer-ID und Kennwort erhalten Sie ebenfalls von Ihrem zuständigen An-
                                        sprechpartner im A+W Support oder Qualified Service.
                                        Nachdem Sie die Einstellungen vorgenommen haben, können Sie über die
                                        Symbol-Schaltfläche [Test] eine Testverbindung zur Datenbank aufbauen.

                                           Datenbankverbindung
                                           Bitte beachten Sie, dass diese Einstellungen für jeden Benutzer vorgenom-
                                           men werden müssen.


                                        Ergänzende Informationen
                                         Softwarereferenz, “OTR-Verbindung” auf Seite I-134
2.01 / 01-2017




                 I-16                                                                A+W Business Logistic Optmizer
                 Tutorial                                                                      Grundgedanken zu OTR




                                        Der dynamische Modus
                                        Arbeiten Sie im dynamischen Modus, erscheint, nachdem Sie im Nummern-
                                        verwalter die Symbol-Schaltfläche angeklickt haben, folgender Dialog:




                                        Abb. I-4     Dynamischer Modus, Anzahl Liefergebiete


                                        An dieser Stelle fasst OTR die Bestimmungsorte anhand der Koordinaten un-
                                        ter Berücksichtigung des Gewichtes zu Liefergebieten (Gruppen) zusammen
                                        und es findet bereits die Geolokalisation statt.
                                        Das Feld Anzahl der Liefergebiete zeigt Ihnen, in wie viele Gruppen OTR die
                                        einzelnen Bestimmungsorte zusammengefasst hat.
                                        Sie können diesen Wert akzeptieren, ihn aber auch überschreiben. Wenn Sie
                                        ihn überschreiben, findet im Hintergrund eine neue Berechnung gemäß des
                                        neuen Wertes statt.

                                           Geolokalisation im dynamischen Modus
                                           Wurden alle Adressen erfolgreich lokalisiert, entfällt die Phase Geolokali-
                                           sation im OTR.

                                        Nachdem Sie die Schaltfläche [OK] angeklickt haben, erscheint der Dialog
                                        Fahrzeug wählen.
2.01 / 01-2017




                                        Abb. I-5     Dynamischer Modus, Fahrzeug wählen




                 A+W Business Logistic Optmizer                                                                   I-17
                 Grundgedanken zu OTR                                                                           Tutorial




                                         Dieser Dialog liefert Ihnen einen Überblick zu den einzelnen Fahrzeugen, die
                                         im System angelegt sind. Sie können entweder bestimmte Fahrzeuge aus-
                                         wählen (nur eigene LKWs oder auch Speditionen) oder Alle. Wählen Sie alle
                                         Fahrzeuge aus, bieten Sie dem System die Freiheit, die Aufträge optimal auf
                                         die LKWs zu verteilen. Aktivieren Sie die Checkbox Maximale Beladung und
                                         Zeit vor Ort, dann wird sowohl die maximale Beladung des Fahrzeugs berück-
                                         sichtigt, die Sie in den Stammdaten hinterlegt haben als auch die beim Kunden
                                         hinterlegte Zeit.
                                         Klicken Sie auf [OK], erscheint folgende Anzeige:




                 Abb. I-6   Oberfläche nach dem Start


                                         Mit den oben genannten Eingaben nimmt OTR die entsprechenden Berech-
                                         nungen vor. Auf der linken Seite sehen Sie die Karte mit den einzelnen Grup-
                                         pen, die angefahren werden. Rechts oben sehen Sie die Touren und darunter
                                         die Bestimmungsorte.
                                         Die Nummer, die in den Feldern Gruppen zu sehen ist, ist identisch mit der
                                         entsprechenden Nummer auf der Karte (s.o.).
                                         Die Symbol-Schaltfläche [Liefergebiete] beinhaltet die Menüeinträge:
                                         •   Hierarchisch
                                         •   EM
2.01 / 01-2017




                                         Dabei handelt es sich um zwei Berechnungsarten, die zu verschiedenen Er-
                                         gebnissen führen. Welchen Modus Sie verwenden, hängt davon ab, wie viele
                                         Liefergebiete und wie viele Bestimmungsorte angefahren werden.


                 I-18                                                               A+W Business Logistic Optmizer
                 Tutorial                                                                   Grundgedanken zu OTR




                                        Um dies zu verdeutlichen, haben wir im Anschluss 94 Bestimmungsorte in un-
                                        terschiedlich viele Liefergebiete aufgeteilt und das Ergebnis beider Modi ab-
                                        gebildet:




                                        Werden diese Bestimmungsorte in drei Liefergebiete aufgeteilt, ist das Ergeb-
                                        nis wie folgt:




                                        A Hierarchische Modus                 B EM Modus (empfohlen)


                                        Werden diese Bestimmungsorte in vier Liefergebiete aufgeteilt, ist das Ergeb-
                                        nis wie folgt:
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                                 I-19
                 Grundgedanken zu OTR                                                                         Tutorial




                                        A Hierarchische Modus                  B EM Modus (empfohlen)


                                        Werden diese Bestimmungsorte in sechs Liefergebiete aufgeteilt, ist das Er-
                                        gebnis wie folgt:




                                        A Hierarchische Modus (empfohlen)      B EM Modus


                                        Werden diese Bestimmungsorte in neun Liefergebiete aufgeteilt, ist das Er-
                                        gebnis wie folgt:




                                        A Hierarchische Modus (empfohlen)      B EM Modus


                                        Erfahrungsgemäß liefert der EM Modus bei einer geringen Anzahl von Liefer-
                                        gebieten eine effizientere Aufteilung der Bestimmungsorte. Haben Sie jedoch
                                        eine große Anzahl von Liefergebieten, dann liefert der hierarchische Modus
                                        eine effizientere Aufteilung.
                                        Mithilfe der Menüeinträge Hierarchisch und EM können Sie die Aufteilung je-
                                        derzeit simulieren und sich dann für das passende Ergebnis entscheiden.
2.01 / 01-2017




                                           Berechnung der Liefergebiete
                                           Die Aufteilung in Liefergebiete erfolgt immer unter Berücksichtigung der in
                                           den Stammdaten hinterlegten Werte je Fahrzeug.



                 I-20                                                               A+W Business Logistic Optmizer
                 Tutorial                                                                   Grundgedanken zu OTR




                                        Das Register Tour-Informationen liefert Ihnen einen Überblick zu der LKW-La-
                                        dung, den Gewichten und der jeweiligen Tour-Zeit.
                                        Der Fortschritt-Balken in der Spalte Status zeigt Ihnen, zu welchem Prozent-
                                        satz der LKW beladen ist.
                                        Nächster Schritt:
                                        •   Optimierung, Seite I-88


                                        Ergänzende Informationen
                                         Softwarereferenz, “Bereiche” auf Seite I-189
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                                 I-21
                 Grundgedanken zu OTR                                                                           Tutorial




                                          Die Oberfläche
                                          Das Modul OTR öffnen Sie, indem Sie im Nummernverwalter die Symbol-
                                          Schaltfläche [OTR] betätigen.
                                          Wenn Sie OTR gestartet haben, stellt sich das Modul wie folgt dar:


                 A
                 B
                 C

                                                                                                                        F




                                                                                                                        G




                 D




                 E
                                                                                                                        H

                 A Menüleiste                      D Karte                            G Übersicht der Bestimmungsorte
                 B Symbolleiste                    E Kartenwerkzeuge                  H Schaltfläche
                 C Prozess-Darstellung             F Übersicht der Touren
                 Abb. I-7    Oberfläche nach dem Start


                                          Im oberen Bereich befinden sich jeweils von links nach rechts die Menüleiste
                                          (A), die Symbolleiste (B) sowie die Darstellung des Gesamtprozesses (C) von
                                          der Planung bis zur Datenübertragung und -auswertung. Mittels des Wizards
                                          ist es möglich, den Gesamtprozess (Planung, Geolokalisierung, etc.) mit we-
                                          nigen Eingaben zu durchlaufen.
                                          Über die Symbol-Schaltflächen [Weiter] gehen Sie im Prozess einen Schritt
                                          weiter. Bitte beachten Sie, dass Sie nur dann weitergehen können, wenn im
                                          jeweiligen Prozess-Schritt keine Fehler aufgetreten sind. Beispiel: Im Bereich
                                          Geolokalisierung können Sie nur dann einen Schritt weiter gehen, wenn alle
                                          Bestimmungsorte lokalisiert werden konnten.
                                          Über die Symbol-Schaltfläche [Zurück] gehen Sie im Prozess einen Schritt zu-
                                          rück.
                                          Es werden am Ende des Prozesses die Optimierungsergebnisse angezeigt
2.01 / 01-2017




                                          und Sie können entscheiden, ob Sie die Route und Optimierungsergebnisse
                                          so akzeptieren (speichern) oder mit anderen Einstellungen wiederholen, um
                                          ein besseres Ergebnis zu erzielen.



                 I-22                                                                 A+W Business Logistic Optmizer
                 Tutorial                                                                      Grundgedanken zu OTR




                                        Die Karte (D) zeigt Ihnen die zu Bereichen zusammengefassten Bestim-
                                        mungsorte. Darunter befinden sich die Werkzeuge zum Bearbeiten der Touren
                                        auf der Karte (E). Im Bereich der Touren (F) befinden sich alle anstehenden
                                        Touren und im Bereich der Bestimmungsorte (G) werden Ihnen die einzelnen
                                        Anfahrpunkte aufgelistet. Die Schaltfläche (H) führt Sie im Prozess jeweils ei-
                                        nen Schritt weiter.
                                        Unterhalb der Karte befinden sich folgende Werkzeuge:




                                        Erläuterung der einzelnen Symbole
                                        Im Anschluss finden Sie eine Auflistung der Symbol-Schaltflächen und ihre
                                        Bedeutung.

                                        Symbol               Erläuterung

                                                             Menü
                                                             Wenn Sie diese Symbol-Schaltfläche aktivieren, können Sie
                                                             mithilfe der <Strg>-Taste einen oder mehrere
                                                             Bestimmungsorte auswählen. Diese werden dann in Rot
                                                             angezeigt. Es öffnet sich ein Popup-Menü mit Aktionen, die
                                                             Sie an dieser Stelle ausführen können.

                                                             Bestimmungsorte
                                                             Wenn Sie diese Symbol-Schaltfläche aktivieren, bekommen
                                                             Sie auf der Karte die letzten beiden Ziffern der Tour-ID
                                                             angezeigt.
                                                             Ist die Symbol-Schaltfläche nicht aktiv, werden Ihnen die
                                                             Nummern der Liefergebiete angezeigt.

                                                             Bereiche
                                                             Mittels dieser Symbol-Schaltfläche werden die außen
                                                             liegenden Bestimmungsorte durch Linien verbunden.

                                                             Bereiche
                                                             Mittels dieser Symbol-Schaltfläche werden die Lieferbereiche
                                                             kreisförmig dargestellt.

                                                             Informationen
                                                             Mittels dieser Symbol-Schaltfläche blenden Sie
                                                             Streckeninformationen (Nokia Maps) ein oder aus.

                                                             Optimierte Tour
                                                             Nach erfolgter Optimierung können Sie die Route mit dieser
                                                             Symbol-Schaltfläche ein- und ausblenden.

                                                             Bestimmungsorte
                                                             Mittels dieser Symbol-Schaltfläche blenden Sie die
                                                             Bestimmungsorte ein oder aus.
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                                      I-23
                 Grundgedanken zu OTR                                                                             Tutorial




                                        Symbol              Erläuterung

                                                            Zoom
                                                            Mittels dieser Symbol-Schaltfläche wird die Karte vergrößert.
                                                            Die Bereiche Touren und Bestimmungsorte werden
                                                            ausgeblendet. Ein erneuter Klick auf die Symbol-Schaltfläche
                                                            blendet die Bereich Touren und Bestimmungsorte wieder ein
                                                            und verkleinert die Karte.

                                        Aktivieren Sie die Symbol-Schaltfläche Menü, halten Sie die <Strg> Taste ge-
                                        drückt und klicken Sie auf einen Bestimmungsort. Es öffnet sich folgendes Me-
                                        nü:




                                        Mithilfe dieses Menüs können Sie z. B. Liefergebiete zusammenlegen. Dazu
                                        halten Sie die <Strg>-Taste gedrückt und klicken Sie den Bestimmungsort an,
                                        den Sie verschieben möchten. Das Menü öffnet sich und Sie klicken in dem
                                        Menü das Liefergebiet an, in das der Bestimmungsort verschoben werden
                                        soll. Das Menü schließt sich und der Bestimmungsort befindet sich in dem ge-
                                        wünschten Liefergebiet.
                                        Sie können auch ganz einfach einen Bestimmungsort löschen, indem Sie mit
                                        gedrückter <Strg>-Taste diesen markieren. Im Menü ist dann dieser Bestim-
                                        mungsort im Bereich Bestimmungsort löschen zu finden. Klicken Sie ihn an,
                                        wird er gelöscht.

                                            Bestimmungsort löschen
                                            Wenn Sie einen Bestimmungsort löschen, wird zum jetzigen Programm-
                                            stand der Status für diesen Auftrag (Aufträge) im ERP-System nicht geän-
                                            dert. Für die anderen Aufträge hingegen schon (geplant, optimiert,
                                            freigegeben, etc.)

                                        Im Bereich Bestimmung können Sie dem Bestimmungsort als Priorität kenn-
                                        zeichnen oder ihm einen anderen Punkt zuweisen. Folgende Punkte sind
                                        möglich:
                                        •   Ausgangspunkt
                                        •   Mittelpunkt
                                        •   Endpunkt
2.01 / 01-2017




                 I-24                                                                A+W Business Logistic Optmizer
                 Tutorial                                                                Grundgedanken zu OTR




                                        Ergänzende Informationen
                                         “Die Menü- und Symbolleisten” auf Seite I-26
                                         “Feldhilfe” auf Seite I-33
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                          I-25
                 Grundgedanken zu OTR                                                                               Tutorial




                                        Die Menü- und Symbolleisten
                                        Die Menüleiste beinhaltet die für den Anwender wichtigsten Funktionen. Die
                                        einzelnen Menüs können per Mausklick geöffnet werden. Einige Menüpunkte
                                        können mit Hilfe von Tastenkombinationen (Bsp.: <Strg>+<S> = Starten) di-
                                        rekt geöffnet werden.




                                        Der Bereich Starten beinhaltet folgende Symbol-Schaltflächen:




                                        Erläuterung der einzelnen Symbole
                                        Im Anschluss finden Sie eine Auflistung der Symbol-Schaltflächen und ihre
                                        Bedeutung.

                                        Symbol              Erläuterung

                                                            Schließen
                                                            Mittels dieser Symbol-Schaltfläche schließen Sie das Modul.

                                                            Überprüfen Sie den Service
                                                            Mittels dieser Symbol-Schaltfläche überprüfen Sie die
                                                            Verbindung zum Service.

                                                            Logbuch
                                                            Mittels dieser Symbol-Schaltfläche öffnen Sie das Logbuch,
                                                            welches die täglichen Ereignisse protokolliert.

                                                            Hilfe
                                                            Mittels dieser Symbol-Schaltfläche starten Sie die A+W
                                                            Business-Hilfe.

                                                            Über A+W Business
                                                            Mittels dieser Symbol-Schaltfläche öffnen Sie den Dialog mit
                                                            Informationen zu der Version und dem Lizenzschlüssel.


                                        Der Bereich Ansicht beinhaltet folgende Einträge:
2.01 / 01-2017




                                        Über die einzelnen Einträge können Sie das Erscheinungsbild von OTR ein-
                                        stellen.
                                        Der Bereich Konfiguration beinhaltet folgende Symbol-Schaltflächen:


                 I-26                                                                A+W Business Logistic Optmizer
                 Tutorial                                                                      Grundgedanken zu OTR




                                        Erläuterung der einzelnen Symbole
                                        Im Anschluss finden Sie eine Auflistung der Symbol-Schaltflächen und ihre
                                        Bedeutung.

                                        Symbol              Erläuterung

                                                            Einstellungen
                                                            Mittels dieser Symbol-Schaltfläche haben Sie Zugriff auf die
                                                            Datenbankeinstellungen. Es öffnet sich der Dialog
                                                            Einstellungen.

                                                            Parameter
                                                            Mittels dieser Symbol-Schaltfläche haben Sie Zugriff auf die
                                                            Parameter. Es öffnet sich der Dialog Parameter.

                                                            Import/Export
                                                            Mittels dieser Symbol-Schaltfläche können Sie zu
                                                            Sicherungszwecken die Parameter im XML-Format
                                                            exportieren.

                                                            Sprache
                                                            Mittels dieser Kombobox wählen Sie die Programm-Sprache
                                                            für OTR aus.


                                        Der Bereich Administration beinhaltet folgende Symbol-Schaltflächen:




                                        Erläuterung der einzelnen Symbole
                                        Im Anschluss finden Sie eine Auflistung der Symbol-Schaltflächen und ihre
                                        Bedeutung.

                                        Symbol              Erläuterung

                                                            Benutzer
                                                            Mittels dieser Symbol-Schaltfläche haben Sie Zugriff auf die
                                                            Benutzer. Es öffnet sich der Dialog Benutzer.

                                                            Status
                                                            Mittels dieser Symbol-Schaltfläche haben Sie Zugriff auf die
                                                            Status. Es öffnet sich der Dialog Status.
2.01 / 01-2017




                                                            Kunden
                                                            Mittels dieser Symbol-Schaltfläche können Sie auf die
                                                            Kunden zugreifen. Es öffnet sich der Dialog Kunden.



                 A+W Business Logistic Optmizer                                                                      I-27
                 Grundgedanken zu OTR                                                                                Tutorial




                                        Symbol              Erläuterung

                                                            Abteilungen
                                                            Mittels dieser Symbol-Schaltfläche können Sie auf die
                                                            Abteilungen zugreifen. Es öffnet sich der Dialog Abteilungen.

                                                            Fahrzeuge
                                                            Mittels dieser Symbol-Schaltfläche können Sie auf Ihren
                                                            Fuhrpark zugreifen. Es öffnet sich der Dialog Fahrzeuge.

                                                            Fahrer
                                                            Mittels dieser Symbol-Schaltfläche können Sie auf Ihre
                                                            Fahrer zugreifen. Es öffnet sich der Dialog Fahrer.

                                                            Reports
                                                            Mittels dieser Symbol-Schaltfläche können Sie auf die
                                                            Reports zugreifen. Es öffnet sich der Dialog Reports.

                                                            Packmittel-Typen
                                                            Mittels dieser Symbol-Schaltfläche können Sie auf die
                                                            Packmittel zugreifen. Es öffnet sich der Dialog Packmittel-
                                                            Typen.

                                                            Datenimport
                                                            Mittels dieser Symbol-Schaltfläche können Sie Daten im
                                                            CSV-Format importieren. Es öffnet sich der Dialog
                                                            Datenimport.

                                        Der Bereich Abfrage beinhaltet folgende Symbol-Schaltflächen:




                                        Erläuterung der einzelnen Symbole
                                        Im Anschluss finden Sie eine Auflistung der Symbol-Schaltflächen und ihre
                                        Bedeutung.

                                        Symbol              Erläuterung

                                                            Filtern.
                                                            Mittels dieser Symbol-Schaltfläche können Sie nach
                                                            einzelnen Routen filtern. Es öffnet sich der Dialog Filter
                                                            Routen.

                                                            Tour bearbeiten
                                                            Mittels dieser Symbol-Schaltfläche können Sie den Tour-
                                                            Status und die tatsächlichen Kosten ändern. Es öffnet sich
                                                            der Dialog Tour bearbeiten.

                                                            Tour löschen
                                                            Mittels dieser Symbol-Schaltfläche können Sie eine zuvor
                                                            ausgewählte Tour löschen.
2.01 / 01-2017




                 I-28                                                                 A+W Business Logistic Optmizer
                 Tutorial                                                                       Grundgedanken zu OTR




                                        Symbol              Erläuterung

                                                            Tour exportieren
                                                            Mittels dieser Symbol-Schaltfläche können Sie die Daten an
                                                            ein Navigationssystem exportieren. Es öffnet sich der Dialog
                                                            Export.

                                                            Status ändern
                                                            Mittels dieser Symbol-Schaltfläche können Sie den Status
                                                            einer Tour ändern. Es öffnet sich der Dialog Statusänderung.

                                                            Historie
                                                            Mittels dieser Symbol-Schaltfläche können Sie sich die
                                                            Dokumenten-Historie anzeigen lassen. Es öffnet sich der
                                                            Dialog Historie.

                                                            Ausgewählte Tour
                                                            Mittels dieser Symbol-Schaltfläche öffnet sich der Crystal
                                                            Report Bestätigungs- und Lieferliste für die ausgewählte
                                                            Tour.

                                                            Report Launcher
                                                            Mittels dieser Symbol-Schaltfläche öffnet sich der Dialog
                                                            Report Launcher für die ausgewählte Tour.

                                                            Statistik
                                                            Mittels dieser Symbol-Schaltfläche öffnet sich der Dialog
                                                            Statistik für die ausgewählte Tour.

                                                            Siehe Tour
                                                            Mittels dieser Symbol-Schaltfläche öffnet sich der Dialog
                                                            Tour.

                                                            Siehe Bestimmungsort
                                                            Mittels dieser Symbol-Schaltfläche öffnet sich der Dialog
                                                            Bestimmungsort.

                                                            Kalender
                                                            Mittels dieser Symbol-Schaltfläche öffnet sich der Dialog
                                                            Kalender. Der Kalender zeigt Ihnen die gefahrenen Touren
                                                            nach Fahrzeugen und Fahrer.

                                                            Routen Administrator
                                                            Dieser Eintrag dient dem Online-Tracking der Touren, die
                                                            gerade gefahren werden.

                                                            Dateien anhängen
                                                            Mittels dieser Symbol-Schaltfläche können Sie einer Route,
                                                            einem Bestimmungsort oder Dokument einen Dateipfad
                                                            zufügen.


                                        Die Symbolleiste der Planungs-Phase
                                        Die Symbolleiste der Planungs-Phase beinhaltet den Zugriff auf alle Funktio-
                                        nen bzw. Dialoge, die in dieser Phase von Bedeutung sind.
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                                          I-29
                 Grundgedanken zu OTR                                                                               Tutorial




                                        Erläuterung der einzelnen Symbole
                                        Im Anschluss finden Sie eine Auflistung der Symbol-Schaltflächen und ihrer
                                        Bedeutung.

                                        Symbol              Erläuterung

                                                            Gespeicherte Tour kopieren.
                                                            Mittels dieser Symbol-Schaltfläche können Sie eine
                                                            gespeicherte Tour kopieren. Es öffnet sich der Dialog
                                                            Gespeicherte Touren.

                                                            Gespeicherte Tour laden.
                                                            Mittels dieser Symbol-Schaltfläche können Sie einer neuen
                                                            Tour eine gespeicherte Tour hinzufügen. Es öffnet sich der
                                                            Dialog Gespeicherte Tour-Liste.

                                                            Bestimmungsorte importieren.
                                                            Mittels dieser Symbol-Schaltfläche können Sie
                                                            Bestimmungsorte importieren. Es öffnet sich der Dialog
                                                            Datenimport.

                                                            Neue Tour
                                                            Mittels dieser Symbol-Schaltfläche können Sie eine neue
                                                            Tour zusammenstellen. Es öffnet sich der Dialog Tour.

                                                            Tour bearbeiten
                                                            Mittels dieser Symbol-Schaltfläche können Sie eine zuvor
                                                            ausgewählte Tour bearbeiten.

                                                            Tour löschen
                                                            Mittels dieser Symbol-Schaltfläche können Sie eine zuvor
                                                            ausgewählte Tour löschen.

                                                            Gruppen
                                                            Mittels dieser Symbol-Schaltfläche können können Sie die
                                                            Touren in Bereiche unterteilen.

                                                            Fahrzeuge
                                                            Mittels dieser Symbol-Schaltfläche können Sie der Tour ein
                                                            anderes Fahrzeug zuweisen. Es öffnet sich der Dialog
                                                            Fahrzeug wählen.

                                                            Neuer Bestimmungsort
                                                            Mittels dieser Symbol-Schaltfläche können Sie einer Tour
                                                            einen neuen Bestimmungsort hinzufügen. Es öffnet sich der
                                                            Dialog Bestimmungsort.

                                                            Bestimmungsort bearbeiten
                                                            Mittels dieser Symbol-Schaltfläche können Sie einen zuvor
2.01 / 01-2017




                                                            ausgewählten Bestimmungsort bearbeiten. Es öffnet sich der
                                                            Dialog Bestimmungsort bearbeiten.




                 I-30                                                                A+W Business Logistic Optmizer
                 Tutorial                                                                      Grundgedanken zu OTR




                                        Symbol              Erläuterung

                                                            Bestimmungsort löschen
                                                            Mittels dieser Symbol-Schaltfläche können Sie einen zuvor
                                                            ausgewählten Bestimmungsort löschen.

                                                            Packmittel
                                                            Mittels dieser Symbol-Schaltfläche öffnen Sie das Register
                                                            Packmittel.

                                                            Detailansicht
                                                            Mittels dieser Symbol-Schaltfläche erhalten Sie eine
                                                            Detailansicht zu den Bestimmungsorten einer Tour.

                                                            Initialisieren
                                                            Mittels dieser Symbol-Schaltfläche kehren Sie zur
                                                            Ausgangssituation zurück. Haben Sie z. B. Datensätze
                                                            gruppiert und möchten dies rückgängig machen, dann
                                                            klicken Sie auf diese Schaltfläche.


                                        Die Symbolleiste der Optimierungs-Phase
                                        Die Symbolleiste der Optimierungs-Phase beinhaltet den Zugriff auf alle Funk-
                                        tionen bzw. Dialoge, die in dieser Phase von Bedeutung sind.




                                        Erläuterung der einzelnen Symbole
                                        Im Anschluss finden Sie eine Auflistung der Symbol-Schaltflächen und ihrer
                                        Bedeutung.

                                        Symbol              Erläuterung

                                                            Tour optimieren
                                                            Mittels dieser Symbol-Schaltfläche wird die Route erneut
                                                            optimiert.

                                                            Optimierung stoppen
                                                            Mittels dieser Symbol-Schaltfläche wird die Optimierung der
                                                            Route unterbrochen.

                                                            Verkehr
                                                            Mittels dieser Symbol-Schaltfläche wird die Verkehrslage
                                                            aufgrund von statistischen Werten (Nokia Maps) ermittelt.

                                                            Verkehr stoppen
                                                            Mittels dieser Symbol-Schaltfläche wird die Ermittlung der
                                                            Verkehrslage gestoppt.

                                                            Tour bearbeiten
                                                            Mittels dieser Symbol-Schaltfläche können Sie die
2.01 / 01-2017




                                                            Eigenschaften der Tour bearbeiten. Es öffnet sich der Dialog
                                                            Tour.




                 A+W Business Logistic Optmizer                                                                          I-31
                 Grundgedanken zu OTR                                                                              Tutorial




                                        Die Symbolleiste der Ergebnis-Phase:
                                        Die Symbolleiste der Ergebnis-Phase beinhaltet den Zugriff auf alle Funktio-
                                        nen bzw. Dialoge, die in dieser Phase von Bedeutung sind.




                                        Erläuterung der einzelnen Symbole
                                        Im Anschluss finden Sie eine Auflistung der Symbol-Schaltflächen und ihrer
                                        Bedeutung.

                                        Symbol              Erläuterung

                                                            Ausgewählte Tour
                                                            Mittels dieser Symbol-Schaltfläche öffnet sich der Crystal
                                                            Report Bestätigungs- und Lieferliste für die ausgewählte
                                                            Tour.

                                                            Alle angezeigten Touren
                                                            Mittels dieser Symbol-Schaltfläche öffnet sich der Crystal
                                                            Report Bestätigungs- und Lieferliste für alle optimierten
                                                            Touren.

                                                            Siehe Tour
                                                            Mittels dieser Symbol-Schaltfläche öffnet sich der Dialog
                                                            Tour.

                                                            Siehe Bestimmungsort
                                                            Mittels dieser Symbol-Schaltfläche öffnet sich der Dialog
                                                            Bestimmungsort.

                                                            Tour exportieren
                                                            Mittels dieser Symbol-Schaltfläche können Sie die Daten an
                                                            ein Navigationssystem exportieren. Es öffnet sich der Dialog
                                                            Export.

                                                            Tour bearbeiten
                                                            Mittels dieser Symbol-Schaltfläche können Sie den Tour-
                                                            Status und die tatsächlichen Kosten ändern. Es öffnet sich
                                                            der Dialog Tour bearbeiten.
2.01 / 01-2017




                 I-32                                                                A+W Business Logistic Optmizer
                 Tutorial                                                                  Grundgedanken zu OTR




                                        Feldhilfe
                                        Befindet sich hinter einem Feld die nebenstehende Symbol-Schaltfläche [Hil-
                                        fe], können Sie den Mauszeiger darauf platzieren und erhalten eine Informa-
                                        tion zu dem Feld.




                                        Abb. I-8     Feldhilfe


                                        Ergänzende Informationen
                                         “Die Oberfläche” auf Seite I-22
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                               I-33
                 Administration                                                                    Tutorial




                                  Administration
                                  In diesem Themenblock lernen Sie die Stammdaten in OTR kennen.
                                  Dazu gehören folgende Lerneinheiten:
                                  •   “Parameter” auf Seite I-35
                                  •   “Benutzer” auf Seite I-37
                                  •   “Status” auf Seite I-38
                                  •   “Kunden” auf Seite I-40
                                  •   “Abteilungen” auf Seite I-43
                                  •   “Fahrzeuge” auf Seite I-45
                                  •   “Fahrer” auf Seite I-49
                                  •   “Reports” auf Seite I-52
                                  •   “Datenimport” auf Seite I-58
2.01 / 01-2017




                 I-34                                                    A+W Business Logistic Optmizer
                 Tutorial                                                                               Administration




                                        Parameter
                                        In diesem Bereich nehmen Sie die Standard-Einstellungen zum Arbeiten mit
                                        OTR vor.
                                        Die Parameter werden zunächst in zwei Gruppen unterteilt:
                                        •   Parameter zur Konfiguration der Anwendung
                                            Diese Parameter dienen der allgemeinen Konfiguration, z. B. Textformat,
                                            Einheitensystem, Währung, etc.
                                        •   Parameter für die Routen
                                            Auf Basis dieser Werte werden die Routen gebildet und optimiert. Über den
                                            Dialog Route bearbeiten haben Sie jederzeit die Möglichkeit, auf diese
                                            Werte zuzugreifen und temporäre Änderungen durchzuführen.
                                        Eine detaillierte Erläuterung hierzu finden Sie in der Softwarereferenz.


                                        Ergänzende Informationen
                                         Softwarereferenz, “Parameter” auf Seite I-136
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                                    I-35
                 Administration                                                                               Tutorial




                                  Stammdaten
                                  Lernziele

                                  •   Die Parameter kennenlernen
                                  •   Den Umgang mit dem Fuhrpark kennenlernen und verstehen
                                  •   Den Umgang mit Benutzern und Abteilungen kennenlernen und verstehen
                                  •   Den Umgang mit den Fahrer kennenlernen und verstehen


                                  Nutzen

                                  • Zum Ermitteln der Tourkosten ist es notwendig, die Fuhrparkdaten möglichst
                                    detailliert zu pflegen. Nur so erhalten Sie genaue Werte. Darüber hinaus kann es
                                    jederzeit notwendig sein, Ihre Fahrer telefonisch zu kontaktieren. Daher ist es
                                    empfehlenswert, die Personendaten auf dem aktuellen Stand zu halten.


                                  Definition

                                  Fixkosten                   Kosten, die bei Änderung einer Bezugsgröße
                                                              (Gesamtstrecke, Kraftstoffkosten) konstant bleiben.


                                  Merke

                                  Neue Fahrzeuge anlegen      Zum Anlegen neuer Fahrzeuge ist es ratsam, die
                                                              Fahrzeugpapiere zur Hand zu haben.

                                  Wartungstermin              Sie haben die Möglichkeit, für Ihre Fahrzeuge den
                                                              nächsten Wartungstermin zu hinterlegen. Das Modul
                                                              erinnert Sie dann rechtzeitig, dass dieser Termin
                                                              ansteht.

                                  Fahrer zuweisen             Sie können einem Fahrzeug einen festen Fahrer
                                                              zuweisen.

                                  Kosten                      Die Kosten können pro Fahrer nach der Zeit oder der
                                                              Entfernung hinterlegt werden.

                                  Personal                    OTR unterscheidet eigenes Personal (Mitarbeiter) von
                                                              fremdem Personal (angemietete Fahrer).
2.01 / 01-2017




                 I-36                                                            A+W Business Logistic Optmizer
                 Tutorial                                                                                Administration




                                        Benutzer
                                        Dieser Bereich dient dazu, die Profile der Benutzer, die unter Windows oder in
                                        einer Domäne registriert sind, zu verwalten. Die Daten werden automatisch
                                        generiert, wenn ein Benutzer das Programm (OTR) startet.




                                        Abb. I-9      Benutzer


                                        Die Tabelle oben zeigt Ihnen, welche Profile bereits angelegt sind. Als Admi-
                                        nistrator können Sie z. B. Benutzer mit einem Standard-Profil (Sprache, Aus-
                                        sehen der Oberfläche, etc.) anlegen, die dann einfach kopiert werden können.
                                        Eine detaillierte Erläuterung der einzelnen Felder finden Sie in der Softwarere-
                                        ferenz.

                                           Rechte
                                           Zum Editieren muss der Anwender Mitglied der Administratoren-Gruppe
                                           sein. Die Anwender werden erfasst, wenn OTR aus dem A+W Business
                                           heraus gestartet wird. Ansonsten werden die Anwender vom Betriebssys-
                                           tem erfasst.


                                        Ergänzende Informationen
                                         Softwarereferenz, “Benutzer” auf Seite I-146
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                                    I-37
                 Administration                                                                           Tutorial




                                  Status
                                  Je nachdem, in welchem Zustand sich eine Route befindet, hat sie einen ent-
                                  sprechenden Status.




                                  Abb. I-10    Status


                                  Die Tabelle oben zeigt Ihnen, welche Status-Typen bereits angelegt sind. Sie
                                  können eine neuen Status anlegen oder einen vorhandenen Status ändern.
                                  Welcher Status geändert werden kann, zeigt Ihnen das Feld Editierbar. Hat
                                  der Status dort einen grünen Haken, kann er geändert werden. Alle Status-Ty-
                                  pen ohne grünen Haken können nicht geändert werden.
                                  Eine manuelle Änderung des Status kann nötig sein, wenn Sie z. B. eine ge-
                                  plante Tour für den Fahrer manuell freigeben und damit die Daten in die Cloud
                                  hochladen wollen.
                                  Die einzelnen Status sind zu Gruppen zusammengefasst. So gibt es z. B. eine
                                  Gruppe (650), die sich mit unterschiedlichen Gegebenheiten bezüglich des
                                  Bestimmungsortes befasst. Die Gruppe enthält folgende Status:
                                  •   Bestimmungsort Problem: Bei diesem Status war es dem LKW z. B. nicht
                                      möglich, den Bestimmungsort anzufahren.
                                  •   Bestimmungsort nicht gefunden: Hier wurde der Bestimmungsort schlicht-
                                      weg nicht gefunden.
2.01 / 01-2017




                                  Eine detaillierte Erläuterung der einzelnen Felder finden Sie in der Softwarere-
                                  ferenz.



                 I-38                                                          A+W Business Logistic Optmizer
                 Tutorial                                                                             Administration




                                        Die Status-Typen verwalten
                                        In dieser Einheit lernen Sie, wie Sie neue Status-Typen anlegen, bearbeiten
                                        oder auch löschen.
                                        Zu dieser Lerneinheit gibt es folgende Handlungsanweisungen:
                                        •   “So legen Sie einen neuen Status an” auf Seite I-39
                                        •   “So löschen Sie einen bestehenden Status” auf Seite I-39
                                        •   “So nehmen Sie Änderungen an einem bestimmten Status vor” auf
                                            Seite I-39


                                         So legen Sie einen neuen Status an
                                        1 Gehen Sie in der Menü-Leiste auf den Eintrag Administration.
                                        2 Betätigen Sie die Symbol-Schaltfläche [Status].
                                            Es öffnet sich der Dialog Status.
                                        3 Betätigen Sie die Symbol-Schaltfläche [Neu].
                                            Der untere Teil des Dialogs wird zur Bearbeitung freigegeben.
                                        4 Klicken Sie auf die Symbol-Schaltfläche. Es öffnet sich der Dialog Status
                                          Typ. Wählen Sie aus der Liste den Typ aus, zu dem der Status gehören
                                          wird. Klicken Sie auf [OK]. Der Dialog wird geschlossen. Die Informationen
                                          werden übernommen.
                                        5 Das Feld Status wird mit der nächst freien Nummer vorbelegt.
                                        6 Geben Sie im Feld Statusnamen den Namen ein.
                                        7 Ob die Checkboxen Touren und Bestimmungsorte aktiv oder nicht aktiv
                                          sind, richtet sich nach der Gruppe, der sie zugeordnet sind.
                                        8 Im Feld Beschreibung können Sie eine detaillierte Beschreibung zu dem
                                          Status hinterlegen.


                                         So löschen Sie einen bestehenden Status
                                        1 Gehen Sie in der Menü-Leiste auf den Eintrag Administration.
                                        2 Betätigen Sie die Symbol-Schaltfläche [Status].
                                            Es öffnet sich der Dialog Status.
                                        3 Markieren Sie in der Tabelle den Status, das gelöscht werden soll.
                                        4 Betätigen Sie die Symbol-Schaltfläche [Löschen].
                                            Der Eintrag wird gelöscht.


                                         So nehmen Sie Änderungen an einem bestimmten Status vor
                                        1 Gehen Sie in der Menü-Leiste auf den Eintrag Administration.
                                        2 Betätigen Sie die Symbol-Schaltfläche [Status].
2.01 / 01-2017




                                            Es öffnet sich der Dialog Status.




                 A+W Business Logistic Optmizer                                                                I-39
                 Administration                                                                           Tutorial




                                  3 Markieren Sie in der Tabelle den Status, der geändert werden soll. Ob ein
                                    Status geändert werden kann, sehen Sie in der Tabelle daran, dass im Feld
                                    Editierbar ein Hacken ist.
                                  4 Betätigen Sie die Symbol-Schaltfläche [Bearbeiten].
                                  5 Nehmen Sie die gewünschten Änderungen vor.
                                  6 Betätigen Sie die Symbol-Schaltfläche [Speichern].
                                     Die Daten werden gespeichert.


                                  Ergänzende Informationen
                                   Softwarereferenz, “Status” auf Seite I-147


                                  Kunden
                                  In OTR haben Sie die Möglichkeit, eigene, zusätzliche Kundendaten (Adres-
                                  sen) zu verwalten. Dies ist hilfreich, um bspw. Adressen für Be- und Entlade-
                                  stationen zu verwalten, ohne dass diese Daten im ERP-System (A+W
                                  Business Kundenstammdaten) angelegt sein müssen. Diese Eigenschaft ak-
                                  tivieren Sie in den Parametern, indem Sie den Eintrag
                                  USE_CUSTOMERS_OTR auf den Wert Ja setzen.




                                  Abb. I-11     Kunden
2.01 / 01-2017




                                  Ist der Parameter aktiv, prüft OTR während des Imports im Hintergrund, ob der
                                  Kunden bereits gespeichert ist. Ist er nicht gespeichert, speichert ihn das Pro-
                                  gramm und er steht ab sofort zur Verfügung.


                 I-40                                                            A+W Business Logistic Optmizer
                 Tutorial                                                                                Administration




                                        Eine detaillierte Erläuterung der einzelnen Felder finden Sie in der Softwarere-
                                        ferenz.

                                        Die Kunden verwalten
                                        In dieser Einheit lernen Sie, wie Sie neue Kunden anlegen (manuell), bearbei-
                                        ten oder auch löschen.
                                        Zu dieser Lerneinheit gibt es folgende Handlungsanweisungen:
                                        •   “So legen Sie einen neuen Kunden manuell an” auf Seite I-41
                                        •   “So löschen Sie einen bestehenden Kunden” auf Seite I-41
                                        •   “So nehmen Sie Änderungen an einem bestimmten Kunden vor” auf
                                            Seite I-42


                                         So legen Sie einen neuen Kunden manuell an
                                        1 Gehen Sie in der Menü-Leiste auf den Eintrag Administration.
                                        2 Betätigen Sie die Symbol-Schaltfläche [Kunden].
                                            Es öffnet sich der Dialog Kunden.
                                        3 Betätigen Sie die Symbol-Schaltfläche [Neu].
                                            Der untere Teil des Dialogs wird zur Bearbeitung freigegeben.
                                        4 Geben Sie im Feld Kunden-Nr. die gewünschte Nummer ein. Hinweis:
                                          Jede Nummer darf nur einmal vorkommen.
                                        5 Geben Sie im Feld Namen den Namen des Kunden ein.
                                        6 Geben Sie im Feld Telefon die Telefonnummer des Kunden ein.
                                        7 Im Feld Adresse geben Sie die Kunden-Adresse ein.
                                            Bitte achten Sie darauf, den Straßennamen und den Ortsnamen komma-
                                            separiert einzugeben.
                                        8 Sind die Felder Längen- und Breitengrad nicht gefüllt, klicken Sie auf die
                                          Symbol-Schaltfläche [Geolokalisieren].
                                        9 Im Feld Zeit (Minuten) haben Sie die Möglichkeit zu hinterlegen, in welcher
                                          Zeitspanne der Fahrer beim Kunden sein soll.
                                        10 Im Feld Zeitbereich haben Sie die Möglichkeit zu hinterlegen, von welcher
                                           Uhrzeit bis zu welcher Uhrzeit der Fahrer beim Kunden abladen kann.
                                        11 Im Feld Ansprechpartner können Sie eine Kontaktperson beim Kunden
                                           hinterlegen.
                                        12 Im Feld E-Mail-Adresse Kontakt können Sie die E-Mail-Adresse des Kon-
                                           taktes hinterlegen.


                                         So löschen Sie einen bestehenden Kunden
                                        1 Gehen Sie in der Menü-Leiste auf den Eintrag Administration.
2.01 / 01-2017




                                        2 Betätigen Sie die Symbol-Schaltfläche [Kunden].
                                            Es öffnet sich der Dialog Kunden.



                 A+W Business Logistic Optmizer                                                                    I-41
                 Administration                                                                         Tutorial




                                  3 Markieren Sie in der Tabelle den Kunden, das gelöscht werden soll.
                                  4 Betätigen Sie die Symbol-Schaltfläche [Löschen].
                                     Der Eintrag wird gelöscht.


                                   So nehmen Sie Änderungen an einem bestimmten Kunden vor
                                  1 Gehen Sie in der Menü-Leiste auf den Eintrag Administration.
                                  2 Betätigen Sie die Symbol-Schaltfläche [Kunden].
                                     Es öffnet sich der Dialog Kunden.
                                  3 Markieren Sie in der Tabelle den Kunden, der geändert werden soll.
                                  4 Betätigen Sie die Symbol-Schaltfläche [Bearbeiten].
                                  5 Nehmen Sie die gewünschten Änderungen vor.
                                  6 Betätigen Sie die Symbol-Schaltfläche [Speichern].
                                     Die Daten werden gespeichert.


                                  Ergänzende Informationen
                                   Softwarereferenz, “Kunden” auf Seite I-149
2.01 / 01-2017




                 I-42                                                            A+W Business Logistic Optmizer
                 Tutorial                                                                                Administration




                                        Abteilungen
                                        In diesem Bereich können Sie einzelne Abteilungen hinzufügen, ändern oder
                                        löschen. Das dient später einmal statistischen Zwecken. So können Sie z. B.
                                        statistische Auswertungen auf Basis von Abteilungen erstellen. Fremdfirmen
                                        (Speditionen) die für Sie ausliefern könnten beispielsweise als Abteilung defi-
                                        niert und so erfasst werden.




                                        Abb. I-12     Abteilungen


                                        Die Tabelle oben zeigt Ihnen, welche Abteilungen bereits angelegt sind.
                                        Eine detaillierte Erläuterung der einzelnen Felder finden Sie in der Softwarere-
                                        ferenz.

                                        Die Abteilungen verwalten
                                        In dieser Einheit lernen Sie, wie Sie neue Abteilungen anlegen, bearbeiten
                                        oder auch löschen.
                                        Zu dieser Lerneinheit gibt es folgende Handlungsanweisungen:
                                        •   “So legen Sie eine neue Abteilung an” auf Seite I-43
                                        •   “So löschen Sie eine bestehende Abteilung” auf Seite I-44
                                        •   “So nehmen Sie Änderungen an einer bestimmten Abteilung vor” auf
                                            Seite I-44


                                         So legen Sie eine neue Abteilung an
                                        1 Gehen Sie in der Menü-Leiste auf den Eintrag Administration.
                                        2 Betätigen Sie die Symbol-Schaltfläche [Abteilungen].
                                            Es öffnet sich der Dialog Abteilungen.
                                        3 Geben Sie im Feld Abteilung die Nummer der Abteilung ein, z. B. 5318.
2.01 / 01-2017




                                        4 Geben Sie im Feld Namen den Namen der Abteilung ein, z. B. Versand.




                 A+W Business Logistic Optmizer                                                                    I-43
                 Administration                                                                        Tutorial




                                  5 Im Feld Beschreibung können Sie eine Beschreibung zur Abteilung hinter-
                                    legen.


                                   So löschen Sie eine bestehende Abteilung
                                  1 Gehen Sie in der Menü-Leiste auf den Eintrag Administration.
                                  2 Betätigen Sie die Symbol-Schaltfläche [Abteilungen].
                                     Es öffnet sich der Dialog Abteilungen.
                                  3 Markieren Sie in der Tabelle die Abteilung, die gelöscht werden soll.
                                  4 Betätigen Sie die Symbol-Schaltfläche [Löschen].
                                     Der Eintrag wird gelöscht.


                                   So nehmen Sie Änderungen an einer bestimmten Abteilung vor
                                  1 Gehen Sie in der Menü-Leiste auf den Eintrag Administration.
                                  2 Betätigen Sie die Symbol-Schaltfläche [Abteilungen].
                                     Es öffnet sich der Dialog Abteilungen.
                                  3 Markieren Sie in der Tabelle die Abteilung, die geändert werden soll.
                                  4 Betätigen Sie die Symbol-Schaltfläche [Bearbeiten].
                                  5 Nehmen Sie die gewünschten Änderungen vor.
                                  6 Betätigen Sie die Symbol-Schaltfläche [Speichern].
                                     Die Daten werden gespeichert.


                                  Ergänzende Informationen
                                   Softwarereferenz, “Abteilungen” auf Seite I-151
2.01 / 01-2017




                 I-44                                                           A+W Business Logistic Optmizer
                 Tutorial                                                                                Administration




                                        Fahrzeuge
                                        In diesem Bereich sind alle Fahrzeuge zu finden, die zur Auslieferung von
                                        Ware zur Verfügung stehen. Das können sein:
                                        •   LKW
                                        •   Auto
                                        •   Anhänger




                                        Abb. I-13      Fahrzeuge


                                        Die Tabelle oben zeigt Ihnen, welche Fahrzeuge bereits angelegt sind. Sie
                                        können neue Fahrzeuge anlegen, aber auch Änderungen an bereits angeleg-
                                        ten Fahrzeugen vornehmen.
                                        Eine detaillierte Erläuterung der einzelnen Felder finden Sie in der Softwarere-
                                        ferenz.

                                            Fahrzeugdaten
                                            Zum Anlegen neuer Fahrzeuge ist es ratsam, die Fahrzeugpapiere (Fahr-
                                            zeugschein und/oder Fahrzeugbrief) zur Hand zu haben. Es werden Daten
                                            abgefragt, die in diesen Papieren zu finden sind, wie z. B. Leergewicht.


                                        Ergänzende Informationen
2.01 / 01-2017




                                         Softwarereferenz, “Fahrzeuge” auf Seite I-152




                 A+W Business Logistic Optmizer                                                                    I-45
                 Administration                                                                         Tutorial




                                  Die Fahrzeuge verwalten
                                  In dieser Einheit lernen Sie, wie Sie neue Fahrzeuge anlegen, bearbeiten oder
                                  auch löschen.
                                  Zu dieser Lerneinheit gibt es folgende Handlungsanweisungen:
                                  •   “So legen Sie ein neues Fahrzeug an” auf Seite I-46
                                  •   “So löschen Sie ein bestehendes Fahrzeug” auf Seite I-47
                                  •   “So nehmen Sie Änderungen an einem bestimmten Fahrzeug vor” auf
                                      Seite I-47
                                  •   “So weisen Sie einem Fahrzeug einen festen Fahrer zu” auf Seite I-48
                                  •   “So entfernen Sie einen fest zugewiesenen Fahrer” auf Seite I-48


                                   So legen Sie ein neues Fahrzeug an
                                  1 Gehen Sie in der Menü-Leiste auf den Eintrag Administration.
                                  2 Betätigen Sie die Symbol-Schaltfläche [Fahrzeuge].
                                      Es öffnet sich der Dialog Fahrzeuge.
                                  3 Betätigen Sie die Symbol-Schaltfläche [Neu].
                                      Der untere Teil des Dialogs wird zur Bearbeitung freigegeben. Für die nun
                                      folgenden Einträge ist es sinnvoll, die Fahrzeugpapiere (Fahrzeugschein
                                      und/oder -brief) zur Hand zu haben.
                                  4 Erfassen Sie die Felder Nummernschild, Marke, Modell und Fahrgestell-
                                    Nummer auf Grund der Angaben in den Fahrzeugpapieren.
                                  5 Erfassen Sie das Feld Kaufdatum.
                                  6 Im Feld Nächste Wartung können Sie das Datum für die nächste Wartung
                                    eingeben. In den Parametern gibt es den Eintrag Nächster Wartungstermin
                                    für Fahrzeuge.
                                      Steht dieser Eintrag auf Ja, dann wird dieses Feld hier entsprechend aus-
                                      gewertet.
                                  7 Im Feld Abteilung können Sie dem Fahrzeug eine Abteilung fest zuordnen.
                                    Dies dient später statistischen Auswertungen. Über dieSymbol-Schaltflä-
                                    che öffnen Sie den Dialog Abteilung auswählen, in dem alle definierten Ab-
                                    teilungen gelistet sind.
                                  8 Erfassen Sie die Felder Maximale Breite, Maximale Höhe, Maximale Län-
                                    ge, Maximale Beladung und Leergewicht auf Grund der Angaben in den
                                    Fahrzeugpapieren.
                                  9 Im Feld Verbrauch geben Sie den durchschnittlichen Kraftstoff-Verbrauch
                                    des Fahrzeugs in Litern ein, z. B. 18,5.
                                  10 Im Feld Kraftstoffkosten geben Sie die durchschnittlichen Kosten für einen
                                     Liter Kraftstoff ein, z. B. 1,43.
                                      Die entsprechende Währungseinheit können Sie in den Parametern hinter-
                                      legen.
2.01 / 01-2017




                                  11 Im Feld Fixkosten geben Sie die durchschnittlichen Kosten für einen Liter
                                     Kraftstoff ein, z. B. 1,43.



                 I-46                                                         A+W Business Logistic Optmizer
                 Tutorial                                                                               Administration




                                           Die entsprechende Währungseinheit können Sie in den Parametern hinter-
                                           legen.
                                        12 Aus der Kombobox Fortbewegungstyp wählen Sie den Fahrzeug-Typ aus.
                                        13 Die Felder Fahrer ID, Name und Nachname stehen in Verbindung mit der
                                           Symbol-Schaltfläche [Fahrer hinzufügen].
                                           Wenn Sie die Schaltfläche betätigen, öffnet sich der Dialog Fahrer. Aus die-
                                           sem Dialog können Sie einen Fahrer auswählen. Das macht Sinn, wenn
                                           Mitarbeiter fest einem Fahrzeug zugeordnet sind.
                                        14 Die im Feld Touren aufgeführten Tournummern werden durch AWBusiness
                                           übergeben und dienen dazu, LKWs bestimmten Tournummern zuzuord-
                                           nen.
                                        15 Das Feld Reihenfolge steht in Zusammenhang mit dem Feld Touren. Ist für
                                           zwei oder mehrere LKWs die gleiche Tournummer erlaubt, dann können
                                           Sie über dieses Feld die Reihenfolge (Priorität) der LKWs bestimmen. Das
                                           Feld wird nur ausgewertet, wenn in den Parametern der Eintrag
                                           ROUTE_ORIGIN den Wert Ja hat.
                                        16 Über die Checkbox Fahrzeug verfügbar steuern Sie, ob das Fahrzeug ge-
                                           nerell und für alle Touren zur Verfügung steht.
                                        17 Sollte Ihr Fahrzeug über eine Anhängevorrichtung verfügen, aktivieren Sie
                                           die Checkbox LKW mit Anhänger.


                                         So löschen Sie ein bestehendes Fahrzeug
                                        1 Gehen Sie in der Menü-Leiste auf den Eintrag Administration.
                                        2 Betätigen Sie die Symbol-Schaltfläche [Fahrzeuge].
                                           Es öffnet sich der Dialog Fahrzeuge.
                                        3 Markieren Sie in der Tabelle das Fahrzeug, das gelöscht werden soll.
                                        4 Betätigen Sie die Symbol-Schaltfläche [Löschen].
                                           Der Eintrag wird gelöscht.


                                         So nehmen Sie Änderungen an einem bestimmten Fahrzeug vor
                                        1 Gehen Sie in der Menü-Leiste auf den Eintrag Administration.
                                        2 Betätigen Sie die Symbol-Schaltfläche [Fahrzeuge].
                                           Es öffnet sich der Dialog Fahrzeuge.
                                        3 Markieren Sie in der Tabelle das Fahrzeug, das geändert werden soll.
                                        4 Betätigen Sie die Symbol-Schaltfläche [Bearbeiten].
                                        5 Nehmen Sie die gewünschten Änderungen vor.
                                        6 Betätigen Sie die Symbol-Schaltfläche [Speichern].
                                           Die Daten werden gespeichert.
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                                   I-47
                 Administration                                                                       Tutorial




                                   So weisen Sie einem Fahrzeug einen festen Fahrer zu
                                  1 Gehen Sie in der Menü-Leiste auf den Eintrag Administration.
                                  2 Betätigen Sie die Symbol-Schaltfläche [Fahrzeuge].
                                     Es öffnet sich der Dialog Fahrzeuge.
                                  3 Markieren Sie in der Tabelle das Fahrzeug, dem ein Fahrer zugewiesen-
                                    werden soll.
                                  4 Betätigen Sie die Symbol-Schaltfläche [Bearbeiten].
                                  5 Betätigen Sie die Symbol-Schaltfläche [Fahrer hinzufügen].
                                     Es öffnet sich der Dialog Fahrer.
                                  6 Wählen Sie den gewünschten Fahrer aus.
                                  7 Betätigen Sie die Symbol-Schaltfläche [OK].
                                     Der Dialog wird geschlossen und Sie befinden sich wieder im Dialog Fahr-
                                     zeuge.
                                  8 Betätigen Sie die Symbol-Schaltfläche [Speichern].
                                     Die Daten werden gespeichert.


                                   So entfernen Sie einen fest zugewiesenen Fahrer
                                  1 Gehen Sie in der Menü-Leiste auf den Eintrag Administration.
                                  2 Betätigen Sie die Symbol-Schaltfläche [Fahrzeuge].
                                     Es öffnet sich der Dialog Fahrzeuge.
                                  3 Markieren Sie in der Tabelle das Fahrzeug, von dem der Fahrer entfernt
                                    werden soll.
                                  4 Betätigen Sie die Symbol-Schaltfläche [Bearbeiten].
                                  5 Betätigen Sie die Symbol-Schaltfläche [Fahrer löschen].
                                     Der Fahrer wird gelöscht.
                                  6 Betätigen Sie die Symbol-Schaltfläche [Speichern].
                                     Die Daten werden gespeichert.


                                  Ergänzende Informationen
                                   Softwarereferenz, “Fahrzeuge” auf Seite I-152
                                   Softwarereferenz, “Fahrer” auf Seite I-155
2.01 / 01-2017




                 I-48                                                          A+W Business Logistic Optmizer
                 Tutorial                                                                                Administration




                                        Fahrer
                                        In diesem Bereich können Sie die Daten zu Ihren Fahrern verwalten. Es sind
                                        alle Fahrer zu finden, die zur Auslieferung von Ware zur Verfügung stehen.
                                        Das können sein:
                                        •   Angestellte Fahrer
                                        •   Fahrer anderer Unternehmen (angemietete Fahrer)




                                        Abb. I-14     Fahrer


                                        Die Tabelle oben zeigt Ihnen, welche Fahrer bereits angelegt sind. Sie können
                                        neue Fahrer anlegen, aber auch Änderungen an bereits angelegten Fahrern
                                        vornehmen.
                                        Eine detaillierte Erläuterung der einzelnen Felder finden Sie in der Softwarere-
                                        ferenz.


                                        Ergänzende Informationen
                                         Softwarereferenz, “Fahrer” auf Seite I-155
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                                    I-49
                 Administration                                                                        Tutorial




                                  Die Fahrer verwalten
                                  In dieser Einheit lernen Sie, wie Sie neue Fahrer anlegen, bearbeiten oder
                                  auch löschen.
                                  Zu dieser Lerneinheit gibt es folgende Handlungsanweisungen:
                                  •   “So legen Sie einen neuen Fahrer an” auf Seite I-50
                                  •   “So löschen Sie einen bestehenden Fahrer” auf Seite I-51
                                  •   “So nehmen Sie Änderungen an einem bestimmten Fahrer vor” auf
                                      Seite I-51


                                   So legen Sie einen neuen Fahrer an
                                  1 Gehen Sie in der Menü-Leiste auf den Eintrag Administration.
                                  2 Betätigen Sie die Symbol-Schaltfläche [Fahrer].
                                      Es öffnet sich der Dialog Fahrer.
                                  3 Betätigen Sie die Symbol-Schaltfläche [Neu].
                                      Der untere Teil des Dialogs wird zur Bearbeitung freigegeben.
                                  4 Im Feld Fahrer ID geben Sie eine Kurzbezeichnung für den Fahrer ein.
                                  5 Erfassen Sie die Felder Name, Nachname und Nachname 2.
                                  6 Im Feld Steuer ID geben Sie die Steuernummer des Mitarbeiters ein.
                                  7 Im Feld E-Mail können Sie die E-Mail-Adresse des Mitarbeiters hinterle-
                                    gen.
                                  8 Im Feld Kosten können Sie für den Mitarbeiter einen Betrag hinterlegen,
                                    den dieser als Kosten auf der Tour verursacht.
                                      Es werden Kosten nach Zeit und nach Entfernung unterschieden. Bitte ak-
                                      tivieren Sie die dahinter liegenden Radiotasten (Nach Zeit/Nach Entfer-
                                      nung) entsprechend. Der hier eingetragene Wert kommt im Register
                                      Kosten mit zur Auswertung.
                                  9 Erfassen Sie im Felder Adresse die Adresse des Mitarbeiters und in den
                                    Feldern Telefon und Telefon 2 die entsprechenden Telefonnummern.
                                  10 Im Feld Ansprechpartner können Sie den Namen einer Kontaktperson hin-
                                     terlegen, falls der Fahrer nicht in Ihrem Unternehmen angestellt ist.
                                      Beispiel: Sie buchen für eine Tour den Fahrer einer Spedition.
                                  11 Im Feld Kontakt-Adresse geben Sie die Adresse Ihres Kontaktes an.
                                  12 Im Feld Telefon-Kontakt geben Sie die entsprechende Telefonnummer an.
                                  13 Im Feld Beschreibung können Sie eine Beschreibung zu dem Fahrer oder
                                     dem Kontakt hinterlegen und im Feld E-Mail-Adresse Kontakt die entspre-
                                     chende E-Mail-Adresse.
                                  14 Im Feld Abteilung können Sie dem Fahrer eine Abteilung fest zuordnen.
                                     Dies dient später statistischen Auswertungen. Über die Symbol-Schaltflä-
2.01 / 01-2017




                                     che öffnen Sie den Dialog Abteilung auswählen, in dem alle definierten Ab-
                                     teilungen gelistet sind.




                 I-50                                                         A+W Business Logistic Optmizer
                 Tutorial                                                                            Administration




                                        15 Über die Checkbox Firmen-Mitarbeiter geben Sie an, ob der Fahrer in Ih-
                                           rem Unternehmen angestellt ist und über die Checkbox Verfügbar steuern
                                           Sie, ob der Fahrer immer verfügbar ist.
                                        16 Über die Checkbox Kennwort zurücksetzen wird das Kennwort, das der
                                           Fahrer beim Starten der GDC APP (mobile App für den Fahrer) eingeben
                                           muss, zurückgesetzt.


                                         So löschen Sie einen bestehenden Fahrer
                                        1 Gehen Sie in der Menü-Leiste auf den Eintrag Administration.
                                        2 Betätigen Sie die Symbol-Schaltfläche [Fahrer].
                                           Es öffnet sich der Dialog Fahrer.
                                        3 Markieren Sie in der Tabelle den Fahrer, der gelöscht werden soll.
                                        4 Betätigen Sie die Symbol-Schaltfläche [Löschen].
                                           Der Eintrag wird gelöscht.


                                         So nehmen Sie Änderungen an einem bestimmten Fahrer vor
                                        1 Gehen Sie in der Menü-Leiste auf den Eintrag Administration.
                                        2 Betätigen Sie die Symbol-Schaltfläche [Fahrer].
                                           Es öffnet sich der Dialog Fahrer.
                                        3 Markieren Sie in der Tabelle den Fahrer, der geändert werden soll.
                                        4 Betätigen Sie die Symbol-Schaltfläche [Bearbeiten].
                                        5 Nehmen Sie die gewünschten Änderungen vor.
                                        6 Betätigen Sie die Symbol-Schaltfläche [Speichern].
                                           Die Daten werden gespeichert.


                                        Ergänzende Informationen
                                         Softwarereferenz, “Fahrer” auf Seite I-155
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                                I-51
                 Administration                                                                           Tutorial




                                  Reports
                                  In diesem Bereich können Sie die Daten zu Ihren Reports verwalten. Im Dialog
                                  sind alle Reports aufgeführt, die in Ihrem System angelegt sind. OTR verwen-
                                  det hierzu Reports auf Basis von SAP Crystal Reports.




                                  Abb. I-15     Reports


                                  Die Tabelle oben zeigt Ihnen, welche Reports bereits angelegt sind. Sie kön-
                                  nen neue Reports anlegen, aber auch Änderungen an bereits angelegten
                                  oben vornehmen.
                                  Eine detaillierte Erläuterung der einzelnen Felder finden Sie in der Softwarere-
                                  ferenz.


                                  Ergänzende Informationen
                                   Softwarereferenz, “Reports” auf Seite I-158
2.01 / 01-2017




                 I-52                                                             A+W Business Logistic Optmizer
                 Tutorial                                                                             Administration




                                        Die Reports verwalten
                                        In dieser Einheit lernen Sie, wie Sie neue Reports anlegen, bearbeiten oder
                                        auch löschen.
                                        Zu dieser Lerneinheit gibt es folgende Handlungsanweisungen:
                                        •   “So legen Sie einen neuen Report an” auf Seite I-53
                                        •   “So löschen Sie einen bestehenden Report” auf Seite I-53
                                        •   “So nehmen Sie Änderungen an einem bestimmten Packmittel vor” auf
                                            Seite I-57


                                         So legen Sie einen neuen Report an
                                        1 Gehen Sie in der Menü-Leiste auf den Eintrag Administration.
                                        2 Betätigen Sie die Symbol-Schaltfläche [Reports].
                                            Es öffnet sich der Dialog Reports.
                                        3 Betätigen Sie die Symbol-Schaltfläche [Neu].
                                            Der untere Teil des Dialogs wird zur Bearbeitung freigegeben.
                                        4 Geben Sie im Feld Report-Name den Namen ein, z. B. Kurz.
                                        5 Geben Sie im Feld Report-Pfad ein, wo der Report gespeichert werden
                                          soll.
                                        6 Im Feld Beschreibung haben Sie die Möglichkeit, eine Information zu dem
                                          Report zu hinterlegen.
                                        7 Über die Checkboxen im Bereich Parameter können Sie festlegen, welche
                                          Informationen auf dem Report ausgegeben werden sollen.


                                         So löschen Sie einen bestehenden Report
                                        1 Gehen Sie in der Menü-Leiste auf den Eintrag Administration.
                                        2 Betätigen Sie die Symbol-Schaltfläche [Reports].
                                            Es öffnet sich der Dialog Report.
                                        3 Markieren Sie in der Tabelle den Report, der gelöscht werden soll.
                                        4 Betätigen Sie die Symbol-Schaltfläche [Löschen].
                                            Der Eintrag wird gelöscht.


                                         So nehmen Sie Änderungen an einem bestimmten Report vor
                                        1 Gehen Sie in der Menü-Leiste auf den Eintrag Administration.
                                        2 Betätigen Sie die Symbol-Schaltfläche [Reports].
                                            Es öffnet sich der Dialog Report.
                                        3 Markieren Sie in der Tabelle den Report, der geändert werden soll.
2.01 / 01-2017




                                        4 Betätigen Sie die Symbol-Schaltfläche [Bearbeiten].
                                        5 Nehmen Sie die gewünschten Änderungen vor.



                 A+W Business Logistic Optmizer                                                                I-53
                 Administration                                                                          Tutorial




                                  6 Betätigen Sie die Symbol-Schaltfläche [Speichern].
                                     Die Daten werden gespeichert.


                                  Ergänzende Informationen
                                   Softwarereferenz, “Reports” auf Seite I-158
2.01 / 01-2017




                 I-54                                                             A+W Business Logistic Optmizer
                 Tutorial                                                                                Administration




                                        Packmittel-Typen
                                        In diesem Bereich können Sie die Daten zu Ihren Packmitteln verwalten. Im
                                        Dialog sind alle Packmittel aufgeführt, die in Ihrem System angelegt sind. Ein
                                        Packmittel kann ein Gestell aber auch eine Kiste sein.




                                        Abb. I-16     Packmittel


                                        Die Tabelle oben zeigt Ihnen, welche Packmittel bereits angelegt sind. Sie
                                        können neue Pachmittel anlegen, aber auch Änderungen an bereits angeleg-
                                        ten vornehmen.
                                        Eine detaillierte Erläuterung der einzelnen Felder finden Sie in der Softwarere-
                                        ferenz.

                                           Ladeflächenoptimierung
                                           In der aktuellen Programmversion ist eine LKW-Ladeflächenoptimierung
                                           nicht umgesetzt. Bei den hier angelegten Packmitteln geht es um die Ver-
                                           buchung der Ablade- / Aufladestation (im Sinne eines Packmittel-Tra-
                                           ckings).


                                        Ergänzende Informationen
                                         Softwarereferenz, “Packmittel” auf Seite I-159
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                                    I-55
                 Administration                                                                         Tutorial




                                  Die Packmittel verwalten
                                  In dieser Einheit lernen Sie, wie Sie neue Packmittel anlegen, bearbeiten oder
                                  auch löschen.
                                  Zu dieser Lerneinheit gibt es folgende Handlungsanweisungen:
                                  •   “So legen Sie ein neues Packmittel an” auf Seite I-56
                                  •   “So löschen Sie ein bestehendes Packmittel” auf Seite I-56
                                  •   “So nehmen Sie Änderungen an einem bestimmten Packmittel vor” auf
                                      Seite I-57


                                   So legen Sie ein neues Packmittel an
                                  1 Gehen Sie in der Menü-Leiste auf den Eintrag Administration.
                                  2 Betätigen Sie die Symbol-Schaltfläche [Packmittel-Typen].
                                      Es öffnet sich der Dialog Packmittel-Typen.
                                  3 Betätigen Sie die Symbol-Schaltfläche [Neu].
                                      Der untere Teil des Dialogs wird zur Bearbeitung freigegeben.
                                  4 Geben Sie im Feld Packmittel ID die Nummer ein, z. B. 1000100.
                                  5 Geben Sie im Feld Packmittel-Typ ein, um welchen Typ es sich handelt,
                                    z. B. A-Bock, L-Bock, Holzkiste.
                                  6 Im Feld Abteilung können Sie dem Packmittel eine Abteilung fest zuord-
                                    nen. Dies dient später statistischen Auswertungen. Über die Symbol-
                                    Schaltfläche öffnen Sie den Dialog Abteilung auswählen, in dem alle defi-
                                    nierten Abteilungen gelistet sind.
                                  7 Geben Sie in den Feldern Breite, Höhe, Länge und Leergewicht die ent-
                                    sprechenden Werte an.
                                  8 Im Feld Kosten haben Sie die Möglichkeit, die Anschaffungskosten für das
                                    Packmittel zu hinterlegen.
                                  9 Aktivieren Sie die Checkbox Keine Rückholung, wenn das Packmittel beim
                                    Kunden verbleiben soll.
                                  10 Im Feld Beschreibung haben Sie die Möglichkeit, eine Information zu dem
                                     Packmittel zu hinterlegen.


                                   So löschen Sie ein bestehendes Packmittel
                                  1 Gehen Sie in der Menü-Leiste auf den Eintrag Administration.
                                  2 Betätigen Sie die Symbol-Schaltfläche [Packmittel-Typen].
                                      Es öffnet sich der Dialog Packmittel-Typen.
                                  3 Markieren Sie in der Tabelle das Packmittel, das gelöscht werden soll.
                                  4 Betätigen Sie die Symbol-Schaltfläche [Löschen].
                                      Der Eintrag wird gelöscht.
2.01 / 01-2017




                 I-56                                                         A+W Business Logistic Optmizer
                 Tutorial                                                                             Administration




                                         So nehmen Sie Änderungen an einem bestimmten Packmittel vor
                                        1 Gehen Sie in der Menü-Leiste auf den Eintrag Administration.
                                        2 Betätigen Sie die Symbol-Schaltfläche [Packmittel-Typen].
                                           Es öffnet sich der Dialog Packmittel-Typen.
                                        3 Markieren Sie in der Tabelle das Packmittel, das geändert werden soll.
                                        4 Betätigen Sie die Symbol-Schaltfläche [Bearbeiten].
                                        5 Nehmen Sie die gewünschten Änderungen vor.
                                        6 Betätigen Sie die Symbol-Schaltfläche [Speichern].
                                           Die Daten werden gespeichert.


                                        Ergänzende Informationen
                                         Softwarereferenz, “Packmittel” auf Seite I-159
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                                I-57
                 Administration                                                                           Tutorial




                                  Datenimport
                                  In diesem Bereich können Sie Daten im CSV-Datenformat (MS Excel) impor-
                                  tieren.




                                  Abb. I-17     Datenimport


                                  Über die Kombobox Importieren können Sie wählen, für wen oder was die Da-
                                  ten importiert werden. Folgende Auswahl ist möglich:
                                  •   Kunden
                                  •   Abteilungen
                                  •   Fahrer
                                  •   Fahrzeuge
                                  Eine detaillierte Erläuterung der einzelnen Felder finden Sie in der Softwarere-
                                  ferenz.


                                  Ergänzende Informationen
                                   Softwarereferenz, “Datenimport” auf Seite I-161
2.01 / 01-2017




                 I-58                                                           A+W Business Logistic Optmizer
                 Tutorial                                                                         Touren planen




                                        Touren planen
                                        In diesem Themenblock lernen Sie, wie Sie Touren planen und neue Bestim-
                                        mungsorte anlegen.
                                        Dazu gehören folgende Lerneinheiten:
                                        •   “Allgemein” auf Seite I-61
                                        •   “Import” auf Seite I-62
                                        •   “Touren” auf Seite I-63
                                        •   “Bestimmungsorte” auf Seite I-73
                                        •   “Die Detailansicht” auf Seite I-77
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                             I-59
                 Touren planen                                                                              Tutorial




                                 Touren und Bestimmungsorte
                                 Lernziele

                                 •   Die beiden Arbeitsmodi kennenlernen
                                 •   Den Import kennenlernen und verstehen
                                 •   Die Planungs-Phase kennenlernen und verstehen
                                 •   Touren kennenlernen und verstehen
                                 •   Bestimmungsorte kennenlernen und verstehen


                                 Nutzen

                                 • Die Routenplanung ermittelt für Sie den effizientesten Weg von A nach D über B
                                   und C. Das spart Zeit und Geld.


                                 Definition

                                 Route                      Die Route beschreibt den genauen Weg zwischen
                                                            mehreren Wegpunkten.

                                 Tour                       Die Tour wird aus den A+W Business Kundendaten
                                                            übernommen.


                                 Merke

                                 Liefertermin               Liefertermin, der von A+W Business übergeben wurde.

                                 Ursprüngliche Tour         Bei dieser Nummer handelt es sich um die Tour-Nummer
                                                            aus A+W Business.

                                 Tour ID                    Die von OTR vergebene Tour ID.

                                 Reihenfolge                Die Reihenfolge der Wegpunkte innerhalb der Tour.

                                 Dynamischer Modus          Liefer-Bereiche und Touren werden automatisch
                                                            gebildet.
2.01 / 01-2017




                 I-60                                                          A+W Business Logistic Optmizer
                 Tutorial                                                                               Touren planen




                                        Allgemein
                                        OTR kann in zwei unterschiedlichen Modi betrieben werden. Für welchen Mo-
                                        dus Sie sich entscheiden, hängt von Ihrer Arbeitsweise ab. Die Einstellungen
                                        werden in den Parametern vorgenommen:
                                        •   Modus 1: Hier wird mit den Routen gearbeitet, die in A+W Business zusam-
                                            men gestellt und übergeben werden. OTR verwendet dann diese Routen
                                            für die Planung und Optimierung der Touren (Wegstrecke, Reihenfolge der
                                            Haltepunkte).
                                        •   Modus 2: Diesen Modus bezeichnen wir als den dynamischen Modus. Hier
                                            erstellt OTR die Routen selbst. Es ist keine Arbeit in A+W Business nötig.
                                            Nach dem Import gruppiert OTR die Touren automatisch aufgrund der Ad-
                                            ressen in Bereiche. In diesem Schritt geschieht bereits die Geolokalisation
                                            der Adressdaten. Diese erfolgt nach folgenden Kriterien:
                                            – Adressen
                                            – Gewicht je Adresse (Aufträge werden je Kunde gruppiert)
                                            Die Zuordnungen basieren auf Zeitvorgaben, zusätzlichen Stopps z. B. zur
                                            Abholung von Gestellen und der statistischen Ermittlung von Verkehrs-
                                            staus (Nokia Maps).
                                            Um die Lieferscheine in der korrekten Reihenfolge zu drucken, können die
                                            Daten auch in diesem Modus an A+W Business zurückgemeldet werden.
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                                   I-61
                 Touren planen                                                                                    Tutorial




                                          Import
                                          Der Datenimport erfolgt über den Nummernverwalter. Während des Imports
                                          prüft OTR die Adressen und verwendet entweder die Adresse aus dem Auf-
                                          tragskopf, eine abweichende Lieferadresse (wenn vorhanden) oder aber die
                                          Adresse aus den OTR-eigenen Stammdaten.
                                          In diesem Schritt erfolgt bereits die Geolokalisation der Adressen und eine da-
                                          mit verbundene Gruppierung in Bereiche. Das System kalkuliert anhand der
                                          Längen- und Breitengrade die Abstände zwischen den einzelnen Bestim-
                                          mungsorten und kann die Aufträge dann - unter Berücksichtung des Gewichts
                                          und den zur Verfügung stehenden LKWs - in Bereiche und Touren zusammen-
                                          fassen.




                 Abb. I-18   Bereiche und tabellarische Übersicht


                                          Die Tabelle oben zeigt Ihnen im Bereich Touren, wie viele Touren zu fahren
                                          sind.
                                          Die Grafik darunter zeigt auf der linken Seite die Bereiche in unterschiedlichen
                                          Farben. So können Sie schnell erkennen, wie viele Bestimmungsorte in einem
                                          Bereich liegen. Die Tabelle rechts daneben listet Ihnen die entsprechenden
                                          Touren und Bestimmungsorte.
                                          Wenn Sie in der Karte einen Bestimmungsort markieren, wird dieser auch im
                                          Tabellengrid hervorgehoben. So ist die Identifizierung leicht und Sie können
                                          schnell und einfach Haltepunkte manuell einer anderen Tour zuweisen (grup-
2.01 / 01-2017




                                          pieren).




                 I-62                                                                  A+W Business Logistic Optmizer
                 Tutorial                                                                                Touren planen




                                        Touren
                                        Dieser Bereich zeigt Ihnen alle Touren, die zur Auslieferung anstehen.




                                        Abb. I-19     Tour-Informationen


                                        Die Inhalte des Feldes Name der Tour (TOUR NORD) kommen aus den OTR
                                        Stammdaten. Die Tour ID (8) wird von OTR vergeben und für jede Tour um 1
                                        erhöht. Der Liefertermin (21.03.2014) kommt aus A+W Business, ebenso wie
                                        der Inhalt des Feldes Ursprüngliche Tour (21).
                                        Den LKW-Fahrer, das Nummerschild sowie Marke und Modell weisen Sie zu.
                                        Die Inhalte der Felder Kraftstoffkosten und Kraftstoffverbrauch kommen aus
                                        den OTR-Stammdaten (Parameter: Kraftstoffkosten, Durchschnittlicher Kraft-
                                        stoffverbrauch).
                                        Klicken Sie eine Tour doppelt an, öffnet sich der Dialog Tour.
                                        Eine detaillierte Erläuterung der einzelnen Felder finden Sie in der Softwarere-
                                        ferenz.
                                        Sollten im Nummernverwalter Aufträge mit unterschiedlichen Lieferterminen
                                        enthalten sein, so berücksichtigt das System dies und erstellt bzw. splittet au-
                                        tomatisch verschiedene Touren. Sie können dies manuell im Schritt der Pla-
                                        nung übersteuern.


                                        Ergänzende Informationen
                                         Softwarereferenz, “Eine neue Tour zusammenstellen – Allgemein” auf Seite I-170

                                        Eine gespeicherte Tour laden
                                        OTR speichert nach dem letzten Prozess-Schritt (Ergebnis) die Touren auto-
                                        matisch.
                                        Sie können dann jederzeit auf eine Tour zugreifen, um diese mit veränderten
                                        Parametern neu zu optimieren. Die ID wird dabei nicht verändert. Es können
                                        nur Touren mit folgendem Status geladen werden:
                                        •   Grobgeplant (geplant)
                                        •   Feingeplant (optimiert)
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                                     I-63
                 Touren planen                                                                            Tutorial




                                 Abb. I-20     Gespeicherte Tour-Liste


                                 Eine detaillierte Erläuterung der einzelnen Felder finden Sie in der Softwarere-
                                 ferenz.


                                 Ergänzende Informationen
                                  Softwarereferenz, “Eine neue Tour zusammenstellen – Allgemein” auf Seite I-170>

                                 Eine gespeicherte Tour kopieren
                                 Über diese Funktion haben Sie die Möglichkeit, durch das Kopieren einer Tour
                                 verschiedene Simulationen durchzuführen, damit Sie die bestmögliche Ent-
                                 scheidung treffen können.
                                 Durch das Kopieren der Tour wird die ID verändert. Für dieses Vorgehen ist
                                 der Tour-Status unerheblich, d. h. Sie können Touren mit allen Tour-Status ko-
                                 pieren.




                                 Abb. I-21     Gespeicherte Tour kopieren
2.01 / 01-2017




                                 Eine detaillierte Erläuterung der einzelnen Felder finden Sie in der Softwarere-
                                 ferenz.



                 I-64                                                         A+W Business Logistic Optmizer
                 Tutorial                                                                                  Touren planen




                                        Ergänzende Informationen
                                         Softwarereferenz, “Eine gespeicherte Tour kopieren” auf Seite I-165>
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                                    I-65
                 Touren planen                                                                        Tutorial




                                 Mit Touren arbeiten
                                 In dieser Einheit lernen Sie, wie Sie neue Touren anlegen, bearbeiten oder
                                 auch löschen.
                                 Zu dieser Lerneinheit gibt es folgende Handlungsanweisungen:
                                 •   “So legen Sie eine neue Tour an” auf Seite I-66
                                 •   “So laden Sie eine gespeicherte Tour” auf Seite I-70
                                 •   “So kopieren Sie eine gespeicherte Tour” auf Seite I-71
                                 •   “So löschen Sie eine aktuelle Tour” auf Seite I-71
                                 •   “So legen Sie Touren zusammen” auf Seite I-72


                                  So legen Sie eine neue Tour an
                                 1 Betätigen Sie die Symbol-Schaltfläche [Neue Tour].
                                     Es öffnet sich der Dialog Tour, Register Allgemein.




                                 2 Geben Sie im Feld Liefertermin an, an welchem Tag die Tour gefahren wer-
                                   den soll.
                                     Ein Klick auf den kleinen Pfeil am Ende des Feldes, öffnet den Kalender,
                                     aus dem Sie bequem per Mausklick das entsprechende Datum wählen
                                     können.
                                 3 Geben Sie im Feld Startzeit an, um wie viel Uhr die Tour beginnen soll.
                                     Über die Pfeile hoch und runter am Ende des Feldes können Sie die Zeit
2.01 / 01-2017




                                     einstellen.




                 I-66                                                        A+W Business Logistic Optmizer
                 Tutorial                                                                              Touren planen




                                        4 Vergeben Sie im Feld Tour-Name einen Namen für die Tour.
                                        5 Im Feld Beschreibung können Sie eine detaillierte Beschreibung zur Tour
                                          hinterlegen.
                                        6 Die Inhalte der Felder Name, Adresse, im Bereich Ausgangspunkt sind
                                          Werte, die Sie in den Parametern (Felder: Start-Firmenname, Start-Adres-
                                          se) hinterlegt haben.
                                           Sollte Ihre Tour nicht dort beginnen, können Sie die Einträge überschrei-
                                           ben.
                                        7 Soll die unter Punkt 6 angegebene Adresse auch als Ausgangspunkt der
                                          Tour dienen, aktivieren Sie die Checkbox Ausgangspunkt verwenden.
                                           Wenn Adresse und Ausgangspunkt nicht übereinstimmen, könnte das da-
                                           ran liegen, dass Sie einen Hauptsitz mit mehreren Filialen haben. Dann ist
                                           der Hauptsitz nicht der Ausgangspunkt der Tour.
                                        8 Sind die Felder Längen- und Breitengrad nicht gefüllt, klicken Sie auf die
                                          Symbol-Schaltfläche [Geolokalisieren].
                                           Es öffnet sich der Dialog Einfache Geolokalisierung.




                                           In der Kartenansicht wird Ihnen die Adresse mit einem roten Punkt ange-
                                           zeigt. Handelt es sich um die korrekte Adresse, werden die Felder Breiten-
                                           und Längengrad automatisch gefüllt.
                                        9 Sie können die Daten mit der Symbol-Schaltfläche [Akzeptieren] überneh-
                                          men.
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                                 I-67
                 Touren planen                                                                     Tutorial




                                 10 Wechseln Sie anschließend in das Register Fahrzeuge.




                                 11 Betätigen Sie die Symbol-Schaltfläche [Fahrzeug wählen].
                                    Es öffnet sich der Dialog Fahrzeug wählen.




                                 12 Wählen Sie das Fahrzeug aus, mit dem die Tour gefahren werden soll.
                                 13 Betätigen Sie die Symbol-Schaltfläche [OK].
                                    Das Fahrzeug wird übernommen.
2.01 / 01-2017




                 I-68                                                      A+W Business Logistic Optmizer
                 Tutorial                                                                          Touren planen




                                        14 Wechseln Sie in das Register Parameter.




                                        15 Treffen Sie die gewünschte Auswahl für Maut-, Autobahn- und Tunnel-Mo-
                                           dus.
                                        16 Wählen Sie den Tour-Modus.
                                        17 Wenn gewünscht, verändern Sie die Tour-Faktoren im Bereich Optimie-
                                           rung.




                                        18 Betätigen Sie die Symbol-Schaltfläche [OK].
                                           Die Einstellungen werden übernommen. Sie befinden sich wieder im Be-
                                           reich Planung.
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                             I-69
                 Touren planen                                                                        Tutorial




                                  So laden Sie eine gespeicherte Tour
                                 1 Betätigen Sie die Symbol-Schaltfläche [Gespeicherte Touren laden].
                                    Es öffnet sich der Dialog Gespeicherte Tour-Listen.




                                 2 Wählen Sie die gewünschte Tour aus.
                                 3 Betätigen Sie die Symbol-Schaltfläche [OK].
                                    Sie werden gefragt, ob Sie die gespeicherte Tour den aktuellen Touren hin-
                                    zufügen möchten.
                                 4 Betätigen Sie die Schaltfläche [Ja].
                                    Die ausgewählte Tour wird übernommen. Sie befinden sich wieder im Be-
                                    reich Planung.


                                  So löschen Sie eine gespeicherteTour
                                 1 Betätigen Sie die Symbol-Schaltfläche [Gespeicherte Touren laden].
                                    Es öffnet sich der Dialog Gespeicherte Tour-Listen.
                                 2 Wählen Sie die Tour aus, die kopiert werden soll.
                                 3 Betätigen Sie die Symbol-Schaltfläche [Tour löschen].
                                    Sie werden gefragt, ob Sie die Tour wirklich löschen möchten.
                                 4 Betätigen Sie die Schaltfläche [Ja].
                                    Die ausgewählte Tour wird gelöscht.
2.01 / 01-2017




                 I-70                                                       A+W Business Logistic Optmizer
                 Tutorial                                                                             Touren planen




                                         So kopieren Sie eine gespeicherte Tour
                                        1 Betätigen Sie die Symbol-Schaltfläche [Tour kopieren].
                                           Es öffnet sich der Dialog Gespeicherte Touren.




                                        2 Wählen Sie die gewünschte Tour aus.
                                        3 Betätigen Sie die Symbol-Schaltfläche [Tour].
                                           Sie werden gefragt, ob Sie die gespeicherte Tour der aktuellen Tour hinzu-
                                           fügen möchten.
                                        4 Betätigen Sie die Schaltfläche [Ja].
                                           Die ausgewählte Tour wird übernommen. Sie befinden sich wieder im Be-
                                           reich Planung.


                                         So löschen Sie eine aktuelle Tour
                                        1 Wählen Sie im Bereich Touren die Tour aus, die gelöscht werden soll.
                                        2 Betätigen Sie die Symbol-Schaltfläche [Tour löschen].
                                           Sie werden gefragt, ob Sie die Tour wirklich löschen möchten.
                                        3 Betätigen Sie die Schaltfläche [Ja].
                                           Die ausgewählte Tour wird gelöscht.
                                        4 Betätigen Sie die Symbol-Schaltfläche [Tour löschen].
                                           Sie werden gefragt, ob Sie die Tour wirklich löschen möchten.
                                        5 Betätigen Sie die Schaltfläche [Ja].
                                           Die ausgewählte Tour wird gelöscht.
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                                 I-71
                 Touren planen                                                                           Tutorial




                                  So legen Sie Touren zusammen
                                    Unter Umständen kann es sinnvoll sein, zwei Touren zu einer Tour zusam-
                                    menzufassen. Dazu gehen Sie wie folgt vor:
                                 1 Markieren Sie im Bereich Bestimmungsorte die Datensätze, die zusam-
                                   mengefasst werden sollen.




                                 2 Öffnen Sie mit der rechten Maustaste das Kontextmenü. Wichtig ist hier,
                                   wo (auf welcher Tour) Sie die rechte Maustaste betätigen. Dieser Tour wei-
                                   sen Sie die zusätzlichen Haltepunkte zu.
                                    Es erscheint folgende Meldung:




                                 3 Gehen Sie mit dem Mauszeiger auf die Meldung und klicken Sie diese an.
                                 4 Die beiden Touren werden zu einer Tour zusammengefügt.




                                 Ergänzende Informationen
                                  Tutorial, “Touren und Bestimmungsorte” auf Seite I-60
                                  Tutorial, “Fahrzeuge” auf Seite I-45
                                  Softwarereferenz, “Eine gespeicherte Tour laden” auf Seite I-168
                                  Softwarereferenz, “Eine neue Tour zusammenstellen – Allgemein” auf Seite I-170
                                  Softwarereferenz, “Eine neue Tour zusammenstellen – Fahrzeuge” auf Seite I-174
2.01 / 01-2017




                                  Softwarereferenz, “Eine neue Tour zusammenstellen – Parameter” auf Seite I-180
                                  Softwarereferenz, “Fahrzeuge” auf Seite I-152




                 I-72                                                         A+W Business Logistic Optmizer
                 Tutorial                                                                                 Touren planen




                                        Bestimmungsorte
                                        Dieser Bereich enthält Informationen zu den einzelnen Bestimmungsorten, die
                                        auf der Tour angefahren werden. An einem Bestimmungsort wird entweder
                                        Ware abgeladen oder Gestelle werden abgeholt.

                                           Anzahl an Wegpunkten
                                           Bitte beachten Sie, dass eine Route nicht mehr als 37 Wegpunkte (Bestim-
                                           mungsorte) haben darf. Dies ist die maximale Anzahl, mit der Nokia inner-
                                           halb einer Route arbeiten kann.




                                        Abb. I-22    Bestimmungsorte


                                        Die Inhalte des Feldes Tour-Name (TOUR NORD) kommen aus den A+W
                                        Business-Stammdaten. Die Tour ID (8) wird von OTR vergeben und für jede
                                        Tour um 1 erhöht. Die Reihenfolge der Wegpunkte kommt aus A+W Business,
                                        wobei 0 den Startpunkt kennzeichnet. Im Feld Auftrag wird Ihnen die Auftrags-
                                        Nummer angezeigt, im Feld Kunde die Kunden-Nummer, im Feld Name der
                                        Kunden-Name und im Feld Adresse die Kunden-Adresse.
                                        Das Feld Versandgewicht enthält das Gewicht der Waren, die ausgeliefert
                                        werden. Im Feld Rückholgewicht sehen Sie, wie schwer Rückholungen sind.
                                        Das können z. B. leere Gestelle sein, die Sie unterwegs mitnehmen.
                                        Die Checkboxen Lieferung und Abholung zeigen Ihnen, ob es sich bei dem
                                        Wegpunkt um eine Anlieferstelle, eine Abholstelle oder um beides handelt.
                                        Klicken Sie einen Bestimmungsort doppelt an, öffnet sich der Dialog Bestim-
                                        mungsort bearbeiten.
                                        Eine detaillierte Erläuterung der einzelnen Felder finden Sie in der Software-
                                        referenz.


                                        Ergänzende Informationen
                                         Softwarereferenz, “Bestimmungsort bearbeiten” auf Seite I-191
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                                   I-73
                 Touren planen                                                                           Tutorial




                                 Dokumente anzeigen
                                 Möchten Sie wissen, was ein Kunde alles bestellt hat, können Sie sich die ein-
                                 zelnen Aufträge anzeigen lassen.
                                 Dazu öffnen Sie einfach das Register Dokumente.




                                 Abb. I-23    Dokumente


                                 Eine detaillierte Erläuterung der einzelnen Felder finden Sie in der Softwarere-
                                 ferenz.


                                 Ergänzende Informationen
                                  Softwarereferenz, “Informationen anzeigen” auf Seite I-198

                                 Dokumente löschen
                                 Über das Kontextmenü haben Sie die Möglichkeit, Dokumente zu löschen.
                                 Das kann z. B. nötig sein für Dokumente, deren Inhalte nicht geliefert werden.




                                 Abb. I-24    Dokumente
2.01 / 01-2017




                 I-74                                                          A+W Business Logistic Optmizer
                 Tutorial                                                                                Touren planen




                                        Positionen anzeigen
                                        Möchten Sie wissen, welcher Kunde was bestellt hat, können Sie sich die ein-
                                        zelnen Positionen pro Bestimmungsort anzeigen lassen.
                                        Dazu öffnen Sie einfach das Register Positionen.




                                        Abb. I-25    Positionen


                                        Eine detaillierte Erläuterung der einzelnen Felder finden Sie in der Softwarere-
                                        ferenz.


                                        Ergänzende Informationen
                                         Softwarereferenz, “Positionen anzeigen” auf Seite I-196
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                                    I-75
                 Touren planen                                                                           Tutorial




                                 Informationen anzeigen
                                 Möchten Sie wissen, welche Informationen zu einem Kunden hinterlegt sind,
                                 können Sie sich diese anzeigen lassen.
                                 Dazu öffnen Sie einfach das Register Informationen.




                                 Abb. I-26    Informationen


                                 Eine detaillierte Erläuterung der einzelnen Felder finden Sie in der Softwarere-
                                 ferenz.


                                 Ergänzende Informationen
                                  Softwarereferenz, “Informationen anzeigen” auf Seite I-198
2.01 / 01-2017




                 I-76                                                          A+W Business Logistic Optmizer
                 Tutorial                                                                              Touren planen




                                        Die Detailansicht
                                        Haben Sie einen großen Fuhrpark und einem großen Versandbereich, kann
                                        es sein, dass die Inhalte der Bereiche Touren und Bestimmungsorte sehr un-
                                        übersichtlich werden.
                                        Über die Detailansicht haben Sie die Möglichkeit, die angezeigten Daten zu li-
                                        mitieren.




                                        Abb. I-27    Detailansicht nicht eingeschaltet


                                        Ist die Detailansicht aktiv, werden Ihnen nur die Bestimmungsorte der Tour an-
                                        gezeigt, die Sie im Bereich Touren selektiert haben.
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                                  I-77
                 Touren planen                                                                           Tutorial




                                 Abb. I-28     Detailansicht eingeschaltet


                                 Wenn Sie im Bereich Touren Detailansicht eine Tour markieren, können Sie
                                 diese über die Symbol-Schaltfläche Gruppen in mehrere Gruppen unterteilen.
                                 Eine detaillierte Erläuterung der einzelnen Felder finden Sie in der Softwarere-
                                 ferenz.


                                 Ergänzende Informationen
                                  Softwarereferenz, “Detailansicht” auf Seite I-202
2.01 / 01-2017




                 I-78                                                           A+W Business Logistic Optmizer
                 Tutorial                                                                                Touren planen




                                        Kundenadressen bearbeiten
                                        OTR bietet die Möglichkeit, Kundendaten zu speichern. Dazu muss in den Pa-
                                        rametern der entsprechende Wert (Parameter: OTR-Kundenadressen) akti-
                                        viert werden.
                                        Anschließend ist sowohl die Symbol-Schaltfläche als auch der entsprechende
                                        Dialog aktiv.




                                        Abb. I-29    Kunden


                                        Klicken Sie einen Eintrag doppelt an, öffnet sich der Dialog Bestimmungsort
                                        bearbeiten. Änderungen, die Sie in diesem Dialog vornehmen, werden in der
                                        OTR-Datenbank gespeichert und stehen Ihnen das nächste Mal zur Verfü-
                                        gung. Es werden die folgenden Werte gespeichert:
                                        •   Geolokalisation
                                        •   Adresse
                                        •   Anfahrzeiten (Von / Bis)
                                        •   Abladezeit
                                        Eine detaillierte Erläuterung der einzelnen Felder finden Sie in der Softwarere-
                                        ferenz.

                                            Änderungen an Kundenadressen
                                            Bitte beachten Sie, dass Änderungen an Kundenadressen, die Sie hier vor-
                                            nehmen, nicht zurück geschrieben werden an A+W Business. Die Ände-
                                            rungen werden in der OTR-Datenbank gespeichert.


                                        Ergänzende Informationen
                                         Softwarereferenz, “Kunden” auf Seite I-200
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                                    I-79
                 Touren planen                                                                        Tutorial




                                 Mit Bestimmungsorten arbeiten
                                 In dieser Einheit lernen Sie, wie Sie Bestimmungsorte einer Tour hinzufügen,
                                 ändern oder auch löschen.
                                 Zu dieser Lerneinheit gibt es folgende Handlungsanweisungen:
                                 •   “So fügen Sie einer Tour einen neuen Bestimmungsort hinzu” auf Seite I-80
                                 •   “So löschen Sie einen Bestimmungsort aus der Tour” auf Seite I-81
                                 •   “So bearbeiten Sie einen Bestimmungsort” auf Seite I-82


                                  So fügen Sie einer Tour einen neuen Bestimmungsort hinzu
                                 1 Markieren Sie im Bereich Touren die Tour, der Sie einen neuen Bestim-
                                   mungsort hinzufügen möchten.
                                 2 Betätigen Sie die Symbol-Schaltfläche [Neuer Bestimmungsort].
                                     Es öffnet sich der Dialog Neuer Bestimmungsort.




                                     Das Feld Kunden-Nr. ist mit der Nummer 9999 vorbelegt.
                                 3 Geben Sie im Feld Kunde den entsprechenden Namen ein oder öffnen Sie
                                   über die Symbol-Schaltfläche [Kunde] den gleichnamigen Dialog dazu.
                                     Dort sind alle in der OTR-Datenbank gespeicherten Kunden gelistet.
                                 4 Geben Sie im Feld Typ an, ob es sich bei dem Bestimmungsort um den
                                   Startpunkt, den Endpunkt oder den Mittelpunkt der Tour handelt.
                                 5 In den Feldern Von und Bis können Sie Zeiten hinterlegen, zu denen der
2.01 / 01-2017




                                   Fahrer am Bestimmungsort sein soll.
                                     Das kommt z. B. zum Tragen, wenn eine Firma feste Anlieferzeiten hat.




                 I-80                                                       A+W Business Logistic Optmizer
                 Tutorial                                                                             Touren planen




                                        6 Im Feld Zeit (Minuten) können Sie die Aufenthaltsdauer vor Ort hinterle-
                                          gen.
                                        7 Das Feld Ausgewählte Tour enthält alle Touren, die Sie zur Zeit in Planung
                                          haben.
                                           So können Sie den neuen Bestimmungsort einfach der gewünschten Tour
                                           zuordnen.
                                        8 Im Feld Versandgewicht geben Sie das Gewicht der Lieferung an.
                                        9 Im Feld Rückholgewicht können Sie, falls Sie an diesem Bestimmungsort
                                          auch leere Gestelle einsammeln, das Gewicht dieser Gestelle eingeben.
                                           Diese Werte sind für eine korrekte Ermittlung der Kosten nötig aber nicht
                                           zwingend erforderlich.
                                        10 Im Feld Beschreibung können Sie eine detaillierte Erläuterung für den Fah-
                                           rer hinterlegen.
                                        11 Im Feld Adresse geben Sie die Kunden-Adresse ein.
                                           Bitte achten Sie darauf, den Straßennamen und den Ortsnamen komma-
                                           separiert einzugeben.
                                        12 Anschließend betätigen Sie dieSymbol-Schaltfläche [Vorschläge].
                                           Unter der Adresse erscheint eine Liste mit entsprechenden Vorschlägen
                                           sowie die Kartenansicht. Sie können den Eintrag in der Liste markieren,
                                           dann wird er in das Adressfeld übernommen. Sie können aber auch den ro-
                                           ten Markierungspunkt in der Kartenansicht anklicken und ihn mit gedrück-
                                           ter und gehaltener Maustaste an eine andere Stelle in der Karte ziehen.
                                        13 Schließen Sie den Dialog über die Schaltfläche [OK].


                                         So löschen Sie einen Bestimmungsort aus der Tour
                                        1 Markieren Sie im Bereich Bestimmungsorte den Ort, den Sie löschen
                                          möchten.
                                        2 Betätigen Sie die Symbol-Schaltfläche [Bestimmungsort löschen].
                                           Es öffnet sich die Meldung Bestimmungsort löschen.
                                        3 Schließen Sie die Meldung über die Schaltfläche [Ja].
                                           Der Eintrag wird gelöscht.
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                                 I-81
                 Touren planen                                                                       Tutorial




                                  So bearbeiten Sie einen Bestimmungsort
                                 1 Markieren Sie im Bereich Bestimmungsorte den Ort, den Sie bearbeiten
                                   möchten.
                                 2 Betätigen Sie die Symbol-Schaltfläche [Bestimmungsort bearbeiten].
                                    Es öffnet sich der Dialog Bestimmungsort bearbeiten.
                                 3 Führen Sie die entsprechenden Änderungen durch.
                                 4 Schließen Sie den Dialog über die Schaltfläche [OK].


                                 Ergänzende Informationen
                                  Softwarereferenz, “Bestimmungsort bearbeiten” auf Seite I-191
                                  Softwarereferenz, “Kunden” auf Seite I-200
                                  “Mit Touren arbeiten” auf Seite I-66
2.01 / 01-2017




                 I-82                                                         A+W Business Logistic Optmizer
                 Tutorial                                                                                  Touren planen




                                        Kosten
                                        Lernziele

                                        • Den Dialog Kosten erarbeiten
                                        • Den Umgang mit den unterschiedlichen Kosten kennenlernen und verstehen
                                        • Kosten anlegen und bearbeiten


                                        Nutzen

                                        • Zum Ermitteln der Tourkosten ist es notwendig, die Fuhrparkdaten möglichst
                                          genau zu pflegen. Nur so erhalten Sie genaue Werte.


                                        Definition

                                        Variable Kosten            Kosten, die sich bei Änderungen einer Bezugsgröße
                                                                   (Gesamtstrecke, Kraftstoffkosten) ebenfalls ändern.

                                        Fixkosten                  Kosten, die bei Änderung einer Bezugsgröße
                                                                   (Gesamtstrecke, Kraftstoffkosten) konstant bleiben.

                                        Tourkosten                 Das, was die Tour effektiv kostet.


                                        Merke

                                        Tatsächliche Kosten        Können erst erfasst werden, wenn der Fahrer von der
                                                                   Tour zurück ist.
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                                          I-83
                 Touren planen                                                                           Tutorial




                                 Ausgaben
                                 Dieser Bereich zeigt Ihnen, mit welchen Ausgaben Sie bei der Tour rechnen
                                 müssen.




                                 Abb. I-30     Kosten


                                 Die Felder werden nach durchlaufener Optimierung automatisch gefüllt. An-
                                 hand der Werte können Sie unterschiedliche Reports erstellen, die Sie dann
                                 als Kostenanalyse dem Kunden gegenüber darstellen können.
                                 Das Register ist in drei Bereiche unterteilt:
                                 •   Variable Kosten / Tatsächliche variable Kosten
                                 •   Fixkosten / Tatsächliche Fixkosten
                                 •   Tourkosten / Tatsächliche Tourkosten


                                 Variable Kosten
                                 In diesem Bereich befinden sich die Kosten, die beweglich sind und die sich
                                 bei Änderungen einer Bezugsgröße (Gesamtstrecke, Kraftstoffkosten) eben-
                                 falls ändern. Dabei handelt es sich z. B. um den durchschnittlichen Kraftstoff-
                                 preis und den durchschnittlichen Verbrauch. Die Werte ergeben sich aus den
                                 jeweiligen Parametern (Konfiguration > Parameter > Fahrzeuge).
                                 Die Werte im Bereich Tatsächliche variable Kosten können erst eingetragen
                                 werden, wenn Ihr Fahrer mit dem Tourbericht zurück ist. Dann wissen Sie, wie
                                 hoch die tatsächlichen Kosten waren. Diese tragen Sie im Dialog Tour bear-
2.01 / 01-2017




                                 beiten Register Tour-Informationen ein.
                                 Eine detaillierte Erläuterung der einzelnen Felder finden Sie in der Softwarere-
                                 ferenz.


                 I-84                                                            A+W Business Logistic Optmizer
                 Tutorial                                                                                Touren planen




                                        Fixkosten
                                        In diesem Bereich befinden sich die festen Kosten, die bei Änderung einer Be-
                                        zugsgröße (Gesamtstrecke, Kraftstoffkosten) konstant bleiben. Dabei handelt
                                        es sich z. B. um die Versicherung, die Steuer und die Reparaturen.
                                        Beispiel:

                                        Kostenart                 Kosten/Jahr

                                        Versicherung pro Jahr     1.200,00 €

                                        Steuer pro Jahr           800,00 €

                                        Wartung pro Jahr          300,00 €


                                        In Summe: 2.300,00 €. Bei einer geschätzten Anzahl an Routen von ca. 220
                                        pro Jahr, ergibt das einen Fixkostenbetrag von 10,45 € pro Route. Dieser Wert
                                        sollte in den Fahrzeug-Stammdaten hinterlegt werden. Wird das Fahrzeug
                                        dann einer Route zugeordnet, werden die Fixkosten um die 10,45 € erhöht.
                                        Eine detaillierte Erläuterung der einzelnen Felder finden Sie in der Softwarere-
                                        ferenz.


                                        Tourkosten
                                        In diesem Bereich befinden sich die Gesamtkosten der Tour. Die Tourkosten
                                        setzen sich aus den variablen Kosten und den Fixkosten zusammen. Sie kön-
                                        nen manuell nicht geändert werden.
                                        Eine detaillierte Erläuterung der einzelnen Felder finden Sie in der Softwarere-
                                        ferenz.


                                        Ergänzende Informationen
                                         Softwarereferenz, “Eine neue Tour zusammenstellen – Kosten” auf Seite I-186
                                         Softwarereferenz, “Tour-Informationen” auf Seite I-209
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                                    I-85
                 Touren optimieren                                                                   Tutorial




                                     Touren optimieren
                                     Dieser Themenblock befasst sich mit der Optimierung der Tour.
                                     Dazu gehören folgende Lerneinheiten:
                                     •   “Touren optimieren” auf Seite I-88
                                     •   “Touren verändern” auf Seite I-92
2.01 / 01-2017




                 I-86                                                         A+W Business Logistic Optmizer
                 Tutorial                                                                               Touren optimieren




                                        Überblick
                                        Lernziele

                                        • Optimierung der Tour kennenlernen und verstehen


                                        Nutzen

                                        • Je effizienter die Tour gefahren wird, um so mehr reduzieren sich die Kosten. Die
                                          Fahrtstrecken werden optimal kalkuliert und Ihre Fahrer sind weniger belastet.


                                        Merke

                                        Optimierte Tour             Reihenfolge der Wegpunkte nach der Optimierung.

                                        Ursprüngliche Tour          Reihenfolge der Wegpunkte vor der Optimierung.
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                                        I-87
                 Touren optimieren                                                                          Tutorial




                                     Touren optimieren
                                     Nachdem alle Wegpunkte lokalisiert werden konnten, erfolgt im nächsten
                                     Schritt die Optimierung der Fahrstrecke (Route). D. h., OTR bringt – unter Be-
                                     rücksichtigung der eingestellten Faktoren – die einzelnen Wegpunkte in eine
                                     optimale Reihenfolge.




                                     Abb. I-31    Optimierung der Tour


                                     Der Dialog zeigt Ihnen das Ergebnis der Optimierung, sowohl grafisch als
                                     auch tabellarisch.
                                     Auf der linken Seite befindet sich die Karte mit der eingezeichneten Route. Die
                                     Routenbreite und die Routentransparenz können Sie in den Parametern ein-
                                     stellen (Parameter: Optimized_Route_Opacity, Optimized_Route_Width).
                                     Rechts sehen Sie die Route in Listenform.
                                     Die Kombobox oben rechts enthält alle Touren, die Sie optimiert haben. Haben
                                     Sie mehr als eine Tour optimiert, können Sie über die Kombobox die entspre-
                                     chende Tour auswählen.




                                     Die beiden Register darunter (Optimierte Tour/Ursprüngliche Tour) zeigen Ih-
                                     nen die Reihenfolge der einzelnen Stationen nach der Optimierung (Register
                                     Optimierte Tour) und vor der Optimierung (Register Ursprüngliche Tour).
2.01 / 01-2017




                                     Die darunter liegende Liste gibt Ihnen im oberen Bereich eine Zusammenfas-
                                     sung der Tour.



                 I-88                                                            A+W Business Logistic Optmizer
                 Tutorial                                                                                 Touren optimieren




                                        Im Beispiel oben besteht die Tour aus vier Stationen, wobei der Startpunkt der
                                        Tour immer als eine Station angesehen wird.
                                        Mit Hilfe des daneben liegenden Symbols können Sie die Route in der Karten-
                                        ansicht ein- und ausblenden. Mögliche Einstellungen sind:

                                        Symbol       Erläuterung

                                                     Verkehr
                                                     Dieses Symbol zeigt an, dass die Verkehrslage eingeschaltet
                                                     ist.

                                                     Route einblenden
                                                     Ist dieses Symbol aktiviert, wird die Route in der Kartenansicht
                                                     eingeblendet.

                                                     Route ausblenden
                                                     Ist dieses Symbol aktiviert, wird die Route in der Kartenansicht
                                                     ausgeblendet.


                                        Über das Farben-Symbol haben Sie die Möglichkeit, die Routenfarbe in der
                                        Kartenansicht temporär zu ändern. Klicken Sie das Symbol doppelt an, öffnet
                                        sich der Dialog Farbe. Dort können Sie der Route eine andere Farbe zuwei-
                                        sen. Der Standardwert der Farbe kommt aus den Parametern
                                        (Optimized_Route_Color).
                                        Die kleinen, weißen Pfeile in der Route zeigen Ihnen die Fahrtrichtung an.
                                        Die Tour hat eine Gesamtstrecke von 152,13 km. Die Fahrtzeit beträgt zwei
                                        Stunden und 2 Minuten. Die Kosten der Tour belaufen sich auf 15,44 €. Dieser
                                        Wert errechnet sich durch den Verbrauch des Fahrzeuges, den Kraftstoffkos-
                                        ten und der Gesamtstrecke.

                                           Kosten der Tour
                                           Die Kosten der Tour errechnen sich aus den Werten, die Sie für die Fahr-
                                           zeuge hinterlegen. Je genauer diese Werte sind, um so genauer sind die
                                           Tourkosten. Das betrifft in erster Linie die Kraftstoffkosten, die mitunter
                                           sehr schwanken.

                                        Das daneben liegende Feld Maut informiert Sie darüber, ob die Route Straßen
                                        enthält, auf denen eine Maut zu entrichten ist.
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                                         I-89
                 Touren optimieren                                                                                Tutorial




                                     Der Startpunkt wird durch einen grünen Punkt gekennzeichnet. Dieser Weg-
                                     punkt wurde von Ihnen bei der Planung der Tour als solcher deklariert. Sie
                                     können ihn hier weder verschieben noch ändern. Für solche Änderungen
                                     müssen Sie wieder in die Planung wechseln.
                                     Alle nachfolgenden Wegpunkte haben einen roten Punkt. Darüber hinaus gibt
                                     es folgende Informations-Symbole:

                                     Symbol      Erläuterung

                                                 Lieferung
                                                 Dieses Symbol zeigt Ihnen, dass bei der Adresse Waren abgeladen
                                                 werden.

                                                 Abholung
                                                 Dieses Symbol zeigt Ihnen, dass bei der Adresse Waren (in der Regel
                                                 Gestelle) aufgeladen werden.

                                                 Rechtzeitig
                                                 Dieses Symbol zeigt Ihnen, dass es für die Adresse eine festgelegte
                                                 Zeit gibt, zu der abgeladen oder aufgeladen werden soll. Dies kann
                                                 der Fall sein, wenn der Kunde feste Zeiten für Warenannahmen hat
                                                 oder nur zu bestimmten Zeiten an Baustellen abgeladen werden
                                                 kann.

                                                 Priorität
                                                 Dieses Symbol zeigt Ihnen, dass die Adresse ein Priorität hat.


                                     Durch Drag & Drop können Sie Wegpunkte in der Liste an eine andere Stelle
                                     schieben. Nachdem ein Wegpunkt verschoben wurde, führt das System auto-
                                     matisch eine Neu-Optimierung durch.
                                     Klicken Sie einen Wegpunkt in der Liste doppelt an, erscheint in der Karten-
                                     ansicht ein Feld mit entsprechenden Detailinformationen. Dieses Feld er-
                                     scheint auch, wenn Sie den Wegpunkt in der Kartenansicht doppelt anklicken.




                                     Klicken Sie einen Routenabschnitt in der Kartenansicht doppelt an, erscheint
                                     ein Feld mit entsprechenden Streckeninformationen, z. B. Distanz von A
                                     nach B.
2.01 / 01-2017




                 I-90                                                              A+W Business Logistic Optmizer
                 Tutorial                                                                           Touren optimieren




                                        Unterschiedliche Kartenmodi
                                        Hier können Sie zwischen verschiedenen Kartenansichten wählen:




                                        In der Geländeansicht können Sie sich die Topografie und Höhe ansehen. Die
                                        Satellitenansicht liefert Ihnen 2D-Bilder und die Kartenansicht zeigt Ihnen die
                                        Karte.
                                        Nächster Schritt:
                                        •   Ergebnis der Optimierung, Seite I-97


                                        Ergänzende Informationen
                                         Softwarereferenz, “Tour optimieren” auf Seite I-204
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                                   I-91
                 Touren optimieren                                                                          Tutorial




                                     Touren verändern
                                     In dieser Einheit lernen Sie, wie Sie Tourkriterien ändern können.
                                     Zu dieser Lerneinheit gibt es folgende Handlungsanweisungen:
                                     •   “So weißen Sie einem Wegpunkt eine Priorität zu” auf Seite I-92
                                     •   “So entfernen Sie die Priorität eines Wegpunktes” auf Seite I-92
                                     •   “So ändern Sie die Reihenfolge manuell” auf Seite I-92
                                     •   “So stoppen Sie eine Optimierung” auf Seite I-93
                                     •   “So bearbeiten Sie die Tour” auf Seite I-93
                                     •   “So verändern Sie die Faktoren” auf Seite I-94


                                      So weißen Sie einem Wegpunkt eine Priorität zu
                                     1 Markieren Sie den Wegpunkt in der Liste.
                                     2 Klicken Sie mit der Maus auf das Fähnchen.
                                         Das Fähnchen wird jetzt in grüner Farbe dargestellt und symbolisiert damit,
                                         dass die Adresse Priorität hat.
                                         Nach erneuter Optimierung befindet sich dieser Wegpunkt an erster Stelle
                                         (Priorität).


                                      So entfernen Sie die Priorität eines Wegpunktes
                                     1 Markieren Sie den Wegpunkt mit der Priorität.
                                     2 Klicken Sie mit der Maus auf das Fähnchen.
                                         Das Fähnchen wird jetzt in grauer Farbe dargestellt und symbolisiert damit,
                                         dass die Adresse keine Priorität mehr hat.
                                     3 Nach erneuter Optimierung befindet sich dieser Wegpunkt an beliebiger
                                       Stelle in der Reihenfolge.


                                      So ändern Sie die Reihenfolge manuell
                                     1 Markieren Sie den Wegpunkt in der Liste und halten Sie die Maustaste ge-
                                       drückt.
                                     2 Ziehen Sie den Wegpunkt an die gewünschte Stelle innerhalb der Liste.
                                     3 An dieser Stelle angekommen, lassen Sie die Maustaste wieder los.
                                         Der Wegpunkt wird dort hin verschoben

                                         Neu optimieren nicht vergessen
                                         Wenn Sie die Reihenfolge der Wegpunkte manuell ändern, müssen Sie an-
                                         schließend die Tour nochmal optimieren um die Werte zu aktualisieren.
2.01 / 01-2017




                 I-92                                                             A+W Business Logistic Optmizer
                 Tutorial                                                                           Touren optimieren




                                         So stoppen Sie eine Optimierung
                                           Sollte es, aus welchen Gründen auch immer, nötig sein, die Optimierung
                                           zu stoppen, gehen Sie bitte wie folgt vor.
                                        1 Betätigen Sie die Symbol-Schaltfläche [Optimierung stoppen].
                                           Die Optimierung wird gestoppt.
                                           Die Daten der vorhergehenden Optimierung bleiben erhalten und werden
                                           angezeigt.


                                         So bearbeiten Sie die Tour
                                        1 Betätigen Sie die Symbol-Schaltfläche [Tour bearbeiten].
                                           Es öffnet sich der Dialog Tour für die ausgewählte Tour. In diesem Register
                                           können Sie den Liefertermin, die Startzeit und den Tour-Namen ändern.




                                        2 Im Register Fahrzeuge können Sie das Fahrzeug und den Fahrer ändern.
                                        3 Im Register Parameter können Sie die Tour-Modi und die Optimierungs-
                                          Faktoren ändern.
                                        4 Im Register Kosten können Sie die Mautkosten und die Extrakosten än-
                                          dern.
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                                  I-93
                 Touren optimieren                                                                          Tutorial




                                      So verändern Sie die Faktoren
                                     1 Betätigen Sie die Symbol-Schaltfläche [Optimierungs-Faktoren].
                                        Es öffnet sich der Dialog Tour-Faktoren für die ausgewählte Tour.




                                     2 Sie können jetzt für jeden einzelnen Faktor die Regler hin und her bewe-
                                       gen.
                                        Da die Summe immer 100 % ergibt, hat das Verändern eines Faktors im-
                                        mer auch Auswirkungen auf die anderen Faktoren.
                                     3 Möchten Sie einen Wert fixieren, betätigen Sie die Symbol-Schaltfläche
                                       [Sperren].
                                        Dann wird dieser Wert gesperrt und nicht mehr verändert.
                                     4 Um die Faktoren auf die Standardwerte zurück zu setzen, betätigen Sie die
                                       Symbol-Schaltfläche [Standardwerte].
                                        Die Werte werden dann gemäß den Einstellungen in den Parametern ge-
                                        ändert.


                                     Ergänzende Informationen
                                      Softwarereferenz, “Tour-Faktoren” auf Seite I-184
2.01 / 01-2017




                 I-94                                                              A+W Business Logistic Optmizer
                 Tutorial                                                                      Ergebnisse prüfen




                                        Ergebnisse prüfen
                                        Dieser Themenblock befasst sich mit dem Ergebnis der Optimierung.
                                        Dazu gehören folgende Lerneinheiten:
                                        •   “Das Ergebnis der Optimierung” auf Seite I-97
                                        •   “Tourstatus ändern” auf Seite I-99
                                        •   “Tatsächliche Tourkosten” auf Seite I-100
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                             I-95
                 Ergebnisse prüfen                                                                                 Tutorial




                                     Überblick
                                     Lernziele

                                     •   Den Tour-Status ändern
                                     •   Die Daten für ein Navigationssystem exportieren
                                     •   Lieferlisten für Ihre Fahrer drucken
                                     •   Tatsächliche Tourkosten nachträglich erfassen


                                     Nutzen

                                     • Durch das Erfassen der tatsächlichen Tourkosten werden die geschätzten
                                       Tourkosten immer genauer. Dadurch haben Sie, was die Kosten betrifft, eine
                                       immer bessere Grundlage zur Planung.


                                     Definition

                                     Polylinien                  Linien werden auf der Karte mit Hilfe von Polylinien
                                                                 dargestellt, die für eine sortierte Abfolge von Standorten
                                                                 stehen.

                                     Markierungen                Sind Objekte auf der Karte, die an Breitengrad- und
                                                                 Längengradkoordinaten gebunden sind.


                                     Merke

                                     Weiß hinterlegte Felder     Die weiß hinterlegten Felder in den Dialogen Tour und
                                                                 Bestimmungsort dienen zum Kopieren des Feldinhaltes.
                                                                 Es können keine Änderungen an den Inhalten
                                                                 vorgenommen werden.

                                     Tatsächliche Kosten         Die tatsächlichen Tourkosten können erst ermittelt
                                                                 werden, wenn der Fahrer von der Tour zurück ist und
                                                                 seinen Tourbericht abgegeben hat.
2.01 / 01-2017




                 I-96                                                                A+W Business Logistic Optmizer
                 Tutorial                                                                           Ergebnisse prüfen




                                          Das Ergebnis der Optimierung
                                          Nachdem auch die Optimierung durchlaufen wurde, erfolgt im letzten Schritt
                                          die Darstellung des Ergebnisses.




                 Abb. I-32   Ergebnis der Optimierung


                                          Der Dialog zeigt Ihnen das Ergebnis der Optimierung mit allen Einzelheiten.
                                          Er ist in drei Bereiche unterteilt:
                                          •   Touren
                                          •   Tourenplan
                                          •   Bestimmungsort

                                          Touren
                                          In diesem Bereich finden Sie die Touren der aktuellen Optimierung.




                 Abb. I-33   Ergebnis der Optimierung, Bereich Touren
2.01 / 01-2017




                                          Im Feld Tour Status bekommen Sie den Status der Tour angezeigt. Nach der
                                          Optimierung ist der Status Grobgeplant. Anschließend wird Ihnen der Liefer-
                                          termin angezeigt.


                 A+W Business Logistic Optmizer                                                                  I-97
                 Ergebnisse prüfen                                                                         Tutorial




                                     Das Feld Ursprüngliche Tour zeigt Ihnen die von A+W Business vergebene
                                     Tour-Nummer. Das Feld Tour ID zeigt die von OTR vergebene Tour ID. Im Feld
                                     Name der Tour steht der Name, den Sie im Bereich Planung vergeben bzw.
                                     ausgewählt haben. Bei den Kosten handelt es sich um die Kosten für einen
                                     Liter Kraftstoff und im Feld Verbrauch sehen Sie den Verbrauch des Fahrzeu-
                                     ges auf 100 km. Das Feld Zurückgelegt KM zeigt Ihnen die gesamte Strecke
                                     und das Feld Tour-Zeit, wie viel Zeit diese Strecke in Anspruch nimmt. Die
                                     Tourkosten errechnen sich durch die Strecke, den Verbrauch je Fahrzeug so-
                                     wie den Kraftstoffpreis. Im Feld Gewicht sehen Sie, wie schwer die Ladung ist,
                                     wobei zurückgeholte Gestelle mit einem Minus-Zeichen dargestellt werden.
                                     Das Feld Fahrzeuge zeigt Ihnen, mit welchen Fahrzeug die Tour gefahren wird
                                     und im Feld LKW-Fahrer sehen Sie den Namen des Fahrers.
                                     Ein Doppelklick auf eine Tour öffnet den Dialog Tour, der bereits weiter oben
                                     ausführlich beschrieben wurde.

                                     Tourenplan




                                     Abb. I-34    Tourenplan


                                     In diesem Bereich wird Ihnen die Route mit den Bestimmungsorten angezeigt.
                                     Über die Symbol-Schaltfläche [Vergrößern/Verkleinern] können Sie die Dar-
                                     stellung vergrößern bzw. verkleinern.

                                     Bestimmungsort
                                     In diesem Bereich werden Ihnen die einzelnen Bestimmungsorte angezeigt.
                                     Ein Doppelklick auf einen Bestimmungsort öffnet den Dialog Siehe Bestim-
                                     mungsort, der ebenfalls weiter oben ausführlich beschrieben wurde.


                                     Ergänzende Informationen
                                      Tutorial, “Bestimmungsorte” auf Seite I-73
                                      Softwarereferenz, “Bestimmungsort bearbeiten” auf Seite I-191
2.01 / 01-2017




                 I-98                                                             A+W Business Logistic Optmizer
                 Tutorial                                                                         Ergebnisse prüfen




                                        Tourstatus ändern
                                        Wenn die Optimierung durchlaufen wurde, können Sie in diesem Bereich den
                                        Status der Tour ändern. Es stehen folgende Werte zur Verfügung:
                                        •   Grobgeplant: Das ist der Status der Tour nach der Optimierung.
                                        •   Feingeplant: Dieser Status wird zur Zeit noch nicht ausgewertet.
                                        •   Freigegeben: Wenn Sie den Status in Freigegeben ändern, wird der Liefer-
                                            termin, die Reihenfolge und die Tour an A+W Business zurückgemeldet.
                                            Darüber hinaus werden die Daten an die Cloud gegeben. Sie können den
                                            Status nur einmal auf Freigegeben ändern.
                                        Abgesehen von dem Status können Sie auch die Abteilung ändern und die
                                        Route bearbeiten.


                                         So ändern Sie den Status einer Tour
                                        1 Markieren Sie die Tour in der Liste.
                                        2 Klicken Sie mit der Maus auf die Symbol-Schaltfläche [Tour bearbeiten].
                                            Es öffnet sich der Dialog Tour bearbeiten.




                                        3 Wählen Sie aus der Kombobox Tour-Status den gewünschten Status aus.
                                        4 Den Dialog verlassen Sie mit der Schaltfläche [OK].


                                        Ergänzende Informationen
2.01 / 01-2017




                                         Softwarereferenz, “Tour-Status” auf Seite I-207




                 A+W Business Logistic Optmizer                                                                I-99
                 Ergebnisse prüfen                                                                          Tutorial




                                     Tatsächliche Tourkosten
                                     Erst wenn Ihr Fahrer von der Tour zurück ist, wissen Sie, wie hoch die tatsäch-
                                     lichen Kosten waren. So kann es z. B. sein, dass ein kostenfreier Streckenab-
                                     schnitt gesperrt war und Ihr Fahrer auf einen kostenpflichtigen Strecken-
                                     abschnitt ausweichen musste. Das war bei der Planung der Tour nicht vorher-
                                     sehbar. Somit weichen die tatsächlichen Kosten von den geplanten Kosten für
                                     die Tour ab.
                                     In OTR haben Sie die Möglichkeit, diese tatsächlich angefallenen Kosten im
                                     Nachhinein zu erfassen. Sie stehen dann für zukünftige Tourplanungen zur
                                     Verfügung.


                                      So erfassen Sie die tatsächlichen Kosten
                                     1 Öffnen Sie in der Menüleiste den Punkt Abfrage.
                                     2 Wählen Sie im Bereich Touren die entsprechende Tour aus.
                                     3 Klicken Sie mit der Maus auf die Symbol-Schaltfläche [Tour bearbeiten].
                                        Es öffnet sich der Dialog Tour bearbeiten.
                                     4 Wechseln Sie in das Register Tour-Informationen.
                                        Die Felder der Tatsächlichen Kosten haben zunächst die gleichen Werte
                                        wie die Kosten-Felder auf der rechten Seite.




                                     5 Korrigieren Sie die Felder der Tatsächlichen Kosten.
                                        Sie können die Werte überschreiben oder vorher über die Symbol-Schalt-
                                        fläche [Kosten entfernen] alle Werte auf 0 setzen.
2.01 / 01-2017




                 I-100                                                           A+W Business Logistic Optmizer
                 Tutorial                                                                          Ergebnisse prüfen




                                        6 Wenn Sie mit den Eingaben fertig sind, sehen Sie im Feld Tatsächliche
                                          Tourkosten, wie viel die Tour wirklich gekostet hat.


                                        Ergänzende Informationen
                                         Softwarereferenz, “Tour-Informationen” auf Seite I-209
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                               I-101
                 Touren fahren und überwachen                                                            Tutorial




                                       Touren fahren und überwa-
                                       chen
                                       Dieser Themenblock befasst sich zum einen damit, welche Aktivitäten dem
                                       Fahrer auf der Tour zukommen und welche Möglichkeiten der Mitarbeiter in
                                       der Firma bezüglich des Trackings hat.
                                       Dazu gehören folgende Lerneinheiten:
                                       •   “Vorbereitungen” auf Seite I-104
                                       •   “Touren fahren” auf Seite I-106
                                       •   “Touren überwachen” auf Seite I-114
2.01 / 01-2017




                 I-102                                                           A+W Business Logistic Optmizer
                 Tutorial                                                                  Touren fahren und überwachen




                                        Überblick
                                        Lernziele

                                        •   Dokumente in die Cloud laden.
                                        •   Die GDC-App für die Fahrer kennenlernen und verstehen.
                                        •   Das Buchen über einen Browser kennenlernen und verstehen.
                                        •   Die Möglichkeiten der Lieferüberwachung (im Folgenden auch Tracking genannt)
                                            kennenlernen und verstehen.


                                        Nutzen

                                        • Über die Trackingfunktion werden die Mitarbeiter in der Firma ständig über den
                                          Stand der Route informiert. Auf viele Situationen kann direkt reagiert werden. So
                                          kann z. B. eine zu Bruch gegangene Scheibe nachproduziert werden, während der
                                          LKW noch auf der Tour ist.


                                        Definition

                                        GDC-App                     App für Android, die über den Google Playstore
                                                                    kostenlos heruntergeladen werden kann.


                                        Merke

                                        Android                     Für Android Systeme gibt es die im Google Playstore die
                                                                    App GDC.

                                        und Andere                  Die Benutzer von Nicht-Android-Systemen können sich
                                                                    über den Browser direkt einloggen.

                                        Aktualisieren               Vergessen Sie nicht, im Routen Administrator von Zeit
                                                                    zu Zeit die Schaltfläche [Aktualisieren] zu drücken, damit
                                                                    Ihre Daten abgegelichen werden.
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                                         I-103
                 Touren fahren und überwachen                                                                Tutorial




                                       Vorbereitungen
                                       Damit die App und das GPS-Tracking korrekt funktionieren, sind folgende Vor-
                                       arbeiten nötig:

                                       Entsprechender Tourstatus
                                       Damit die Tourdaten an die Cloud gegeben werden können, müssen Sie den
                                       Tourstatus auf Freigegeben setzen.
                                       Dazu markieren Sie die entsprechende Tour im Bereich Ergebnis, klicken auf
                                       die Symbol-Schaltfläche Tour bearbeiten und wählen aus der Kombobox Tour-
                                       Status den Status Freigegeben.
                                       Eine detaillierte Erläuterung zum Ändern des Tourstatus finden Sie unter:
                                        “So ändern Sie den Status einer Tour” auf Seite I-99

                                          Tourstatus Freigegeben
                                          Sobald Sie den Tourstatus auf freigegeben setzen, ist es nicht mehr mög-
                                          lich, die Aufträge noch einmal aus A+W Business an OTR zu übergeben.
                                          Sollte dies notwendig sein, so müssen Sie zunächst den Nummernverwal-
                                          ter kopieren um neue Auftragsnummern zu bekommen. Achten Sie dabei
                                          darauf, dass der neue Auftragsstatus im korrekten Statusbereich (meist 01
                                          bis 800) liegt.

                                       Dokumente in die Cloud laden
                                       Möchten Sie dem Fahrer die Dokumente in digitaler Form zu Verfügung stel-
                                       len, müssen Sie diese ebenfalls in die Cloud laden.
2.01 / 01-2017




                                       Dazu gehen Sie wie folgt vor:




                 I-104                                                                A+W Business Logistic Optmizer
                 Tutorial                                                            Touren fahren und überwachen




                                         So laden Sie Dokumente in die Cloud und referenzieren diese
                                        1 Öffnen Sie das Menü Abfrage.
                                        2 Klicken Sie auf die Symbol-Schaltfläche [Dateien anhängen]. Es öffnet sich
                                          der gleichnamige Dialog.
                                        3 Im Feld Tour ID wird Ihnen die zuvor ausgewählte Tour angezeigt. In den
                                          Feldern Kunde und Auftrag können Sie für den Fahrer die entsprechenden
                                          Informationen hinterlegen.
                                        4 Im Bereich Bestimmungsorte werden Ihnen die Orte angezeigt, die auf der
                                          Tour angefahren werden. Wählen Sie den Ort aus, zu dem Sie das Doku-
                                          ment hinterlegen möchten.
                                        5 Klicken Sie auf die Symbol-Schaltfläche [Plus]. Es öffnet sich der Dialog
                                          Datei anhängen.
                                            •   Im Feld Dateinamen können Sie einen Namen hinterlegen, z. B. Liefer-
                                                schein.
                                            •   Im Feld Dateipfad geben Sie den entsprechenden Pfad zur Cloud ein,
                                                z. B. https://drive.google.com/file/d/....
                                            •   Das Feld Beschreibung dient der Eingabe weiterer Informationen.
                                            •   Den Dialog verlassen Sie mit der Schaltfläche [OK].
                                            •   Die entsprechenden Dokumente sind dann im Bereich Dateien zu fin-
                                                den.

                                        App installieren oder Browser verwenden
                                        Das Buchen der Daten kann auf zwei unterschiedliche Arten erfolgen:
                                        •   Über eine App (für Android-Geräte)
                                        •   Über einen Browser (Nicht-Android-Geräte)


                                         So installieren Sie die App (Android)
                                        1 Gehen Sie in den Google Play Store.
                                        2 Laden Sie sich für Android-Geräte die App GDC: Goods Delivery Control.
                                        3 Installieren Sie diese.


                                         Sie arbeiten mit dem Browser (Nicht-Android-Geräte)
                                        1 Starten Sie den Browser (Safari).
                                        2 Geben Sie die URL ein. Die entsprechende Adresse finden Sie in OTR un-
                                          ter Starten > Über A+W Logistics Optimizer, im Bereich GDC Web App. In
                                          unserem Beispiel ist diese: http://gdcapp.onerbox.com.
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                                I-105
                 Touren fahren und überwachen                                                               Tutorial




                                       Touren fahren
                                       In diesem Bereich befinden sich die Informationen für den Fahrer:
                                       •   Kennwort eingeben
                                       •   Bedienung der App bzw. des Browsers
                                       •   Daten buchen

                                       Kennwort eingeben
                                       Logt der Fahrer sich über die App oder den Browser das erste Mal mit seiner
                                       ID ein, sind folgende Angaben zu machen:




                                       1 Im Feld Firma geben Sie die entsprechende ID aus den Lizenzinformatio-
                                         nen ein (Starten > Über A+W Logistics Optimizer, Schaltfläche [Lizenzin-
                                         formationen], Feld CompanyId).
                                       2 Im Feld Benutzer geben Sie die Fahrer ID ein (Administration > Fahrer,
                                         Feld Fahrer ID).
                                       3 Im Feld Kennwort geben Sie ein Kennwort ein.
                                       4 Im Feld Kennwort wiederholen müssen Sie das Kennwort noch einmal wie-
                                         derholen.
                                       5 Klicken Sie auf <Einloggen>, um sich anzumelden.

                                           Kennwort vergessen
                                           Sollten Sie das Kennwort einmal vergessen, kann dieses im Dialog Fahrer,
2.01 / 01-2017




                                           Checkbox Kennwort zurücksetzen wieder zurück gesetzt werden.




                 I-106                                                            A+W Business Logistic Optmizer
                 Tutorial                                                              Touren fahren und überwachen




                                        Ergänzende Informationen
                                         Softwarereferenz, “Fahrer” auf Seite I-155

                                        Bedienung der App bzw. des Browsers
                                        Nachdem der Fahrer sich eingeloggt hat, erscheinen die Touren, die der ent-
                                        sprechenden Fahrer ID zugeordnet sind. Mit einem Klick auf die Tour öffnet
                                        sich das Übersichtsfenster mit drei Registern:
                                        •   Bestimmungsorte
                                        •   Informationen
                                        •   Karte

                                        Register Bestimmungsorte
                                        Im Register Bestimmungsorte finden Sie alle Bestimmungsorte, die auf der
                                        Tour angefahren werden.




                                        Klicken Sie auf <Start>, erfolgt die Abfrage, ob Ihr Standort via GPS weiterge-
                                        geben werden soll. Stimmen Sie dem bitte zu, damit die Positionskoordinaten
                                        der Buchung zurück gemeldet werden und dem Routenadministrator in der
                                        Firma zur Verfügung stehen.
                                        Nachdem Sie zugestimmt haben, wird der erste Eintrag (Startpunkt, Beispiel
2.01 / 01-2017




                                        oben: A+W) auf Akzeptiert gesetzt.




                 A+W Business Logistic Optmizer                                                                  I-107
                 Touren fahren und überwachen                                                             Tutorial




                                       Daten buchen
                                       Kommt der Fahrer am ersten Bestimmungsort an (Beispiel oben: Becker Glas-
                                       bau), klickt er diesen in der Liste an und es erscheint folgendes Fenster:




                                       Über die Kombobox Status kann der Lieferung der entsprechende Status zu-
                                       wiesen werden. Folgende Möglichkeiten stehen zur Verfügung:
                                       •   Akzeptiert
                                       •   Teilweise angenommen
                                       •   Abgelehnt
                                       •   Abgelehnt (Bruch)
                                       •   In Auslieferung
                                       Wählen Sie den entsprechenden Status aus.
                                       Im Bereich Kommentar können Informationen hinterlegt werden. So können
                                       Sie z. B. eintragen, wenn eine Scheibe zu Bruch gegangen ist. Da die Daten
                                       an die Cloud zurück gemeldet werden, stehen diese Daten auch sofort in der
                                       Firma zur Verfügung. Im Falle von Bruch kann dieser dann umgehend nach-
                                       produziert werden.
                                       Im Bereich Dokumente werden Ihnen die Auftrags-Nummern angezeigt. Ab-
                                       hängig vom Status, können Sie diese an- oder abwählen. Bsp.: Wählen Sie
                                       den Status Akzeptiert, werden alle Dokumente automatisch angewählt. Wäh-
                                       len Sie den Status Teilweise angenommen, können Sie einzelne Dokumente
2.01 / 01-2017




                                       anwählen. Sie wählen dann die Dokumente an, zu denen die Lieferung akzep-
                                       tiert wurde.



                 I-108                                                           A+W Business Logistic Optmizer
                 Tutorial                                                               Touren fahren und überwachen




                                        Der Bereich Firma
                                        Klicken Sie in den Bereich Firma öffnet sich ein neues Fenster. In dem gelben
                                        Bereich kann der Mitarbeiter, der die Lieferung entgegennimmt, unterschrei-
                                        ben.




                                        Klicken Sie anschließend auf <Akzeptieren>, wird das Fenster geschlossen
                                        und die Unterschrift wird am rechten Bildschirmrand angezeigt.




                                        Unter dem Eintrag Firma, sehen Sie jetzt das Wort Ja. Das bedeutet, eine Un-
                                        terschrift ist vorhanden. Sollte die Unterschrift falsch sein oder wiederholt wer-
                                        den müssen, können Sie den Papierkorb oben rechts anklicken. Die
                                        Unterschrift wird dann gelöscht und kann wiederholt werden.

                                        Der Bereich Packmittel
                                        Klicken Sie im Bereich Packmittel auf <Hinzufügen>, öffnet sich das Fenster
                                        Packmittel.
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                                    I-109
                 Touren fahren und überwachen                                                               Tutorial




                                       Geben Sie unter dem Eintrag Barcode die entsprechende ID an. Im Feld Akti-
                                       on können Sie wählen, ob es sich bei dem Packmittel um eine Lieferung oder
                                       um eine Rückholung handelt. Im Bereich Kommentare haben Sie dann noch
                                       die Möglichkeit, Informationen zu dem Packmittel zu hinterlegen.
                                       Klicken Sie auf <Hinzufügen>, öffnet sich ein neues Fenster:




                                       Hier können Sie noch den Lauf, die Auftrags-Nr. und die Position hinterle-
                                       gen.Klicken Sie auf [Hinzufügen], werden die Daten übernommen und Sie be-
                                       finden sich wieder im Fenster Packmittel.
                                       Klicken Sie auf [Speichern], wird auch dieses Fenster geschlossen.
2.01 / 01-2017




                 I-110                                                            A+W Business Logistic Optmizer
                 Tutorial                                                             Touren fahren und überwachen




                                        Gebuchte Bestimmungsorte
                                        In der Übersicht Bestimmungsorte werden diese in Abhängigkeit vom Status
                                        in verschiedenen Farben dargestellt. Wurde eine Lieferung akzeptiert, ist die-
                                        se Grün hinterlegt. Lieferungen, die teilweise angenommen oder abgelehnt
                                        wurden, werden in Gelb hinterlegt.
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                                 I-111
                 Touren fahren und überwachen                                                                Tutorial




                                       Register Informationen
                                       In diesem Register befinden sich alle Informationen, die die Tour betreffen.
2.01 / 01-2017




                 I-112                                                             A+W Business Logistic Optmizer
                 Tutorial                                                           Touren fahren und überwachen




                                        Register Karte
                                        In diesem Register sehen Sie die Karte mit der zu fahrenden Route.
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                              I-113
                 Touren fahren und überwachen                                                              Tutorial




                                       Touren überwachen
                                       Der Routen Administrator ermöglicht Ihnen ein ständiges Online-Tracking Ih-
                                       rer Fahrzeuge und Fahrer. Wann immer der Fahrer über die App oder Safari
                                       etwas bucht, werden die Daten via Cloud an Ihr Haus übertragen.

                                       Beispiel für eine Lieferung, die teilweise angenommen wurde
                                       In der App:




                                       In OTR:
2.01 / 01-2017




                 I-114                                                           A+W Business Logistic Optmizer
                 Tutorial                                                             Touren fahren und überwachen




                                        Register Stationen
                                        Die unterschiedlichen Farben zeigen Ihnen den aktuellen Stand. Wird ein Be-
                                        stimmungsort in grüner Farbe dargestellt, wurde die gesamte Lieferung abge-
                                        laden und angenommen. Bestimmungsorte, die in gelber Farbe dargestellt
                                        werden, wurden entweder nur teilweise angenommen oder aber abgelehnt.
                                        Ein Doppelklick auf den Bestimmungsort rechts neben der Karte zeigt diesen
                                        auf der Karte zusammen mit einem Fenster, dem Sie alle wichtigen Informati-
                                        onen entnehmen können.

                                        Register Logbuch
                                        Das Register Logbuch liefert Ihnen eine tabellarische Übersicht zu der Tour.




                                        Im Feld Datum sehen Sie das Datum der Tour und im Feld Tour die Tournum-
                                        mer. Das Feld Kunde zeigt Ihnen die Kundennummer und das Feld Name den
                                        entsprechenden Kundennamen. Im Feld Status sehen Sie den Status des je-
                                        weiligen Bestimmungsortes. Das Feld steht so lange auf Initiieren, bis Ihr Fah-
                                        rer über die App oder über Safari den entsprechenden Status ausgewählt und
                                        anschließlichen auch gebucht hat. Dann werden die Daten über die Cloud zu
                                        Ihnen übertragen. Mögliche Werte sind:
                                        •   Akzeptiert
                                        •   Teilweise angenommen
                                        •   Abgelehnt
                                        •   Abgelehnt (Bruch)
                                        •   In Auslieferung
                                        Sollte der Fahrer eine Information hinterlegt haben, sehen Sie diese im Feld
                                        Kommentar. Im Feld Benutzer wird Ihnen der Name des Fahrers angezeigt.
                                        Klicken Sie in diesem Register auf einen Bestimmungsort, erscheint an dem
                                        Ort, an dem der Fahrer die Buchung abgesetzt hat, ein Punkt. Somit sehen Sie
                                        jederzeit, an welchem Ort die Ware tatsächlich gebucht wurde.

                                        Register Dokumente
                                        Das Register Dokumente liefert Ihnen eine tabellarische Übersicht zu den Auf-
                                        trägen für den jeweiligen Kunden (Bestimmungsort).
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                                  I-115
                 Touren fahren und überwachen                                                                 Tutorial




                                       Im Feld Auftrags-Nr. sehen Sie die Auftragsnummer. Das Feld Kunde zeigt Ih-
                                       nen die Kundennummer und das Feld Name den entsprechenden Kundenna-
                                       men. Im Feld Status sehen Sie den Status des jeweiligen Auftrags. Das Feld
                                       steht so lange auf Initiieren, bis Ihr Fahrer über die App oder über Safari den
                                       entsprechenden Status ausgewählt und anschließlichen auch gebucht hat. Im
                                       Feld Versandgewicht sehen Sie das Gewicht des Auftrags in kg. Sollte der
                                       Fahrer Gestelle beim Kunden abholen, sehen Sie das Gewicht dieser Gestelle
                                       im Feld Rückholgewicht.

                                          Anzeige aktualisieren
                                          Bitte vergessen Sie nicht, die Symbol-Schaltfläche [Aktualisieren] anzukli-
                                          cken um die neuesten Daten übermittelt zu bekommen.
2.01 / 01-2017




                 I-116                                                             A+W Business Logistic Optmizer
                 Tutorial                                                                                Abfragen




                                        Abfragen
                                        Dieser Themenblock befasst sich mit den unterschiedlichen Abfragetools.
                                        Dazu gehören folgende Lerneinheiten:
                                        •   “Touren” auf Seite I-119
                                        •   “Reports” auf Seite I-125
                                        •   “Ansicht” auf Seite I-130
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                             I-117
                 Abfragen                                                                              Tutorial




                            Überblick
                            Lernziele

                            • Die unterschiedlichen Abfragen kennenlernen und verstehen.
                            • Die Statistiken kennenlernen und verstehen.
                            • Die Kalenderfunktion kennenlernen und verstehen.


                            Nutzen

                            • Über die Statistikfunktion steht Ihnen ein mächtiges Werkzeug für Planungs- und
                              Auswertungszwecke zur Verfügung.


                            Merke

                            ITN-Format                 Export-Format z. B. für TomTom Navigationssysteme.

                            GPX-Format                 Export-Format z. B. für Garmin Navigationssysteme.
2.01 / 01-2017




                 I-118                                                    A+W Business Logistic Optmizer
                 Tutorial                                                                                    Abfragen




                                        Unterschiedliche Abfragen
                                        In diesem Bereich können Sie – in Abhängigkeit des Tourstatus – verschiede-
                                        ne Informationen abfragen. Das Register ist in folgende Gruppen unterteilt:
                                        •   Touren
                                        •   Reports
                                        •   Ansicht
                                        •   Aktualisieren


                                        Touren
                                        Dieser Bereich liefert Ihnen alle Informationen, die mit den Routen an sich in
                                        Verbindung stehen. Er hat folgende Einträge:
                                        •   Filtern
                                        •   Ändern
                                        •   Löschen
                                        •   Exportieren
                                        •   Status
                                        •   Historie

                                        Filtern
                                        In diesem Bereich können Sie die Routen nach dem Datum, der Tour ID, dem
                                        Tour-Namen, etc. filtern.




                                        Abb. I-35    Route filtern
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                                 I-119
                 Abfragen                                                                         Tutorial




                             So filtern Sie
                            1 Möchten Sie in einem bestimmten Zeitraum filtern, aktivieren Sie die
                              Checkbox Datum und tragen Sie anschließend in den Feldern von bis das
                              gewünschte Datum ein.
                            2 Wenn Sie nach einer bestimmten Tour filtern möchten, tragen Sie im Feld
                              Tour ID die entsprechende Nummer ein.
                            3 Wenn Sie nach einem bestimmten Tour-Namen filtern möchten, tragen Sie
                              im Feld Tour-Name den entsprechenden Namen ein.
                            4 Wenn Sie nach einem bestimmten Status filtern möchten, wählen Sie die
                              gewünschten Status aus der Checkbox Tour-Status.
                            5 Wenn Sie nach einem bestimmten Fahrer filtern möchten, öffnen Sie die
                              Kombobox im Feld Fahrer ID und wählen den gewünschten Fahrer aus.
                            6 Wenn Sie nach einer bestimmten Abteilung filtern möchten, öffnen Sie die
                              Kombobox im Feld Abteilung und wählen die gewünschte Abteilung aus.
                            7 Im Feld Kunde können Sie zusätzlich noch nach einem Kunden filtern.

                            Ändern und Status
                            In diesem Bereich können Sie, in Abhängigkeit des Tourstatus, diesen ändern,
                            oder die tatsächlichen Werte (tatsächliche Entfernung und tatsächlichen Kos-
                            ten) der Route ändern.
                            Die Felder in diesem Dialog sind identisch mit den Feldern im Dialog Tour-In-
                            formationen.
                             Softwarereferenz, “Tour-Informationen” auf Seite I-209
                             Tutorial, “Tourstatus ändern” auf Seite I-99

                            Löschen
                            Über diesen Eintrag können Sie selektierte Routen löschen. Es erfolgt eine Si-
                            cherheitsabfrage. Bestätigen Sie diese mit [Ja], wird die Route gelöscht.
2.01 / 01-2017




                 I-120                                                    A+W Business Logistic Optmizer
                 Tutorial                                                                                     Abfragen




                                        Export
                                        Das System bietet Ihnen die folgenden Exportfunktionen:
                                        •   Export an Navigationssysteme
                                        •   Laden der Daten auf mobile Endgeräte (über die Cloud)

                                        Export an Navigationssysteme
                                        Mit dieser Funktion haben Sie die Möglichkeit, die Tour an ein Navigationssys-
                                        tem zu exportieren.
                                        Die Daten können in folgenden Dateiformaten exportiert werden:
                                        •   ITN-Format (z. B. TomTom)
                                        •   GPX-Format (z. B. Garmin)
                                        Mit welchem Dateiformat Ihr Navigationssystem arbeitet, entnehmen Sie bitte
                                        der Bedienungsanleitung Ihres Gerätes.

                                        Markierungen
                                        Beim Exportieren haben Sie die Möglichkeit zu wählen, ob die einzelnen Mar-
                                        kierungen mit exportiert werden sollen oder nicht. Bei den Markierungen han-
                                        delt es sich um Objekte auf der Karte, die an Breitengrad- und
                                        Längengradkoordinaten gebunden sind.
                                        Die Unterschiede werden im folgenden Beispiel deutlich. Es wird eine Tour mit
                                        drei Bestimmungsorten exportiert.
                                        Ohne die Markierungen zu exportieren, sieht der Ordner im Explorer wie folgt
                                        aus:




                                        Wird die Datei mit einem Editor geöffnet, ist der Inhalt wie folgt:




                                        Es werden nur die Koordinaten der einzelnen Wegpunkte gelistet, nicht jedoch
                                        der Weg dorthin.
                                        Mit den Markierungen sieht der Ordner im Explorer wie folgt aus:
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                                 I-121
                 Abfragen                                                                           Tutorial




                            Wird eine der Dateien mit einem Editor geöffnet, ist der Inhalt wie folgt:




                            Die Werte kennzeichnen die Koordinaten.
                            Im Beispiel oben liegt die Adresse auf dem Längengrad 7,82888 und auf dem
                            Breitengrad 50,43582. Anschließend folgen die einzelnen Markierungen bis
                            zur Zieladresse auf dem Längengrad 6,95058 und dem Breitengrad 50,92786.


                             So exportieren Sie die Daten
                            1 Klicken Sie mit der Maus auf die Symbol-Schaltfläche [Export].
                               Es öffnet sich der Dialog Export.
2.01 / 01-2017




                 I-122                                                   A+W Business Logistic Optmizer
                 Tutorial                                                                               Abfragen




                                        2 Je nachdem, über welches Navigationssystem Sie verfügen, aktivieren Sie
                                          die Radiotaste ITN (z. B. TomTom) oder GPX (z. B. Garmin).
                                        3 Aktivieren Sie die Checkbox Markierungen einfügen, wenn die einzelnen
                                          Markierungen mit exportiert werden sollen.
                                        4 Aktivieren Sie die Checkbox Neuen Ordner für diese Tour erstellen, wenn
                                          für jede zu exportierende Tour ein neuer Ordner angelegt werden soll.
                                        5 Geben Sie im Feld Exportpfad an, wo die Datei gespeichert werden soll.

                                           Standardpfad für Exportdateien
                                           Den Standardpfad zum Exportieren der Daten legen Sie in den Parametern
                                           fest (Parameter: Path_Export_ITN_GPS_File).


                                        Ergänzende Informationen
                                         Softwarereferenz, “Export” auf Seite I-214
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                             I-123
                 Abfragen                                                                        Tutorial




                            Historie
                            Die Historie gibt Ihnen Auskunft, welche Person zu welcher Zeit Änderungen
                            an den Dokumenten durchgeführt hat.
                            In der Historie können Sie nach folgenden Kriterien filtern:
                            •   Tour ID
                            •   Auftrags-Nummer
                            •   Kunde


                             So erstellen Sie eine Historie für eine Auftrags-Nummer
                            1 Öffnen Sie in der Menüleiste den Punkt Abfrage.
                            2 Klicken Sie mit der Maus auf die Symbol-Schaltfläche [Historie].
                                Es öffnet sich der Dialog Historie.




                            3 Geben Sie im Feld Dokument die Auftrags-Nummer ein.
                            4 Klicken Sie mit der Maus auf die Symbol-Schaltfläche [OK].
                                Die Daten werden angezeigt.


                            Ergänzende Informationen
                             Softwarereferenz, “Routen filtern” auf Seite I-212
                             Softwarereferenz, “Tour-Informationen” auf Seite I-209
                             Softwarereferenz, “Export” auf Seite I-214
                             Softwarereferenz, “Historie” auf Seite I-217
2.01 / 01-2017




                 I-124                                                    A+W Business Logistic Optmizer
                 Tutorial                                                                                   Abfragen




                                        Reports
                                        In diesem Bereich sind alle Abfragen, die mit Reports und Statistiken zu tun
                                        haben, untergebracht. Er hat folgende Einträge:
                                        •   Ausgewählte Tour
                                        •   Report Launcher
                                        •   Statistiken

                                        Ausgewählte Tour
                                        Die Bestätigungs- und Lieferliste(n) öffnen Sie über die Symbol-Schaltfläche
                                        entweder für eine oder für alle Touren der Optimierung.
2.01 / 01-2017




                                        Abb. I-36   Bestätigungs- und Lieferliste




                 A+W Business Logistic Optmizer                                                                I-125
                 Abfragen                                                                          Tutorial




                            Die Liste können Sie ausdrucken und dem Fahrer mitgegeben. Sie enthält alle
                            wichtigen Informationen zu der Tour.


                            Ergänzende Informationen
                             Softwarereferenz, “Bestätigungs- und Lieferliste” auf Seite I-219

                            Listen drucken
                            In dieser Einheit lernen Sie, wie Sie Listen drucken.


                             So drucken Sie die Liste für eine bestimmte Tour der Optimierung
                            1 Markieren Sie im Bereich Touren die Tour, für die die Liste gedruckt werden
                              soll.
                            2 Klicken Sie mit der Maus auf die Symbol-Schaltfläche [Ausgewählte Tour].
                              Die Liste wird geöffnet.




                            3 Über die Baumstruktur auf der linken Seite können Sie sich die Liste für je-
                              den einzelnen Bestimmungsort anzeigen lassen und diese dann drucken.


                            Ergänzende Informationen
2.01 / 01-2017




                             Softwarereferenz, “Bestätigungs- und Lieferliste” auf Seite I-219




                 I-126                                                      A+W Business Logistic Optmizer
                 Tutorial                                                                                       Abfragen




                                        Report Launcher
                                        Über den Eintrag Report Launcher öffnet sich der gleichnamige Dialog. Hier
                                        sind alle Reports aufgeführt, die Sie im System angelegt haben.
                                        Wählen Sie das gewünschte Report-Format aus und klicken Sie auf die
                                        Schaltfläche [Bericht drucken]. Es öffnet sich der entsprechende Crystal Re-
                                        port.

                                        Statistiken
                                        Über den Eintrag Statistik haben Sie Zugriff auf umfassende Statistiken, die
                                        den gesamten OTR-Bereich abdecken. Klicken Sie den Eintrag an, öffnet sich
                                        der Dialog Statistik. Dieser beinhaltet folgende Register:
                                        •   Allgemein
                                        •   Allgemeine Grafik
                                        •   Fahrzeuge
                                        •   Fahrer
                                        •   Abteilungen
                                        •   Kunden

                                        Register Allgemein
                                        Hier finden Sie allgemeine Angaben zu den Touren. Die geplanten Kosten
                                        werden den tatsächlichen Kosten gegenübergestellt. Darüber hinaus sehen
                                        Sie die Abweichung sowohl in der Währung als auch in Prozent.




                                        Abb. I-37     Statistik, Register Allgemein
2.01 / 01-2017




                                        Der Dialog ist in zwei Bereiche unterteilt. Auf der linken Seite befinden sich die
                                        Filterfunktionen, die die Grundlage für das Ergebnis auf der rechten Seite sind.




                 A+W Business Logistic Optmizer                                                                     I-127
                 Abfragen                                                                          Tutorial




                            Abb. I-38    Filterfunktion


                            Aktivieren Sie die Checkbox Datum, können Sie in den darunter liegenden
                            Feldern von und bis das Datum eingeben, für das die Werte angezeigt werden
                            sollen.
                            Wählen Sie aus der Checkbox Tour Status den bzw. die gewünschten Status.
                            Über die darunter liegenden Symbol-Schaltflächen können Sie alle aktivieren
                            bzw. deaktivieren.
                            Aus der Kombobox Tour-Status können Sie den gewünschten Status auswäh-
                            len. Über die Kombobox Abteilung haben Sie die Möglichkeit, Daten einer be-
                            stimmten Abteilung zu filtern. Die Kombobox Fahrzeuge ermöglicht es Ihnen,
                            Touren zu filtern, die von einem bestimmten Fahrzeug gefahren wurden. Mit
                            Hilfe der Kombobox Fahrer ID filtern Sie bestimmte Fahrer und im Feld Tour-
                            Namen können Sie den Namen einer Tour eingeben, die gefiltert werden soll.
                            Darüber hinaus können Sie im Bereich Kunde noch eine Kundennummer aus
                            der Kombobox auswählen.
                            Die oben genannten Felder und Komboboxen sind frei miteinander kombinier-
                            bar. Sind keine Einträge ausgewählt bzw. eingetragen, werden für dieses Feld
                            alle vorhandenen Daten angezeigt.

                            Eine Statistik erstellen
                            In dieser Einheit lernen Sie, wie Sie Statistiken erstellen.
                            Zu dieser Lerneinheit gibt es folgende Handlungsanweisungen:
                            •   “So erstellen Sie eine Statistik für einen Kunden” auf Seite I-129
                            •   “So erstellen Sie eine Statistik für ein Fahrzeug” auf Seite I-129
                            •   “So erstellen Sie eine Statistik für einen Fahrer und ein Fahrzeug” auf
2.01 / 01-2017




                                Seite I-129




                 I-128                                                    A+W Business Logistic Optmizer
                 Tutorial                                                                                    Abfragen




                                         So erstellen Sie eine Statistik für einen Kunden
                                           Sie möchten wissen, wie hoch die Tour-Kosten für einen Kunde in einem
                                           bestimmten Zeitraum waren.
                                        1 Aktivieren Sie die Checkbox Datum und wählen Sie aus den darunter lie-
                                          genden Feldern den gewünschten Zeitraum aus, z. B. 01.07.2015 bis
                                          31.08.2015.
                                        2 Tragen Sie im Bereich Kunde die gewünschte Kundennummer ein oder
                                          wählen Sie über die Schaltfläche Kunde den gewünschten Kunden aus der
                                          Liste aus.
                                        3 Wählen Sie aus der Kombobox Tour-Status den gewünschten Status aus,
                                          z. B. Abgeschlossen.
                                        4 Im Bereich Kunde von bis tragen Sie die Kundennummer des Kunden ein.
                                        5 Klicken Sie auf [OK]. Auf der rechten Seite des Dialogs werden die Daten
                                          aktualisiert.
                                        6 Im Register Kunden finden Sie die Daten grafisch aufbereitet.


                                         So erstellen Sie eine Statistik für ein Fahrzeug
                                           Sie möchten wissen, wie hoch die gesamten Tour-Kosten für ein Fahrzeug
                                           waren.
                                        1 Wählen Sie aus der Kombobox Fahrzeuge das gewünschte Fahrzeug aus.
                                        2 Klicken Sie auf [OK]. Auf der rechten Seite des Dialogs werden die Daten
                                          aktualisiert.
                                        3 Im Register Fahrzeuge finden Sie die Daten grafisch aufbereitet.


                                         So erstellen Sie eine Statistik für einen Fahrer und ein Fahrzeug
                                           Sie möchten wissen, wie hoch die Tour-Kosten für einen Fahrer und einem
                                           bestimmten Fahrzeug waren.
                                        1 Wählen Sie aus der Kombobox Fahrer den gewünschten Fahrer aus.
                                        2 Wählen Sie aus der Kombobox Fahrzeuge das gewünschte Fahrzeug aus.
                                        3 Klicken Sie auf [OK]. Auf der rechten Seite des Dialogs werden die Daten
                                          aktualisiert.
                                        4 In den Registern Fahrzeuge und Fahrer finden Sie die Daten grafisch auf-
                                          bereitet.


                                        Ergänzende Informationen
                                         Softwarereferenz, “Statistik” auf Seite I-223
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                                I-129
                 Abfragen                                                                           Tutorial




                            Ansicht
                            In diesem Bereich sind alle Ansichten untergebracht. Er hat folgende Einträge:
                            •   Tour
                            •   Bestimmungsort
                            •   Kalender

                            Tour
                            In diesem Dialog können Sie sich allgemeine Informationen, die Fahrzeuge,
                            die Parameter und die Kosten für die ausgewählte Tour anzeigen lassen.
                            Die Felder in diesem Dialog sind identisch mit den Feldern im Dialog Tour.
                             Softwarereferenz, “Eine neue Tour zusammenstellen – Allgemein” auf Seite I-170
                             Softwarereferenz, “Eine neue Tour zusammenstellen – Fahrzeuge” auf Seite I-174
                             Softwarereferenz, “Eine neue Tour zusammenstellen – Parameter” auf Seite I-180
                             Softwarereferenz, “Eine neue Tour zusammenstellen – Kosten” auf Seite I-186

                            Bestimmungsort
                            In diesem Dialog können Sie sich allgemeine Informationen zu den Bestim-
                            mungsorten der ausgewählte Tour anzeigen lassen.
                            Die Felder in diesem Dialog sind identisch mit den Feldern im Dialog Bestim-
                            mungsorte.
                             Softwarereferenz, “Bestimmungsort bearbeiten” auf Seite I-191

                            Kalender
                            Der Kalender gibt Ihnen eine Übersicht über die zu fahrenden Touren bzw. die
                            Touren, die bereits gefahren wurden.
2.01 / 01-2017




                            Abb. I-39    Kalender


                 I-130                                                   A+W Business Logistic Optmizer
                 Tutorial                                                                                     Abfragen




                                        Der Kalender ist in zwei Typen unterteilt:
                                        •   Fahrzeuge
                                        •   Fahrer
                                        Ändern Sie im oberen Teil den Kalendertyp, ändern sich im unteren Bereich
                                        die Einträge. D. h., haben Sie den Kalendertyp Fahrzeuge gewählt, werden im
                                        unteren Bereich die Fahrzeuge dargestellt. Haben Sie den Kalendertyp Fahrer
                                        gewählt, werden die Fahrer dargestellt.
                                        Über die Symbol-Schaltflächen Tag und Monat können Sie zwischen den an-
                                        zuzeigenden Zeiträumen wechseln. Klicken Sie in der Monatsansicht einen
                                        Tag doppelt an, öffnet sich eine Übersicht für diesen Tag. Auf der linken Seite
                                        befindet sich eine Zeitleiste im halben Stunden Intervall. Die Überschriftzeile
                                        richtet sich nach dem ausgewählten Kalendertyp.




                                        Abb. I-40    Kalender im Tag-Layout


                                        Klicken Sie auf dieser Ebene einen Eintrag doppelt an, öffnet sich der Dialog
                                        Abfrage. Dort erhalten Sie einen tabellarischen Überblick zu der Tour inklusive
                                        aller Bestimmungsorte.
                                        Rote Einträge signalisieren immer eine Überschneidung. Entweder in Bezug
                                        auf den Fahrer oder aber das Fahrzeug. Klicken Sie einen solchen Eintrag
                                        doppelt an, öffnet sich der Dialog Tour bearbeiten. Hier können Sie dann ein-
                                        fach und schnell einen anderen Fahrer oder ein anderes Fahrzeug zuweisen.
                                        Die Inhalte können mit Hilfe der Kombobox Tour-Status eingegrenzt werden.
                                        D. h., Sie können sich die Touren in Abhängigkeit ihren Status anzeigen las-
                                        sen.
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                                  I-131
                 Abfragen                          Tutorial
2.01 / 01-2017




                 I-132      A+W Business Logistic Optmizer
Logistic Optimizer                 I

                     Softwarereferenz




                     A+W Business
                 Softwarereferenz                                                                      Konfiguration




                                        Konfiguration
                                        Menü Konfiguration
                                        In diesem Bereich werden alle Daten eingerichtet und gepflegt, die zu einer
                                        korrekten Arbeitsweise benötigt werden.
                                        Der Bereich beinhaltet:
                                        •   Datenbank-Einstellungen:
                                            Hier nehmen Sie die Einstellungen zu den Datenbankverbindungen (OTR
                                            und ERP) vor.
                                             “OTR-Verbindung” auf Seite I-134
                                        •   Parameter:
                                            Dieser Bereich behandelt allgemeine Einstellungen, wie z. B. Berücksich-
                                            tigung der Verkehrslage, Prioritätsfaktoren, Zeitfaktoren, etc.
                                             “Parameter” auf Seite I-136
                                        •   Sprache:
                                            Über die Kombobox können Sie die Sprache zur Laufzeit umstellen. Das
                                            Programm steht zur Zeit in folgenden Sprachen zur Verfügung:
                                            – Spanisch
                                            – Englisch (US)
                                            – Deutsch
                                            – Portugiesisch
                                            – Katalanisch

                                            Schaltflächen in den Dialogen
                                            Die Standard-Schaltflächen und -menüs sind ausführlich im Part Übersicht
                                            und in den Tutorials beschrieben. Auf sie wird daher in der Beschreibung
                                            der Dialoge nicht eingegangen.
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                               I-133
                 Konfiguration                                                               Softwarereferenz




                                 OTR-Verbindung
                                 Konfiguration > Einstellungen




                                 Abb. I-41     OTR-Verbindung


                                 Der Dialog ist in zwei Register unterteilt:
                                 •   OTR-Verbindung
                                 •   ERP-Verbindung
                                 Dieses Register bezieht sich auf die Einstellungen zum OTR Datenbank-Ser-
                                 ver.

                                 Erläuterung der Felder

                                 Datenquelle Hier geben Sie den Pfad zur OTR-Datenbank ein.

                                 Start-Katalog In diesem Feld geben Sie die Standard-Datenbank ein. Diese
                                 ist OTR.

                                 Benutzer-ID In diesem Feld geben Sie die Benutzer-ID ein.

                                 Kennwort In diesem Feld geben Sie das Kennwort ein.

                                 Test Über diese Symbol-Schaltfläche können Sie die Verbindung zur OTR-
                                 Datenbank testen.

                                     Datenbankverbindung
                                     Bitte beachten Sie, dass diese Einstellungen für jeden Benutzer vorgenom-
                                     men werden müssen.


                                 Ergänzende Informationen
                                  Tutorial, “Datenbankverbindungen” auf Seite I-15
2.01 / 01-2017




                 I-134                                                         A+W Business Logistic Optmizer
                 Softwarereferenz                                                                     Konfiguration




                                        ERP-Verbindung
                                        Konfiguration > Datenbank-Einstellungen > Register ERP-Verbindung




                                        Abb. I-42     ERP-Verbindung


                                        Dieses Register bezieht sich auf die Einstellungen zum ERP Datenbank-Ser-
                                        ver.

                                        SQL ERP-Anbindung verwenden Über diese Checkbox steuern Sie, ob
                                        eine Verbindung zur A+W Business-Datenbank besteht oder nicht.
                                         OTR ist nicht mit der A+W Business Datenbank verbunden.
                                         OTR verwendet die folgenden Einstellungen, um sich mit der A+W Busi-
                                        ness-Datenbank zu verbinden.

                                        Datenquelle Hier geben Sie den Pfad zur A+W Business-Datenbank ein.

                                        Start-Katalog In diesem Feld geben Sie die A+W Business-Standard-Daten-
                                        bank ein.

                                        Benutzer-ID Her geben Sie die Benutzer-ID ein.

                                        Kennwort In diesem Feld geben Sie das Kennwort ein.

                                        Test Über diese Symbol-Schaltfläche können Sie die Verbindung zur A+W
                                        Business-Datenbank testen.

                                           Datenbankverbindung
                                           Bitte beachten Sie, dass diese Einstellungen für jeden Benutzer vorgenom-
                                           men werden müssen.


                                        Ergänzende Informationen
                                         Tutorial, “Datenbankverbindungen” auf Seite I-15
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                               I-135
                 Konfiguration                                                               Softwarereferenz




                                 Parameter
                                 Konfiguration > Parameter




                                 Abb. I-43    Parameter


                                 Hier finden Sie alle Parameter inklusive deren Erläuterung und der jeweiligen
                                 Einstellung.

                                 Erläuterung der Parameter

                                 Delivery_Date/Route_Origin Über diesen Eintrag steuern Sie, wie die Rou-
                                 ten gebildet werden. Mögliche Werte sind:
                                 • Ja: Es erfolgt eine Bildung von sogenannten Multi-Routen. Multi-Routen
                                    bedeutet, die Original-Routen aus dem A+W Business bleibt erhalten.
                                 • Nein: Es werden keine Multi-Routen gebildet. Es wird eine einzige Route
                                    auf Basis des Liefertermins gebildet
                                 Technische Info: Parametername: Multiroutes

                                 Liefertermin Dieses Feld hat nur Auswirkungen, wenn der Eintrag für das
                                 Feld Delivery_Date/Route_Origin auf Ja steht. Mögliche Werte sind:
                                 • Ja: Es erfolgt die Bildung der Route aufgrund der Original-Route.
                                 • Nein: Es erfolgt die Bildung der Route aufgrund des Liefertermins.
2.01 / 01-2017




                                 Technische Info: Parametername: Delivery_Date




                 I-136                                                      A+W Business Logistic Optmizer
                 Softwarereferenz                                                                     Konfiguration




                                        Eine Tour für jede Ursprungs-Tour generieren Mit diesem Feld steuern
                                        Sie, ob für jede Tour aus dem A+W Business eine eigene Tour generiert wird.
                                        Mögliche Werte sind:
                                        • Ja: Es wird eine Tour für jede Ursprungs-Tour des A+W Business gebildet.
                                        • Nein: Es wird eine Tour für jeden Liefertermin gebildet.
                                        Technische Info: Parametername: Route_Origin

                                        Dynamische Fahrzeugzuordnung Mit diesem Feld steuern Sie, ob Fahr-
                                        zeuge dynamisch für jede Tour zugeordnet werden. Mögliche Werte sind:
                                        • Ja: Jeder Tour wird das Fahrzeug dynamisch zugeordnet.
                                        • Nein: Die Fahrzeuge werden den Touren fest zugeordnet.
                                        Technische Info: Parametername: Dynamic_Vehicle_Assignment

                                        LKWs nicht erlaubt Mit diesem Feld steuern Sie, ob bei der Routenberech-
                                        nung auch Straßen verwendet werden können, auf denen keine LKWs fahren
                                        dürfen. Mögliche Werte sind:
                                        • Ja: Es dürfen auch Straßen verwendet werden, die nicht für LKWs zuge-
                                           lassen sind.
                                        • Nein: Es sind nur solche Straßen erlaubt, auf denen LKWs fahren dürfen.
                                        Technische Info: Parametername: Allow_Routes_Without_Trucks

                                        Maut-Modus Mit diesem Feld steuern Sie, ob Mautstraßen für die Strecken-
                                        führung erlaubt sind. Mögliche Werte sind:
                                        • Mautstraßen gänzlich vermeiden: Die Optimierung garantiert, dass Ver-
                                           kehrsverbindungen, die Mautstraßen enthalten, gänzlich ausgeschlossen
                                           werden. Wenn die Bedingung nicht erfüllt werden kann, wird keine Route
                                           ermittelt.
                                        • Mautstraßen teilweise vermeiden: Die Optimierung berücksichtigt keine
                                           Verkehrverbindungen, die Mautstraßen enthalten. Wenn durch diese Ein-
                                           schränkung keine Route gefunden werden kann, wird die Bedingung gelo-
                                           ckert.
                                        • Strafe für Mautstraßen: Die Optimierung belegt Verbindungen, die Maut-
                                           straßen enthalten, mit Strafen.
                                        • Normal: Die Optimierung behält die Reihenfolge der Verbindungen, die
                                           Mautstraßen enthalten.
                                        • Bevorzugte: Die Optimierung bevorzugt Verkehrsverbindungen, die Maut-
                                           straßen enthalten.
                                        Technische Info: Parametername: Nokia_Avoid_Tolls

                                        Zug-Modus Mit diesem Feld steuern Sie, ob Züge für die Streckenführung er-
                                        laubt sind. Mögliche Werte sind:
                                        • Züge gänzlich vermeiden: Die Optimierung garantiert, dass Verkehrsver-
                                           bindungen, die Züge enthalten, gänzlich ausgeschlossen werden. Wenn
                                           die Bedingung nicht erfüllt werden kann, wird keine Route ermittelt.
                                        • Züge teilweise vermeiden: Die Optimierung berücksichtigt keine Verkehr-
2.01 / 01-2017




                                           verbindungen, die Züge enthalten. Wenn durch diese Einschränkung keine
                                           Route gefunden werden kann, wird die Bedingung gelockert.




                 A+W Business Logistic Optmizer                                                              I-137
                 Konfiguration                                                               Softwarereferenz




                                 •   Strafe für Züge: Die Optimierung belegt Verbindungen, die Züge enthalten,
                                     mit Strafen.
                                 •   Normal: Die Optimierung behält die Reihenfolge der Verbindungen, die
                                     Züge enthalten.
                                 •   Bevorzugte: Die Optimierung bevorzugt Verkehrsverbindungen, die Züge
                                     enthalten.
                                 Technische Info: Parametername: Nokia_Avoid_Trains

                                 Fähren-Modus Mit diesem Feld steuern Sie, ob Fähren für die Streckenfüh-
                                 rung erlaubt sind. Mögliche Werte sind:
                                 • Fähren gänzlich vermeiden: Die Optimierung garantiert, dass Verkehrsver-
                                    bindungen, die Fähren enthalten, gänzlich ausgeschlossen werden. Wenn
                                    die Bedingung nicht erfüllt werden kann, wird keine Route ermittelt.
                                 • Fähren teilweise vermeiden: Die Optimierung berücksichtigt keine Ver-
                                    kehrverbindungen, die Fähren enthalten. Wenn durch diese Einschrän-
                                    kung keine Route gefunden werden kann, wird die Bedingung gelockert.
                                 • Strafe für Fähren: Die Optimierung belegt Verbindungen, die Fähren ent-
                                    halten, mit Strafen.
                                 • Normal: Die Optimierung behält die Reihenfolge der Verbindungen, die
                                    Fähren enthalten.
                                 • Bevorzugte: Die Optimierung bevorzugt Verkehrsverbindungen, die Fäh-
                                    ren enthalten.
                                 Technische Info: Parametername: Nokia_Avoid_Ferrys

                                 Autobahn-Modus Mit diesem Feld steuern Sie, ob Autobahnen für die Stre-
                                 ckenführung erlaubt sind. Mögliche Werte sind:
                                 • Autobahnen gänzlich vermeiden: Die Optimierung garantiert, dass Ver-
                                    kehrsverbindungen, die Autobahnen enthalten, gänzlich ausgeschlossen
                                    werden. Dies ist z. B. bei HOV Lanes in USA und Kanada der Fall. Wenn
                                    die Bedingung nicht erfüllt werden kann, wird keine Route ermittelt.
                                 • Autobahnen teilweise vermeiden: Die Optimierung berücksichtigt keine
                                    Verkehrverbindungen, die Autobahnen enthalten. Wenn durch diese Ein-
                                    schränkung keine Route gefunden werden kann, wird die Bedingung gelo-
                                    ckert.
                                 • Strafe für Autobahnen: Die Optimierung belegt Verbindungen, die Auto-
                                    bahnen enthalten, mit Strafen.
                                 • Normal: Die Optimierung behält die Reihenfolge der Verbindungen, die Au-
                                    tobahnen enthalten.
                                 • Bevorzugte: Die Optimierung bevorzugt Verkehrsverbindungen, die Auto-
                                    bahnen enthalten.
                                 Technische Info: Parametername: Nokia_Avoid_Motorways
2.01 / 01-2017




                 I-138                                                       A+W Business Logistic Optmizer
                 Softwarereferenz                                                                         Konfiguration




                                        Tunnel-Modus Mit diesem Feld steuern Sie, ob Straßen mit Tunnel für die
                                        Streckenführung erlaubt sind. Mögliche Werte sind:
                                        • Tunnel gänzlich vermeiden: Die Optimierung garantiert, dass Verkehrsver-
                                           bindungen, die Tunnel enthalten, gänzlich ausgeschlossen werden. Wenn
                                           die Bedingung nicht erfüllt werden kann, wird keine Route ermittelt.
                                        • Tunnel teilweise vermeiden: Die Optimierung berücksichtigt keine Verkehr-
                                           verbindungen, die Tunnel enthalten. Wenn durch diese Einschränkung kei-
                                           ne Route gefunden werden kann, wird die Bedingung gelockert.
                                        • Strafe für Autobahnen: Die Optimierung belegt Verbindungen, die Tunnel
                                           enthalten, mit Strafen.
                                        • Normal: Die Optimierung behält die Reihenfolge der Verbindungen, die Au-
                                           tobahnen enthalten.
                                        • Bevorzugte: Die Optimierung bevorzugt Verkehrsverbindungen, die Auto-
                                           bahnen enthalten.
                                        Technische Info: Parametername: Nokia_Avoid_Tunnels

                                        Fortbewegungs-Typ Hier stellen Sie den Fahrzeug-Typ ein. Mögliche Werte
                                        sind:
                                        • LKW
                                        • Auto
                                        Technische Info: Parametername: Nokia_Vehicles

                                        Routen-Typ Hier stellen Sie das gewünschte Merkmal der Route ein. Mögli-
                                        che Werte sind:
                                        • Schnellste: Mit dieser Einstellung wird die schnellste Verbindung zwischen
                                           den Wegpunkten ermittelt. Die Optimierung basiert auf der Fahrtzeit.
                                        • Kürzeste: Mit dieser Einstellung wird die kürzeste Verbindung zwischen
                                           den Wegpunkten ermittelt. Die Optimierung basiert auf der Entfernung.
                                        • Wirtschaftlichste: Mit dieser Einstellung wird die wirtschaftlichste Route er-
                                           mittelt. Die Optimierung basiert auf dem Benzinverbrauch.
                                        Technische Info: Parametername: Nokia_Mode

                                        Kosten Durchschnittliche Preis pro Liter Kraftstoff. Dieser wird verwendet,
                                        wenn kein Fahrzeug ausgewählt ist.
                                        Technische Info: Parametername: Average_Cost_Fuel

                                        Durchschnittlicher Kraftstoffverbrauch Durchschnittliche Kraftstoffver-
                                        brauch in Liter auf 100 km. Dieser wird verwendet, wenn kein Fahrzeug aus-
                                        gewählt ist.
                                        Technische Info: Parametername: Average_Consumption_Fuel

                                        Entfernungs-Faktor Der Entfernungsfaktor basiert auf der Länge der Tour.
                                        Er sucht die kürzeste Entfernung.
                                        Technische Info: Parametername: Ga_Distance_Proportion
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                                  I-139
                 Konfiguration                                                               Softwarereferenz




                                 Gewichts-Faktor Dieser Faktor wertet das Verhältnis von Gewicht und Ent-
                                 fernung der Tour aus. Er multipliziert das Gewicht der Ladung mit der Entfer-
                                 nung jedes einzelnen Wegpunktes und berücksichtigt die Entladungen sowie
                                 etwaige Abholungen an jedem Wegpunkt.
                                 Technische Info: Parametername: Ga_Weight_Proportion

                                 Termin-Faktor Dieser Faktor zählt die Anzahl an Zielen, die innerhalb der
                                 vorgegebenen Auslieferungs- und Abholzeiten erreicht werden. Er sucht die
                                 Tour mit der größten Anzahl an Zielen mit zeitgerechter Lieferung.
                                 Technische Info: Parametername: Ga_OnTime_Proportion

                                 Prioritäts-Faktor Dieser Faktor bewertet die Tour nach der Anzahl der als
                                 vorrangig gekennzeichneten Ziele, die als erste angefahren werden. Er sucht
                                 Touren mit einer größeren Zahl von vorrangigen Zielen in den ersten Orten.
                                 Technische Info: Parametername: Ga_Priority_Proportion

                                 Zeit-Faktor Dieser Faktor basiert auf der Länge der Tour. Er sucht den
                                 schnellsten Weg.
                                 Technische Info: Parametername: Ga_Time_Proportion

                                 Allgemeine Tour Mit diesem Parameter legen Sie den Namen für Touren
                                 fest, die Sie in OTR manuell erstellen.
                                 Technische Info: Parametername: Default_Route_Name

                                 Ursprüngliche Abteilung Dieser Parameter legt fest, mit welchem Eintrag
                                 das Feld Abteilung standardmäßig gefüllt wird. Der Wert ist in den jeweiligen
                                 Dialogen änderbar.
                                 Technische Info: Parametername: Initial_Department

                                 Lizenz-WebService In diesem Feld steht die Adresse des WebService.
                                 Technische Info: Parametername: Ort_License_Web_Service

                                 Startzeit der Tour Über diesen Parameter können Sie die Startzeit für die
                                 Touren festlegen. Die entsprechenden Felder werden dann später in den Dia-
                                 logen mit diesem Wert gefüllt. Der Wert ist im Dialog änderbar.
                                 Technische Info: Parametername: Default_Route_Init_Time

                                 Dauer der Tour Über diesen Parameter können Sie die maximale Dauer für
                                 die Touren festlegen, z. B. 8 Stunden. Die entsprechenden Felder werden
                                 dann später in den Dialogen mit diesem Wert gefüllt. Der Wert ist im Dialog
                                 änderbar Bitte beachten Sie die gesetzlichen Bestimmungen der einzelnen
                                 Länder.
                                 Technische Info: Parametername: Initial_Max_Route_Time
2.01 / 01-2017




                 I-140                                                      A+W Business Logistic Optmizer
                 Softwarereferenz                                                                        Konfiguration




                                        Standard-Anfangsadresse verwenden In diesem Feld geben Sie den Fir-
                                        mennamen an, wo die Touren starten, z. B. A+W Software GmbH. Mögliche
                                        Werte sind:
                                        • Ja: Die Standard-Adresse wird als Anfangsadresse für die Tour verwendet.
                                        • Nein: Die Standard-Adresse wird nicht als Anfangsadresse verwendet.
                                        Technische Info: Parametername: Use_Intitial_Point

                                        Start-Firmenname In diesem Feld geben Sie den Firmennamen an, wo die
                                        Touren starten, z. B. A+W Software GmbH.
                                        Technische Info: Parametername: Intitial_Companyname

                                        Start-Adresse In diesem Feld geben Sie die Start-Adresse für die Touren an,
                                        z. B. Konrad-Adenauer-Str. 15, 35440 Linden.
                                        Technische Info: Parametername: Intitial_Address

                                        Zeit vor Ort Über diesen Parameter können Sie die Zeit in Minuten vor Ort
                                        zum Abladen oder Beladen festlegen, z. B. 12 Minuten. Die entsprechenden
                                        Felder werden dann später in den Dialogen mit diesem Wert gefüllt. Der Wert
                                        ist im Dialog änderbar.
                                        Technische Info: Parametername: Default_Visiting_Time

                                        Ursprünglichen Tour anzeigen Über diesen Eintrag steuern Sie, ob die ur-
                                        sprünglichen Touren ebenfalls angezeigt werden. Mögliche Werte sind:
                                        • Ja: Die ursprünglichen Tour wird neben der optimierten Tour angezeigt
                                        • Nein: Die ursprünglichen Tour wird nicht angezeigt.
                                        Technische Info: Parametername: Show_Original_Route

                                        Optimierte Tour mit gerader Linie anzeigen Mit diesem Eintrag legen Sie
                                        fest, ob die Tour lediglich durch eine gerade Linie dargestellt wird. Mögliche
                                        Werte sind:
                                        • Ja: Die Verbindung der einzelnen Wegpunkte erfolgt durch eine gerade Li-
                                           nie
                                        • Nein: Die Route wird entlang den Straßen dargestellt.
                                        Technische Info: Parametername: Straigh_Optimized_Routes

                                        Transparenz der optimierten Tour (Karte) Hier geben Sie den Wert für die
                                        Transparenz der optimierten Tour ein, z. B. 0,5.
                                        Technische Info: Parametername: Optimized_Route_Opacity

                                        Darstellungsbreite der optimierten Tour Hier geben Sie ein, in welcher
                                        Breite die optimierte Tour in der Karte angezeigt wird, z. B. 10 = 10 Pixel.
                                        Technische Info: Parametername: Optimized_Route_Width

                                        Transparenz der ursprünglichen Tour (Karte) Hier geben Sie den Wert für
2.01 / 01-2017




                                        die Transparenz der ursprünglichen Tour ein, z. B. 0,5.
                                        Technische Info: Parametername: Original_Route_Opacity




                 A+W Business Logistic Optmizer                                                                  I-141
                 Konfiguration                                                                Softwarereferenz




                                 Darstellungsbreite der ursprünglichen Tour Hier geben Sie ein, in wel-
                                 cher Breite die ursprüngliche Tour in der Karte angezeigt wird, z. B. 10 = 10
                                 Pixel.
                                 Technische Info: Parametername: Original_Route_Width

                                 Darstellungsfarbe der optimierten Tour Hier geben Sie den Farbwert für
                                 die optimierte Tour ein, z. B. #0000FF. Die Felder Farbe der optimierten Tour
                                 und Ursprüngliche Tour-Farbe sollten sich deutlich voneinander unterschei-
                                 den. So werden die Unterschiede optisch deutlich.
                                 Technische Info: Parametername: Optimized_Route_Color

                                 Darstellungsfarbe der ursprünglichen Tour Hier geben Sie den Farbwert
                                 für die ursprüngliche Tour ein, z. B. #585858.
                                 Technische Info: Parametername: Original_Route_Color

                                 Mehr als eine Route Mit diesem Eintrag steuern Sie, ob der WebServer
                                 mehrere Routen ermittelt. Mögliche Werte sind:
                                 • Ja: Der WebServer ermittelt mehrer Routen
                                 • Nein: Der WebServer ermittelt nur eine Route
                                 Technische Info: Parametername: Alternatives

                                 Einheitensystem für Entfernungen Hier legen Sie die Längeneinheit fest,
                                 in dem das Modul arbeiten soll. Mögliche Werte sind:
                                 • Metrisch: Kilometer und Meter
                                 • Imperial: Meilen und Fuß
                                 Technische Info: Parametername: Units

                                 Länder-Code Hier geben Sie das Landeskürzel nach ISO-Kodierung für das
                                 Land, in dem OTR installiert ist, ein. Mögliche Werte sind:
                                 • de: Deutschland
                                 • es: Spanien
                                 • uk: England
                                 • fr: Frankreich
                                 • us: USA
                                 • it: Italien
                                 • sv: Schweden
                                 • pl: Polen
                                 • mx: Mexiko
                                 Technische Info: Parametername: Region

                                 Großbuchstaben Über diesen Eintrag steuern Sie, ob die Inhalte der Felder
                                 in Großbuchstaben erscheinen sollen. Mögliche Werte:
                                 • Ja: Die Inhalte erscheinen in Großbuchstaben (z. B.: TOUR NORD)
                                 • Nein: Die Inhalte erschienen nicht in Großbuchstaben (z. B.: Tour Nord).
2.01 / 01-2017




                                 Technische Info: Parametername: Upper_Case




                 I-142                                                       A+W Business Logistic Optmizer
                 Softwarereferenz                                                                     Konfiguration




                                        Zuordnung von Fahrzeugen Über diesen Eintrag steuern Sie, ob beim Im-
                                        port der Aufträge aus A+W Business Fahrzeuge automatisch zugeordnet wer-
                                        den sollen. Mögliche Werte:
                                        • Ja: Die Fahrzeuge werden beim Import automatisch zugeordnet.
                                        • Nein: Die Fahrzeuge werden beim Import nicht automatisch zugeordnet.
                                        Technische Info: Parametername: Automatic_Vehicle_Assignment

                                        Bilder für Tourenbericht Über diesen Eintrag steuern Sie, ob Bilder für die
                                        einzelnen Streckenabschnitte generiert werden oder nicht. Mögliche Werte:
                                        • Ja: Die Bilder werden generiert.
                                        • Nein: Die Bilder werden nicht generiert.
                                        Technische Info: Parametername: Generate_Destinations_Image

                                        Darstellung der Anwendung Hier legen Sie fest, mit welchem Design die
                                        Anwendung laufen soll. Mögliche Einstellungen sind:
                                        • Office 2007 oder 2010 Blue
                                        • Office 2008 oder 2010 Black
                                        • Office 2007 oder 2010 Silver
                                        • Sparkle Blue
                                        • Professional System
                                        • Sparkle Orange
                                        • Sparkle Purple
                                        Nachdem Sie Änderungen an den Einstellungen vorgenommen haben, müs-
                                        sen Sie das Modul neu starten.
                                        Technische Info: Parametername: Overall_Appearance_Application

                                        Anmeldung aktivieren Über diesen Eintrag steuern Sie, ob das Anmelde-
                                        Modul aktiviert ist oder nicht. Mögliche Werte:
                                        • Ja: Anmeldung ist erforderlich.
                                        • Nein: Anmeldung ist nicht erforderlich.
                                        Technische Info: Parametername: Enable_Login

                                        Kein Passwort nötig Über diesen Eintrag steuern Sie, ob die App ohne
                                        Passwort verwendet werden kann oder nicht. Mögliche Werte:
                                        • Ja: Verwendung ohne Passwort möglich.
                                        • Nein: Verwendung nur mit Passwort möglich.
                                        Technische Info: Parametername: Allow_No_Password

                                        ERP-Stammdaten Über diesen Eintrag steuern Sie, ob die Stammdaten des
                                        ERP-Systems verwendet werden sollen. Steht dieser Eintrag auf Ja, werden
                                        die OTR-Stammdaten nicht berücksichtigt. Mögliche Werte:
                                        • Ja: Die ERP-Stammdaten werden verwendet.
                                        • Nein: Die ERP-Stammdaten werden nicht verwendet.
2.01 / 01-2017




                                        Technische Info: Parametername: Use_ERP_Masterdata




                 A+W Business Logistic Optmizer                                                               I-143
                 Konfiguration                                                              Softwarereferenz




                                 Lieferadresse verwenden Mit diesem Eintrag steuern Sie, welche Adresse
                                 als Lieferadresse verwendet wird. Mögliche Werte:
                                 • Ja: Im Modul kann die Lieferadresse geändert werden. Die geänderte Lie-
                                     feradresse gilt dann als Bestimmungsort und die Adresse aus dem Auftrag
                                     wird überschrieben.
                                 • Nein: Adressen aus dem A+W Business können nicht geändert werden.
                                 Technische Info: Parametername: Use_Delivery_Address

                                 Währung Hier stellen Sie die lokale Währungseinheit ein. Bsp.: € für Euro
                                 oder $ für Dollar.
                                 Technische Info: Parametername: Currency

                                 OTR-Kundenadresse Mit diesem Eintrag steuern Sie, ob Kundenadressen
                                 in OTR geändert und gespeichert werden können. Mögliche Werte:
                                 • Ja: Im Modul kann die Kundenadresse geändert und gespeichert werden.
                                    Steht der Parameter auf Ja, ist die neben stehende Symbol-Schaltfläche im
                                    Dialog Bestimmungsort bearbeiten aktiv. Über diese kommen Sie in den
                                    Dialog Kunde.
                                 • Nein: Adressen aus dem A+W Business können nicht geändert werden.
                                 Technische Info: Parametername: Use_Customers_OTR

                                 Nächste Wartungstermin Mit diesem Eintrag steuern Sie, ob Sie mit den
                                 Wartungsterminen der einzelnen Fahrzeuge arbeiten möchten. Mögliche Wer-
                                 te:
                                 • Ja: Sie möchten, dass der nächste Wartungstermin für Ihren Fuhrpark be-
                                     rücksichtigt wird.
                                 • Nein: Der nächste Wartungstermin wird nicht berücksichtigt.
                                 Technische Info: Parametername: Use_Vehicle_Maintenance

                                 Anzahl der Tage Hier geben Sie die gewünschte Anzahl an Tagen ein, nach
                                 deren Ablauf die nächste Wartung fällig ist. Wird dieses Datum erreicht, er-
                                 scheint eine entsprechende Meldung am Bildschirm.
                                 Technische Info: Parametername: Days_Before_Vehicles_Maintenance

                                 Exportpfad Hier geben Sie an, wo die Exportdateien für die Navigationssys-
                                 teme gespeichert werden sollen.
                                 Technische Info: Parametername: Path_Export_ITN_GPX_File

                                 Export Mit diesem Eintrag steuern Sie, ob Exportdateien für Navigationssys-
                                 teme erstellt werden können oder nicht. Mögliche Werte:
                                 • Ja: Die Export-Funktion kann genutzt werden.
                                 • Nein: Es können keine Dateien für Navigationssysteme exportiert werden.
                                 Technische Info: Parametername: Use_Export_To_GPS_Systems
2.01 / 01-2017




                                 Ergänzende Informationen
                                  Tutorial, “Parameter” auf Seite I-35




                 I-144                                                      A+W Business Logistic Optmizer
                 Softwarereferenz                                                                     Administration




                                        Administration
                                        Menü Administration
                                        In diesem Bereich werden alle Daten eingerichtet und gepflegt, die zu einer
                                        korrekten Arbeitsweise benötigt werden.
                                        Der Bereich beinhaltet:
                                        •   Benutzer:
                                            Hier können Benutzer ändern, löschen oder bearbeiten.
                                             “Benutzer” auf Seite I-146
                                        •   Status:
                                            Hier können Sie einen Status ändern, löschen oder bearbeiten.
                                             “Status” auf Seite I-147
                                        •   Kunden:
                                            Hier können Sie Kunden ändern, löschen oder bearbeiten.
                                             “Kunden” auf Seite I-149
                                        •   Abteilungen:
                                            Hier können Sie Abteilungen ändern, löschen oder bearbeiten.
                                             “Abteilungen” auf Seite I-151
                                        •   Fahrzeuge:
                                            Hier können Sie Fahrzeuge ändern, löschen oder bearbeiten.
                                             “Fahrzeuge” auf Seite I-152
                                        •   Fahrer:
                                            Hier können Sie Fahrer ändern, löschen oder bearbeiten.
                                             “Fahrer” auf Seite I-155
                                        •   Reports:
                                            Hier greifen Sie auf die Reports zu.
                                             “Reports” auf Seite I-158
                                        •   Datenimport:
                                            Hier können Sie Daten importieren.
                                             “Datenimport” auf Seite I-161

                                            Schaltflächen in den Dialogen
                                            Die Standard-Schaltflächen und -menüs sind ausführlich im Part Übersicht
                                            und in den Tutorials beschrieben. Auf sie wird daher in der Beschreibung
                                            der Dialoge nicht eingegangen.
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                               I-145
                 Administration                                                             Softwarereferenz




                                  Benutzer
                                  Administration > Benutzer




                                  Abb. I-44     Benutzer


                                  Dieser Dialog dient dem Steuern von Benutzerprofilen, die unter Windows
                                  oder in einer Domäne registriert sind.

                                  Erläuterung der Felder im Bereich Detail

                                  Benutzer-ID In diesem Feld sehen Sie die Benutzer-ID, z. B. Windows-Au-
                                  thentifizierung. Die Daten werden beim Programmstart automatisch generiert.

                                  Name In diesem Feld sehen Sie den Namen des Benutzers. Dieses Feld
                                  kann geändert werden.

                                  Kopieren von Hier haben Sie als Administrator die Möglichkeit, eine bereits
                                  angelegten Benutzer zu kopieren. Öffnen Sie die Kombobox und wählen Sie
                                  den Benutzer aus, den Sie kopieren möchten.


                                  Ergänzende Informationen
                                   Tutorial, “Benutzer” auf Seite I-37
2.01 / 01-2017




                 I-146                                                      A+W Business Logistic Optmizer
                 Softwarereferenz                                                                       Administration




                                        Status
                                        Administration > Status




                                        Abb. I-45    Status


                                        In diesem Dialog werden Ihnen die angelegten Status angezeigt. Sie können
                                        einen neuen Status anlegen oder einen vorhandenen Status ändern. Welcher
                                        Status geändert werden kann, zeigt Ihnen das Feld Editierbar. Hat der Status
                                        dort einen grünen Haken, kann er geändert werden. Alle Status ohne grünen
                                        Haken können nicht geändert werden.

                                        Erläuterung der Felder

                                        Status Typ In diesem Feld wird Ihnen der Status Typ angezeigt. Die Typen
                                        sind wie folgt unterteilt:
                                        1: Temporärer Status. Die Information kommt vom A+W Business-System und
                                        wird automatisch vergeben, wenn der Assistent durchlaufen wird und nicht ge-
                                        speichert wird.
                                        50: In Änderung: Nach dem Laden einer gespeicherten Tour befindet sich die
                                        Tour in diesem Modus.
                                        100: Geplant: Diesen Status erhält eine Tour, nachdem sie gespeichert wurde.
                                        150: Organisiert: Bei diesem Status handelt es sich um einen freien Status, der
2.01 / 01-2017




                                        für die Firmen-Organisation verwendet werden kann.
                                        200: Freigegeben: In diesem Status können Touren an die GDC App übertra-
                                        gen werden und sind auf mobilen Endgeräten darstellbar.


                 A+W Business Logistic Optmizer                                                                  I-147
                 Administration                                                                 Softwarereferenz




                                  250: Initiieren: Aus der GDC App heraus kann der Anwender das Tracking
                                  durch klicken auf Start Route einschalten.
                                  860: Abschluss gelöscht: Aus der GDC App heraus kann der Anwender die
                                  Tour stornieren.
                                  870: Abschluss komplett: Aus der GDC App heraus kann der Anwender die
                                  Tour abschließen, wenn alle Bestimmungsorte ordnungsgemäß abgeschlos-
                                  sen wurden.
                                  880: Abschluss unvollständig: Aus der GDC App heraus kann der Anwender
                                  die Tour abschließen. In diesem Fall wurde mindestens ein Bestimmungsort
                                  abgewiesen oder nur teilweise akzeptiert.
                                  890: Gelöscht: Aus der GDC App heraus kann der Anwender die Tour stornie-
                                  ren.
                                  900: Fertig unvollständig: Aus der GDC App heraus wurden alle Dokumente
                                  zurückgewiesen.
                                  1000: Archiviert: Der OTR-Anwender hat den Status manuell auf Archiviert ge-
                                  setzt. Die Tour verschwindet aus der GDC App und wird in der OTR-Daten-
                                  bank gespeichert.

                                  Status In diesem Feld wird Ihnen der Status angezeigt. Bei dem Status, der
                                  nicht geändert werden kann, sind die Felder Status Typ und Status identisch.

                                  Name Hier wird Ihnen der Statusname angezeigt.

                                  Editierbar Dieses Feld zeigt Ihnen, ob der Status editierbar ist oder nicht. Hat
                                  das Feld einen grünen Haken, können Sie den Status editieren.


                                  Ergänzende Informationen
                                   Tutorial, “Status” auf Seite I-38
                                   Tutorial, “Die Status-Typen verwalten” auf Seite I-39
2.01 / 01-2017




                 I-148                                                            A+W Business Logistic Optmizer
                 Softwarereferenz                                                                     Administration




                                        Kunden
                                        Administration > Kunden




                                        Abb. I-46    Kunden


                                        In diesem Dialog können Sie grundlegende Kundendaten hinzufügen, ändern
                                        oder löschen. Kunden werden automatisch gespeichert, wenn in den Parame-
                                        tern der Eintrag USE_CUSTOMERS_OTR den Wert Ja hat.

                                        Erläuterung der Felder im Register Haupt

                                        Kunden-Nr. In diesem Feld wird Ihnen die Kundennummer angezeigt.

                                        Name In diesem Feld wird Ihnen der Kundenname angezeigt.

                                        Telefon Hier wird Ihnen die Telefonnnummer angezeigt.

                                        Adresse In diesem Feld wird Ihnen die Adresse des Kunden angezeigt.

                                        Priorität Diese Checkbox ist aktiv, wenn es sich bei der Adresse um eine Pri-
                                        oritätsadresse handelt.

                                        Breitengrad In diesem Feld finden Sie den Breitengrad der Firmen-Adresse.
2.01 / 01-2017




                                        Längengrad In diesem Feld finden Sie den Längengrad der Firmen-Adresse.




                 A+W Business Logistic Optmizer                                                                I-149
                 Administration                                                                Softwarereferenz




                                  Zeit In diesem Feld können Sie die Zeit in Minuten hinterlegen, die dem Fah-
                                  rer zum Abladen und eventuellen neu Laden (Leergestelle) zur Verfügung
                                  steht.

                                  Uhr IWenn Sie auf diese Schaltfläche klicken, öffnet sich ein Dialog, in dem
                                  Sie den Zeitbereich eingeben können, in dem der Fahrer beim Kunden sein
                                  soll. Geben Sie einen solchen Bereich an, wird Ihnen dieser im Feld Zeitbe-
                                  reich angezeigt.

                                  Ansprechpartner In diesem Feld können Sie einen Ansprechpartner beim
                                  Kunden hinterlegen.

                                  E-Mail-Adresse Kontakt In diesem Feld können Sie die E-Mail-Adresse des
                                  Kontaktes hinterlegen.

                                  Erläuterung der Felder im Register Informationen

                                  Name 2 In diesem Feld können Sie einen weiteren Namen hinterlegen.

                                  Name 3 In diesem Feld können Sie noch einen weiteren Namen hinterlegen.

                                  Telefon 2 In diesem Feld können Sie eine weitere Telefonnummer hinterle-
                                  gen.

                                  Fax In diesem Feld können Sie eine Faxnummer eingeben.

                                  Web Wenn der Kunde über eine eigene Internetseite verfügt, können Sie hier
                                  die entsprechende Adresse hinterlegen.

                                  Beschreibung In diesem Feld können Sie eine weitere Beschreibung zu
                                  dem Kunden hinterlegen.


                                  Ergänzende Informationen
                                   Tutorial, “Kunden” auf Seite I-40
                                   Tutorial, “Die Kunden verwalten” auf Seite I-41
2.01 / 01-2017




                 I-150                                                           A+W Business Logistic Optmizer
                 Softwarereferenz                                                                   Administration




                                        Abteilungen
                                        Administration > Abteilungen




                                        Abb. I-47     Abteilungen


                                        In diesem Dialog können Sie Abteilungen hinzufügen, ändern oder löschen.
                                        Dies dient später einmal statischen Auswertungen.

                                        Erläuterung der Felder

                                        Abteilung In diesem Feld geben Sie die Abteilung ein, z. B. Versand.

                                        Name In diesem Feld geben Sie den Namen der Abteilung ein, z. B. Versand
                                        Nord.

                                        Beschreibung In diesem Feld können Sie eine weitere Beschreibung hinter-
                                        legen.


                                        Ergänzende Informationen
                                         Tutorial, “Abteilungen” auf Seite I-43
                                         Tutorial, “Die Abteilungen verwalten” auf Seite I-43
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                                I-151
                 Administration                                                                 Softwarereferenz




                                  Fahrzeuge
                                  Administration > Fahrzeuge




                                  Abb. I-48    Fahrzeuge


                                  In diesem Dialog befinden sich alle angelegten Fahrzeuge, mit denen OTR ar-
                                  beiten kann. Ein Fahrzeug kann ein LKW, ein Anhänger oder auch ein größe-
                                  rer Transporter sein.
                                  Der Dialog ist in zwei Bereiche unterteilt. Der obere Bereich liefert Ihnen eine
                                  Übersicht zu allen angelegten Fahrzeugen. Klicken Sie im oberen Bereich ein
                                  Fahrzeug an, zeigt Ihnen der untere Bereich Detail-Informationen zu dem aus-
                                  gewählten Fahrzeug.

                                  Erläuterung der Felder im Bereich Detail

                                  Nummernschild In diesem Feld geben Sie das Nummernschild des Fahr-
                                  zeugs an, z. B. HH-XY-123. Wenn Sie das Nummernschild nicht kennen, ent-
                                  nehmen Sie dieses den Fahrzeugpapieren (Fahrzeugschein oder -brief).

                                  Marke In diesem Feld geben Sie die Fahrzeugmarke ein, z. B. Iveco. Wenn
                                  Sie die Fahrzeugmarke nicht kennen, entnehmen Sie diese den Fahrzeugpa-
                                  pieren (Fahrzeugschein oder -brief).
2.01 / 01-2017




                                  Modell In diesem Feld geben Sie das Fahrzeugmodell ein, z. B. Daily 50 C
                                  14. Wenn Sie das Fahrzeugmodell nicht kennen, entnehmen Sie dieses den
                                  Fahrzeugpapieren (Fahrzeugschein oder -brief).


                 I-152                                                         A+W Business Logistic Optmizer
                 Softwarereferenz                                                                     Administration




                                        Fahrgestell-Nummer In diesem Feld geben Sie die Fahrgestell-Nummer des
                                        Fahrzeugs an, z. B. WWW1256425DERE. Wenn Sie die Fahrgestell-Nummer
                                        nicht kennen, entnehmen Sie dieses den Fahrzeugpapieren (Fahrzeugschein
                                        oder -brief).

                                        Kaufdatum In diesem Feld geben Sie ein, wann Sie das Fahrzeug gekauft
                                        haben. So haben Sie einen Überblick, wie viele Kilometer mit dem Fahrzeug
                                        gefahren wurden.

                                        Nächste Wartung In diesem Feld haben Sie die Möglichkeit, den nächsten
                                        Wartungstermin für das entsprechende Fahrzeug zu hinterlegen. In dem Pa-
                                        rameter (Das Programm zeigt die Anzahl der Tage an, nach deren Ablauf die
                                        nächste Wartung fällig ist), können Sie die gewünschte Anzahl an Tagen ein-
                                        stellen.

                                        Abteilung In diesem Feld können Sie dem Fahrzeug eine Abteilung zuord-
                                        nen. Der Wert kommt aus Administration > Abteilung.

                                        Maximale Breite In diesem Feld geben Sie die maximale Breite des Fahr-
                                        zeugs in Metern ein, z. B. 2,85. Wenn Sie die Breite nicht kennen, entnehmen
                                        Sie diese den Fahrzeugpapieren (Fahrzeugschein oder -brief).

                                        Maximale Höhe In diesem Feld geben Sie die maximale Höhe des Fahr-
                                        zeugs in Metern ein, z. B. 3,85. Wenn Sie die Höhe nicht kennen, entnehmen
                                        Sie diese den Fahrzeugpapieren (Fahrzeugschein oder -brief).

                                        Maximale Länge In diesem Feld geben Sie die maximale Länge des Fahr-
                                        zeugs in Metern ein, z. B. 7,6. Wenn Sie die Länge nicht kennen, entnehmen
                                        Sie diese den Fahrzeugpapieren (Fahrzeugschein oder -brief).

                                        Maximale Beladung In diesem Feld geben Sie die maximale Beladung des
                                        Fahrzeugs in kg ein, z. B. 25650. Wenn Sie die Breite nicht kennen, entneh-
                                        men Sie diese den Fahrzeugpapieren (Fahrzeugschein oder -brief). Bitte be-
                                        achten Sie, dass auch die Transportgestelle zur Beladung dazu gehören.

                                        Leergewicht In diesem Feld geben Sie das Leergewicht des Fahrzeugs in
                                        Kilogramm ein, z. B. 7800. Wenn Sie das Leergewicht nicht kennen, entneh-
                                        men Sie dieses den Fahrzeugpapieren (Fahrzeugschein oder -brief).

                                        Verbrauch In diesem Feld geben Sie den durchschnittlichen Kraftstoff-Ver-
                                        brauch des Fahrzeugs in Litern auf 100 km ein, z. B. 18,5. Das bedeutet, dass
                                        das Fahrzeug auf 100 km 18,5 Liter Kraftstoff verbraucht. Wenn Sie hier kei-
                                        nen Wert eingeben, wird der Standard-Wert aus den Parametern zur Kalkula-
                                        tion der Tour-Kosten herangezogen.

                                        Kosten In diesem Feld geben Sie die durchschnittlichen Kosten für einen Li-
                                        ter Kraftstoff ein, z. B. 1,43. Die entsprechende Währungseinheit können Sie
                                        in den Parametern hinterlegen. Wenn Sie hier keinen Wert eingeben, wird der
                                        Standard-Wert aus den Parametern zur Kalkulation der Tour-Kosten herange-
2.01 / 01-2017




                                        zogen.

                                        Fortbewegungstyp Wählen Sie aus der Kombobox das entsprechende
                                        Fahrzeug aus, z. B. LKW, Auto, etc.


                 A+W Business Logistic Optmizer                                                                I-153
                 Administration                                                                Softwarereferenz




                                  Von/bis Zeitfenster, in dem das Fahrzeug zur Verfügung steht. Sollte die
                                  Start- oder Endzeit der Tour außerhalb des Fensters liegen, erscheint in der
                                  Spalte Status in den Planungsanzeigen ein Warnsymbol.

                                  Fahrer ID In diesem Feld wird Ihnen die Fahrer ID angezeigt. Der Wert
                                  kommt aus Konfiguration > Fahrer > Fahrer ID.

                                  Vorname In diesem Feld wird Ihnen der Vorname des Fahrers angezeigt. Der
                                  Wert kommt aus Konfiguration > Fahrer > Vorname.

                                  Nachname In diesem Feld wird Ihnen der Nachname des Fahrers angezeigt.
                                  Der Wert kommt aus Konfiguration > Fahrer > Nachname.

                                  Fahrer Wenn Sie diese Symbol-Schaltfläche betätigen, öffnet sich der Dialog
                                  Fahrer. Aus diesem können Sie den entsprechenden Fahrer auswählen.

                                  Touren Die in diesem Feld aufgeführten Tournummern werden durch AW-
                                  Business übergeben und dienen dazu, LKWs bestimmten Tournummern zu-
                                  zuordnen.

                                  Reihenfolge Ist für zwei oder mehrere LKWs die gleiche Tournummer er-
                                  laubt, dann können Sie über dieses Feld die Reihenfolge der LKWs bestim-
                                  men. Das Feld wird nur ausgewertet, wenn in den Parametern der Eintrag
                                  ROUTE_ORIGIN den Wert Ja hat.

                                  mit Anhänger Über diese Checkbox steuern Sie, ob das Fahrzeug einen An-
                                  hänger mitführen kann.
                                   Das Fahrzeug kann keinen Anhänger mit sich führen.
                                   Das Fahrzeug kann mit Anhänger fahren.

                                  Fahrzeug verfügbar Über diese Checkbox steuern Sie, ob das Fahrzeug ge-
                                  nerell zur Verfügung steht.
                                   Das Fahrzeug steht nicht generell zur Verfügung.
                                   Das Fahrzeug ist verfügbar und kann verplant werden.

                                  GPS-Typ Wählen Sie aus der Kombobox den entsprechenden GPS-Typ aus,
                                  z. B. GDC (eigene Lieferapp), Atlantis (spanischer LKW-GPS-Systemanbie-
                                  ter) oder SkyeEye (US LKW-GPS-Systemanbieter).

                                  Kennung Tragen Sie in diesem Feld die Kennung des entpsrechenden GPS-
                                  Systems ein.

                                  Beschreibung Hier haben Sie die Möglichkeit, eine Beschreibung zum Fahr-
                                  zeug zu hinterlegen.


                                  Ergänzende Informationen
                                   Tutorial, “Fahrzeuge” auf Seite I-45
                                   Tutorial, “Die Fahrzeuge verwalten” auf Seite I-46
2.01 / 01-2017




                 I-154                                                           A+W Business Logistic Optmizer
                 Softwarereferenz                                                                      Administration




                                        Fahrer
                                        Administration > Fahrer




                                        Abb. I-49    Fahrer


                                        In diesem Dialog befinden sich alle angelegten Fahrer, die Sie im Zugriff ha-
                                        ben. Es kann sich dabei sowohl um fest angestellte Mitarbeiter als auch um
                                        Personen handeln, die temporär für Sie arbeiten.

                                        Erläuterung der Felder im Bereich Detail

                                        Fahrer-ID In diesem Feld geben Sie ein Kürzel für den Fahrer ein.

                                        Name In diesem Feld geben Sie den Vornamen des Fahrers ein.

                                        Nachname In diesem Feld geben Sie den Nachnamen des Fahrers ein.

                                        Nachname 2 In diesem Feld haben Sie die Möglichkeit, einen zweiten Nach-
                                        namen für den Fahrer zu hinterlegen.
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                                 I-155
                 Administration                                                                  Softwarereferenz




                                  Steuer-ID In diesem Feld geben Sie den Steuer-ID des Fahrers ein. Die ID
                                  können Sie bei dem Fahrer erfragen.

                                  E-Mail In diesem Feld geben Sie die E-Mail-Adresse des Fahrers ein.

                                  Kosten In diesem Feld haben Sie die Möglichkeit, für die unterschiedlichen
                                  Fahrer Kosten zu hinterlegen. Dieses Feld steht in Zusammenhang mit den
                                  dahinter liegenden Radiotasten Nach Zeit und Nach Entfernung. Der Wert,
                                  den Sie hier eintragen, bezieht sich darauf, welche Radiotaste Sie aktiviert ha-
                                  ben.

                                  Nach Zeit Über diese Radiotaste steuern Sie, ob sich die Kosten, die Sie im
                                  Feld Kosten pro Fahrer eingetragen haben auf die Tour-Zeit beziehen.

                                  Nach Entfernung Über diese Radiotaste steuern Sie, ob sich die Kosten, die
                                  Sie im Feld Kosten pro Fahrer eingetragen haben auf die Tour-Entfernung be-
                                  ziehen.

                                  Adresse In diesem Feld haben Sie die Möglichkeit, die Adresse des Fahrers
                                  zu hinterlegen.

                                  Telefon In diesem Feld haben Sie die Möglichkeit, die Telefon-Nummer des
                                  Fahrers zu hinterlegen, z. B. Festnetz.

                                  Telefon 2 In diesem Feld haben Sie die Möglichkeit, die Telefon-Nummer des
                                  Fahrers zu hinterlegen, z. B. Mobil.

                                  Ansprechpartner In diesem Feld geben Sie den Namen des Ansprechpart-
                                  ners ein, falls der Fahrer nicht in Ihrem Hause angestellt ist, sondern evtl. bei
                                  einer anderen Firma.

                                  Kontakt-Adresse In diesem Feld geben Sie die Kontakt-Adresse ein, falls
                                  der Fahrer nicht in Ihrem Hause angestellt ist, sondern evtl. bei einer anderen
                                  Firma.

                                  Telefon Kontakt In diesem Feld geben Sie die Kontakt-Telefonnummer ein,
                                  falls der Fahrer nicht in Ihrem Hause angestellt ist, sondern evtl. bei einer an-
                                  deren Firma.

                                  Beschreibung In diesem Feld haben Sie die Möglichkeit, ein Beschreibung
                                  zu dem Fahrer oder dem Kontakt zu hinterlegen.

                                  E-Mail-Adresse-Kontakt In diesem Feld geben Sie die E-Mail-Adresse des
                                  Kontaktes ein.

                                  Abteilung In diesem Feld können Sie dem Fahrzeug eine Abteilung zuord-
                                  nen. Der Wert kommt aus Administration > Abteilung.

                                  Firmen-Mitarbeiter In diesem Feld legen Sie fest, ob es sich bei dem Fahrer
2.01 / 01-2017




                                  um einen Mitarbeiter Ihres Unternehmens handelt oder nicht.
                                   Der Fahrer ist kein Mitarbeiter Ihrer Firma.
                                   Der Fahrer ist in Ihrem Unternehmen angestellt.



                 I-156                                                          A+W Business Logistic Optmizer
                 Softwarereferenz                                                                   Administration




                                        Verfügbar Über diese Checkbox steuern Sie, ob der Fahrer generell zur Ver-
                                        fügung steht.
                                         Der Fahrer steht nicht generell zur Verfügung.
                                         Der Fahrer ist verfügbar und kann verplant werden.

                                        Kennwort zurücksetzen Über diese Checkbox wird das Kennwort, das beim
                                        Starten der GDC APP notwendig ist, zurückgesetzt.


                                        Ergänzende Informationen
                                         Tutorial, “Fahrer” auf Seite I-49
                                         Tutorial, “Die Fahrer verwalten” auf Seite I-50
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                             I-157
                 Administration                                                                 Softwarereferenz




                                  Reports
                                  Administration > Reports




                                  Abb. I-50     Reports


                                  In diesem Dialog können Sie neue Reports anlegen oder Änderungen an be-
                                  stehenden Reports vornehmen. Die Tabelle oben zeigt Ihnen alle bereits an-
                                  gelegten Reports.

                                  Erläuterung der Felder

                                  Report-Name In diesem Feld geben Sie den Namen des Reports ein.

                                  Report-Pfad In diesem Feld geben Sie ein, wo der Report gespeichert wer-
                                  den soll.

                                  Beschreibung In diesem Feld können Sie eine weitere Beschreibung hinter-
                                  legen.

                                  Parameter Über die Checkboxen wählen Sie aus, welche Parameter auf dem
                                  Report ausgegeben werden sollen.


                                  Ergänzende Informationen
                                   Tutorial, “Reports” auf Seite I-52
                                   Tutorial, “Die Reports verwalten” auf Seite I-53
2.01 / 01-2017




                 I-158                                                            A+W Business Logistic Optmizer
                 Softwarereferenz                                                                    Administration




                                        Packmittel
                                        Administration > Packmittel-Typen




                                        Abb. I-51   Packmittel


                                        In diesem Dialog können Sie neue Packmittel anlegen oder Änderungen an
                                        bestehenden Packmitteln vornehmen. Die Tabelle oben zeigt Ihnen alle be-
                                        reits angelegten Packmittel.

                                           Ladeflächenoptimierung
                                           In der aktuellen Programmversion ist eine LKW-Ladeflächenoptimierung
                                           nicht umgesetzt. Bei den hier angelegten Packmitteln geht es um die Ver-
                                           buchung der Ablade- / Aufladestation (im Sinne eines Packmittel-Tra-
                                           ckings).

                                        Erläuterung der Felder

                                        Packmittel ID In diesem Feld geben Sie die Packmittel ID ein.

                                        Packmittel-Typ In diesem Feld geben Sie ein, um welches Packmittel es sich
                                        handelt, z. B. A-Bock, L-Bock, Kiste.

                                        Abteilung In diesem Feld können Sie dem Packmittel eine Abteilung zuord-
                                        nen. Der Wert kommt aus Administration > Abteilung. Über die dahinter lie-
                                        gende Symbol-Schaltfläche öffnen Sie den Dialog Abteilung auswählen.
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                              I-159
                 Administration                                                                 Softwarereferenz




                                  Breite In diesem Feld können Sie die Breite des Packmittels in Metern einge-
                                  ben, z. B. 2,50. Dieses Feld dient der zukünftigen Programmerweiterung (La-
                                  deflächen-Optimierung).

                                  Höhe In diesem Feld können Sie die Höhe des Packmittels in Metern einge-
                                  ben, z. B. 1,98. Dieses Feld dient der zukünftigen Programmerweiterung (La-
                                  deflächen-Optimierung).

                                  Länge In diesem Feld können Sie die Länge des Packmittels in Metern ein-
                                  geben, z. B. 0,95. Dieses Feld dient der zukünftigen Programmerweiterung
                                  (Ladeflächen-Optimierung).

                                  Leergewicht In diesem Feld geben Sie das Leergewicht des Packmittels in
                                  Kilogramm ein, z. B. 250,00. Dieser Wert wird benötigt, um das zur Verfügung
                                  stehende Gesamtgewicht des Transportfahrzeug effizient zu nutzen.

                                  Kosten In diesem Feld können Sie die Anschaffungskosten für das Packmit-
                                  tel eingeben, z. B. 300,00. Dieser Wert kann dann später zu statischen Aus-
                                  wertungen herangezogen werden.

                                  Keine Rückholung Diese Checkbox können Sie aktivieren, wenn das Pack-
                                  mittel nicht zurückgeholt werden soll. Das kann z. B. bei Holzkisten der Fall
                                  sein. Diese verbleiben dann beim Kunden.

                                  Beschreibung In diesem Feld können Sie eine weitere Beschreibung hinter-
                                  legen.


                                  Ergänzende Informationen
                                   Tutorial, “Packmittel-Typen” auf Seite I-55
2.01 / 01-2017




                 I-160                                                            A+W Business Logistic Optmizer
                 Softwarereferenz                                                                      Administration




                                        Datenimport
                                        Administration > Datenimport




                                        Abb. I-52    Datenimport


                                        Über diesen Dialog können Sie Daten im CSV-Format importieren.

                                        Erläuterung der Felder

                                        Importieren CSV Über die Kombobox wählen Sie aus, was Sie importieren
                                        möchten. Mögliche Werte sind:
                                        • Kunden
                                        • Abteilungen
                                        • Fahrer
                                        • Fahrzeuge

                                        Optionen Wenn die erste Zeile ignoriert werden soll, aktivieren Sie bitte die
                                        Checkbox Erste Zeile ignorieren. In der Zeile darunter geben Sie an, welche
                                        Trennzeichen die Datei der zu importierenden Daten enthält, z. B. Semikolon,
                                        Komma, etc.

                                        Importiere CSV Über diese Radiotasten steuern Sie, wie der Import abläuft.
                                        Ist diese Radiotaste aktiv, erfolgt der Import und die zu importierenden Daten
                                        (csv-Datei) bleiben erhalten. Aktivieren Sie die Radiotaste Löschen und Im-
                                        port, dann werden die zu importierenden Daten (csv-Datei) nach dem Import
2.01 / 01-2017




                                        gelöscht.




                 A+W Business Logistic Optmizer                                                                 I-161
                 Administration                                                              Softwarereferenz




                                  Import-Pfad Wählen Sie hier aus, wo die zu importierende Datei liegt.

                                  Tabelle Die darunter liegende Tabelle zeigt Ihnen, welche Felder importiert
                                  werden.


                                  Ergänzende Informationen
                                   Tutorial, “Datenimport” auf Seite I-58
2.01 / 01-2017




                 I-162                                                       A+W Business Logistic Optmizer
                 Softwarereferenz                                                                             Planung




                                        Planung
                                        Menü Planung
                                        In diesem Bereich werden alle Daten eingerichtet und gepflegt, die zur Pla-
                                        nung der Tour benötigt werden.
                                        Der Bereich beinhaltet:
                                        •   Tour kopieren:
                                            Über diesen Dialog können Sie eine gespeicherte Tour kopieren.
                                             “Eine gespeicherte Tour kopieren” auf Seite I-165
                                        •   Gespeicherte Touren laden:
                                            Über diesen Dialog können Sie eine gespeicherte Tour laden.
                                             “Eine gespeicherte Tour laden” auf Seite I-168
                                        •   Neue Tour:
                                            In diesem Dialog erstellen Sie eine neue Tour.
                                             “Eine neue Tour zusammenstellen – Allgemein” auf Seite I-170
                                             “Eine neue Tour zusammenstellen – Fahrzeuge” auf Seite I-174
                                             “Eine neue Tour zusammenstellen – Parameter” auf Seite I-180
                                             “Eine neue Tour zusammenstellen – Kosten” auf Seite I-186
                                        •   Tour bearbeiten:
                                            Die Felder in diesem Dialog sind identisch mit den Feldern im Dialog Eine
                                            neue Tour zusammenstellen.
                                             “Eine neue Tour zusammenstellen – Allgemein” auf Seite I-170
                                        •   Tour löschen:
                                            Über diese Symbol-Schaltfläche können Sie die aktuelle Tour löschen.
                                        •   Bereiche:
                                            In diesem Dialog geben Sie die Anzahl der Bereiche ein.
                                             “Bereiche” auf Seite I-189
                                        •   Fahrzeuge:
                                            In diesem Dialog weisen Sie einer Tour ein anderes Fahrzeug zu.
                                             “Fahrzeug wählen” auf Seite I-177
                                        •   Neuer Bestimmungsort:
                                            In diesem Dialog erfassen Sie einen neuen Bestimmungsort.
                                             “Eine neue Tour zusammenstellen – Allgemein” auf Seite I-170
                                        •   Bestimmungsort bearbeiten:
                                            In diesem Dialog können Sie einen bestehenden Bestimmungsort ändern.
                                             “Bestimmungsort bearbeiten” auf Seite I-191
                                        •   Bestimmungsort löschen:
                                            Über diese Symbol-Schaltfläche können Sie einen markierten Bestim-
                                            mungsort löschen.
                                        •   Positionen:
                                            Hier sehen Sie die einzelnen Positionen der Tour.
                                             “Positionen anzeigen” auf Seite I-196
                                        •   Detailansicht:
                                            Die Detailansicht liefert Ihnen einen Überblick zu den einzelnen Bestim-
2.01 / 01-2017




                                            mungsorten einer Tour.
                                             “Detailansicht” auf Seite I-202




                 A+W Business Logistic Optmizer                                                                 I-163
                 Planung                                                              Softwarereferenz




                           •   Initialisieren:
                               Mittels dieser Symbol-Schaltfläche kehren Sie zur Ausgangssituation zu-
                               rück. Haben Sie z. B. Datensätze gruppiert und möchten dies rückgängig
                               machen, dann klicken Sie auf diese Schaltfläche.
2.01 / 01-2017




                 I-164                                                A+W Business Logistic Optmizer
                 Softwarereferenz                                                                             Planung




                                        Eine gespeicherte Tour kopieren
                                        Planung > Gespeicherte Tour kopieren




                                        Abb. I-53    Gespeicherte Tour kopieren


                                        Dieser Dialog enthält alle im System gespeicherten Touren. Sie können Tou-
                                        ren kopieren, um verschiedene Simulationen durchzuführen. Dazu markieren
                                        Sie die Tour, die Sie kopieren möchten und betätigen die Symbol-Schaltfläche
                                        [Tour].

                                        Erläuterung der Felder im Bereich Touren

                                        TourStatus In diesem Feld wird Ihnen der Tour-Status angezeigt.

                                        Liefertermin Hier wird Ihnen der Liefertermin der ursprünglichen Tour ange-
                                        zeigt.

                                        Ursprüngliche Tour Hier wird Ihnen die ursprüngliche Tour-Nummer ange-
                                        zeigt. Diese Tour-Nummer kommt von A+W Business.

                                        Tour-ID Das Feld zeigt Ihnen die von A+W Business vergebene Tour-ID.

                                        Name der Tour Hier wird Ihnen der Name der Tour angezeigt, den Sie sei-
                                        nerzeit vergeben haben.

                                        Entfernung Hier sehen Sie, wie viele Kilometer die ursprüngliche Tour hatte.
2.01 / 01-2017




                                        Tour-Zeit Hier sehen Sie, wie lange die ursprüngliche Tour dauerte.

                                        Tour-Kosten Hier sehen Sie, was die ursprüngliche Tour gekostet hat.


                 A+W Business Logistic Optmizer                                                                 I-165
                 Planung                                                              Softwarereferenz




                           Zugewiesenes Gewicht Hier sehen Sie das Gewicht der ursprünglichen
                           Tour.

                           Nummernschild Hier wird Ihnen das Nummernschild angezeigt. Anhand des
                           Nummernschildes wissen Sie, welches Fahrzeug die ursprüngliche Tour ge-
                           fahren hat.

                           Marke und Modell Hier wird Ihnen Marke und Modell des Fahrzeuges ange-
                           zeigt, welches die ursprüngliche Tour gefahren hat.

                           LKW-Ladung In diesem Feld wird Ihnen das Gewicht der LKW-Ladung an-
                           gezeigt.

                           Abteilung In diesem Feld sehen Sie, welche Abteilung die Tour veranlasst
                           hat.

                           Verkehr In diesem Feld wird Ihnen angezeigt, ob die Route Verkehrsinforma-
                           tionen enthielt.

                           Maut In diesem Feld wird Ihnen angezeigt, ob die Route Mautgebühren
                           enthielt.

                           Erläuterung der Felder im Bereich Bestimmungsorte

                           Tour-Name In diesem Feld wird Ihnen der Tour-Name angezeigt.

                           Tour ID In diesem Feld wird Ihnen die Tour ID angezeigt.

                           Reihenfolge Hier wird Ihnen angezeigt, in welcher Reihenfolge die einzelnen
                           Bestimmungsorte angefahren wurden.

                           Kunde In diesem Feld wird Ihnen die Kundennummer angezeigt.

                           Kunde In diesem Feld wird Ihnen der Kundenname angezeigt.

                           Adresse In diesem Feld wird Ihnen die Kundenadresse angezeigt.

                           Auftrag In diesem Feld wird Ihnen die Auftragsnummer angezeigt.

                           Versandgewicht In diesem Feld wird Ihnen das Versandgewicht pro Bestim-
                           mungsort angezeigt.

                           Rückholgewicht In diesem Feld wird Ihnen das Rückholgewicht pro Bestim-
                           mungsort angezeigt.

                           Vor. Lieferung In diesem Feld wird Ihnen das voraussichtliche Lieferdatum
                           angezeigt.

                           Priorität In diesem Feld sehen Sie, ob es sich bei der Adresse um eine Prio-
2.01 / 01-2017




                           ritätsadresse handelt.

                           Rechtzeitig In diesem Feld sehen Sie, ob die Adresse pünktlich angefahren
                           wurde.


                 I-166                                               A+W Business Logistic Optmizer
                 Softwarereferenz                                                                             Planung




                                        Typ In diesem Feld sehen Sie, um welchen Typ (Anfangstyp, Mitteltyp, etc.)
                                        es sich bei dem Bestimmungsort handelte.

                                        Erläuterung der Schaltfläche

                                        Filter Nachdem Sie auf diese Schaltfläche geklickt haben, öffnet sich der Di-
                                        alog Filter Routen.

                                        Kopieren Nachdem Sie auf diese Schaltfläche geklickt haben, werden Sie
                                        gefragt, ob Sie die gespeicherte Tour der aktuellen Tour hinzufügen möchten.


                                        Ergänzende Informationen
                                         Tutorial, “Eine gespeicherte Tour kopieren” auf Seite I-64
                                         Tutorial, “So kopieren Sie eine gespeicherte Tour” auf Seite I-71
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                                 I-167
                 Planung                                                                      Softwarereferenz




                           Eine gespeicherte Tour laden
                           Planung > Gespeicherte Tour laden




                           Abb. I-54     Gespeicherte Tour-Liste


                           Dieser Dialog enthält alle im System gespeicherten Touren. Touren werden
                           automatisch gespeichert, wenn Sie im Ergebnis die Symbol-Schaltfläche [Be-
                           enden] betätigen. Sie können einer in Planung befindlichen Tour eine gespei-
                           cherte Tour dieser Liste hinzufügen. Dazu markieren Sie die Tour, die Sie
                           hinzufügen möchten und betätigen die Symbol-Schaltfläche [OK]. Sie können
                           auch einzelne Touren der Liste löschen, indem Sie die Tour markieren und an-
                           schließend die Symbol-Schaltfläche [Tour löschen] anklicken.

                           Erläuterung der Felder
                           Die Felder dieses Dialoges sind identisch mit den Feldern des Dialoges Eine
                           gespeicherte Tour kopieren.
                            “Eine gespeicherte Tour kopieren” auf Seite I-165


                           Ergänzende Informationen
                            Tutorial, “Eine gespeicherte Tour laden” auf Seite I-63
                            Tutorial, “So laden Sie eine gespeicherte Tour” auf Seite I-70
2.01 / 01-2017




                 I-168                                                     A+W Business Logistic Optmizer
                 Softwarereferenz                                                                            Planung




                                        Bestimmungsorte importieren
                                        Planung > Bestimmungsorte importieren




                                        Abb. I-55    Bestimmungsorte importieren


                                        Über diesen Dialog können Sie Bestimmungsorte im CSV-Format importieren.

                                        Erläuterung der Felder

                                        Optionen Wenn die erste Zeile ignoriert werden soll, aktivieren Sie bitte die
                                        Checkbox Erste Zeile ignorieren. In der Zeile darunter geben Sie an, welche
                                        Trennzeichen die Datei der zu importierenden Daten enthält, z. B. Semikolon,
                                        Komma, etc.

                                        Import-Pfad Wählen Sie hier aus, wo die zu importierende Datei liegt.

                                        Tabelle Die darunter liegende Tabelle zeigt Ihnen, welche Felder importiert
                                        werden.
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                                 I-169
                 Planung                                                              Softwarereferenz




                           Eine neue Tour zusammenstellen – All-
                           gemein
                           Planung > Tour hinzufügen




                           Abb. I-56   Neue Tour, Register Allgemein


                           In diesem Dialog nehmen Sie alle Einstellungen vor, die notwendig sind, um
                           eine neue Tour zu planen. Er ist in drei Register unterteilt:
                           •   Eine neue Tour zusammenstellen – Allgemein
                           •   Eine neue Tour zusammenstellen – Fahrzeuge
                           •   Eine neue Tour zusammenstellen – Parameter

                           Erläuterung der Felder im Bereich Information

                           Liefertermin Öffnen Sie die Kombobox und wählen Sie den gewünschten
                           Liefertermin aus.

                           Startzeit Geben Sie in diesem Feld geben die Uhrzeit an, wann die Tour star-
                           ten soll. Sie können die Zeit entweder über die Tastatur eingeben oder über
                           die Pfeiltasten einstellen.
2.01 / 01-2017




                 I-170                                                 A+W Business Logistic Optmizer
                 Softwarereferenz                                                                             Planung




                                        Tour Status Hier wird Ihnen der Status der Tour angezeigt. Der Wert kann an
                                        dieser Stelle nicht geändert werden. Erst, wenn die Optimierung durchlaufen
                                        wurde, können Sie im Bereich Ergebnis den Status ändern. Dann stehen fol-
                                        gende Werte zur Verfügung:
                                        • Grobgeplant: Das ist der Status der Tour nach der Optimierung.
                                        • Feingeplant: Dieser Status wird zur Zeit noch nicht ausgewertet.
                                        • Freigegeben: Wenn Sie den Status in Freigegeben ändern, wird der Liefer-
                                           termin, die Reihenfolge und die Tour an A+W Business zurückgemeldet.
                                           Sie können den Status nur einmal auf Freigegeben ändern.

                                        Tour-ID Das Feld zeigt Ihnen die von OTR vergebene Tour-ID. Der Wert kann
                                        nicht geändert werden.

                                        Tour-Name In diesem Feld geben Sie den Namen der Tour an. Der Eintrag
                                        ist vorbelegt mit dem Inhalt des Feldes lblGeneralRoute, dem heutigen Datum
                                        und der ursprünglichen Tour.

                                        Ursprüngliche Tour Hier wird Ihnen die ursprüngliche Tour-Nummer ange-
                                        zeigt. Diese Tour-Nummer kommt von A+W Business. Da Sie eine neue Tour
                                        anlegen, ist das Feld mit 0 belegt. Der Wert kann nicht geändert werden.

                                        Tour-Name (Original) In diesem Feld wird Ihnen der Original Tour-Name an-
                                        gezeigt. Dieser Name kommt von A+W Business und kann nicht geändert
                                        werden.

                                        Abteilung In diesem Feld wird Ihnen die Abteilung angezeigt. Über die dar-
                                        unter liegenden Symbol-Schaltflächen können Sie die Vorbelegung ändern.

                                        Beschreibung In diesem Feld können Sie eine detaillierte Beschreibung zur
                                        Tour hinterlegen.

                                        Erläuterung der Felder im Bereich Ausgangspunkt

                                        Firmen-Name In diesem Feld steht der Firmen-Name, bei dem die Tour an-
                                        fängt. Der Wert kommt aus den Parametern (Initial_Companyname).

                                        Adresse In diesem Feld steht die Firmen-Adresse, wo die Tour anfängt. Der
                                        Wert kommt aus den Parametern (Initial_Address). Straße, Ort und Land
                                        müssen durch Komma separiert sein. Bsp.: Hauptstr. 15, 35440 Mittelstadt,
                                        Deutschland.

                                        Breitengrad In diesem Feld finden Sie den Breitengrad der Firmen-Adresse.
                                        Ist das Feld leer, können Sie den Standort durch Betätigen der Symbol-Schalt-
                                        fläche [Geolokalisieren] ermitteln. Es öffnet sich der Dialog Einfache Geoloka-
                                        lisierung.

                                        Längengrad In diesem Feld finden Sie den Längengrad der Firmen-Adresse.
                                        Ist das Feld leer, können Sie den Standort durch Betätigen der Symbol-Schalt-
                                        fläche [Geolokalisieren] ermitteln. Es öffnet sich der Dialog Einfache Geoloka-
2.01 / 01-2017




                                        lisierung.




                 A+W Business Logistic Optmizer                                                                  I-171
                 Planung                                                                 Softwarereferenz




                           Ausgangspunkt verwenden Über diese Checkbox steuern Sie, ob die Fir-
                           men-Adresse als Ausgangpunkt verwendet werden soll.
                            Die Firmen-Adresse wird nicht als Ausgangspunkt verwendet
                            Die Firmen-Adresse dient als Ausgangspunkt.

                           Geolokalisieren Wenn Sie die Symbol-Schaltfläche [Geolokalisieren] betäti-
                           gen, öffnet sich der Dialog Einfache Geolokalisierung.


                           Ergänzende Informationen
                            “Geolokalisieren” auf Seite I-173
                            Tutorial, “So legen Sie eine neue Tour an” auf Seite I-66
2.01 / 01-2017




                 I-172                                                    A+W Business Logistic Optmizer
                 Softwarereferenz                                                                           Planung




                                         Geolokalisieren
                                         Planung > Neue Tour > Allgemein > [Geolokalisieren]




                 Abb. I-57   Einfache Geolokalisierung


                                         Dieser Dialog dient zur Geolokalsierung Ihrer Adresse.

                                         Erläuterung der Felder

                                         Adresse In diesem Feld steht die Firmen-Adresse. Der Inhalt des Feldes
                                         kommt aus dem Feld Adresse im Dialog Tour Allgemein. Sie können die Ad-
                                         resse bei Bedarf ändern. Achten Sie darauf, dass die Straße, der Ort sowie
                                         das Land durch Komma getrennt werden.

                                         Breitengrad In diesem Feld finden Sie den Breitengrad der Firmen-Adresse.

                                         Längengrad In diesem Feld finden Sie den Längengrad der Firmen-Adresse.

                                         Vorschläge Wenn Sie die Symbol-Schaltfläche [Vorschläge] betätigen, öffnet
                                         sich eine kleine Tabelle, die entsprechende Vorschläge zu der Adresse ent-
                                         hält. Bei mehreren Einträgen, können Sie einen auswählen. Betätigen Sie die
                                         Schaltfläche [Akzeptieren], werden die Daten in den Dialog Tour übernom-
                                         men.


                                         Ergänzende Informationen
2.01 / 01-2017




                                          “Eine neue Tour zusammenstellen – Allgemein” auf Seite I-170




                 A+W Business Logistic Optmizer                                                               I-173
                 Planung                                                                Softwarereferenz




                           Eine neue Tour zusammenstellen –
                           Fahrzeuge
                           Planung > Neue Tour > Fahrzeuge




                           Abb. I-58    Neue Tour, Register Fahrzeuge


                           In diesem Register nehmen Sie alle Einstellungen vor, die das Fahrzeug be-
                           treffen, mit dem die Tour gefahren wird. Das Register ist in folgende Bereiche
                           unterteilt:
                           •   Fahrzeuge
                           •   Fahrer

                           Erläuterung der Felder im Bereich Fahrzeuge

                           Nummernschild In diesem Feld geben Sie das Nummernschild des Fahr-
                           zeugs an, z. B. HH-XY-123. Wenn Sie das Nummernschild nicht kennen, ent-
                           nehmen Sie dieses den Fahrzeugpapieren (Fahrzeugschein oder -brief).

                           Marke und Modell In diesem Feld geben Sie die Fahrzeugmarke und das
                           Modell ein, z. B. Iveco. Wenn Sie die Angaben nicht kennen, entnehmen Sie
                           diese den Fahrzeugpapieren (Fahrzeugschein oder -brief).
2.01 / 01-2017




                 I-174                                                  A+W Business Logistic Optmizer
                 Softwarereferenz                                                                            Planung




                                        Kraftstoffkosten In diesem Feld geben Sie die durchschnittlichen Kosten für
                                        einen Liter Kraftstoff ein, z. B. 1,43. Die entsprechende Währungseinheit kön-
                                        nen Sie in den Parametern hinterlegen.

                                        Kraftstoffverbrauch In diesem Feld geben Sie den durchschnittlichen Kraft-
                                        stoff-Verbrauch des Fahrzeugs in Litern ein, z. B. 18,5.

                                        Maximale Breite In diesem Feld geben Sie die maximale Breite des Fahr-
                                        zeugs in Metern ein, z. B. 2,85. Wenn Sie die Breite nicht kennen, entnehmen
                                        Sie diese den Fahrzeugpapieren (Fahrzeugschein oder -brief).

                                        Maximale Höhe In diesem Feld geben Sie die maximale Höhe des Fahr-
                                        zeugs in Metern ein, z. B. 3,85. Wenn Sie die Höhe nicht kennen, entnehmen
                                        Sie diese den Fahrzeugpapieren (Fahrzeugschein oder -brief).

                                        Maximale Länge In diesem Feld geben Sie die maximale Länge des Fahr-
                                        zeugs in Metern ein, z. B. 7,6. Wenn Sie die Länge nicht kennen, entnehmen
                                        Sie diese den Fahrzeugpapieren (Fahrzeugschein oder -brief).

                                        LKW Ladung In diesem Feld geben Sie das zulässige Gesamtgewicht des
                                        Fahrzeugs an. Wenn Sie die Angaben nicht kennen, entnehmen Sie diese den
                                        Fahrzeugpapieren (Fahrzeugschein oder -brief).

                                        Fahrzeug-Typ Wählen Sie aus der Kombobox den entsprechenden Fahr-
                                        zeug-Typ aus. Mögliche Werte.
                                        • LKW
                                        • Auto

                                        LKW mit Anhänger Über diese Checkbox steuern Sie, ob der LKW einen
                                        Anhänger hat. Das ist wichtig, um die korrekte Route zu berechnen. OTR be-
                                        rücksichtigt unter anderem harte Kurven.
                                         Der LKW oder das Auto haben keinen Anhänger.
                                         Der LKW oder das Auto haben einen Anhänger.

                                        Fahrzeug wählen Wenn Sie diese Symbol-Schaltfläche [Fahrzeug wählen]
                                        betätigen, öffnet sich der Dialog Fahrzeug wählen.

                                        Erläuterung der Felder im Bereich Fahrer

                                        Fahrer ID In diesem Feld wird Ihnen die Fahrer ID angezeigt. Der Wert
                                        kommt aus Konfiguration > Fahrer > Fahrer ID.

                                        Vorname In diesem Feld wird Ihnen der Vorname des Fahrers angezeigt. Der
                                        Wert kommt aus Konfiguration > Fahrer > Vorname.

                                        Nachname In diesem Feld wird Ihnen der Nachname des Fahrers angezeigt.
                                        Der Wert kommt aus Konfiguration > Fahrer > Nachname.
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                                 I-175
                 Planung                                                                Softwarereferenz




                           Kosten pro Fahrer In diesem Feld werden Ihnen die Kosten pro Fahrer an-
                           gezeigt. Der Wert kommt aus Konfiguration > Fahrer > Kosten.

                           Nach Zeit Ist diese Checkbox aktiv, beziehen sich die Kosten pro Fahrer auf
                           die Tour-Zeit.

                           Nach Entfernung Ist diese Checkbox aktiv, beziehen sich die Kosten pro
                           Fahrer auf die Entfernung.


                           Ergänzende Informationen
                            Tutorial, “Fahrzeuge” auf Seite I-45
                            Tutorial, “Die Fahrzeuge verwalten” auf Seite I-46
2.01 / 01-2017




                 I-176                                                    A+W Business Logistic Optmizer
                 Softwarereferenz                                                                           Planung




                                        Fahrzeug wählen
                                        Planung > Neue Tour > Fahrzeuge > [Fahrzeug wählen]




                                        Abb. I-59     Fahrzeug wählen


                                        Aus diesem Dialog können Sie das Fahrzeug auswählen, mit dem die Tour ge-
                                        fahren werden soll. Die Daten kommen aus den Parametern.

                                        Erläuterung der Felder

                                        Nummernschild In diesem Feld wird Ihnen das Nummernschild des Fahr-
                                        zeugs angezeigt.

                                        Marke In diesem Feld wird Ihnen die Fahrzeug-Marke angezeigt.

                                        Modell In diesem Feld wird Ihnen das Fahrzeug-Modell angezeigt.

                                        Maximale Beladung In diesem Feld wird Ihnen die maximale Beladung des
                                        Fahrzeugs in kg angezeigt.

                                        Kraftstoffverbrauch In diesem Feld wird Ihnen der durchschnittliche Kraft-
                                        stoffverbrauch in Litern angezeigt.

                                        Kraftstoffkosten In diesem Feld werden Ihnen die durchschnittlichen Kosten
                                        für einen Liter Kraftstoff angezeigt.

                                        Von/bis Das Zeitfenster, in dem das Fahrzeug zur Verfügung steht.

                                        Abteilung In diesem Feld wird Ihnen die Abteilung angezeigt.


                                        Ergänzende Informationen
2.01 / 01-2017




                                         “Fahrzeuge” auf Seite I-152
                                         Tutorial, “Fahrzeuge” auf Seite I-45




                 A+W Business Logistic Optmizer                                                               I-177
                 Planung                                                              Softwarereferenz




                           Fahrer hinzufügen
                           Planung > Neue Tour > Fahrzeuge > [Fahrer hinzufügen]




                           Abb. I-60   Fahrer Übersicht


                           In diesem Dialog werden Ihnen alle gespeicherten Fahrer angezeigt.

                           Erläuterung der Felder

                           Text finden Dieses Feld dient dem Filtern der angezeigten Daten. Es steht in
                           direktem Zusammenhang mit dem Feld Filter-Typ. Wählen Sie zunächst den
                           Filter-Typ (Fahrer ID, Vorname, Nachname oder Adresse) aus und geben Sie
                           dann im Feld Text finden die Angaben ein, nach denen gefiltert werden soll.

                           Filter-Typ Über diese Kombobox steuern Sie, nach welchen Einträgen gefil-
                           tert werden soll, Fahrer ID, Vorname, Nachname oder Adresse. Anschließend
                           geben Sie im Feld Text finden die Angaben ein, nach denen gefiltert werden
                           soll.

                           Filtern Nachdem Sie die entsprechenden Kriterien in den Feldern Text finden
                           und Filter-Typ eingegeben haben, betätigen Sie diese Symbol-Schaltfläche.
                           Danach wird die Liste der Einträge entsprechend aktualisiert.

                           Filter löschen Um die eingegebenen Filter-Kriterien zu löschen, betätigen
                           Sie diese Symbol-Schaltfläche. Danach wird die Liste der Einträge entspre-
                           chend aktualisiert und es werden wieder alle Einträge angezeigt.

                           Fahrer ID In diesem Feld wird Ihnen die Fahrer ID angezeigt. Der Wert
                           kommt aus Konfiguration > Fahrer > Fahrer ID.
2.01 / 01-2017




                 I-178                                                A+W Business Logistic Optmizer
                 Softwarereferenz                                                                       Planung




                                        Vorname In diesem Feld wird Ihnen der Vorname des Fahrers angezeigt. Der
                                        Wert kommt aus Konfiguration > Fahrer > Vorname.

                                        Nachname In diesem Feld wird Ihnen der Nachname des Fahrers angezeigt.
                                        Der Wert kommt aus Konfiguration > Fahrer > Nachname.

                                        Adresse In diesem Feld wird Ihnen die Adresse des Kunden angezeigt. Der
                                        Wert kommt aus Konfiguration > Fahrer > Adresse.


                                        Ergänzende Informationen
                                         Tutorial, “Die Fahrer verwalten” auf Seite I-50
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                           I-179
                 Planung                                                                 Softwarereferenz




                           Eine neue Tour zusammenstellen – Pa-
                           rameter
                           Planung > Neue Tour > Parameter




                           Abb. I-61    Neue Tour, Register Parameter


                           In diesem Register legen Sie die Kriterien fest, anhand derer die Tour gefahren
                           wird.

                           Erläuterung der Felder im Bereich Parameter

                           Tour-Modus Hier stellen Sie das gewünschte Merkmal der Route ein. Mögli-
                           che Werte sind:
                           • Schnellste: Mit dieser Einstellung wird die schnellste Verbindung zwischen
                              den Wegpunkten ermittelt. Die Optimierung basiert auf der Fahrtzeit.
                           • Kürzeste: Mit dieser Einstellung wird die kürzeste Verbindung zwischen
                              den Wegpunkten ermittelt. Die Optimierung basiert auf der Entfernung.
                           • Wirtschaftlichste: Mit dieser Einstellung wird die wirtschaftlichste Route er-
                              mittelt. Die Optimierung basiert auf dem Benzinverbrauch.
                           Der Standardwert, mit dem das Feld vorbelegt ist, kommt aus den Parametern
                           und kann dort geändert werden (Parameter: Nokia_Mode).

                           Multi-Tour Diese Checkbox ist für Touren, die Sie manuell erstellen, nicht ak-
                           tiv.
2.01 / 01-2017




                           Liefertermin Diese Checkbox ist für Touren, die Sie manuell erstellen, nicht
                           aktiv.



                 I-180                                                  A+W Business Logistic Optmizer
                 Softwarereferenz                                                                             Planung




                                        Start der Tour Diese Checkbox ist für Touren, die Sie manuell erstellen, nicht
                                        aktiv.

                                        Verkehr Ist diese Checkbox nicht aktiv, wird die Verkehrslage nicht ermittelt.
                                        Sie können diese Option später im Dialog Optimierung über die Schaltfläche
                                        Verkehr aufrufen.

                                        Optimierung überspringen Ist diese Checkbox aktiv, wird die Optimierung
                                        zunächst übersprungen. Sie können diese Option später im Dialog Optimie-
                                        rung über die Schaltfläche Route optimieren aufrufen.

                                        Maut-Modus Mit diesem Feld steuern Sie, ob Mautstraßen für die Strecken-
                                        führung erlaubt sind. Mögliche Werte sind:
                                        • Mautstraßen gänzlich vermeiden: Die Optimierung garantiert, dass Ver-
                                           kehrsverbindungen, die Mautstraßen enthalten, gänzlich ausgeschlossen
                                           werden. Wenn die Bedingung nicht erfüllt werden kann, wird keine Route
                                           ermittelt.
                                        • Mautstraßen teilweise vermeiden: Die Optimierung berücksichtigt keine
                                           Verkehrverbindungen, die Mautstraßen enthalten. Wenn durch diese Ein-
                                           schränkung keine Route gefunden werden kann, wird die Bedingung gelo-
                                           ckert.
                                        • Strafe für Mautstraßen: Die Optimierung belegt Verbindungen, die Maut-
                                           straßen enthalten, mit Strafen.
                                        • Normal: Die Optimierung behält die Reihenfolge der Verbindungen, die
                                           Mautstraßen enthalten.
                                        • Bevorzugte: Die Optimierung bevorzugt Verkehrsverbindungen, die Maut-
                                           straßen enthalten.
                                        Der Standardwert, mit dem das Feld vorbelegt ist, kommt aus den Parametern
                                        und kann dort geändert werden (Parameter: Nokia_Avoid_Tolls).

                                        Autobahn-Modus Mit diesem Feld steuern Sie, ob Autobahnen für die Stre-
                                        ckenführung erlaubt sind. Mögliche Werte sind:
                                        • Autobahnen gänzlich vermeiden: Die Optimierung garantiert, dass Ver-
                                           kehrsverbindungen, die Autobahnen enthalten, gänzlich ausgeschlossen
                                           werden. Dies ist z. B. bei HOV Lanes in USA und Kanada der Fall. Wenn
                                           die Bedingung nicht erfüllt werden kann, wird keine Route ermittelt.
                                        • Autobahnen teilweise vermeiden: Die Optimierung berücksichtigt keine
                                           Verkehrverbindungen, die Autobahnen enthalten. Wenn durch diese Ein-
                                           schränkung keine Route gefunden werden kann, wird die Bedingung gelo-
                                           ckert.
                                        • Strafe für Autobahnen: Die Optimierung belegt Verbindungen, die Auto-
                                           bahnen enthalten, mit Strafen.
                                        • Normal: Die Optimierung behält die Reihenfolge der Verbindungen, die Au-
                                           tobahnen enthalten.
                                        • Bevorzugte: Die Optimierung bevorzugt Verkehrsverbindungen, die Auto-
                                           bahnen enthalten.
                                        Der Standardwert, mit dem das Feld vorbelegt ist, kommt aus den Parametern
2.01 / 01-2017




                                        und kann dort geändert werden (Parameter: Nokia_Avoid_Motorways).




                 A+W Business Logistic Optmizer                                                                 I-181
                 Planung                                                              Softwarereferenz




                           Tunnel-Modus Mit diesem Feld steuern Sie, ob Straßen mit Tunnel für die
                           Streckenführung erlaubt sind. Mögliche Werte sind:
                           • Tunnel gänzlich vermeiden: Die Optimierung garantiert, dass Verkehrsver-
                              bindungen, die Tunnel enthalten, gänzlich ausgeschlossen werden. Wenn
                              die Bedingung nicht erfüllt werden kann, wird keine Route ermittelt.
                           • Tunnel teilweise vermeiden: Die Optimierung berücksichtigt keine Verkehr-
                              verbindungen, die Tunnel enthalten. Wenn durch diese Einschränkung kei-
                              ne Route gefunden werden kann, wird die Bedingung gelockert.
                           • Strafe für Tunnel: Die Optimierung belegt Verbindungen, die Tunnel enthal-
                              ten, mit Strafen.
                           • Normal: Die Optimierung behält die Reihenfolge der Verbindungen, die
                              Tunnel enthalten.
                           • Bevorzugte: Die Optimierung bevorzugt Verkehrsverbindungen, die Tunnel
                              enthalten.
                           Der Standardwert, mit dem das Feld vorbelegt ist, kommt aus den Parametern
                           und kann dort geändert werden (Parameter: Nokia_Avoid_Tunnels).

                           Fähren-Modus Mit diesem Feld steuern Sie, ob Fähren für die Streckenfüh-
                           rung erlaubt sind. Mögliche Werte sind:
                           • Fähren gänzlich vermeiden: Die Optimierung garantiert, dass Verkehrsver-
                              bindungen, die Fähren enthalten, gänzlich ausgeschlossen werden. Wenn
                              die Bedingung nicht erfüllt werden kann, wird keine Route ermittelt.
                           • Fähren teilweise vermeiden: Die Optimierung berücksichtigt keine Ver-
                              kehrverbindungen, die Fähren enthalten. Wenn durch diese Einschrän-
                              kung keine Route gefunden werden kann, wird die Bedingung gelockert.
                           • Strafe für Fähren: Die Optimierung belegt Verbindungen, die Fähren ent-
                              halten, mit Strafen.
                           • Normal: Die Optimierung behält die Reihenfolge der Verbindungen, die
                              Fähren enthalten.
                           • Bevorzugte: Die Optimierung bevorzugt Verkehrsverbindungen, die Fäh-
                              ren enthalten.
                           Der Standardwert, mit dem das Feld vorbelegt ist, kommt aus den Parametern
                           und kann dort geändert werden (Parameter: Nokia_Avoid_Ferrys).

                           Zug-Modus Mit diesem Feld steuern Sie, ob Züge für die Streckenführung er-
                           laubt sind. Mögliche Werte sind:
                           • Züge gänzlich vermeiden: Die Optimierung garantiert, dass Verkehrsver-
                              bindungen, die Züge enthalten, gänzlich ausgeschlossen werden. Wenn
                              die Bedingung nicht erfüllt werden kann, wird keine Route ermittelt.
                           • Züge teilweise vermeiden: Die Optimierung berücksichtigt keine Verkehr-
                              verbindungen, die Züge enthalten. Wenn durch diese Einschränkung keine
                              Route gefunden werden kann, wird die Bedingung gelockert.
                           • Strafe für Züge: Die Optimierung belegt Verbindungen, die Züge enthalten,
                              mit Strafen.
                           • Normal: Die Optimierung behält die Reihenfolge der Verbindungen, die
                              Züge enthalten.
                           • Bevorzugte: Die Optimierung bevorzugt Verkehrsverbindungen, die Züge
2.01 / 01-2017




                              enthalten.
                           Der Standardwert, mit dem das Feld vorbelegt ist, kommt aus den Parametern
                           und kann dort geändert werden (Parameter: Nokia_Avoid_Trains).


                 I-182                                               A+W Business Logistic Optmizer
                 Softwarereferenz                                                                             Planung




                                        Erläuterung der Felder im Bereich Optimierung

                                        Entfernungs-Faktor In diesem Bereich wird Ihnen der Entfernungs-Faktor
                                        angezeigt.

                                        Gewichts-Faktor In diesem Bereich wird Ihnen der Gewichts-Faktor ange-
                                        zeigt.

                                        Termin-Faktor In diesem Bereich wird Ihnen der Termin-Faktor angezeigt.

                                        Prioritäts-Faktor In diesem Bereich wird Ihnen der Prioritäts-Faktor ange-
                                        zeigt.

                                        Zeit-Faktor In diesem Bereich wird Ihnen der Zeit-Faktor angezeigt.

                                        Tour-Faktoren Wenn Sie die Symbol-Schaltfläche [Tour-Faktoren] betätigen,
                                        öffnet sich der Dialog Tour-Faktoren. Hier können Sie die einzelnen Faktoren
                                        ändern.


                                        Ergänzende Informationen
                                         Tutorial, “Mit Touren arbeiten” auf Seite I-66
                                         Tutorial, “So legen Sie eine neue Tour an” auf Seite I-66
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                                 I-183
                 Planung                                                               Softwarereferenz




                           Tour-Faktoren
                           Planung > Neue Tour > Parameter > [Tour-Faktoren]




                           Abb. I-62    Tour-Faktoren


                           In diesem Dialog legen Sie die Einflussgrößen der einzelnen Merkmale fest.
                           Bitte beachten Sie, dass die einzelnen Prozentzahlen addiert 100 % ergeben
                           müssen. Um die Werte zu verändern, klicken Sie den Schieber des jeweiligen
                           Wertes an und bewegen ihn in die gewünschte Richtung. Über die Symbol-
                           Schaltfläche [Sperren] können Sie einzelne Werte sperren, deren Wert dann
                           nicht mehr verändert wird.
                           Es stehen folgende Einflussgrößen zur Verfügung:
                           •   Entfernungs-Faktor:
                               Der Entfernungs-Faktor basiert auf der Länge der Tour. Er sucht die kür-
                               zeste Strecke.
                           •   Gewichts-Faktor:
                               Der Gewichts-Faktor bewertet das Verhältnis von Gewicht zur Länge der
                               Tour. Er multipliziert das Gewicht der transportierten Güter mit der Länge
                               jedes einzelnen Abschnitts der Tour und berücksichtigt dabei die an jedem
                               Bestimmungsort ausgelieferten und abgeholten Güter. Der Faktor sucht
                               ein geringeres Gewicht-Strecken-Verhältnis.
                           •   Termin-Faktor:
                               Der Termin-Faktor zählt die Anzahl an Zielen, die innerhalb der vorgegebe-
                               nen Auslieferungs- und Abholzeiten erreicht werden. Er sucht die Tour mit
                               der größten Anzahl an Zielen mit zeitgerechter Lieferung.
2.01 / 01-2017




                 I-184                                                 A+W Business Logistic Optmizer
                 Softwarereferenz                                                                               Planung




                                        •   Prioritäts-Faktor:
                                            Der Prioritäts-Faktor bewertet die Tour nach der Anzahl der als vorrangig
                                            gekennzeichneten Ziele, die als erste angefahren werden. Er sucht Touren
                                            mit einer größeren Zahl von vorrangigen Zielen in den ersten Orten.
                                        •   Zeit-Faktor:
                                            Der Zeit-Faktor basiert einfach auf der Zeitdauer der Tour. Er sucht die Tour
                                            mit der kürzesten Zeit.

                                        Standardwerte Wenn Sie die Symbol-Schaltfläche [Standardwerte] betäti-
                                        gen, werden die vorgenommenen Änderungen verworfen und die Werte wer-
                                        den auf die Standardwerte aus den Parametern (Ga_Distance_Proportion,
                                        Ga_Weight_Proportion, Ga_OnTime_Proportion, Ga_Priority_Proportion,
                                        Ga_Time_Proportion) zurückgesetzt. Das gilt ebenfalls für gesperrte Werte!


                                        Ergänzende Informationen
                                         Tutorial, “So bearbeiten Sie die Tour” auf Seite I-93
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                                    I-185
                 Planung                                                             Softwarereferenz




                           Eine neue Tour zusammenstellen – Kos-
                           ten
                           Planung > Neue Tour > Kosten




                                                                                                 o
                           Abb. I-63    Neue Tour, Register Kosten


                           In diesem Register erhalten Sie eine Übersicht zu allen Kosten, die während
                           der Tour anfallen. Es wird unterschieden, zwischen geschätzten und tatsäch-
                           lichen Kosten. Die Felder des rechten Bereiches (Tatsächliche Kosten) wer-
                           den ergänzt, wenn der Fahrer von seiner Tour zurück ist und Ihnen den Tour-
                           Report gegeben hat. Dann können Sie diese tatsächlichen Werte eintragen.

                           Erläuterung der Felder im Bereich Variable Kosten

                           Gesamtstrecke In diesem Feld wird Ihnen die Gesamtstrecke der Tour ange-
                           zeigt.
2.01 / 01-2017




                 I-186                                               A+W Business Logistic Optmizer
                 Softwarereferenz                                                                           Planung




                                        Zeit Hier sehen Sie, wie viel Zeit die Tour in Anspruch nimmt.

                                        Kraftstoffkosten In diesem Feld werden Ihnen die Kraftstoffkosten ange-
                                        zeigt, die Sie im Register Allgemein im Feld Krafststoffkosten eingegeben ha-
                                        ben.

                                        Kraftstoffverbrauch In diesem Feld wird Ihnen der Verbrauch angezeigt,
                                        den Sie im Register Allgemein im Feld Krafststoffverbrauch eingegeben ha-
                                        ben.

                                        Kosten pro Fahrer In diesem Feld werden Ihnen die Kosten angezeigt, die
                                        pro Fahrer anfallen.

                                        Mautkosten Falls Mautstraßen in der Tour enthalten sind, können Sie die zu
                                        erwartenden Mautkosten hier hinterlegen.

                                        Kraftstoffkosten In diesem Feld werden Ihnen die Kraftstoffkosten für die
                                        Tour angezeigt.

                                        Extrakosten In diesem Feld werden Ihnen die Extrakosten für die Tour ange-
                                        zeigt.

                                        Erläuterung der Felder im Bereich Tatsächliche variable Kosten

                                        Tatsächliche Kosten pro Fahrer In diesem Feld werden Ihnen die Kosten
                                        angezeigt, die pro Fahrer anfallen.

                                        Tatsächliche Mautkosten Falls Mautstraßen in der Tour enthalten sind, wer-
                                        den Ihnen hier die Mautkosten angezeigt.

                                        Tatsächliche Kraftstoffkosten In diesem Feld werden Ihnen die Kraftstoff-
                                        kosten für die Tour angezeigt.

                                        Tatsächliche Gesamtstrecke In diesem Feld wird Ihnen die Gesamtstrecke
                                        der Tour angezeigt.

                                        Tatsächliche Zeit Hier sehen Sie, wie viel Zeit die Tour in Anspruch nimmt.

                                        Tatsächliche Extrakosten In diesem Feld werden Ihnen die Extrakosten für
                                        die Tour angezeigt.

                                        Erläuterung der Felder im Bereich Fixe Kosten

                                        Fixkosten In diesem Feld sehen Sie, wie groß der Anteil der Fixkosten ist.

                                        Erläuterung der Felder im Bereich Tatsächliche Fixkosten

                                        Tatsächliche Fixkosten In diesem Feld sehen Sie, wie groß der Anteil der
                                        Fixkosten ist.
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                                I-187
                 Planung                                                             Softwarereferenz




                           Erläuterung der Felder im Bereich Tourkosten

                           Tourkosten In diesem Feld sehen Sie, wie viel die gesamte Tour kosten wird.

                           Erläuterung der Felder im Bereich Tatsächliche Tourkosten

                           Tatsächliche Tourkosten In diesem Feld sehen Sie, wie viel die gesamte
                           Tour kosten wird.


                           Ergänzende Informationen
                            Tutorial, “Fahrzeuge” auf Seite I-45
                            Tutorial, “Fahrer” auf Seite I-49
2.01 / 01-2017




                 I-188                                               A+W Business Logistic Optmizer
                 Softwarereferenz                                                                              Planung




                                        Bereiche
                                        Planung > Gruppen




                                        Abb. I-64    Bereiche


                                        In diesem Dialog stellen Sie ein, in wie viele Bereiche die Touren aufgeteilt
                                        werden.
                                        Geben Sie die Anzahl ein und schließen Sie den Dialog. Die Bereiche werden
                                        automatisch angepasst.


                                        Ergänzende Informationen
                                         Tutorial, “Der dynamische Modus” auf Seite I-17
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                                  I-189
                 Planung                                                               Softwarereferenz




                           Fahrzeuge
                           Planung > Fahrzeuge




                           Abb. I-65     Fahrzeug wählen


                           Über diesen Dialog können Sie einer Tour ein anderes Fahrzeug zuweisen.
                           Markieren Sie das gewünschte Fahrzeug und verlassen Sie den Dialog über
                           die Schaltfläche [OK].
                           Der ausgewählten Tour wird das oder die gewünschten Fahrzeuge zugewie-
                           sen.
                           Die Checkbox Maximale Beladung und Zeit vor Ort ist standardmäßig aktiv.
                           Damit wird sichergestellt, dass das gewünschte Fahrzeug nicht überladen
                           wird und dass z. B. die zulässigen Fahrzeiten, sowie die Be- und Entladezei-
                           ten eingehalten werden. Ist dies nicht der Fall, wird automatisch ein weiteres
                           Fahrzeug eingesetzt.


                           Ergänzende Informationen
                            Tutorial, “Fahrzeuge” auf Seite I-45
2.01 / 01-2017




                 I-190                                                 A+W Business Logistic Optmizer
                 Softwarereferenz                                                                            Planung




                                        Bestimmungsort bearbeiten
                                        Planung > Bestimmungsort bearbeiten




                                        Abb. I-66    Bestimmungsort bearbeiten


                                        In diesem Dialog können Sie den Bestimmungsort innerhalb einer Tour bear-
                                        beiten.

                                           Adresse ändern
                                           Die Änderungen, die Sie hier machen, haben keinen Einfluss auf die ei-
                                           gentlichen Stammdaten aus A+W Business. Die Änderungen werden in
                                           der OTR-Datenbank gespeichert und stehen dort zur Verfügung.

                                        Erläuterung der Felder

                                        Kunden-Nr. In diesem Feld wird Ihnen die Kunden-Nr. angezeigt.

                                        Kunden In diesem Feld wird Ihnen der Kunden-Name angezeigt.

                                        Symbol-Schaltfläche Diese Symbol-Schaltfläche ist nur aktiv, wenn in den
                                        Parametern der Wert OTR-Kundenadresse aktiv ist. Wenn Sie diese Symbol-
                                        Schaltfläche betätigen, öffnet sich der Dialog Kunde. Er enthält alle in der
                                        OTR-Datenbank gespeicherten Kunden.

                                        Typ Wählen Sie aus der Kombobox den entsprechenden Tour-Typ aus. Mög-
                                        lichen Werte sind:
                                        • Mittelpunkt: Der Mittelpunkt ist ein beliebiger Wegpunkt innerhalb der Tour.
                                        • Start-Punkt: Der Start-Punkt ist der Anfangspunkt der Tour.
                                        • End-Punkt: Der End-Punkt ist der Endpunkt der Tour.
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                                 I-191
                 Planung                                                              Softwarereferenz




                           Zeit In diesem Feld können Sie die Zeit in Minuten hinterlegen, die dem Fah-
                           rer zum Abladen und eventuellen neu Laden (Leergestelle) zur Verfügung
                           steht.

                           Ausgewählte Tour Hier werden Ihnen die Touren angezeigt, die in der Tabel-
                           le Touren im Bereich Planung zu sehen sind. Sie können die Kombobox auf-
                           klappen und eine andere Tour auswählen.

                           Liefertermin In diesem Feld wird Ihnen der Liefertermin angezeigt. Den Wert
                           können Sie an dieser Stelle nicht ändern, da Liefertermine nur für gesamte
                           Touren geändert werden können und nicht für einzelne Bestimmungsorte. Um
                           den Termin zu ändern, öffnen Sie den Dialog Touren, indem Sie eine Tour dop-
                           pelt anklicken.

                           Tour Hier sehen Sie die ursprünglichen Tour-Nummer. Dieser Wert kann
                           nicht geändert werden.

                           Reihenfolge Ist für zwei oder mehrere LKWs die gleiche Tournummer er-
                           laubt, dann können Sie über dieses Feld die Reihenfolge der LKWs bestim-
                           men. Das Feld wird nur ausgewertet, wenn in den Parametern der Eintrag
                           ROUTE_ORIGIN den Wert Ja hat.

                           Versandgewicht In diesem Feld wird Ihnen das Gewicht der Lieferung für
                           den jeweiligen Kunden angezeigt. Sie können den Wert überschreiben.

                           Rückholgewicht Sollte der Fahrer an einem Bestimmungsort leere Gestelle
                           aufladen und zurück transportieren, haben Sie in diesem Feld die Möglichkeit,
                           das entsprechende Gewicht zu hinterlegen. So haben Sie immer einen Über-
                           blick bezüglich des Gesamtgewichtes der Tour.

                           Priorität Aktivieren Sie diese Checkbox, wenn es sich bei der Adresse um
                           eine Prioritätsadresse handelt.

                           Rechtzeitig Aktivieren Sie diese Checkbox, wenn die Adresse pünktlich an-
                           gefahren werden soll.

                           Zeitbereich Klicken Sie auf die Symbol-Schaltfläche dahinter und es öffnet
                           sich der Dialog Zeitbereich. In diesem können Sie dann angeben, wann der
                           Kunde angefahren werden kann.

                           Beschreibung In diesem Feld können Sie eine detaillierte Beschreibung hin-
                           terlegen.

                           Adresse In diesem Feld wird Ihnen die Adresse des Kunden angezeigt.

                           Breitengrad In diesem Feld finden Sie den Breitengrad der Firmen-Adresse.

                           Längengrad In diesem Feld finden Sie den Längengrad der Firmen-Adresse.
2.01 / 01-2017




                 I-192                                                A+W Business Logistic Optmizer
                 Softwarereferenz                                                                             Planung




                                        Vorschläge Wenn Sie die Symbol-Schaltfläche [Vorschläge] betätigen, öffnet
                                        sich eine kleine Tabelle, die entsprechende Vorschläge zu der Adresse ent-
                                        hält. Bei mehreren Einträgen, können Sie einen auswählen. Betätigen Sie die
                                        Schaltfläche [Akzeptieren], werden die Daten in den Dialog Tour übernom-
                                        men.


                                        Ergänzende Informationen
                                         Tutorial, “Bestimmungsorte” auf Seite I-73
                                         Tutorial, “So bearbeiten Sie einen Bestimmungsort” auf Seite I-82
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                                 I-193
                 Planung                                                              Softwarereferenz




                           Zeitbereich
                           Planung > Bestimmungsort bearbeiten > von...bis...




                           Abb. I-67   Zeitbereich


                           In diesem Dialog können Sie einen Zeitbereich für einen Kunden hinterlegen.

                           Erläuterung der Felder

                           Von/Bis Sollten Ihre Kunden fixe Abladezeiten haben, dann können Sie die-
                           se hier hinterlegen. Bsp.: von 11.30 Uhr bis 13.00 Uhr. Im Feld Von geben Sie
                           dann 11:30 ein und im Feld Bis 13:00.
2.01 / 01-2017




                 I-194                                                A+W Business Logistic Optmizer
                 Softwarereferenz                                                                         Planung




                                        Dokumente
                                        Planung > Bestimmungsort bearbeiten > Register Dokumente




                                        Abb. I-68    Bestimmungsort bearbeiten, Register Dokumente


                                        In diesem Dialog werden Ihnen die Dokumente für den selektierten Bestim-
                                        mungsort angezeigt. Es handelt sich dabei um reine Anzeigefelder. Sie kön-
                                        nen keine Änderungen vornehmen.

                                        Erläuterung der Felder

                                        Status In diesem Feld wird Ihnen der Status des Wegpunktes angezeigt.

                                        Auftrags-Nr. In diesem Feld wird Ihnen die Auftrags-Nr. des Kundenauftrags
                                        angezeigt.

                                        Kunde In diesem Feld wird Ihnen die Kunden-Nummer angezeigt.

                                        Name In diesem Feld wird Ihnen der Kunden-Name angezeigt.

                                        Versandgewicht In diesem Feld wird Ihnen das Gewicht der Lieferung für
                                        den jeweiligen Kunden angezeigt.

                                        Rückholgewicht Sollte der Fahrer an einem Bestimmungsort leere Gestelle
                                        aufladen und zurück transportieren, wird Ihnen das Gewicht dieser Gestelle
                                        hier angezeigt.


                                        Ergänzende Informationen
                                         Tutorial, “Dokumente anzeigen” auf Seite I-74
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                              I-195
                 Planung                                                                Softwarereferenz




                           Positionen anzeigen
                           Planung > Bestimmungsort bearbeiten > Register Positionen




                           Abb. I-69   Bestimmungsort bearbeiten, Register Positionen


                           In diesem Dialog werden Ihnen die einzelnen Positionen der Tour(en) in einer
                           tabellarischen Übersicht angezeigt.

                           Erläuterung der Felder

                           Auftrag In diesem Feld sehen Sie die Auftragsnummer.

                           Pos. In diesem Feld sehen Sie die Positionsnummer des Auftrages.

                           Produkt In diesem Feld sehen Sie die Artikelnummer.

                           Bezeichnung 1-3 In diesem Feld wird Ihnen die Bezeichnung 1-3 des Pro-
                           duktes angezeigt.

                           Datum In diesem Feld sehen Sie das Bestelldatum des Auftrages.

                           Menge In diesem Feld wird Ihnen die bestellte Menge je Position angezeigt.

                           Breite In diesem Feld wird Ihnen die Breite der Einheit angezeigt.

                           Höhe In diesem Feld wird Ihnen die Höhe der Einheit angezeigt.

                           Dicke In diesem Feld wird Ihnen die Dicke der Einheit angezeigt.
2.01 / 01-2017




                           Gesamtgewicht In diesem Feld wird Ihnen das Gesamtgewicht der Position
                           angezeigt. Es ergibt sich aus dem Gewicht der Einheit multipliziert mit der
                           Menge.



                 I-196                                                 A+W Business Logistic Optmizer
                 Softwarereferenz                                                                       Planung




                                        M2 In diesem Feld werden Ihnen die Quadratmeter der Position angezeigt.
                                        Diese ergeben sich aus den Abmessungen und werden von A+W Business
                                        übergeben.


                                        Ergänzende Informationen
                                         Tutorial, “Positionen anzeigen” auf Seite I-75
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                            I-197
                 Planung                                                                   Softwarereferenz




                           Informationen anzeigen
                           Planung > Bestimmungsort bearbeiten > Register Informationen




                           Abb. I-70   Bestimmungsort bearbeiten, Register Informationen


                           In diesem Dialog werden Ihnen zusätzliche Informationen zum Bestimmungs-
                           ort angezeigt.

                           Erläuterung der Felder

                           Ansprechpartner In diesem Feld können Sie einen Ansprechpartner beim
                           Kunden hinterlegen.

                           Telefon In diesem Feld können Sie die Telefonnummer des Kontaktes hinter-
                           legen.

                           E-Mail-Adresse In diesem Feld können Sie die E-Mail-Adresse des Kontak-
                           tes hinterlegen.

                           Beschreibung In diesem Feld können Sie eine weitere Beschreibung zu
                           dem Kunden hinterlegen.

                           Adresse In diesem Feld wird Ihnen die Adresse des Kunden angezeigt. Die
                           Daten können an dieser Stelle geändert werden.

                           Längengrad In diesem Feld finden Sie den Längengrad der Firmen-Adresse.
                           Die Daten können an dieser Stelle geändert werden.

                           Breitengrad In diesem Feld finden Sie den Breitengrad der Firmen-Adresse.
2.01 / 01-2017




                           Die Daten können an dieser Stelle geändert werden.




                 I-198                                                 A+W Business Logistic Optmizer
                 Softwarereferenz                                                             Planung




                                        Ergänzende Informationen
                                         Tutorial, “Informationen anzeigen” auf Seite I-76
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                 I-199
                 Planung                                                               Softwarereferenz




                           Kunden
                           Planung > Bestimmungsort bearbeiten > Symbol-Schaltfläche [Kunde]




                           Abb. I-71   Kunden Übersicht


                           In diesem Dialog werden Ihnen alle gespeicherten Kundenadressen ange-
                           zeigt.

                           Erläuterung der Felder

                           Filter Dieses Feld dient dem Filtern der angezeigten Daten. Es steht in direk-
                           tem Zusammenhang mit dem Feld Filter-Typ. Wählen Sie zunächst den Filter-
                           Typ (Kunde oder Adresse) aus und geben Sie dann im Feld Filter die Angaben
                           ein, nach denen gefiltert werden soll.

                           Filter-Typ Über diese Kombobox steuern Sie, nach welchen Einträgen gefil-
                           tert werden soll, Kunde oder Adresse. Anschließend geben Sie im Feld Filter
                           die Angaben ein, nach denen gefiltert werden soll.

                           Filtern Nachdem Sie die entsprechenden Kriterien in den Feldern Filter und
                           Filter-Typ eingegeben haben, betätigen Sie diese Symbol-Schaltfläche. Da-
                           nach wird die Liste der Einträge entsprechend aktualisiert.

                           Filter löschen Um die eingegebenen Filter-Kriterien zu löschen, betätigen
                           Sie diese Symbol-Schaltfläche. Danach wird die Liste der Einträge entspre-
                           chend aktualisiert und es werden wieder alle Einträge angezeigt.

                           Kunden-Nr. In diesem Feld wird Ihnen die Kunden-Nr. angezeigt.

                           Kunde In diesem Feld wird Ihnen der Kunden-Name angezeigt.
2.01 / 01-2017




                           Adresse In diesem Feld wird Ihnen die Adresse des Kunden angezeigt.




                 I-200                                                 A+W Business Logistic Optmizer
                 Softwarereferenz                                                                         Planung




                                        Längengrad In diesem Feld finden Sie den Längengrad der Firmen-Adresse.

                                        Breitengrad In diesem Feld finden Sie den Breitengrad der Firmen-Adresse.

                                           Parameter-Einstellungen
                                           Der Dialog und die entsprechende Symbol-Schaltfläche sind nur aktiv,
                                           wenn in den Parametern der entsprechende Eintrag (Parameter: OTR-
                                           Kundenadresse) aktiv ist.


                                        Ergänzende Informationen
                                         Tutorial, “Kundenadressen bearbeiten” auf Seite I-79
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                             I-201
                 Planung                                                                  Softwarereferenz




                           Detailansicht
                           Planung > Detailansicht




                           Abb. I-72     Detailansicht anzeigen


                           Über die Detailansicht haben Sie die Möglichkeit, die angezeigten Daten zu li-
                           mitieren. Ist die Detailansicht deaktiviert, werden Ihnen im Bereich Bestim-
                           mungsorte alle Bestimmungsorte aller Touren angezeigt.
                           Ist die Symbol-Schaltfläche aktiv, werden Ihnen nur die Bestimmungsorte der
                           Tour angezeigt, die Sie im Bereich Touren selektiert haben. Im Beispiel oben
                           sind das die Bestimmungsorte für die Tour 60.


                           Ergänzende Informationen
                            Tutorial, “Die Detailansicht” auf Seite I-77
2.01 / 01-2017




                 I-202                                                      A+W Business Logistic Optmizer
                 Softwarereferenz                                                                Optimierung




                                        Optimierung
                                        In diesem Bereich erfolgt die Optimierung der Route.
                                        Der Bereich beinhaltet:
                                        •   Die Wege zwischen den Bestimmungsorten optimieren:
                                             “Tour optimieren” auf Seite I-204
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                       I-203
                 Optimierung                                                                Softwarereferenz




                               Tour optimieren
                               Planung > [Weiter]




                               Abb. I-73    Tour optimieren


                               In diesem Dialog wird die Tour bzw. die Touren - gemäß den eingestellten Vor-
                               gaben - optimiert. Die Kartenansicht liefert Ihnen eine grafische Übersicht zur
                               aktuellen Tour. Auf der rechten Seite befindet sich oben eine Kombobox, die
                               die optimierten Touren enthält. Die beiden Register darunter (Optimierte Tour
                               / Ursprüngliche Tour) beziehen sich ebenfalls auf die aktuelle Tour. Das Regis-
                               ter Optimierte Tour zeigt Ihnen die anzufahrenden Wegpunkte in der entspre-
                               chenden Reihenfolge (nach der Optimierung). Im Register Ursprüngliche Tour
                               sehen Sie die ursprüngliche Reihenfolge (vor der Optimierung).

                               Erläuterung der Schaltflächen

                               Tour optimieren Diese Schaltfläche müssen Sie betätigen, wenn Sie Ände-
                               rungen an der Tour vorgenommen haben. Sie können z. B. die Reihenfolge
                               der Wegpunkte manuell mit der Maus ändern. Dazu klicken Sie den Wegpunkt
                               an, halten die Maustaste gedrückt und ziehen den Wegpunkt an die neue Stel-
                               le innerhalb der Reihenfolge. Ein solches Vorgehen hat Auswirkung auf die
                               Gesamtstrecke, die Zeit und die Kosten. Um diese Felder zu aktualisieren,
                               müssen Sie die Symbol-Schaltfläche Tour optimieren betätigen und so eine
                               neue Optimierung durchführen. Die Optimierung kann nach folgenden Kriteri-
                               en erfolgen:
                               • Anfangsroute: Die Optimierung erfolgt im Hinblick auf die Anfangsroute.
                               • Schnellste: Die Optimierung erfolgt im Hinblick auf die schnellste Route.
                               • Kürzeste: Die Optimierung erfolgt im Hinblick auf die kürzeste Route. Diese
                                   Option gilt nur für PKWs (mit und ohne Anhänger), nicht für LKWs.
2.01 / 01-2017




                               Alle Routen Wenn Sie diese Checkbox aktivieren, werden alle Routen neu
                               optimiert. Die neuen Ergebnisse bzw. optimierten Routen werden zusätzlich
                               angezeigt und Sie können dann das präferierte Ergebnis auswählen.

                 I-204                                                     A+W Business Logistic Optmizer
                 Softwarereferenz                                                                     Optimierung




                                        Optimierung stoppen Diese Schaltfläche können Sie betätigen, wenn Sie
                                        eine laufende Optimierung stoppen möchten.

                                        Optimierungs-Faktoren Diese Schaltfläche können Sie betätigen, wenn Sie
                                        die Optimierungs-Faktoren verändern möchten. Es öffnet sich der Dialog, der
                                        die einzelnen Faktoren enthält:
                                        • Entfernungs-Faktor
                                        • Gewichts-Faktor
                                        • Termin-Faktor
                                        • Prioritäts-Faktor
                                        • Zeit-Faktor
                                        Haben Sie einen dieser Werte geändert, müssen Sie die Tour erneut optimie-
                                        ren.


                                        Ergänzende Informationen
                                         Tutorial, “Touren optimieren” auf Seite I-88
                                         “Tour-Faktoren” auf Seite I-184
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                              I-205
                 Ergebnis                                                                  Softwarereferenz




                            Ergebnis
                            In diesem Bereich wird das Ergebnis der Optimierung mit allen notwendigen
                            Informationen dargestellt.
                            Der Bereich beinhaltet:
                            •   Das Ergebnis wird grafisch und tabellarisch dargestellt:
                                 “Ergebnis der Optimierung” auf Seite I-207
                            •   Die tatsächlich angefallenen Kosten der Tour erfassen:
                                 “Tour-Informationen” auf Seite I-209
2.01 / 01-2017




                 I-206                                                    A+W Business Logistic Optmizer
                 Softwarereferenz                                                                              Ergebnis




                                          Ergebnis der Optimierung
                                          Planung > Optimierung > [Weiter]




                 Abb. I-74   Ergebnis der Optimierung


                                          Dieser Dialog zeigt Ihnen das Ergebnis der Optimierung. Er enthält alle not-
                                          wendigen Informationen sowohl in grafischer als auch in tabellarischer Form.
                                          Der Dialog ist in drei Bereiche unterteilt:
                                          •   Touren
                                          •   Tourenplan
                                          •   Bestimmungsorte

                                          Erläuterung der Felder im Bereich Touren

                                          Tour-Status In diesem Feld wird Ihnen der Tour-Status angezeigt. Folgende
                                          Werte sind möglich:
                                          • Erstellt: In diesem Status befindet sich die Tour durch den Wizard bis zum
                                            Ergebnis. Dann ändert sich der Status in Grobgeplant. Werden gespeicher-
                                            te Touren geladen, haben diese ebenfalls den Status Erstellt.
                                          • Grobgeplant: Das ist der Status der Tour nach der Optimierung.
                                          • Feingeplant: Dieser Status wird zur Zeit noch nicht ausgewertet.
                                          • Freigegeben: Wenn Sie den Status in Freigegeben ändern, wird der Liefer-
2.01 / 01-2017




                                            termin, die Reihenfolge und die Tour an A+W Business zurückgemeldet.
                                            Sie können den Status nur einmal auf Freigegeben ändern.
                                          Die restlichen Felder sind weiter oben bereits beschrieben worden.


                 A+W Business Logistic Optmizer                                                                  I-207
                 Ergebnis                                                                 Softwarereferenz




                            Erläuterung der Felder im Bereich Tourenplan
                            Hier wird Ihnen die Kartenansicht mit den Routen angezeigt. Enthält das Er-
                            gebnis mehr als eine Route, wählen Sie im Bereich Touren diejenige aus, die
                            Sie hier angezeigt bekommen möchten.

                            Erläuterung der Felder im Bereich Bestimmungsorte
                            In diesem Bereich werden Ihnen die einzelnen Bestimmungsorte je Tour auf-
                            gelistet.
                            DIe einzelnen Felder sind bereits beschrieben worden.
                             “Bestimmungsort bearbeiten” auf Seite I-191

                            Erläuterung der Schaltflächen

                            Tour Wenn Sie diese Schaltfläche betätigen, öffnet sich der Dialog Tour mit
                            den Registern Allgemein, Fahrzeuge, Parameter und Kosten. In den einzel-
                            nen Registern haben Sie Zugriff auf einige Werte. Der Zugriff dient zum Kopie-
                            ren der Werte, nicht zum Ändern!

                            Bestimmungsort Wenn Sie diese Schaltfläche betätigen, öffnet sich der Di-
                            alog Bestimmungsort. An dieser Stelle haben Sie Zugriff auf folgende Werte:
                            • Versandgewicht
                            • Rückholgewicht
                            • Adresse
                            Der Zugriff dient zum Kopieren der Werte, nicht zum Ändern!

                            Tour bearbeiten Wenn Sie diese Schaltfläche betätigen, öffnet sich der Dia-
                            log Tour mit den Registern Status und Tour-Informationen. An dieser Stelle
                            können Sie folgenden Wert ändern:
                            • Tour-Status


                            Ergänzende Informationen
                             “Bestätigungs- und Lieferliste” auf Seite I-219
                             Tutorial, “Das Ergebnis der Optimierung” auf Seite I-97
                             Tutorial, “So exportieren Sie die Daten” auf Seite I-122
                             Tutorial, “Export” auf Seite I-121
2.01 / 01-2017




                 I-208                                                      A+W Business Logistic Optmizer
                 Softwarereferenz                                                                           Ergebnis




                                        Tour-Informationen
                                        Planung > Optimierung > Ergebnis > [Tour bearbeiten]




                                        Abb. I-75    Tour-Informationen


                                        Dieser Dialog gibt Ihnen einen Überblick zu den Tour-Kosten. Auf der linken
                                        Seite befinden sich die für die Tour ermittelten Kosten. Auf der rechten Seite
                                        haben Sie die Möglichkeit, die tatsächlichen Kosten, die während der Tour an-
                                        gefallen sind, zu hinterlegen. Sie werden gespeichert und bei der nächsten
                                        Tour mit berücksichtigt. Bitte beachten Sie, dass Sie die tatsächlichen Kosten
                                        erst eintragen können, wenn Ihr Fahrer mit dem Tourbericht zurück ist.

                                        Erläuterung der Felder im rechten Bereich

                                        Tatsächliche Entfernung In diesem Feld geben Sie ein, wie viele KM die
                                        Tour wirklich hatte.

                                        Tatsächliche Kosten/Fahrer In diesem Feld geben Sie die tatsächlichen
                                        Kosten pro Fahrer an, die auf der Tour entstanden sind.

                                        Tatsächliche Zeit In diesem Feld geben Sie ein, wie lange die Tour wirklich
                                        gedauert hat.

                                        Tage In diesem Feld geben Sie ein, wie viele Tage die Tour wirklich gedauert
                                        hat.
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                                 I-209
                 Ergebnis                                                                 Softwarereferenz




                            Stunden In diesem Feld geben Sie ein, wie viele Stunden die Tour wirklich
                            gedauert hat.

                            Minuten In diesem Feld geben Sie ein, wie viele Minuten die Tour wirklich ge-
                            dauert hat.

                            Tatsächliche Mautkosten In diesem Feld geben Sie die tatsächlichen Maut-
                            kosten an, die auf der Tour entstanden sind.

                            Tatsächliche Kraftstoffkosten In diesem Feld geben Sie die tatsächlichen
                            Kraftstoffkosten an, die auf der Tour entstanden sind.

                            Tatsächliche Extrakosten In diesem Feld geben Sie die tatsächlichen Ext-
                            rakosten an, die auf der Tour entstanden sind.

                            Tatsächliche Fixkosten In diesem Feld geben Sie die tatsächlichen Fixkos-
                            ten an, die auf der Tour entstanden sind.

                            Erläuterung der Schaltflächen

                            Kosten übernehmen Wenn Sie diese Schaltfläche betätigen, werden die
                            Kosten des linken Bereiches in den Bereich der Tatsächlichen Kosten über-
                            nommen.

                            Kosten entfernen Wenn Sie diese Schaltfläche betätigen, werden die Werte
                            im Bereich der Tatsächlichen Kosten gelöscht.

                            Erläuterung der Felder im Bereich Gesamtkosten

                            Tatsächliche Tourkosten In diesem Feld sehen Sie, wie viel die Tour wirk-
                            lich gekostet hat. Es ist die Summe aller Tatsächlicher Kosten.


                            Ergänzende Informationen
                             Tutorial, “Tatsächliche Tourkosten” auf Seite I-100
2.01 / 01-2017




                 I-210                                                      A+W Business Logistic Optmizer
                 Softwarereferenz                                                                            Abfrage




                                        Abfrage
                                        In diesem Bereich können Sie alle notwendigen Informationen abfragen. Bitte
                                        beachten Sie, dass, in Abhängigkeit des Tour-Status (Initiieren, Geplant, in
                                        Änderung, etc.), unterschiedliche Funktionen in der Menüleiste aktiv sind. So
                                        können Sie z. B. für eine Geplante Tour den Status nicht ändern, d. h. die
                                        Schaltfläche Statusänderung ist nicht aktiv.
                                        Der Bereich beinhaltet:
                                        •   Das Filtern von Routen:
                                             “Routen filtern” auf Seite I-212
                                        •   Listen für Ihre Fahrer drucken:
                                             “Bestätigungs- und Lieferliste” auf Seite I-219
                                        •   Reports drucken:
                                             “Bestätigungs- und Lieferliste” auf Seite I-219
                                        •   Statistiken erstellen:
                                             “Statistik” auf Seite I-223
                                        •   Kalender anzeigen:
                                             “Kalender” auf Seite I-229
                                        •   Die Route für Navigationssysteme exportieren:
                                             “Export” auf Seite I-214
                                        •   Sich die Historie anzeigen lassen:
                                             “Historie” auf Seite I-217
                                        •   Dateien anhängen:
                                             “Dateien anhängen” auf Seite I-230
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                                I-211
                 Abfrage                                                               Softwarereferenz




                           Routen filtern
                           Abfrage > [Filtern]




                           Abb. I-76    Route filtern


                           In diesem Dialog haben Sie die Möglichkeit, sich die Routen gefiltert anzeigen
                           zu lassen. Das grenzt die Anzahl der angezeigten Routen ein.

                           Erläuterung der Felder

                           Datum von In diesem Feld geben Sie das Startdatum ein, ab dem gefiltert
                           werden soll.

                           Datum bis In diesem Feld geben Sie das Enddatum ein, bis zu dem gefiltert
                           werden soll.

                           Tour ID Möchten Sie die Anzeige nach der Tour ID filtern, geben Sie hier -
                           nachdem Sie hier die entsprechende Tour ID ein.

                           Tour-Name Möchten Sie die Anzeige nach dem Tour-Namen filtern, geben
                           Sie hier den entsprechenden Tour-Namen ein.

                           Tour-Status Möchten Sie die Anzeige nach dem Tour-Status filtern, wählen
                           Sie aus der Checkbox Tour Status den bzw. die gewünschten Status. Über die
                           darunter liegenden Symbol-Schaltflächen können Sie alle aktivieren bzw. de-
                           aktivieren.

                           Fahrzeuge Möchten Sie die Anzeige nach den Fahrzeugen filtern, wählen
2.01 / 01-2017




                           Sie aus der Kombobox das gewünschte Fahrzeug aus.

                           Fahrer ID Möchten Sie die Anzeige nach der Fahrer ID filtern, wählen Sie aus
                           der Kombobox die gewünschte Fahrer ID aus.


                 I-212                                                 A+W Business Logistic Optmizer
                 Softwarereferenz                                                                         Abfrage




                                        Abteilung Möchten Sie die Anzeige nach der Abteilung filtern, wählen Sie
                                        aus der Kombobox die gewünschte Abteilung aus.

                                        Kunde In diesem Feld können Sie noch einen Kunden eingeben, nach dem
                                        gefiltert werden soll.

                                        Erläuterung der Schaltfläche

                                        Löschen Über diese Schaltfläche setzen Sie die gemachten Eingaben zu-
                                        rück. Der Dialog ist leer.


                                        Ergänzende Informationen
                                         Tutorial, “Touren” auf Seite I-119
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                             I-213
                 Abfrage                                                               Softwarereferenz




                           Export
                           Abfrage > Tour > [Export Tour]




                           Abb. I-77    Export


                           In diesem Dialog haben Sie die Möglichkeit, die Tourdaten für ein Navigations-
                           system zu exportieren.

                              Dateiformate
                              Mit welchem Dateiformat Ihr Navigationssystem arbeitet, entnehmen Sie
                              bitte der Bedienungsanleitung Ihres Gerätes.

                           Erläuterung der Felder

                           ITN Aktivieren Sie diese Radiotaste, um die Daten im ITN-Format (z. B. Tom-
                           Tom) zu exportieren.

                           GPX Aktivieren Sie diese Radiotaste, um die Daten im GPX-Format (z. B.
                           Garmin) zu exportieren.

                           Markierungen einfügen Aktivieren Sie diese Checkbox, wenn neben der
                           Strecke auch die Bestimmungsorte mit exportiert werden sollen.

                           Neuen Ordner für Tour Aktivieren Sie diese Checkbox, wenn für den Export
                           ein neuer Ordner erstellt werden soll.

                           Exportpfad In diesem Feld geben Sie an, wohin die Datei exportiert werden
                           soll.
2.01 / 01-2017




                 I-214                                                 A+W Business Logistic Optmizer
                 Softwarereferenz                                                                        Abfrage




                                           Standardpfad für Exportdateien
                                           Den Standardpfad zum Exportieren der Daten legen Sie in den Parametern
                                           fest (Parameter: Path_Export_ITN_GPS_File).

                                        Kopieren Klicken Sie auf diese Schaltflächem zn die Tour zu kopieren und
                                        per Mail an die Android URL zu senden. Der Anwender kann die entsprechen-
                                        de URL auf seinem Android Gerät über HERE maps aufrufen.


                                        Ergänzende Informationen
                                         Tutorial, “Export” auf Seite I-121
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                            I-215
                 Abfrage                                                              Softwarereferenz




                           Statusänderung
                           Abfrage > [Statusänderung]




                           Abb. I-78   Statusänderung


                           Dieser Dialog dient dazu, den Status einer Tour manuell zu ändern. Das kann
                           z. B. notwendig sein, wenn Sie den Prozess vor dem Register Ergebnis ge-
                           schlossen haben. Dann befindet sich die Tour im Status Erstellt oder in Ände-
                           rung. Dann ist es nötig, den Status der Tour manuell auf Geplant oder
                           Organisiert zu setzen.

                           Erläuterung der Felder

                           Aktueller Routenstatus In diesem Feld wird Ihnen angezeigt, in welchem
                           Status sich die Route momentan befindet. Das Feld kann nicht geändert wer-
                           den.

                           Änderungsdatum In diesem Feld wird Ihnen das Datum der letzten Ände-
                           rung angezeigt. Das Feld kann nicht geändert werden.

                           Tour-Status Die Kombobox enthält alle für die Tour möglichen Status. Wäh-
                           len Sie den gewünschten Status aus.

                           Benutzer In diesem Feld wird Ihnen der aktuelle Benutzer angezeigt. Das
                           Feld kann nicht geändert werden.
2.01 / 01-2017




                 I-216                                                A+W Business Logistic Optmizer
                 Softwarereferenz                                                                              Abfrage




                                        Historie
                                        Abfrage > [Historie]




                                        Abb. I-79    Historie


                                        In diesem Dialog haben Sie die Möglichkeit, sich eine Historie anzeigen zu las-
                                        sen. Im oberen Bereich (Filter) treffen Sie die Auswahl und im unteren Bereich
                                        (Ergebnis) werden Ihnen die entsprechenden Daten angezeigt.

                                        Erläuterung der Felder im Bereich Felder

                                        Tour ID Möchten Sie die Anzeige nach der Tour ID filtern, geben Sie hier die
                                        Tour ID ein.

                                        Dokument Möchten Sie die Anzeige nach der Auftrags-Nr. filtern, geben Sie
                                        hier die Auftrags-Nr. ein. Alternativ können Sie auch die Lieferschein-Nr. ein-
                                        geben.

                                        Kunde Möchten Sie die Anzeige nach dem Kunden filtern, geben Sie hier die
                                        Kunden-Nr. ein.

                                        Archivierte Routen anzeigen Möchten Sie, dass auch archivierte Routen
                                        angezeigt werden, aktivieren Sie diese Checkbox.

                                        Erläuterung der Schaltfläche

                                        OK Über diese Schaltfläche starten Sie die Filterfunktion.
2.01 / 01-2017




                                        Erläuterung der Felder im Register Tour

                                        Datum In diesem Feld wird Ihnen das Tour-Datum angezeigt.



                 A+W Business Logistic Optmizer                                                                  I-217
                 Abfrage                                                              Softwarereferenz




                           Kunde In diesem Feld wird Ihnen Kunden-Nummer angezeigt.

                           Name In diesem Feld wird Ihnen der Kunden-Name angezeigt.

                           Status In diesem Feld wird Ihnen der Tour-Status angezeigt.

                           Kommentar In diesem Feld wird Ihnen ein hinterlegter Kommentar ange-
                           zeigt.

                           Auftrag In diesem Feld wird Ihnen die Auftrags-Nummer angezeigt. Haben
                           Sie eine Lieferschein-Nummer eingegeben, wird Ihnen diese hier angezeigt.

                           Benutzer In diesem Feld sehen Sie, wer an dem Dokument Änderungen vor-
                           genommen hat.

                           Erläuterung der Felder im Register Dokumente

                           Auftrag In diesem Feld wird Ihnen die Auftrags-Nummer angezeigt. Haben
                           Sie eine Lieferschein-Nummer eingegeben, wird Ihnen diese hier angezeigt.

                           Tour ID In diesem Feld wird Ihnen die Tour ID angezeigt.

                           Kunde In diesem Feld wird Ihnen Kunden-Nummer angezeigt.

                           Name In diesem Feld wird Ihnen der Kunden-Name angezeigt.

                           Status In diesem Feld wird Ihnen der Tour-Status angezeigt.

                           Versandgewicht In diesem Feld wird Ihnen das Gewicht für den ausgewähl-
                           ten Bestimmungsort angezeigt.

                           Gewicht Rückholung Wurden bei dem Kunden leere Gestelle mitgenom-
                           men, wird Ihnen hier angezeigt, wie schwer diese Gestelle waren.


                           Ergänzende Informationen
                            Tutorial, “Historie” auf Seite I-124
2.01 / 01-2017




                 I-218                                               A+W Business Logistic Optmizer
                 Softwarereferenz                                                                               Abfrage




                                        Bestätigungs- und Lieferliste
                                        Abfrage > Reports > [Ausgewählte Tour]
                                        Die hier angezeigte Bestätigungs- und Lieferliste stellt ein Bespiel dar. Da die-
                                        ser Report auf SAP Crystal Reports basiert, kann dies in Ihrem System anders
                                        aussehen bzw.andere Daten enthalten.




                                        Abb. I-80    Bestätigungs- und Lieferliste


                                        Diese Liste gibt Ihnen eine detaillierte Übersicht zu dem Ergebnis der Optimie-
                                        rung. Sie enthält alle notwendigen Informationen sowohl in grafischer als auch
2.01 / 01-2017




                                        in tabellarischer Form zu den einzelnen Haltepunkten und Ladestationen. Die
                                        Liste kann gedruckt und dem Fahrer ausgehändigt werden.




                 A+W Business Logistic Optmizer                                                                   I-219
                 Abfrage                                                               Softwarereferenz




                           Erläuterung der Felder

                           Tour In diesem Feld wird Ihnen die Tour-Nummer angezeigt.

                           Name Hier wird Ihnen der Name der Tour angezeigt, den Sie seinerzeit ver-
                           geben bzw. ausgewählt haben.

                           Datum Hier wird Ihnen das Datum angezeigt, an dem die Tour gefahren wird.

                           Name des Fahrers In diesem Feld wird Ihnen der Name des Fahrers ange-
                           zeigt.

                           Fahrzeug In diesem Feld sehen Sie, mit welchem Fahrzeug die Tour gefah-
                           ren wird.

                           KM Gesamt In diesem Feld wird Ihnen angezeigt, wie viele Kilometer die ge-
                           samte Tour hat.

                           Gewicht Gesamt In diesem Feld wird Ihnen angezeigt, wie viele Kilogramm
                           auf der gesamten Tour zu transportieren sind. Das Gewicht beinhaltet auch die
                           Rückholungen.

                           Zeit Gesamt In diesem Feld wird Ihnen angezeigt, wie viele Kilogramm auf
                           der gesamten Tour zu transportieren sind. Das Gewicht beinhaltet auch die
                           Rückholungen.

                           Startzeit In diesem Feld wird Ihnen angezeigt, um wie viel Uhr die Tour star-
                           tet.

                           Verfügbar Sollten Sie für Ihren Kunden fixe Abladezeiten hinterlegt haben,
                           dann werden Ihnen diese hier angezeigt.

                           Adresse In diesem Feld wird Ihnen die Ausgangsadresse für den nächsten
                           Streckenabschnitt angezeigt. Bsp.: Von A nach B. Dann sehen Sie hier die Ad-
                           resse von A und im Feld Ziel die Adresse von B.

                           Ziel In diesem Feld wird Ihnen die Zieladresse für den nächsten Streckenab-
                           schnitt angezeigt. Bsp.: Von A nach B. Dann sehen Sie hier die Adresse von
                           B und im Feld Adresse die Adresse von A.

                           KM vom Ausgangs- zum Zielort In diesem Feld sehen Sie die Entfernung
                           zum nächsten Bestimmungsort.

                           Versandgewicht In diesem Feld wird Ihnen das Gewicht für den ausgewähl-
                           ten Bestimmungsort angezeigt.

                           Gewicht Rückholung Nehmen Sie bei einem Kunden leere Gestelle mit,
                           wird Ihnen hier angezeigt, wie schwer diese Gestelle sind.
2.01 / 01-2017




                 I-220                                                A+W Business Logistic Optmizer
                 Softwarereferenz                                                                           Abfrage




                                        Fahrtzeit Hier wird Ihnen die Fahrtzeit zum nächsten Bestimmungsort ange-
                                        zeigt.

                                        Abladezeit Sollte für Ihren Fahrer eine Zeit zum Abladen und Aufladen (Leer-
                                        gestelle) hinterlegt worden sein, wird Ihnen diese hier angezeigt.

                                        Bemerkung In diesem Feld hat Ihr Fahrer die Möglichkeit, eine Bemerkung
                                        zu notieren.

                                        Unterschrift In diesem Feld unterschreibt Ihr Kunde bei der Auslieferung.


                                        Ergänzende Informationen
                                         Tutorial, “Ausgewählte Tour” auf Seite I-125
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                               I-221
                 Abfrage                                                              Softwarereferenz




                           Report Launcher
                           Abfrage > [Report Launcher]




                           Abb. I-81    Report Launcher


                           Über diesen Dialog können Sie die Reports drucken, die Sie vorher definiert
                           haben.

                           Erläuterung der Felder

                           Berichts-Name In diesem Feld wird Ihnen der Berichts-Name angezeigt, den
                           Sie beim Definieren des Reports vergeben haben.

                           Berichts-Pfad In diesem Feld wird Ihnen der Berichts-Pfad angezeigt, den
                           Sie beim Definieren des Reports vergeben haben.

                           Parameter In diesem Feld werden Ihnen die Parameter angezeigt, die Sie
                           beim Definieren des Reports ausgewählt haben.

                           Erläuterung der Schaltfläche

                           Bericht drucken Über diese Schaltfläche starten Sie den Druck.


                           Ergänzende Informationen
                            “Reports” auf Seite I-125
2.01 / 01-2017




                 I-222                                               A+W Business Logistic Optmizer
                 Softwarereferenz                                                                              Abfrage




                                        Statistik
                                        Abfrage > [Statistik]




                                        Abb. I-82    Statistik, Register Allgemein


                                        Über diesen Dialog können Sie sich globale Statistiken erstellen.
                                        Der Dialog ist in folgende Register unterteilt:
                                        •   Allgemein
                                        •   Allgemeine Grafik
                                        •   Fahrzeuge
                                        •   Fahrer
                                        •   Abteilungen
                                        •   Kunden


                                        Register Allgemein
                                        Dieses Register gibt Ihnen einen Überblick zu den Tour-Kosten. Es werden die
                                        tatsächlichen Kosten den geplanten Kosten gegenüber gestellt. Darüber hin-
                                        aus sehen Sie die Abweichung sowohl in der Währung als auch in Prozent.
                                        Sie bekommen Informationen zu den Gewichten, dem Verbrauch, der Entfer-
                                        nung, etc.
                                        In dem Dialog befindet sich auf der linken Seite der Bereich Filter. Hier können
                                        Sie die anzuzeigenden Daten bequem Ihren Wünschen entsprechend anpas-
                                        sen. Haben Sie eine Auswahl getroffen, klicken Sie bitte auf [OK]. Anschlie-
                                        ßend wird die Anzeige aktualisiert.
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                                  I-223
                 Abfrage                                                                  Softwarereferenz




                           Register Allgemeine Grafik
                           Abfrage > [Statistik] > Register Allgemeine Grafik




                           Abb. I-83     Statistik, Register Allgemeine Grafik


                           Dieses Register liefert Ihnen eine Diagramm-Ansicht gemäß den Filterkriteri-
                           en, die Sie auf der linken Seite eingestellt haben.


                           Ergänzende Informationen
                            Tutorial, “Reports” auf Seite I-125
2.01 / 01-2017




                 I-224                                                      A+W Business Logistic Optmizer
                 Softwarereferenz                                                                            Abfrage




                                        Register Fahrzeuge
                                        Abfrage > [Statistik] > Register Fahrzeuge




                                        Abb. I-84     Statistik, Register Fahrzeuge


                                        Dieses Register liefert Ihnen eine Diagramm-Ansicht zu den Fahrzeugen ge-
                                        mäß den Filterkriterien, die Sie auf der linken Seite eingestellt haben.
                                        Zusätzlich zu den Filterkriterien können Sie innerhalb der Ansicht noch zwi-
                                        schen folgenden Kriterien wechseln:
                                        •   Entfernung
                                        •   Zeit
                                        •   Zugewiesenes Gewicht
                                        •   Kraftstoffkosten
                                        •   Geplante Kosten
                                        •   Tatsächliche Kosten


                                        Ergänzende Informationen
                                         Tutorial, “Reports” auf Seite I-125
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                                I-225
                 Abfrage                                                               Softwarereferenz




                           Register Fahrer
                           Abfrage > [Statistik] > Register Fahrer




                           Abb. I-85     Statistik, Register Fahrer


                           Dieses Register liefert Ihnen eine Diagramm-Ansicht zu den Fahrern gemäß
                           den Filterkriterien, die Sie auf der linken Seite eingestellt haben.
                           Zusätzlich zu den Filterkriterien können Sie innerhalb der Ansicht noch zwi-
                           schen folgenden Kriterien wechseln:
                           •   Entfernung
                           •   Zeit
                           •   Zugewiesenes Gewicht
                           •   Kosten pro Fahrer
                           •   Geplante Kosten
                           •   Tatsächliche Kosten


                           Ergänzende Informationen
                            Tutorial, “Reports” auf Seite I-125
2.01 / 01-2017




                 I-226                                                A+W Business Logistic Optmizer
                 Softwarereferenz                                                                            Abfrage




                                        Register Abteilungen
                                        Abfrage > [Statistik] > Register Abteilungen




                                        Abb. I-86     Statistik, Register Abteilungen


                                        Dieses Register liefert Ihnen eine Diagramm-Ansicht zu den Abteilungen ge-
                                        mäß den Filterkriterien, die Sie auf der linken Seite eingestellt haben.
                                        Zusätzlich zu den Filterkriterien können Sie innerhalb der Ansicht noch zwi-
                                        schen folgenden Kriterien wechseln:
                                        •   Entfernung
                                        •   Zeit
                                        •   Zugewiesenes Gewicht
                                        •   Abteilung
                                        •   Geplante Kosten
                                        •   Tatsächliche Kosten


                                        Ergänzende Informationen
                                         Tutorial, “Reports” auf Seite I-125
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                                I-227
                 Abfrage                                                               Softwarereferenz




                           Register Kunden
                           Abfrage > [Statistik] > Register Kunden




                           Abb. I-87     Statistik, Register Kunden


                           Dieses Register liefert Ihnen eine Diagramm-Ansicht zu den Kunden gemäß
                           den Filterkriterien, die Sie auf der linken Seite eingestellt haben.
                           Zusätzlich zu den Filterkriterien können Sie innerhalb der Ansicht noch zwi-
                           schen folgenden Kriterien wechseln:
                           •   Menge
                           •   Entfernung
                           •   Ziel Entfernung
                           •   Zeit
                           •   Zugewiesenes Gewicht


                           Ergänzende Informationen
                            Tutorial, “Reports” auf Seite I-125
2.01 / 01-2017




                 I-228                                                A+W Business Logistic Optmizer
                 Softwarereferenz                                                                              Abfrage




                                        Kalender
                                        Abfrage > [Kalender]




                                        Abb. I-88     Kalender


                                        Der Kalender liefert Ihnen eine Übersicht zu den Fahrern oder den Fahrzeu-
                                        gen. Sie können sich diese täglich oder monatlich anzeigen lassen. Klicken
                                        Sie einen Eintrag doppelt an, öffnet sich der Dialog Abfrage mit einer tabella-
                                        rischen Übersicht der Touren und Bestimmungsorte. Darüber hinhaus können
                                        Sie die Anzeige auf einen bestimmten Tour-Status (geplant, freigegeben, ar-
                                        chiviert, etc.) beschränken. Klicken Sie auf die Schaltfläche [Löschen], wird
                                        die Auswahl im Bereich Tour-Status zurück gesetzt und die Anzeige aktuali-
                                        siert.
                                        Sollten Sie versehentlich oder unwissentlich einen Fahrer oder einen LKW auf
                                        zwei unterschiedlichen Touren - aber zeitgleich geplant haben - so können Sie
                                        den Konflikt hier lösen und manuell einen anderen Fahrer oder LKW zuord-
                                        nen. So entfällt ein erneutes Planen und Optimieren, um den Konflikt zu lösen.


                                        Ergänzende Informationen
                                         Tutorial, “Kalender” auf Seite I-130
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                                  I-229
                 Abfrage                                                              Softwarereferenz




                           Dateien anhängen
                           Abfrage > [Dateien anhängen]




                           Abb. I-89    Dateien anhängen


                           Über diesen Dialog können Sie dem Fahrer Dokumente in digitaler Form zur
                           Verfügung stellen.
                           Der Dialog ist in folgende Bereiche unterteilt:
                           •   Filtern
                           •   Bestimmungsorte
                           •   Dateien

                           Erläuterung der Felder im Bereich Filtern

                           Tour ID In diesem Feld geben Sie die Tour ID ein, für die Sie Dokumente in
                           die Cloud laden möchten. Wenn Sie die Tour ID nicht wissen, jedoch den Tour-
                           Namen, dann können Sie auch im Bereich Touren den entsprechenden Tour-
                           Namen mit einem Doppelklick auswählen. Das Feld wird dann automatisch
                           mit der gewählten Tour ID gefüllt. Im Bereich Bestimmungsorte werden jetzt
                           nur noch die Bestimmungsorte für die gewählte Tour ID angezeigt.

                           Kunde In diesem Feld geben Sie die Kundennummer ein, für die Sie Doku-
                           mente in die Cloud laden möchten. Im Bereich Bestimmungsorte, Feld Kun-
                           den-Nr. werden Ihnen alle Kunden angezeigt, die auf der entsprechenden Tour
                           angefahren werden.

                           Auftrag Bekommt ein Kunde mehrere Auftrags-Nummern geliefert, geben
2.01 / 01-2017




                           Sie in diesem Feld die Autrags-Nummer ein, für die Sie Dokumente in die
                           Cloud laden möchten.




                 I-230                                                  A+W Business Logistic Optmizer
                 Softwarereferenz                                                                            Abfrage




                                        Erläuterung der Felder im Bereich Dokumente

                                        Tour ID In diesem Feld wird Ihnen die Tour ID des Auftrags angezeigt, für den
                                        Sie Dokumente in die Cloud laden möchten.

                                        Tour-Name In diesem Feld wird Ihnen der Tour-Name des Auftrags ange-
                                        zeigt, für den Sie Dokumente in die Cloud laden möchten.

                                        Kunden-Nr. In diesem Feld wird Ihnen die Kunden-Nummer des Auftrags an-
                                        gezeigt, für den Sie Dokumente in die Cloud laden möchten.

                                        Kunde In diesem Feld wird Ihnen der Kunden-Name des Auftrags angezeigt,
                                        für den Sie Dokumente in die Cloud laden möchten.

                                        Auftrag In diesem Feld wird Ihnen die Auftrags-Nummer angezeigt, für die
                                        Sie Dokumente in die Cloud laden möchten.

                                        Erläuterung der Felder im Bereich Dateien
                                        Dieser Bereich wird erst dann mit Daten gefüllt, wenn Sie Dokumente in die
                                        Cloud geladen haben.

                                        Name In diesem Feld wird Ihnen der Dokumenten-Name angezeigt, den Sie
                                        hinterlegt haben.

                                        Beschreibung In diesem Feld wird Ihnen die Beschreibung angezeigt, die
                                        Sie hinterlegt haben.

                                        Dateipfad In diesem Feld wird Ihnen der Pfad zu der Datei angezeigt.

                                        Erläuterung der Schaltflächen

                                        Dokument hinzufügen Wenn Sie auf diese Schaltfläche klicken, öffnet sich
                                        der Dialog Datei anhängen. In diesem Dialog geben Sie das Dokument ein,
                                        das in die Cloud geladen werden soll.

                                        Dokument bearbeiten Wenn Sie auf diese Schaltfläche klicken, öffnet sich
                                        für das selektierte Dokument der Dialog Datei anhängen. Auf diese Weise
                                        können Sie Änderungen an dem angehängten Dokument vornehmen.

                                        Dokument löschen Wenn Sie auf diese Schaltfläche klicken, wird das selek-
                                        tierte Dokument gelöscht.


                                        Ergänzende Informationen
                                         “Dokumente in die Cloud laden” auf Seite I-104
2.01 / 01-2017




                 A+W Business Logistic Optmizer                                                                I-231
                 Abfrage                                                                   Softwarereferenz




                           Datei anhängen
                           Abfrage > [Dateien anhängen] > Symbol-Schaltfläche




                           Abb. I-90    Datei anhängen


                           Über diesen Dialog laden Sie die Dokumente in die Cloud.

                           Erläuterung der Felder

                           Dateiname In diesem Feld können Sie einen Namen hinterlegen, z. B. Lie-
                           ferschein.

                           Dateipfad In diesem Feld geben Sie den entsprechenden Pfad zur Cloud ein,
                           z. B. https://drive.google.com/file/d/....

                           Beschreibung In diesem Feld können Sie eine weitere Beschreibung hinter-
                           legen.


                           Ergänzende Informationen
                            Tutorial, “So laden Sie Dokumente in die Cloud und referenzieren diese” auf
                             Seite I-105
2.01 / 01-2017




                 I-232                                                   A+W Business Logistic Optmizer
Logistic Optimizer               I

                          Partindex




                     A+W Business
                 Partindex                                                                         Index




                 Index
                 A                                       Datenbank
                 Abteilungen I-135, I-142                – Quelle I-118, I-119
                 – Abteilung I-135                       – Verbindung (OTR) I-118
                 – Beschreibung I-135                    Datenimport I-143
                 – Name I-135                            Dokumentation
                                                         – Arten I-12
                                                         Dokumente
                 B
                                                         – Auftrags-Nr. I-176
                 Benutzer I-130
                                                         – Kunden-Name I-176
                 – ID I-130
                                                         – Kunden-Nummer I-176
                 – Kopieren von I-130
                                                         – Status I-176
                 – Name I-130
                 Benutzer-ID I-118, I-119
                 Bestätigungs- und Lieferliste           E
                 – Abladezeit I-202                      Ergebnis
                 – Bemerkung I-202                       – Bestimmungsort I-189
                 – Datum der Tour I-201                  – Tour I-189
                 – Fahrtzeit I-202                       – Tour bearbeiten I-189
                 – Fahrzeug I-201                        ERP-Verbindung
                 – Gesamtgewicht I-201                   – SQL ERP-Anbindung verwenden     I-119
                 – Gesamtstrecke I-201                   Export
                 – Gesamtzeit I-201                      – Exportpfad I-195
                 – KM vom Ausgangs- zum Zielort I-201    – GPX-Format I-195
                 – Name der Tour I-201                   – ITN-Format I-195
                 – Name des Fahrers I-201                – Kopieren I-196
                 – Tour I-201                            – Markierungen einfügen I-195
                 – Unterschrift I-202                    – Neuen Ordner für Tour I-195
                 – Versandgewicht I-201
                 – Ziel I-201                            F
                 Bestimmungsort bearbeiten               Fahrer I-139
                 – Abladezeit I-173                      – Abteilung I-140
                 – Abladezeit von ... bis ... I-175      – Adresse I-140
                 – Adresse I-173                         – Ansprechpartner I-140
                 – Ausgewählte Tour I-173                – Beschreibung I-140
                 – Beschreibung I-173                    – E-Mail I-140
                 – Bestimmungsort Typ I-172              – E-Mail Kontakt I-140
                 – Kunden-Name I-172                     – Fahrer-ID I-139
                 – Kunden-Nr. I-172                      – Kennwort zurücksetzen I-141
                 – Liefertermin I-173                    – Kontakt-Adresse I-140
                 – Priorität I-173                       – Kontakt-Telefon I-140
                 – Rechtzeitig I-173                     – Kosten I-140
                 – Tour-Nr. I-173                        – Kosten pro Faher nach Zeit I-140
                 – Versandgewicht I-173, I-176           – Kosten pro Fahrer nach Entfernung   I-140
                 – Zeitbereich I-173                     – Mitarbeiter I-140
                 – Zurückgeholtes Gewicht I-173, I-176   – Nachname I-139
                                                         – Nachname 2 I-139
2.01 / 01-2017




                 D                                       – Name I-139
                 Darstellungskonventionen   I-13         – Steuer-ID I-140
                 Daten importieren I-151                 – Telefonnummer I-140
                                                         – Telefonnummer 2 I-140

                 A+W Business Logistic Optmizer                                                    I-213
                 Index                                                                        Partindex




                 Fahrer bearbeiten                      Gespeicherte Tour laden   I-150
                 – Text finden I-160                    Gruppen I-170
                 Fahrzeug
                 – Abteilung I-137                      H
                 – Beschreibung I-138                   Historie
                 – Durchschnittliche Kosten I-137       – Archivierte Routen anzeigen I-198
                 – Durchschnittlicher Verbrauch I-137   – Auftrags-Nr. (Dokumente) I-199
                 – Fahrer ID I-138, I-160               – Auftrags-Nr. (Tour) I-199
                 – Fahrgestell-Nummer I-137             – Benutzer (Tour) I-199
                 – Feahrzeug verfügbar I-138, I-141     – Dokument I-198
                 – Kaufdatum I-137                      – Filtern I-198
                 – Leergewicht I-137                    – Kommentar (Tour) I-199
                 – Maixmale Höhe I-137                  – Kunde I-198
                 – Marke I-136                          – Kunde (Dokumente) I-199
                 – Maximale Beladung I-137              – Kunde (Tour) I-199
                 – Maximale Breite I-137                – Kunden-Name (Dokumente) I-199
                 – Maximale Länge I-137                 – Kunden-Name (Tour) I-199
                 – mit Anhänger I-138                   – Rückholgewicht (Dokumente) I-199
                 – Modell I-136                         – Tour ID I-198
                 – Nachname I-138, I-161                – Tour ID (Dokumente) I-199
                 – Nächste Wartung I-137                – Tour-Datum (Tour) I-198
                 – Nummernschild I-136                  – Tour-Status (Dokumente) I-199
                 – Reihenfolge I-138, I-173             – Tour-Status (Tour) I-199
                 – Symbol-Schaltfläche Fahrer I-138     – Versandgewicht (Dokumente) I-199
                 – Touren I-138
                 – Von/bis I-138
                 – Vorname I-138, I-161                 I
                 Fahrzeug auswählen                     Import
                 – Abteilung I-159                      – Bestimmungsort, Import-Pfad I-151
                 – Kraftstoffkosten I-159               – Bestimmungsort, Optionen I-151
                 – Kraftstoffverbrauch I-159            – Bestimmungsort, Tabelle I-151
                 – Marke I-159                          – Daten, Importiere CSV I-143
                 – Maximale Beladung I-159              – Daten, Import-Pfad I-144
                 – Modell I-159                         – Daten, Optionen I-143
                 – Von/bis I-159                        – Daten, Tabelle I-144
                 Fahrzeuge I-136                        – Daten, Was soll importiert werden I-143
                 Filtern                                Informationen
                 – Abteilung I-194                      – Ansprechpartner I-179
                 – Datum bis I-193                      – Beschreibung I-179
                 – Datum von I-193                      – E-Mail-Adresse I-179
                 – Fahrer ID I-193
                 – Fahrzeuge I-193                      K
                 – Kunde I-194                          Kalender I-210
                 – Löschen I-194                        Kennwort I-118, I-119
                 – Tour ID I-193                        Kopieren
                 – Tour-Name I-193                      – Gespeicherte Tour I-147
                 – Tour-Status I-193                    Kunde bearbeiten
                                                        – Adresse I-161, I-179, I-181
                 G                                      – Breitengrad I-179, I-182
2.01 / 01-2017




                 Gespeicherte Tour                      – Filter I-181
                 – Ladung I-148                         – Filter löschen I-160, I-181
                 Gespeicherte Tour kopieren   I-147     – Filtern I-160, I-181
                                                        – Filter-Typ I-160, I-181


                 I-214                                                 A+W Business Logistic Optmizer
                 Partindex                                                                                Index




                 – Kunden-Name I-181                           – Startzeit I-152, I-156
                 – Kunden-Nr. I-181                            – Tatsächliche Extratkosten I-169
                 – Längengrad I-179, I-182                     – Tatsächliche Fixkosten I-169
                 Kunden I-34, I-133                            – Tatsächliche Gesamtstrecke I-169
                 – Adresse I-133                               – Tatsächliche Kosten pro Fahrer I-169
                 – Ansprechpartner I-134                       – Tatsächliche Kraftstoffkosten I-169
                 – Beschreibung I-134                          – Tatsächliche Mautkosten I-169
                 – Breitengrad I-133                           – Tatsächliche Tourkosten I-169
                 – E-Mail-Adresse I-134                        – Tatsächliche Zeit I-169
                 – Fax I-134                                   – Termin-Faktor I-165
                 – Längengrad I-133                            – Tour-Faktoren I-165
                 – Name 2 I-134                                – Tourkosten I-169
                 – Name 3 I-134                                – Tour-Modus I-162
                 – Nummer I-133                                – Tunnel-Modus I-164
                 – Priorität I-133, I-134                      – Verkehr I-163
                 – Telefon I-133, I-134                        – Vorname I-157
                 – Zeit I-134                                  – Zeit I-169
                 – Zeitbereich I-134                           – Zeit-Faktor I-165
                                                               – Zug-Modus I-164
                 L                                             NeueTour
                 Laden                                         – Abteilung I-153
                 – Gespeicherte Tour   I-150                   – Ausgangspunkt verwenden I-154
                                                               – Beschreibung I-153
                                                               – Breitengrad des Ausgangspunktes I-153,
                 M                                               I-155, I-173
                 Modul                                         – Fahrzeug wählen I-157
                 – Funktion   I-11                             – Fortbewegungs-Typ I-157
                                                               – Geolokalisieren I-154
                 N                                             – Geolokalisieren Vorschläge I-155, I-174
                 Neue Tour                                     – Kraftstoffkosten I-157
                 – Autobahn-Modus I-163                        – Kraftstoffverbrauch I-157
                 – Entfernungs-Faktor I-165                    – Längengrad des Ausgangspunktes I-153,
                 – Extratkosten I-169                            I-155, I-173
                 – Fähren-Modus I-164                          – LKW Ladung I-157
                 – Fahrer ID I-157                             – LKW mit Anhänger I-157
                 – Fixkosten I-169                             – Maximale Höhe I-157
                 – Gesamtstrecke I-168                         – Maximale Länge I-157
                 – Gewichts-Faktor I-165                       – Name des Ausgangspunktes I-153
                 – Kosten pro Faher nach Zeit I-158            – Straße des Ausgangspunktes I-153, I-155
                 – Kosten pro Fahrer I-158, I-168              – Tour Status I-153
                 – Kosten pro Fahrer nach Entfernung   I-158   – Tour-ID I-153
                 – Kraftstoffkosten I-168                      – Tour-Name I-153
                 – Liefertermin I-152, I-162                   – Tour-Name (Original) I-153
                 – Mautkosten I-168                            – Ursprüngliche Nummer I-153
                 – Maut-Modus I-163                            NeueTour zusammenstellenladen I-152
                 – Maximale Breite I-157
                 – Multi-Tour I-162                            O
                 – Nachname I-157                              Optimierung
                 – Nummernschild I-156                         – Faktoren I-186
2.01 / 01-2017




                 – Optimierung überspringen I-163              – stoppen I-186
                 – Prioritäts-Faktor I-165                     – Tour optimieren I-185
                 – Standard-Tour-Faktoren I-167                OTR Datenbankquelle (OTR)   I-118, I-119
                 – Start der Tour I-163


                 A+W Business Logistic Optmizer                                                           I-215
                 Index                                                                                   Partindex




                 OTR Datenbankverbindung                           – Ursprüngliche Tour-Farbe I-126
                 – Benutzer ID I-118, I-119                        – Währung I-128
                 – Kennwort I-118, I-119                           – Zeit vor Ort I-125
                 OTR Datenbankverbindung testen     I-118, I-119   – Zeit-Faktor I-124
                                                                   – Zug-Modus I-121
                 P                                                 – Zuordnung von Fahrzeugen I-127
                 Parameter I-120                                   Positionen anzeigen
                 – Allgemeine Tour I-124                           – Auftragsnummer I-177
                 – Anwendungsdarstellung I-127                     – Bestelldatum I-177
                 – Autobahn-Modus I-122                            – Bestellte Menge I-177
                 – Bilder für Tourenbericht I-127                  – Bezeichnung 1-3 I-177
                 – Darstellung der Tour-Breite I-126               – Breite der Einheit I-177
                 – Darstellungsbreite der optimierten Tour I-125   – Dicke der Einheit I-177
                 – Dauer der Tour I-124                            – Gewicht der Position I-177
                 – Durchschnittlicher Kraftstoffverbrauch I-123    – Höhe der Einheit I-177
                 – Dynamische Fahrzeugzuordnung I-121              – M2 I-178
                 – Eine Tour für jede Ursprungs-Tour I-121         – Positionsnummer I-177
                 – Einheitensystem I-126
                 – Entfernungs-Faktor I-123                        R
                 – ERP Stammdaten verwenden I-127                  Report
                 – Export aktivieren I-128                         – Beschreibung I-142
                 – Exportpfad für Navigationssysteme I-128         – Parameter I-142
                 – Fähren-Modus I-122                              – Pfad I-142
                 – Fortbewegungs-Typ I-123                         Report Launcher I-203
                 – Gewichts-Faktor I-124                           – Bericht drucken I-203
                 – Großbuchstaben I-126                            – Berichts-Name I-203
                 – Kein Passwort I-127                             – Berichts-Pfad I-203
                 – Keine LKWs erlaubt I-121                        – Parameter I-203
                 – Kosten I-123                                    Reports
                 – Länder-Code I-126                               – Name I-142
                 – Lieferadresse anstelle von
                   Auftragsadresse I-128                           S
                 – Liefertermin I-120                              SQL ERP-Anbindung verwenden       I-119
                 – Lizenz-WebService I-124                         Statistik I-204
                 – Maut-Modus I-121                                Status
                 – Mehrere Routen I-126                            – Editierbar I-132
                 – Nächster Wartungstermin I-128                   – Name I-132
                 – Nächster Wartungstermin in ... Tagen I-128      – Status I-132, I-133
                 – Optimierte Tour durch gerade Linie I-125        – Typ I-131
                 – OTR-Kundenadresse verwenden I-128               Statusänderung I-197
                 – Prioritäts-Faktor I-124                         – Aktueller Status I-197
                 – Routen-Typ I-123                                – Änderungsdatum I-197
                 – Standard-Anfangsadresse I-125                   – Benutzer I-197
                 – Start-Adressse I-125                            – Tour-Status I-197
                 – Start-Firmenname I-125                          Symbole
                 – Startzeit der Tour I-124                        – Öffnen I-80
                 – Termin-Faktor I-124
                 – Transparenz der Tour I-125
                 – Transparenz der ursprünglichen Tour I-125       T
2.01 / 01-2017




                 – Tunnel-Modus I-123                              Tour Informationen
                 – Ursprüngliche Abteilung I-124                   – Kosten entfernen I-191
                 – Ursprüngliche Tour anzeigen I-125               – Kosten übernehmen I-191
                                                                   – Tatsächliche Entfernung I-190


                 I-216                                                           A+W Business Logistic Optmizer
                 Partindex                               Index




                 – Tatsächliche Extrakosten I-191
                 – Tatsächliche Fixkosten I-191
                 – Tatsächliche Kosten/Fahrer I-190
                 – Tatsächliche Kraftstoffkosten I-191
                 – Tatsächliche Mautkosten I-191
                 – Tatsächliche Minuten I-191
                 – Tatsächliche Stunden I-191
                 – Tatsächliche Tage I-190
                 – Tatsächliche Tourkosten I-191
                 – Tatsächliche Zeit I-190
                 Tour kopieren
                 – Abteilung I-148
                 – Adresse I-148
                 – Auftrag I-148
                 – Entfernung I-147
                 – Gewicht I-148
                 – Kosten der Tour I-147
                 – Kundenname I-148
                 – Kundennummer I-148
                 – Liefertermin I-147
                 – Marke und Modell I-148
                 – Maut I-148
                 – Name der Tour I-147
                 – Nummernschild I-148
                 – Priorität I-148
                 – Rechtzeitig I-148
                 – Reihenfolge I-148
                 – Rückholgewicht I-148
                 – Schaltfläche Filter I-149
                 – Schaltfläche kopieren I-149
                 – Status I-147
                 – Tour ID I-148
                 – Tour-ID I-147
                 – Tour-Name I-148
                 – Tour-Zeit I-147
                 – Typ I-149
                 – Ursprüngliche Nummer I-147
                 – Verkehr I-148
                 – Versandgewicht I-148
                 – Vorauss. Lieferung I-148
                 Tourstatus I-131

                 V
                 Verbindung
                 – Datenbank   I-118
2.01 / 01-2017




                 A+W Business Logistic Optmizer          I-217
                 Index                        Partindex
2.01 / 01-2017




                 I-218   A+W Business Logistic Optmizer

