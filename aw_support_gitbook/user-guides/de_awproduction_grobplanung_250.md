---
title: "DE AWProduction Grobplanung 2.50"
category: "user_manuals"
product: "Unknown"
doc_type: "Unknown"
language: "EN"
tags: ["DE_AWProduction_Grobplanung_2.50"]
version: "1.0"
last_updated: "2025-12-10"
description: "Grobplanung              E                              deutsch                   A+W Production                                        Revisionsübersicht                                        Part                    Beschreibung                                        Version / Datum                                         2.50 / 01-2023          Vorgang suchen ergänzt.                                         2.01 / 01-2017          Produkt- und Firmennamen angepasst."
source_file: "DE_AWProduction_Grobplanung_2.50.pdf"
---


# DE AWProduction Grobplanung 2.50

Grobplanung              E




                         deutsch




              A+W Production
                                       Revisionsübersicht
                                       Part                    Beschreibung
                                       Version / Datum

                                       2.50 / 01-2023          Vorgang suchen ergänzt.

                                       2.01 / 01-2017          Produkt- und Firmennamen angepasst.

                                       2.00 / 07-2014          Neuerstellung Tutorial und Softwarereferenz.

                                       1.50 / 08-2013          Vollständige Überarbeitung der ALCIM-Dokumentation
                                                               und Anpassung auf A+W Production

                                       1.00 / 03-2006          Ersterstellung.



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
                                       © 2023, A+W Software GmbH, alle Rechte, auch des Nachdrucks, der Her-
                                       stellung von Kopien und der Übersetzung, bleiben vorbehalten.
                                       Die Dokumentation darf nur gemäß dem Lizenzvertrag ganz oder in Teilen ko-
                                       piert, in einem Archivierungssystem gespeichert oder in irgendeiner anderen
                                       Form übertragen werden. Ohne die vorherige schriftliche Genehmigung der
                                       A+W Software GmbH darf die Dokumentation weder elektronisch, mecha-
2.50 / 01-2023




                                       nisch, per Aufzeichnung oder in sonstiger Form übertragen werden.




                 A+W Production Grobplanung                                                                    E-3
                       Warenzeichen
                       Alle in der Dokumentation erwähnten Hard- und Softwarebezeichnungen kön-
                       nen gleichzeitig auch eingetragene Marken oder sonstige gewerbliche
                       Schutzrechte Dritter sein. Die Schutzrechte Dritter sind insoweit zu beachten.
                          Revisionsübersicht .............................................................................................. E-3
                          Editorial ............................................................................................................... E-3

                       Tutorial                                                                                                              E-7
                       Überblick ................................................................................................................. E-9
                         Dokumentation .................................................................................................. E-10
                           Aufbau des Tutorials ...................................................................................... E-10
                           Darstellungskonventionen .............................................................................. E-11
                       Grobplanung ......................................................................................................... E-12
                         Prozess der Arbeitsvorbereitung ....................................................................... E-13
                         Ansichten ........................................................................................................... E-16
                           Ansichten in der Grobplanung ....................................................................... E-17
                           Ansichten konfigurieren, arbeiten mit Ansichten ............................................ E-19
                             Register anlegen und konfigurieren ............................................................ E-19
                             Spalten anlegen und konfigurieren ............................................................. E-21
                             Summenzeile anlegen und konfigurieren ................................................... E-24
                             Neue Spalte oder Summenzeile definieren ................................................ E-26
                             Filter anlegen und konfigurieren ................................................................. E-29
                             Weißer Screen in einer Ansicht .................................................................. E-32
                           Übungen: Konfigurieren von Ansichten, Arbeiten mit Ansichten ................... E-33
                         Aufträge / Pool ................................................................................................... E-34
                           Aufträge in der Grobplanung .......................................................................... E-35
                         Töpfe ................................................................................................................. E-37
                           Töpfe in der Grobplanung .............................................................................. E-38
                         Läufe und Laufstrategien ................................................................................... E-43
                           Läufe in der Grobplanung .............................................................................. E-44
                         Positionen .......................................................................................................... E-50
                           Positionen in der Grobplanung ...................................................................... E-51
                         Vorgang suchen ................................................................................................ E-53

                       Softwarereferenz                                                                                                   E-55
                       Grobplanung ......................................................................................................... E-57
                       Aufträge in der Grobplanung ................................................................................ E-58
                         Aufträge ............................................................................................................. E-59
                         Auftragsübersicht .............................................................................................. E-62
                         Füllaufträge ....................................................................................................... E-65
                         Übermengen-Editor ........................................................................................... E-68
                         Änderung der Beschaffungsart .......................................................................... E-70
                       Töpfe in der Grobplanung ..................................................................................... E-72
                         Töpfe ................................................................................................................. E-73
                         Reservierungsaufträge-Topf .............................................................................. E-76
                         Bestellteile-Topf ................................................................................................. E-80
                         Topf-Bildung ...................................................................................................... E-83
                         Topfbezeichnung ändern ................................................................................... E-85
                       Läufe in der Grobplanung ..................................................................................... E-86
                         Läufe ................................................................................................................. E-87
                         Lauf-Bildung ...................................................................................................... E-90
2.50 / 01-2023




                         Sonderglas-Lauf bilden ..................................................................................... E-92
                         Laufbezeichnung ändern ................................................................................... E-93
                       Positionen in der Grobplanung ............................................................................. E-94
                         Positionen .......................................................................................................... E-95


                 E-4                                                                               A+W Production Grobplanung
                                         Auftrag zu Positionen hinzufügen ...................................................................... E-98
                                         Positionssplit ..................................................................................................... E-99
                                         Felddefinition ................................................................................................... E-101
                                         Export/Import Positionsansicht ........................................................................ E-103
                                       Bearbeitungen in der Grobplanung ..................................................................... E-104
                                         Bearbeitungen ................................................................................................. E-105
                                         Vorgabezeiten ändern ..................................................................................... E-108
                                       Glasarten, Details, BDE und Lose ...................................................................... E-109
                                         Glasarten ......................................................................................................... E-110
                                         Details ............................................................................................................. E-113
                                         BDE ................................................................................................................. E-117
                                         Lose ................................................................................................................. E-121
                                       Übergreifende Dialoge ........................................................................................ E-124
                                         Arbeitsplan ...................................................................................................... E-125
                                         Eigenschaften von (Register) .......................................................................... E-128
                                         Spaltendefinition .............................................................................................. E-129
                                         (Filter Name) ................................................................................................... E-130
                                         Filter-Definition ................................................................................................ E-131
                                         Dokumentenverknüpfungen ............................................................................ E-133
                                         Entschichtungsflächen .................................................................................... E-134
                                       Übergreifende Kontextmenüs ............................................................................. E-136

                                       Partindex                                                                                                      E-141
                                       Index ................................................................................................................... E-143
2.50 / 01-2023




                 A+W Production Grobplanung                                                                                                                    E-5
2.50 / 01-2023




                 E-6   A+W Production Grobplanung
Grobplanung               E

                      Tutorial




              A+W Production
                 Tutorial                                                                                  Überblick




                                       Überblick
                                       Das Tutorial zum Prozess der Grobplanung beschäftigt sich mit der Lauf-Bil-
                                       dung in A+W Production. Die Verantwortlichen aus der Arbeitsvorbereitung
                                       verschaffen sich in der Grobplanung mit verschiedenen Ansichten einen Über-
                                       blick und bilden mit verschiedenen Strategien Läufe, die eine optimale Pro-
                                       duktion ermöglichen.

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
2.50 / 01-2023




                 A+W Production Grobplanung                                                                     E-9
                 Überblick                                                                          Tutorial




                             Dokumentation
                             Für das Modul Grobplanung stehen folgende Dokumente zur Verfügung:

                             Handout                 Ausdruck des Tutorials für die Schulung

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

                             Querverweise            Am Ende jeder Lerneinheit finden Sie einen Abschnitt
                                                     mit Querverweisen, die auf ergänzende Informationen in
                                                     der Softwarereferenz und in anderen Parts hinweisen.
                                                     Damit können Sie das neu erworbene Wissen vertiefen.
2.50 / 01-2023




                 E-10                                                       A+W Production Grobplanung
                 Tutorial                                                                                      Überblick




                                       Darstellungskonventionen
                                       Einzelne Satzteile werden in besonderer Form dargestellt. Diese haben fol-
                                       gende Bedeutung:

                                       Kursiv                   sind Zeichenfolgen ausgezeichnet, die Elemente der
                                                                Software bezeichnen, z. B. der Dialog Töpfe.

                                       Fett                      sind Zeichenfolgen ausgezeichnet, die Sie über die
                                                                 Tastatur eingeben, z. B.: Geben Sie den Wert 0 ein.

                                       >                         Mit dem sogenannten Brotkrumenpfad ist der Weg
                                                                 kennzeichnet, auf dem Sie einen Dialog öffnen, z. B.
                                                                 Anzeigen > Füllaufträge > Kontextmenü – Liste >
                                                                 Auftragsübersicht.

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
2.50 / 01-2023




                 A+W Production Grobplanung                                                                        E-11
                 Grobplanung                                                                      Tutorial




                               Grobplanung
                               In diesem Tutorial erfahren Sie, welche Bereiche von A+W Production zur
                               Grobplanung gehören und wie Sie die Grobplanung durchführen.
                               Mit verschiedenen Ansichten (Ansichts-Dialoge) verschaffen Sie sich einen
                               Überblick und wenden Strategien zur Lauf-Bildung an.
2.50 / 01-2023




                 E-12                                                       A+W Production Grobplanung
                 Tutorial                                                                                        Grobplanung




                                       Prozess der Arbeitsvorbereitung

                                              ERP-System                  Aufträge / Pool




                                                                                            auflösen
                                                                            Lauf / Topf
                                                                            Status: 100




                                                                                            rücksetzen
                                                                           Feinplanung




                                                                                                         rücksetzen
                                                                            Status: 150




                                                                          Zur Produktion
                                                                           freigegeben
                                                                            Status: 200



                                                                            Produktion
                                                                            Status: 300


                                       Abb. E-1     Prozess der Arbeitsvorbereitung


                                       In der Grafik oben sehen Sie den Prozess der Arbeitsvorbereitung inklusive
                                       der Grobplanung. Die Aufträge und/oder Positionen befinden sich nach der
                                       Einlastung aus dem ERP-System im Pool, also im Dialog Aufträge. Sie ver-
                                       schaffen sich in den Übersichtsdialogen einen Überblick und wenden Strate-
                                       gien an, um Läufe zu bilden. Haben Sie Läufe gebildet, können Sie diese
                                       feinplanen (Abstellplatz-Zuordnung und Optimierung) und anschließend zur
                                       Produktion freigeben. Während des gesamten Prozesses sind die Aufträge in
                                       den Ansichten der Arbeitsvorbereitung sichtbar. Sie können also nachverfol-
                                       gen, welche Aufträge sich gerade in welchem Status befinden.
                                       Wenn Sie Läufe und Töpfe auflösen, werden diese in den Pool zurück gege-
                                       ben. Sie können Aufträge aus höheren Status rücksetzen und neu feinplanen,
                                       oder neue Läufe oder Töpfe bilden.
2.50 / 01-2023




                 A+W Production Grobplanung                                                                            E-13
                 Grobplanung                                                                                 Tutorial




                               Grobplanung und Kapazitätsplanung
                               Einige Funktionen der Grobplanung stehen in Wechselwirkung mit der Kapa-
                               zitätsplanung. Sie werden in diesem Tutorial an den entsprechenden Stellen
                               darauf hingewiesen.
                               Mit der Kapazitätsplanung haben Sie einen direkten Einstiegspunkt in die
                               Grobplanung und gelangen aus dem Produktionsmonitor heraus in den Dialog
                               Arbeitsplan. Hier können Sie unter Berücksichtigung der Ergebnisse der Ka-
                               pazitätsplanung Läufe erstellen und Auftragspositionen verwalten. Daher
                               empfehlen wir bei aktiver Kapazitätsplanung, die Schritte der Arbeitsvorberei-
                               tung aus dem Produktionsmonitor heraus zu starten.

                               Status setzen
                               Wenn Sie mit der Kapazitätsplanung arbeiten:
                               Wenn Sie den Status von Aufträgen auf produziert, versandfertig oder ausge-
                               liefert setzen, gibt die Kapazitätsplanung die Kapazitäten wieder frei. Die je-
                               weiligen Funktionen sind in der Anleitung der Kapazitätsplanung beschrieben.

                               Begriffe in der Grobplanung
                               In den Beschreibungen für die Grobplanung werden folgende Begriffe verwen-
                               det.

                               Begriff               Beschreibung

                               Aufträge/Pool         Nachdem Auftragsdaten aus dem EPR-System eingelastet
                                                     wurden, sind die Aufträge in der Ansicht Aufträge, die auch
                                                     Pool genannt wird, aufgelistet.

                               Pool_Tabellen         Die Datenbanktabellen Pool_ werden während der Einlastung
                                                     der Auftragsdaten aus dem ERP-System mit Daten gefüllt.
                                                     Pool_Tabellen beschreiben die Stückliste und den
                                                     Auftragskopf eines Produkts.

                               Stückliste            Die Stückliste zeigt die enthaltenen Elemente eines Auftrags
                                                     in einer Baumstruktur. In der Stückliste werden auch die
                                                     Abhängigkeiten der Positionen zueinander beschrieben.

                               Position              Positionen sind Teile von Aufträgen. Eine Position enthält
                                                     verschiedene Teile, z. B. Float 4 mm und Therm 4 mm. An die
                                                     Teile sind verschiedene Bearbeitungen geknüpft, z. B.
                                                     Zuschnitt oder Polieren.

                               Bearbeitung           Fertigungsverfahren, mit dem eine Position bearbeitet wird,
                                                     z. B. Polieren oder Schleifen.

                               Arbeitsgang           Arbeitsgänge bringen die Eigenschaften der Bearbeitung, z. B.
                                                     Polieren, mit den Eigenschaften des Werkstücks zusammen.
                                                     Eine Position aus der Stückliste hat z. B. die Anforderung auf
                                                     eine bestimmt Art geschliffen zu werden. Der Arbeitsgang
                                                     definiert anhand dieser Anforderung die spezielle Art des
                                                     Schleifens.
2.50 / 01-2023




                               Tab. E-1        Begriffe in der Grobplanung




                 E-14                                                              A+W Production Grobplanung
                 Tutorial                                                                                       Grobplanung




                                       Begriff               Beschreibung

                                       Freigabeteile         Explizit für die Produktion zu planende Teile. Freigabeteile
                                                             werden in den Ansichten angezeigt. Freigabeteile werden in
                                                             den Stammdaten definiert.

                                       Nicht-Freigabeteile   Implizit für die Produktion zu planende Teile. Nicht-
                                                             Freigabeteile werden in den Stammdaten definiert.

                                       Lauf                  Gruppe von Aufträgen und/oder Positionen, die zusammen
                                                             produziert werden sollen.

                                       Topf                  Speicher oder Puffer, in dem Sie Aufträge verwalten, bei
                                                             denen die weitere Vorgehensweise noch nicht geklärt ist.
                                                             Sie können z. B. Aufträge so lange in einen Topf legen, bis
                                                             genug Positionen mit der gleichen Glasart zusammen
                                                             gekommen sind. Anschließend bilden Sie aus diesem Topf
                                                             oder diesen Töpfen einen Lauf.

                                       Los                   Teil eines Laufs, der als Gruppe die gleichen Produktions-
                                                             Prozesse durchläuft. Ein Los kann zur gleichen Zeit auf der
                                                             gleichen Maschine mit dem gleichen Werkzeug gefertigt
                                                             werden.

                                       Starttermin           Termin, an dem die Produktion eines Laufs beginnt.

                                       Produktionstermin     Zusammenbautermin des Kopteils.

                                       Tab. E-1        Begriffe in der Grobplanung
2.50 / 01-2023




                 A+W Production Grobplanung                                                                             E-15
                 Grobplanung                                                                               Tutorial




                               Ansichten
                               Lernziele

                               • Was sind Ansichten?
                               • Wie werden Ansichten konfiguriert?
                               • Wie arbeiten Sie mit Ansichten?


                               Nutzen

                               • Mit Ansichten haben Sie eine Übersicht über die Aufträge und/oder Positionen.
                               • Ansichten helfen Ihnen, sich für eine Laufstrategie zu entscheiden.
                               • Mit Ansichten sehen Sie, in welchem Status sich die Aufträge oder Positionen
                                 befinden.
                               • Sie bearbeiten die Aufträge aus den Ansichten heraus, indem Sie z. B. Läufe oder
                                 Töpfe bilden.


                               Merke

                               Ansichten                  Übersichtsdialoge, in denen die Aufträge und/oder
                                                          Positionen thematisch gruppiert dargestellt werden, z. B.
                                                          nach Aufträgen, Bearbeitungen oder Töpfen.
2.50 / 01-2023




                 E-16                                                            A+W Production Grobplanung
                 Tutorial                                                                               Grobplanung




                                       Ansichten in der Grobplanung




                 Abb. E-2   Aufträge


                                       Die Übersichtsdialoge oder Ansichten in der Grobplanung sind vordefiniert,
                                       sodass Sie direkt damit arbeiten können. Sie können aus den Ansichten her-
                                       aus die Aufträge und/oder Positionen bearbeiten, indem Sie z. B. Läufe oder
                                       Töpfe erstellen. Die Steuerung der Dialoge erfolgt dabei zum größten Teil über
                                       Kontextmenüs.

                                       Konfigurierbare Bestandteile
                                       Die meisten Dialoge sind konfigurierbar, sodass Sie genau die Informationen
                                       angezeigt bekommen, die Sie für Ihre Produktion benötigen. In diesem Kapitel
                                       lernen Sie, wie Sie mit Übersichtsdialogen arbeiten und diese konfigurieren.
                                       Folgende Bestandteile der Übersichtsdialoge sind konfigurierbar:
                                       •   Register
                                       •   Spalten
                                       •   Summenzeile
                                       •   Filter
2.50 / 01-2023




                 A+W Production Grobplanung                                                                    E-17
                 Grobplanung                                                                                                 Tutorial




                                              Folgende Dialoge sind Übersichten und in der Softwarereferenz ausführlich
                                              beschrieben:


                 “Aufträge” auf            Im Dialog Aufträge haben Sie eine Übersicht über alle eingelasteten Aufträge, die noch
                 Seite E-59                nicht weiter verarbeitet wurden. Von dieser Ansicht aus können Sie die Aufträge im
                                           Prozess der Arbeitsvorbereitung weiter bearbeiten, z. B. Läufe und Töpfe bilden.

                 “Auftragsübersicht” auf Im Dialog Auftragsübersicht haben Sie eine Übersicht über Details in Aufträgen. Sie
                 Seite E-62              können die Auftragsübersicht nach Positionen, Teilen oder Bearbeitungen ordnen.
                                         Zudem können Sie Rahmen und Folien ein- oder ausblenden. Aus dem Dialog
                                         Auftragsübersicht heraus können Sie keine Läufe oder Töpfe erstellen.

                 “Füllaufträge” auf        Im Dialog Füllaufträge haben Sie eine Übersicht über alle Füllaufträge. Sie können sich
                 Seite E-65                z. B. anzeigen lassen, wie viele Positionen der Füllaufträge bereits produziert sind und
                                           wie viele noch produziert werden müssen.

                 “Töpfe” auf Seite E-73    Im Dialog Töpfe haben Sie eine Übersicht über die Töpfe in A+W Production. Sie können
                                           die Töpfe nach unterschiedlichen Kriterien sortieren und bearbeiten.

                 “Reservierungsaufträge Im Dialog Reservierungsaufträge-Topf können Sie sich Reservierungsaufträge anzeigen
                 -Topf” auf Seite E-76  lassen. Der Dialog dient lediglich als Übersicht über die eingeplanten Kapazitäten, sie
                                        können aus dem Dialog heraus keine Läufe oder Töpfe bilden.

                 “Bestellteile-Topf” auf   Im Dialog Bestellteile-Topf haben Sie eine Übersicht über Töpfe, die mit Bestellteilen
                 Seite E-80                erstellt wurden.

                 “Läufe” auf Seite E-87    Im Dialog Läufe haben Sie eine Übersicht über die erstellten Läufe.

                 “Positionen” auf          Im Dialog Positionen haben Sie eine Übersicht über die Positionen in den Aufträgen.
                 Seite E-95

                 “Bearbeitungen” auf       Im Dialog Bearbeitungen haben Sie eine Übersicht über die Bearbeitungen in den
                 Seite E-105               Aufträgen.

                 “Glasarten” auf           Mit dem Dialog Glasarten können Sie sich in einer Übersicht die enthaltenen Glasarten
                 Seite E-110               ausgewählter Aufträge bzw. Positionen anzeigen lassen und einen Lauf bilden.

                 “Details” auf             Mit dem Dialog Details können Sie sich Details zu ausgewählten Aufträgen, Positionen,
                 Seite E-113               Teilen, Läufen oder Töpfen anzeigen lassen.
                                           Sie können den Dialog Details aus jeder Ansicht in der Grobplanung öffnen, daher ist es
                                           empfehlenswert, diese Ansicht optimal zu konfigurieren.

                 “BDE” auf Seite E-117     Im Dialog BDE bekommen Sie einen Überblick über Informationen, die sich auf die
                                           Betriebsdatenerfassung beziehen.

                 “Lose” auf Seite E-121    Im Dialog Lose bekommen Sie einen Überblick über die erstellten Lose der
                                           ausgewählten Läufe.

                 “Arbeitsplan” auf         Mit dem Dialog Arbeitsplan können Sie sich aus dem Produktionsmonitor heraus einen
                 Seite E-125               Überblick verschaffen. Der Arbeitsplan zeigt die geplanten Läufe auf einer Maschine,
                                           bzw. in einer Schicht.
2.50 / 01-2023




                 E-18                                                                              A+W Production Grobplanung
                 Tutorial                                                                               Grobplanung




                                         Ansichten konfigurieren, arbeiten mit Ansichten
                                         Sie können Ansichten nach Ihren Bedürfnissen konfigurieren. Fassen Sie die
                                         jeweils wichtigsten Informationen im ersten Register des Dialogs zusammen,
                                         andere Informationen folgen dann in weiteren Registern. Lassen Sie sich in
                                         den Ansichten so viel Informationen wie nötig anzeigen und so wenig wie
                                         möglich, um die Dialoge übersichtlich zu halten. Fügen Sie Summenzeilen
                                         ein, um einen schnellen Überblick zu bekommen. Nutzen Sie Filter für spezi-
                                         elle Anwendungsfälle.

                                         Register anlegen und konfigurieren
                                         Zum Einfügen und Konfigurieren von Registern finden Sie folgende Hand-
                                         lungsanweisungen:
                                         •   “So fügen Sie ein Register ein” auf Seite E-19
                                         •   “So konfigurieren Sie ein Register” auf Seite E-20


                                          So fügen Sie ein Register ein
                                         1 Öffnen Sie die Ansicht, in der Sie ein Register einfügen möchten, z. B.
                                           Anzeigen > Aufträge.
                                         2 Öffnen Sie das Kontextmenü des Registers, nach dem Sie ein neues Re-
                                           gister einfügen möchten.
                                             Oder öffnen Sie das Kontextmenü im Kopfteil des Dialogs, falls noch kein
                                             Register existiert.




                 Abb. E-3   Aufträge – Kontextmenü Register
2.50 / 01-2023




                 A+W Production Grobplanung                                                                     E-19
                 Grobplanung                                                                       Tutorial




                               3 Klicken Sie im Kontextmenü auf Einfügen.




                                  Abb. E-4     Eigenschaften von (Register)


                                  Der Dialog Eigenschaften von (Register) wird geöffnet, in dem Sie dem Re-
                                  gister einen Registertext und eine Beschreibung geben. Mit der Checkbox
                                  Systemweite Anzeige legen Sie fest, ob das Register für alle Anwender
                                  oder nur für Sie angezeigt wird.
                                  Das neue Register wird nach dem Register eingefügt, dessen Kontextme-
                                  nü Sie geöffnet haben. Sie können ein Register verschieben, indem Sie es
                                  mit dem Mauszeiger an die gewünschte Stelle ziehen.


                                So konfigurieren Sie ein Register
                               1 Öffnen Sie die Ansicht, die Sie konfigurieren möchten, z. B. Anzeigen >
                                 Aufträge.
                               2 Öffnen Sie das Kontextmenü des Registers, das Sie bearbeiten möchten.
                               3 Sie haben folgende Möglichkeiten:
                                  •   Klicken Sie auf Speicherautomatik, damit alle Änderungen am jeweili-
                                      gen Register automatisch gespeichert werden.
                                      Wenn Sie die Funktion Speicherautomatik nicht wählen, müssen Sie
                                      nach jeder Änderung am Register auf Speichern klicken, damit die Än-
                                      derungen übernommen werden.




                                  Abb. E-5     Aufträge – Aktivierte Speicherautomatik


                                      Die Raute an der Bezeichnung des Registers zeigt, dass die Speicher-
                                      automatik aktiviert ist.
                                  •   Klicken Sie im Kontextmenü des Registers auf Eigenschaften, um die
2.50 / 01-2023




                                      Eigenschaften eines Registers zu bearbeiten.




                 E-20                                                          A+W Production Grobplanung
                 Tutorial                                                                                 Grobplanung




                                                 Der Dialog Eigenschaften von (Register) wird geöffnet, in dem Sie den
                                                 Registertext und die Beschreibung bearbeiten. Mit der Checkbox Sys-
                                                 temweite Anzeige legen Sie fest, ob das Register für alle Anwender
                                                 oder nur für Sie angezeigt wird.
                                             •   Sie können das konfigurierte Register importieren oder exportieren und
                                                 somit als Schablonen für andere Dialoge oder Anwender verwenden.

                                         Spalten anlegen und konfigurieren
                                         Zum Einfügen und Konfigurieren von Spalten finden Sie folgende Handlungs-
                                         anweisungen:
                                         •   “So fügen Sie eine Spalte ein” auf Seite E-21
                                         •   “So konfigurieren Sie eine Spalte” auf Seite E-22


                                          So fügen Sie eine Spalte ein
                                         1 Öffnen Sie die Ansicht, in der Sie eine Spalte einfügen möchten, z. B. An-
                                           zeigen > Aufträge.
                                         2 Öffnen Sie das Kontextmenü der Spalte, nach der Sie eine neue Spalte ein-
                                           fügen möchten.




                 Abb. E-6   Aufträge – Kontextmenü Spalte


                                         3 Klicken Sie im Kontextmenü auf Einfügen. Es stehen verschiedene Kate-
                                           gorien zur Auswahl.
                                             Die neue Spalte wird nach der Spalte eingefügt, deren Kontextmenü Sie
                                             geöffnet haben.
2.50 / 01-2023




                 A+W Production Grobplanung                                                                       E-21
                 Grobplanung                                                                         Tutorial




                                So konfigurieren Sie eine Spalte
                               1 Öffnen Sie die Ansicht, in der Sie eine Spalte konfigurieren möchten, z. B.
                                 Anzeigen > Aufträge.
                               2 Öffnen Sie das Kontextmenü der Spalte, die Sie bearbeiten möchten.
                               3 Sie haben folgende Möglichkeiten:
                                  •   Klicken Sie auf Umsortieren, um die jeweiligen Spalten in der umge-
                                      kehrten Reihenfolge zu sortieren, z. B. nach aufsteigendem oder ab-
                                      steigendem Datum.
                                  •   Klicken Sie im Kontextmenü einer Spalte auf Formatieren, um der Spal-
                                      te eine Einheit zuzuordnen, z. B. eine Angabe in Millimetern. Es stehen
                                      verschiedene Kategorien zur Auswahl.
                                  •   Klicken Sie im Kontextmenü einer Spalte auf Definition anzeigen, um
                                      Details zur Spalte anzuzeigen.




                                  Abb. E-7     Spaltendefinition


                                      Der Dialog Spaltendefinition wird geöffnet.
                                  •   Sie können eine Spalte verschieben, indem Sie sie an die gewünschte
                                      Stelle ziehen.

                                  Farben in Spalten
                                  Setzen Sie sich bitte mit dem Kundenservice der A+W Software GmbH in
                                  Verbindung, wenn Sie den Spalten in Ansichten Farben zuordnen möch-
                                  ten.
                                  Spalten in verschiedenen Farben anzuzeigen, erfordert einen Eintrag in
                                  der Datenbank.
2.50 / 01-2023




                 E-22                                                         A+W Production Grobplanung
                 Tutorial                                                                                Grobplanung




                                          So arbeiten Sie mit der Liste
                                         1 Öffnen Sie die Ansicht, mit der Sie arbeiten möchten, z. B.
                                           Anzeigen > Aufträge.
                                         2 Öffnen Sie das Kontextmenü der Liste.




                 Abb. E-8   Aufträge – Kontextmenü Liste


                                         3 Wählen Sie eine Option aus der Liste.
                                            Die Kontextmenüs sind in der Softwarereferenz beschrieben.
2.50 / 01-2023




                 A+W Production Grobplanung                                                                    E-23
                 Grobplanung                                                                              Tutorial




                                        Summenzeile anlegen und konfigurieren
                                        Zum Einfügen und Konfigurieren von Summenzeilen finden Sie folgende
                                        Handlungsanweisungen:
                                        •   “So fügen Sie eine Summenzeile ein” auf Seite E-24
                                        •   “So konfigurieren Sie eine Summenzeile” auf Seite E-25


                                         So fügen Sie eine Summenzeile ein
                                        1 Öffnen Sie die Ansicht, in der Sie eine Summenzeile einfügen möchten,
                                          z. B. Anzeigen > Aufträge.
                                        2 Öffnen Sie das Kontextmenü der Summenzeile, nach der Sie eine neue
                                          Summenzeile einfügen möchten.
                                            Oder öffnen Sie das Kontextmenü im Feld der Summenzeilen, falls noch
                                            keine Summenzeile besteht.




                 Abb. E-9   Aufträge – Kontextmenü Summenzeile
2.50 / 01-2023




                 E-24                                                                A+W Production Grobplanung
                 Tutorial                                                                             Grobplanung




                                       3 Wählen Sie ein Filter-Kriterium, z. B. Summe Stück gesamt.




                                          A



                                          A Eingefügte Summenzeile
                                          Abb. E-10    Summenzeile


                                          Die Summenzeile wird eingefügt. Jede weitere Summenzeile wird nach der
                                          Summenzeile eingefügt, deren Kontextmenü Sie geöffnet haben.


                                        So konfigurieren Sie eine Summenzeile
                                       1 Öffnen Sie die Ansicht, in der Sie eine Summenzeile konfigurieren möch-
                                         ten, z. B. Anzeigen > Aufträge.
                                       2 Öffnen Sie das Kontextmenü der Summenzeile, die Sie konfigurieren
                                         möchten.
                                       3 Sie haben folgende Möglichkeiten:
                                          •   Klicken Sie auf Formatieren, um der Summenzeile eine Einheit zuzu-
                                              ordnen, z. B. eine Angabe in Millimetern. Es stehen verschiedene Ka-
                                              tegorien zur Auswahl.
                                          •   Wählen Sie im Kontextmenü Definition anzeigen, um Einstellungen zur
                                              Summenzeile anzuzeigen.
                                          Der Dialog Spaltendefinition wird geöffnet.




                                          Abb. E-11    Spaltendefinition
2.50 / 01-2023




                 A+W Production Grobplanung                                                                  E-25
                 Grobplanung                                                                                 Tutorial




                                          Neue Spalte oder Summenzeile definieren

                                           So definieren Sie Spalten oder Summenzeilen
                                          1 Öffnen Sie die Ansicht, in der Sie eine Spalte oder eine Summenzeile de-
                                            finieren möchten, z. B. Anzeigen > Aufträge.
                                          2 Öffnen Sie das Kontextmenü einer Spalte oder Summenzeile.




                 Abb. E-12   Aufträge – Kontextmenü Spalte
2.50 / 01-2023




                 E-26                                                                 A+W Production Grobplanung
                 Tutorial                                                                            Grobplanung




                                       3 Klicken Sie im Kontextmenü auf Einfügen > Felddefinitionen > Editieren.




                                          Abb. E-13    Felddefinition


                                          Der Dialog Felddefinition wird geöffnet.
                                       4 Wählen Sie im Feld Menü-Gruppe, welcher Gruppe im Kontextmenü die
                                         Spalte oder die Summenzeile zugeordnet wird, z. B. Teile kumuliert.
                                       5 Geben Sie im Feld Menü-Eintrag einen Namen für die Spalte oder die
                                         Summenzeile ein, z. B. Fertige Teile.
                                       6 Geben Sie im Feld Spaltenüberschrift den Namen der Spalte oder die Sum-
                                         menzeile ein, mit der die Spalte oder Summenzeile im Dialog angezeigt
                                         wird, z. B. Fertige Teile_alle.
                                       7 Geben Sie in der Zeile Beschreibung eine Beschreibung für die Spalte oder
                                         die Summenzeile ein, z. B. Zeigt alle fertigen Teile an.
                                       8 Wählen Sie mit der Schaltfläche Format, das Format für die Spalte oder
                                         Summenzeile, z. B. Text.
2.50 / 01-2023




                 A+W Production Grobplanung                                                                  E-27
                 Grobplanung                                                                       Tutorial




                               9 Wählen Sie mit der Schaltfläche Auswahl öffnen einen SQL-Ausdruck, der
                                 für die Spalte oder Summenzeile hinterlegt wird.
                                  Wählen Sie den Eintrag SQL-Ausdruck, um einen eigenen SQL-Ausdruck
                                  einzugeben.




                                  Abb. E-14   Felddefinition


                               10 Wählen Sie die Anzeigeoptionen für die Spalte oder die Summenzeile,
                                  z. B. ob die Sortierung der Daten aufsteigend oder absteigend erfolgen
                                  soll.
                               11 Klicken Sie auf [Speichern], um die Änderungen zu übernehmen.
                               12 Klicken Sie auf [Schließen], um den Dialog zu schließen.
                                  Die neue Spalte oder Summenzeile Fertige Teile ist jetzt im Kontextmenü
                                  verfügbar.




                                                                            A




                                  A Neue Spalte
                                  Abb. E-15   Spalten definieren
2.50 / 01-2023




                 E-28                                                       A+W Production Grobplanung
                 Tutorial                                                                                   Grobplanung




                                          Filter anlegen und konfigurieren
                                          Zum Wählen, Einfügen, Konfigurieren und Definieren von Filtern finden Sie
                                          folgende Handlungsanweisungen:
                                          •   “So wählen Sie einen Filter” auf Seite E-29
                                          •   “So fügen Sie einen Filter ein” auf Seite E-30
                                          •   “So konfigurieren Sie Filter oder definieren neue Filter” auf Seite E-30


                                           So wählen Sie einen Filter
                                          1 Öffnen Sie die Ansicht, in der Sie einen Filter wählen möchten, z. B. Anzei-
                                            gen > Aufträge.
                                          2 Öffnen Sie das Dropdown-Menü eines Filters, um einen Filter auszuwäh-
                                            len.




                 Abb. E-16   Aufträge – Dropdown-Menü Filter


                                          3 Wählen Sie einen Filter.
                                              Damit ist die Ansicht gefiltert.
2.50 / 01-2023




                 A+W Production Grobplanung                                                                         E-29
                 Grobplanung                                                                          Tutorial




                                So fügen Sie einen Filter ein
                               1 Öffnen Sie die Ansicht, in der Sie einen Filter einfügen möchten, z. B. An-
                                 zeigen > Aufträge.
                               2 Klicken Sie auf [Filter hinzufügen], um einen Filter einzufügen.




                                  Abb. E-17    Hinzugefügter Filter


                                  Damit wurde der Filter hinzugefügt.


                                So konfigurieren Sie Filter oder definieren neue Filter
                               1 Öffnen Sie die Ansicht, in der Sie Filter konfigurieren oder definieren möch-
                                 ten, z. B. Anzeigen > Aufträge.
                               2 Öffnen Sie das Kontext-Menü des Filters, den Sie konfigurieren, oder nach
                                 dem Sie einen neuen Filter einfügen möchten.
                                  Der Dialog (Filter Name) wird geöffnet.




                                  Abb. E-18    (Filter Name)


                               3 Klicken Sie auf [Verwalten].
                                  Der Dialog Filter-Definition wird geöffnet.
2.50 / 01-2023




                                  Abb. E-19    Filter-Definition


                 E-30                                                           A+W Production Grobplanung
                 Tutorial                                                                               Grobplanung




                                       4 Wählen Sie einen Filter aus der Liste, wenn Sie konfigurieren möchten,
                                         oder wählen Sie Neuer Filter aus der Liste, wenn Sie einen Filter neu defi-
                                         nieren möchten.
                                          Wenn Sie einen bestehenden Filter konfigurieren, sind die Felder rechts im
                                          Dialog ausgefüllt und Sie nehmen Änderungen vor. Wenn Sie einen neuen
                                          Filter definieren, füllen Sie die Felder aus.
                                       5 Bearbeiten Sie im Feld Name die Bezeichnung des Filters, z. B. Nur ISO.
                                       6 Geben Sie im Feld Beschreibung eine Beschreibung des Filters ein, z. B.
                                         Zeigt nur ISO-Aufträge an.
                                       7 Geben Sie im Feld Standard-Parameter einen Standard-Wert ein, z. B. ein
                                         Standard-Datum, auf das zurückgegriffen wird, wenn die entsprechenden
                                         Datenbanktabellen oder -felder keinen Wert ermitteln.
                                       8 Wählen Sie im Feld Zulässig für Ansicht, in welchen Ansichten der Filter
                                         angezeigt wird, z. B. Pool-Ansicht, Topf-Ansicht und Lauf-Ansicht.
                                          Die Schaltflächen der gewählten Dialoge werden optisch verändert.
                                       9 Klicken Sie auf [Speichern], um die Änderungen oder den neuen Filter zu
                                         speichern.
                                          Damit haben Sie den Filter konfiguriert oder angelegt und er steht in den
                                          jeweiligen Ansichten zur Verfügung.




                                          Abb. E-20    Konfigurierter oder neuer Filter


                                          Sie können die Filter mit den Schaltflächen [Exportieren] oder [Importieren]
                                          exportieren oder importieren und somit als Schablonen für andere Dialog
                                          oder Anwender verwenden.
2.50 / 01-2023




                 A+W Production Grobplanung                                                                     E-31
                 Grobplanung                                                                            Tutorial




                               Weißer Screen in einer Ansicht
                               Wenn in einer Ansicht keine Aufträge und/oder Positionen angezeigt werden,
                               sind entweder keine vorhanden, oder Sie haben die Kriterien der Ansicht so
                               gesetzt, dass keine Aufträge oder Positionen den Kriterien entsprechen. Mög-
                               liche Gründe für eine leere Liste sind beispielsweise:
                               •   Sie haben nur eine Spalte in der Ansicht. Der Spalte ist eine Kategorie hin-
                                   terlegt, die nicht in den Aufträgen vorkommt.
                                   Z. B. zeigt die Spalte VSG an und in den Aufträgen sind keine VSG enthal-
                                   ten.
                                   Abhilfe: Hinterlegen Sie der Spalte ein Kriterium, das den Aufträgen ent-
                                   spricht.
                               •   Sie haben mehrere Spalten in der Ansicht. Die Kriterien der Spalten gren-
                                   zen die Aufträge so stark ein, dass keine mehr angezeigt werden, oder die
                                   Kriterien sind widersprüchlich.
                                   Sie haben z. B. zwei Spalten, von denen eine VSG und die andere ISO an-
                                   zeigt. Aufträge, die jeweils nur VSG oder ISO enthalten, können nicht beide
                                   Kriterien gleichzeitig erfüllen.
                                   Abhilfe: Hinterlegen Sie den Spalten Kriterien, die den Aufträgen entspre-
                                   chen.
                               •   Sie haben einen Filter aktiviert, dessen Kriterium keinem Auftrag ent-
                                   spricht.
                                   Wenn z. B. ein Filter nur ISO aktiviert ist und keine ISO in den Aufträgen
                                   enthalten sind, ist die Liste leer.
                                   Abhilfe: Entfernen Sie den Filter oder wählen Sie einen anderen.
                               •   Sie haben eine Spalte eingefügt, die z. B.auf Lauf-bezogene Informationen
                                   filtert. Sofern Sie für die angezeigten Aufträge bzw. Positionen noch keinen
                                   Lauf gebildet haben, filtert die Spalte nicht vorhandene bzw. nicht zulässige
                                   Daten und damit entsteht ein weißer Screen.
                                   Abhilfe: Fügen Sie Spalten für spätere Arbeitsprozesse in der Arbeitsvor-
                                   bereitung auch nur in Ansichten ein, die spätere Prozesse der Arbeitsvor-
                                   bereitung anzeigen, z. B. laufbezogene Daten in der Laufansicht.
2.50 / 01-2023




                 E-32                                                           A+W Production Grobplanung
                 Tutorial                                                                           Grobplanung




                                       Übungen: Konfigurieren von Ansichten, Arbeiten
                                       mit Ansichten
                                       Festigen Sie Ihr neu erworbenes Wissen mit den nachfolgenden Übungen.
                                       •   Öffnen Sie eine Ansicht der Grobplanung.
                                       •   Aktivieren Sie die Speicherautomatik.
                                       •   Überlegen Sie, welche Informationen in dieser Ansicht noch fehlen.
                                       •   Legen Sie ein entsprechendes Register an.
                                       •   Legen Sie zugehörige Spalten an.
                                       •   Fügen Sie eine Summenzeile ein.
                                       •   Fügen Sie einen Filter ein.
                                       •   Definieren Sie eine eigene Spalte und/oder Summenzeile und fügen Sie
                                           diese in der Ansicht ein.


                                       Ergänzende Informationen
                                        Softwarereferenz, “Grobplanung” auf Seite E-57
2.50 / 01-2023




                 A+W Production Grobplanung                                                                E-33
                 Grobplanung                                                                               Tutorial




                               Aufträge / Pool
                               Lernziele

                               • Wie arbeiten Sie mit der Ansicht Aufträge?


                               Nutzen

                               • In der Ansicht Aufträge haben Sie eine Übersicht über alle Aufträge, die aus dem
                                 ERP-System eingelastet wurden.
                               • Mit der Ansicht Aufträge gelangen Sie in andere Ansichten.


                               Merke

                               Aufträge                   Aufträge werden nach dem Import aus dem ERP-
                                                          System im Dialog Aufträge angezeigt.

                               Pool                       Der Dialog Aufträge wird auch Pool genannt.

                               Auftragsübersicht          Die Auftragsübersicht zeigt die Stückliste an.

                               Positionen                 Im Dialog Positionen finden Sie alle Details zu den
                                                          Positionen in Aufträgen.

                               Füllaufträge               Füllaufträge sind keinem Lauf zugeordnet und werden
                                                          von der Feinplanung dazu verwendet, den Verschnitt zu
                                                          optimieren.

                               Übermengen                 Kaufmännische und produktionstechnische
                                                          Übermengen bearbeiten Sie im Übermengen-Editor.
                                                           Softwarereferenz, “Übermengen-Editor” auf
                                                            Seite E-68

                               Beschaffungsart ändern     Im Dialog Änderung der Beschaffungsart können Sie die
                                                          Beschaffungsart von ESG und VSG ändern.
                                                           Softwarereferenz, “Änderung der Beschaffungsart”
                                                            auf Seite E-70
2.50 / 01-2023




                 E-34                                                            A+W Production Grobplanung
                 Tutorial                                                                                Grobplanung




                                        Aufträge in der Grobplanung




                 Abb. E-21   Aufträge


                                        Im Dialog Aufträge haben Sie eine Übersicht über alle eingelasteten Aufträge,
                                        die noch nicht weiter verarbeitet wurden. Von dieser Ansicht aus können Sie
                                        die Aufträge im Prozess der Arbeitsvorbereitung weiter bearbeiten, z. B. Läufe
                                        und Töpfe bilden. Der Dialog Aufträge wird auch Pool genannt.
                                        Aufgelöste Läufe und Töpfe landen automatisch wieder im Pool. Der Dialog
                                        Aufträge ist konfigurierbar.
                                        Vom Pool aus gelangen Sie zur Auftragsübersicht, in der die Stückliste ange-
                                        zeigt wird. Sie können den Übermengen-Editor öffnen, in dem Sie produkti-
                                        onstechnische und kaufmännische Übermengen bearbeiten.
                                        Zudem können Sie aus dem Pool heraus auf die Maschinenumlastung und die
                                        Maschinenzuordnung zugreifen.
                                        Der Dialog Aufträge ist dazu gedacht, Ihnen einen Überblick über in den Auf-
                                        trägen enthaltene Lieferdaten, Produkte und Bearbeitungen zu verschaffen.
                                        Halten Sie den Dialog Aufträge so einfach und übersichtlich wie möglich.
                                        Wenn Sie Aufträge verplant haben, sind diese nicht mehr im Pool sichtbar. Sie
                                        finden die verplanten Aufträge dann in den anderen Ansichten, z. B. im Dialog
2.50 / 01-2023




                                        Läufe. Legen Sie sich im Dialog Aufträge ein Register an, in dem Sie Kunden-
                                        daten finden, z. B. Liefernamen, Lieferadressen und Routen.



                 A+W Production Grobplanung                                                                     E-35
                 Grobplanung                                                                        Tutorial




                                  Maschinenumlastung, -zuordnung und Kapazitätsplanung
                                  Wenn Sie mit der Kapazitätsplanung arbeiten, müssen Sie Folgendes be-
                                  achten:
                                  Eine erneute Maschinenumlastung oder Maschinenzuordnung aus der
                                  Grobplanung heraus hat Auswirkungen auf die geplanten und berechneten
                                  Kapazitäten.
                                  Die jeweiligen Funktionen sind im Handbuch der Kapazitätsplanung be-
                                  schrieben.

                               Aufträge mit fehlerhaften Angaben
                               Bei Aufträgen mit fehlenden oder fehlerhaften Angaben können Sie entweder
                               die fehlerhaften Positionen oder den ganzen Auftrag bearbeiten. Entweder Sie
                               löschen die jeweiligen Aufträge oder Positionen, oder Sie schieben diese zu-
                               rück in den Pool.
                               Entfernen Sie die fehlerhaften Positionen aus den Läufen, um sicher zu ge-
                               hen, dass diese nicht weiter im System bleiben.
2.50 / 01-2023




                 E-36                                                       A+W Production Grobplanung
                 Tutorial                                                                                     Grobplanung




                                       Töpfe
                                       Lernziele

                                       • Was ist ein Topf?
                                       • Wie arbeiten Sie mit der Ansicht Töpfe?
                                       • Wie wird ein Topf erstellt?


                                       Nutzen

                                       • Mit Töpfen können Sie Aufträge im Überblick behalten, die nicht sofort weiter
                                         verarbeitet werden.
                                       • Mit Töpfen können Sie Puffer erstellen, in denen Sie z. B. Aufträge gleichen Typs
                                         sammeln.


                                       Merke

                                       Topf                        Ein Topf ist ein Speicher, in dem Sie Aufträge verwalten,
                                                                   bei denen das weitere Vorgehen unklar ist.

                                       Topf auflösen               Aufträge aus aufgelösten Töpfen landen wieder im Pool.
2.50 / 01-2023




                 A+W Production Grobplanung                                                                           E-37
                 Grobplanung                                                                               Tutorial




                                     Töpfe in der Grobplanung




                 Abb. E-22   Töpfe


                                     Im Dialog Töpfe haben Sie eine Übersicht über alle erstellten Töpfe in der
                                     Grobplanung. Ein Topf ist ein Speicher oder Puffer, in dem Sie Aufträge ver-
                                     walten, bei denen die weitere Vorgehensweise noch nicht geklärt ist. Das kann
                                     z. B. dann der Fall sein, wenn Sie auf Auftragsänderungen, oder auf weitere
                                     Scheiben einer teuren Glasart warten.
                                     Sie können Töpfe aus fast allen Übersichten heraus bilden oder Aufträge be-
                                     stehenden Töpfen zuordnen. Die gebildeten Töpfe landen dann im Dialog
                                     Töpfe. Von dort aus können Sie die Töpfe verwalten, indem Sie z. B. Läufe bil-
                                     den oder Töpfe auflösen. Aufträge aus aufgelösten Töpfen landen wieder im
                                     Pool.
                                     Zur Arbeit mit Töpfen finden Sie folgende Handlungsanweisungen:
                                     •   “So erstellen Sie einen Topf” auf Seite E-39
                                     •   “So fügen Sie Aufträge einem bestehenden Topf hinzu” auf Seite E-40
                                     •   “So lösen Sie einen Topf auf” auf Seite E-42
2.50 / 01-2023




                 E-38                                                              A+W Production Grobplanung
                 Tutorial                                                                                 Grobplanung




                                           So erstellen Sie einen Topf
                                          1 Öffnen Sie die Ansicht, in der Sie einen Topf erstellen möchten, z. B. An-
                                            zeigen > Aufträge.




                 Abb. E-23   Aufträge – Kontextmenü Liste


                                          2 Öffnen Sie das Kontext-Menü der Aufträge, aus denen Sie einen Topf er-
                                            stellen möchten und wählen Sie Topf bilden.
                                             Der Dialog Topf-Bildung wird geöffnet.




                                             Abb. E-24      Topf-Bildung


                                          3 Wählen Sie im Dropdown-Menü Topf-Typ, welchen Typ der Topf haben
                                            soll.
2.50 / 01-2023




                                          4 A+W Production legt im Feld Topf einen neuen Topf an. Übernehmen Sie
                                            diese Bezeichnung, oder geben Sie einen eigenen Namen ein.



                 A+W Production Grobplanung                                                                      E-39
                 Grobplanung                                                                                        Tutorial




                                          5 Wählen Sie im Kalender-Feld Produktionstermin den Produktionsstart.
                                             Beachten Sie dabei, dass ein geänderter Produktionstermin einen Einfluss
                                             auf die Kapazitätsplanung hat.
                                          6 Tragen Sie im Feld Produktionsschicht ein, in welcher Schicht mit der Pro-
                                            duktion begonnen werden soll.
                                             Beachten Sie dabei, dass eine geänderte Schicht einen Einfluss auf die
                                             Kapazitätsplanung hat.
                                          7 Wählen Sie im Feld Artikeltyp-Filter, ob für den Topf ein Artikeltyp-Filter hin-
                                            terlegt wird.
                                          8 Wählen Sie mit der Checkbox Auftrag zusammenhalten, ob der Auftrag in
                                            der Produktion zusammen gehalten werden soll.
                                          9 Klicken Sie auf [OK], um die Daten zu speichern.
                                             Der Topf wurde gebildet und ist in der Ansicht Töpfe gelistet.


                                           So fügen Sie Aufträge einem bestehenden Topf hinzu
                                          1 Öffnen Sie die Ansicht, in der Sie Aufträge einem Topf hinzufügen möch-
                                            ten, z. B. Anzeigen > Aufträge.




                 Abb. E-25   Aufträge – Kontextmenü Liste
2.50 / 01-2023




                 E-40                                                                      A+W Production Grobplanung
                 Tutorial                                                                                  Grobplanung




                                       2 Öffnen Sie das Kontext-Menü der Aufträge, die Sie einem Topf hinzufügen
                                         möchten, und wählen Sie Topf bilden.
                                          Der Dialog Topf-Bildung wird geöffnet.




                                          Abb. E-26     Topf-Bildung


                                       3 Wählen Sie im Dropdown-Menü Topf-Typ, welchen Typ der Topf haben
                                         soll.
                                       4 Wählen Sie im Feld Topf einen bestehenden Topf, um die Aufträge dem
                                         Topf hinzuzufügen.
                                       5 Wählen Sie im Kalender-Feld Produktionstermin den Produktionsstart.
                                          Beachten Sie dabei, dass ein geänderter Produktionstermin einen Einfluss
                                          auf die Kapazitätsplanung hat.
                                       6 Tragen Sie im Feld Produktionsschicht ein, in welcher Schicht mit der Pro-
                                         duktion begonnen werden soll.
                                          Beachten Sie dabei, dass eine geänderte Schicht einen Einfluss auf die
                                          Kapazitätsplanung hat.
                                       7 Wählen Sie im Feld Artikeltyp-Filter, ob für den Topf ein Artikeltyp-Filter hin-
                                         terlegt wird.
                                       8 Wählen Sie mit der Checkbox Auftrag zusammenhalten, ob der Auftrag in
                                         der Produktion zusammen gehalten werden soll.
                                       9 Klicken Sie auf [OK], um die Daten zu speichern.
                                          Die Aufträge wurden dem Topf hinzu gefügt.
2.50 / 01-2023




                 A+W Production Grobplanung                                                                        E-41
                 Grobplanung                                                                                  Tutorial




                                           So lösen Sie einen Topf auf
                                          1 Wählen Sie Stammdaten Anzeigen > Töpfe.




                 Abb. E-27   Töpfe – Kontextmenü Liste


                                          2 Öffnen Sie das Kontextmenü des Topfes oder der Töpfe, die Sie auflösen
                                            möchten und wählen Sie Topf auflösen.
                                             Die Aufträge befinden sich wieder im Pool.
2.50 / 01-2023




                 E-42                                                                     A+W Production Grobplanung
                 Tutorial                                                                                   Grobplanung




                                       Läufe und Laufstrategien
                                       Lernziele

                                       •   Was ist ein Lauf?
                                       •   Wie arbeiten Sie mit der Ansicht Läufe?
                                       •   Wie wird ein Lauf erstellt?
                                       •   Welche Strategien gibt es, um einen Lauf zu planen?


                                       Nutzen

                                       • In der Ansicht Läufe haben Sie einen Überblick über alle erstellten Läufe.
                                       • In der Ansicht Läufe sehen Sie die Status der Läufe.
                                       • In der Ansicht Läufe können Sie Läufe verwalten, indem Sie z. B. Status setzen,
                                         Läufe rücksetzen oder auflösen.
                                       • In der Ansicht Läufe können Sie Läufe an die Feinplanung übergeben.


                                       Merke

                                       Läufe                       Läufe sind eine Gruppierung von Aufträgen und/oder
                                                                   Positionen, die im Prozess der Produktionsvorbereitung
                                                                   und Produktionsfreigabe gemeinsam bearbeitet werden
                                                                   sollen.

                                                                   Auf Basis der Läufe werden die Grobplanung, die
                                                                   Feinplanung, die Optimierung und die Lauffreigabe
                                                                   durchgeführt.
2.50 / 01-2023




                 A+W Production Grobplanung                                                                            E-43
                 Grobplanung                                                                              Tutorial




                                     Läufe in der Grobplanung




                 Abb. E-28   Läufe


                                     Im Dialog Läufe haben Sie eine Übersicht über alle erstellten Läufe. Von die-
                                     ser Ansicht aus können Sie Läufe im Prozess der Arbeitsvorbereitung weiter
                                     bearbeiten, indem Sie z. B. Läufe verlinken, auflösen oder an die Feinplanung
                                     übergeben.
                                     Läufe sind eine Gruppierung von Aufträgen und/oder Positionen, die im Pro-
                                     zess der Produktionsvorbereitung und Produktionsfreigabe gemeinsam bear-
                                     beitet werden sollen. Auf Basis der Läufe werden die Feinplanung, die
                                     Optimierung und die Lauffreigabe durchgeführt.
                                     Aufgelöste Läufe landen automatisch wieder im Pool. Der Dialog Läufe ist
                                     konfigurierbar. Sie können aus dem Dialog Läufe heraus z. B. auf die Maschi-
                                     nenumlastung zugreifen.

                                        Maschinenumlastung, -zuordnung und Kapazitätsplanung
                                        Wenn Sie mit der Kapazitätsplanung arbeiten, müssen Sie Folgendes be-
                                        achten:
                                        Eine erneute Maschinenumlastung oder Maschinenzuordnung aus der
                                        Grobplanung heraus hat Auswirkungen auf die Kapazitätsplanung.
                                        Die jeweiligen Funktionen sind im Handbuch der Kapazitätsplanung be-
                                        schrieben.
2.50 / 01-2023




                 E-44                                                              A+W Production Grobplanung
                 Tutorial                                                                                Grobplanung




                                       Sinnvolle Läufe und Laufstrategien
                                       Generell gilt: Eine Laufstrategie ist dann gut, wenn sie funktioniert. Mischen
                                       Sie unterschiedliche Scheibengrößen in einen Lauf, das verbessert die Aus-
                                       beute. Isolieren Sie keine speziellen Produkte, sondern nehmen Sie die spe-
                                       ziellen Produkte mit in Läufe rein.
                                       Sie können folgende Laufstrategien verfolgen:
                                       •   Nach Glasart: Sie können separate Läufe mit dicken Gläsern bilden. Dicke
                                           Gläser haben meist größere Abmessungen und damit einen schlechteren
                                           Ertrag, somit kann es von Vorteil sein, separate Läufe zu bilden und dicke
                                           Gläser dann zu produzieren, wenn es am besten in die Produktion passt.
                                       •   Nach Produktart: Bei komplexeren Produktionen, z. B. bei ISO, ESG oder
                                           VSG, kann es von Vorteil sein, Produktarten in Läufen zusammen zu fas-
                                           sen. Damit verschaffen Sie sich einen besseren Überblick über die Produk-
                                           tion und nehmen dabei eine schlechtere Ausbeute in Kauf.
                                       •   Nach Bearbeitung: Sie können Aufträge oder Positionen bearbeitungsori-
                                           entiert zu Läufen zusammenfassen, z. B. um Rüstkosten und -zeiten zu mi-
                                           nimieren.
                                       •   Nach Produktionsdatum: Die Kapazitätsplanung weist den einzelnen Bear-
                                           beitungen Produktions-Termine zu. Diese können Sie als Basis nehmen
                                           und aus den jeweiligen Bearbeitungen mit gleichem Datum Läufe bilden.
                                       •   Nach Auftrag und/oder Position: Sie können Läufe aus Positionen oder ein-
                                           zelnen Elementen von Aufträgen bilden. Bei mehrstufigen Produktionen
                                           hilft diese Strategie, die einzelnen Abteilungen zu organisieren. Wenn Sie
                                           Freiraum für Änderungen brauchen, können Sie verschiedene Produktar-
                                           ten eines Auftrags auf mehrere Läufe verteilen.
                                       •   In mehreren Stufen planen: Dabei trennen Sie Aufträge und/oder Positio-
                                           nen nach ihren Hauptkriterien und prüfen das Ergebnis. Je nach Ausbeute,
                                           Menge, Restplatten und Anzahl der benötigten Gestelle trennen Sie die
                                           Teile dann in einzelne Läufe oder fügen Teile Läufen hinzu.
                                       •   Leerer Pool: Bei dieser Strategie packen Sie neue Aufträge und/oder Posi-
                                           tionen möglichst schnell in Töpfe oder Läufe. Der Vorteil dieser Strategie
                                           ist, dass Sie neue Aufträge und/oder Positionen sofort sehen, wenn Sie in
                                           den Pool kommen. Der Nachteil dieser Strategie ist, dass es schwieriger
                                           wird, den Überblick über bestehende Töpfe und Läufe zu behalten.
                                       •   Voller Pool: Sie lassen Aufträge und/oder Positionen möglichst lange im
                                           Pool. Der Vorteil dieser Strategie ist, dass Sie den vollen Überblick behal-
                                           ten. Der Nachteil dieser Strategie ist, dass Sie neue Aufträge und/oder Po-
                                           sitionen schwerer bemerken.

                                           Vorsicht bei Laufstrategien
                                           A+W Production lässt Ihnen die volle Freiheit bei der Planung Ihrer Produk-
                                           tion und damit die volle Verantwortung.
                                           Sie können sich z. B. über Ergebnisse der Kapazitätsplanung hinweg set-
                                           zen.
2.50 / 01-2023




                 A+W Production Grobplanung                                                                      E-45
                 Grobplanung                                                                                    Tutorial




                                          Sie sollten auf folgende Laufstrategien verzichten:
                                          •   Die morgigen kleineren Größen nutzen, um die heutige Ausbeute zu stei-
                                              gern. Diese Strategie führt zu Problemen am Folgetag.
                                          •   Zu viele Produkte oder Glasarten ohne die passende Organisation in den
                                              Läufen mischen. Diese Strategie führt zu einer unübersichtlichen Produkti-
                                              on und Staus.
                                          •   Eine zu kleine Menge an Standardgläsern.
                                          •   Läufe löschen, um Auftragsänderungen anzunehmen. Besser ist es Posi-
                                              tionen oder Läufe zurück in den Pool zu schieben.


                                          Zur Arbeit mit Läufen finden Sie folgende Handlungsanweisungen:
                                          •   “So bilden Sie einen Lauf” auf Seite E-46
                                          •   “So fügen Sie Aufträge einem bestehenden Lauf hinzu” auf Seite E-48
                                          •   “So verwalten Sie Läufe oder lösen Läufe auf” auf Seite E-49


                                           So bilden Sie einen Lauf
                                          1 Öffnen Sie die Ansicht, in der Sie einen Lauf erstellen möchten, z. B. An-
                                            zeigen > Aufträge.




                 Abb. E-29   Aufträge – Kontextmenü Liste
2.50 / 01-2023




                 E-46                                                                    A+W Production Grobplanung
                 Tutorial                                                                                  Grobplanung




                                       2 Öffnen Sie das Kontext-Menü der Aufträge, aus denen Sie einen Lauf er-
                                         stellen möchten und wählen Sie Lauf bilden.
                                          Der Dialog Lauf-Bildung wird geöffnet.




                                          Abb. E-30     Lauf-Bildung


                                       3 A+W Production legt im Feld Lauf automatisch eine neue Laufnummer an.
                                       4 Geben Sie im Feld Bezeichnung eine Bezeichnung für den Lauf ein.
                                       5 Wählen Sie im Kalender-Feld Produktionstermin den Produktionsstart.
                                          Beachten Sie dabei, dass ein geänderter Produktionstermin einen Einfluss
                                          auf die Kapazitätsplanung hat.
                                       6 Geben Sie im Feld Produktionsschicht ein, in welcher Schicht mit der Pro-
                                         duktion begonnen werden soll.
                                          Beachten Sie dabei, dass eine geänderte Schicht einen Einfluss auf die
                                          Kapazitätsplanung hat.
                                       7 Wählen Sie im Feld Artikeltyp-Filter, ob für den Lauf ein Artikeltyp-Filter hin-
                                         terlegt wird.
                                       8 Wählen Sie mit der Checkbox Auftrag zusammenhalten, ob der Auftrag in
                                         der Produktion zusammen gehalten werden soll.
                                       9 Klicken Sie auf [OK], um die Daten zu speichern.
                                          Der Lauf wurde gebildet und ist in der Ansicht Läufe gelistet.
2.50 / 01-2023




                 A+W Production Grobplanung                                                                        E-47
                 Grobplanung                                                                                 Tutorial




                                           So fügen Sie Aufträge einem bestehenden Lauf hinzu
                                          1 Öffnen Sie die Ansicht, in der Sie Aufträge einem Lauf hinzufügen möch-
                                            ten, z. B. Anzeigen > Aufträge.
                                          2 Öffnen Sie das Kontext-Menü der Aufträge, welche Sie einem Lauf hinzu-
                                            fügen möchten, und wählen Sie Lauf bilden.




                 Abb. E-31   Aufträge – Kontextmenü Liste


                                             Der Dialog Lauf-Bildung wird geöffnet.




                                             Abb. E-32      Lauf-Bildung


                                          3 Wählen Sie einen bestehenden Lauf im Dropdown-Menü um die Aufträge
2.50 / 01-2023




                                            einem Lauf hinzuzufügen.
                                          4 Geben Sie im Feld Bezeichnung eine Bezeichnung für den Lauf ein.



                 E-48                                                                 A+W Production Grobplanung
                 Tutorial                                                                                     Grobplanung




                                          5 Wählen Sie im Kalender-Feld Produktionstermin den Produktionsstart.
                                             Beachten Sie dabei, dass ein geänderter Produktionstermin einen Einfluss
                                             auf die Kapazitätsplanung hat.
                                          6 Geben Sie im Feld Produktionsschicht ein, in welcher Schicht mit der Pro-
                                            duktion begonnen werden soll.
                                             Beachten Sie dabei, dass eine geänderte Schicht einen Einfluss auf die
                                             Kapazitätsplanung hat.
                                          7 Wählen Sie im Feld Artikeltyp-Filter, ob für den Lauf ein Artikeltyp-Filter hin-
                                            terlegt wird.
                                          8 Wählen Sie mit der Checkbox Auftrag zusammenhalten, ob der Auftrag in
                                            der Produktion zusammen gehalten werden soll.
                                          9 Klicken Sie auf [OK], um die Daten zu speichern.
                                             Die Aufträge wurden dem Lauf hinzu gefügt.


                                           So verwalten Sie Läufe oder lösen Läufe auf
                                          1 Wählen Sie Anzeigen > Läufe.




                 Abb. E-33   Läufe – Kontextmenü Liste


                                          2 Öffnen Sie das Kontextmenü des Laufes oder der Läufe, die Sie bearbeiten
                                            oder auflösen möchten und wählen Sie die entsprechende Option im Kon-
                                            textmenü.
                                             Der Lauf oder die Aufträge sind nun in den entsprechenden Ansichten zu
                                             finden.
2.50 / 01-2023




                 A+W Production Grobplanung                                                                           E-49
                 Grobplanung                                                                              Tutorial




                               Positionen
                               Lernziele

                               • Was sind Positionen?
                               • Wie arbeiten Sie mit der Ansicht Positionen?


                               Nutzen

                               • In der Ansicht Positionen haben Sie einen Überblick über Positionen in Aufträgen.


                               Merke

                               Positionen                  Positionen sind Teile von Aufträgen.
2.50 / 01-2023




                 E-50                                                             A+W Production Grobplanung
                 Tutorial                                                                                  Grobplanung




                                          Positionen in der Grobplanung




                 Abb. E-34   Positionen


                                          Im Dialog Positionen haben Sie eine Übersicht über die Positionen von einge-
                                          lasteten Aufträgen. Der Dialog Positionen ist konfigurierbar. Sie können je-
                                          doch aus der Ansicht heraus keine Läufe oder Töpfe bilden.
                                          Positionen sind Teile von Aufträgen. Eine Position enthält verschiedene Teile,
                                          z. B. Float 4 mm und Therm 4 mm. An die Teile sind verschiedene Bearbeitun-
                                          gen geknüpft, z. B. Zuschnitt oder Polieren.

                                          Positionen splitten
                                          Im Dialog Positionssplit können Sie Positionen aus Aufträgen nach verschie-
                                          denen Kriterien aufteilen. Sie können die Positionen in weitere Positionen auf-
                                          teilen oder Positionen erzeugen, die eine bestimmte Anzahl von Scheiben
                                          enthalten. Außerdem können Sie die Positionen gemäß der Packmittelopti-
                                          mierung aufteilen.
2.50 / 01-2023




                 A+W Production Grobplanung                                                                        E-51
                 Grobplanung                                                                         Tutorial




                                So splitten Sie eine Position
                               1 Wählen Sie Anzeigen > Aufträge > Kontextmenü auf die markierten Aufträ-
                                 ge > Bearbeitungen > Kontextmenü > Positionen splitten.
                               2 Markieren Sie die Positionen (A), die Sie aufteilen wollen in der Liste Mar-
                                 kierte Positionen.




                                  A




                                  B




                                  A Auftragspositionen                   B Optionen
                                  Abb. E-35    Positionssplit mit gewählter Option


                               3 Wählen Sie die Option (B), mit der Sie aufteilen wollen.
                               4 Klicken Sie auf die Schaltfläche [Splitten].
                                  Die Positionen wurden aufgeteilt und stehen im Feld Neue Positionen.




                                  Abb. E-36    Positionssplit mit neuen Positionen


                               5 Klicken Sie auf die Schaltfläche [Schließen], um den Dialog zu schließen.
2.50 / 01-2023




                 E-52                                                            A+W Production Grobplanung
                 Tutorial                                                                             Grobplanung




                                       Vorgang suchen
                                       Bearbeiten > Vorgang suchen




                                       Abb. E-37   Vorgang suchen


                                       Hier haben Sie die Möglichkeit, Aufträge und/oder Angebote im System zu su-
                                       chen. Wenn Sie den Dialog öffnen, ist dieser leer. Inhalte werden erst ange-
                                       zeigt, nachdem Sie die entsprechenden Auswahlen getroffen haben und die
                                       Schaltfläche Anzeigen betätigt haben.
                                       Im ersten Schritt geben Sie im Bereich Suche nach Vorgangsart an, ob Sie
                                       nach einem Auftrag, einem Angebot oder nach beidem suchen möchten.
                                       Anschließend müssen Sie im Bereich Suchen nach … die entsprechende Vor-
                                       gangsnummer (bei Auftrag oder Angebot) oder die gewünschte Kundennum-
                                       mer eingeben.
                                       Im Bereich Anzeigen nach können Sie wählen, ob die Anzeige nach der Vor-
                                       gangsnummer und der Position oder nach Läufen sortiert werden soll.
                                       Im Bereich Anzeigen von … haben Sie eine weitere Möglichkeit, die angezeig-
                                       ten Inhalte zu untergliedern. Sie können sich z.B. über die Radiotaste Teilen
                                       noch die entsprechenden Teile-Nummern anzeigen lassen. Die Radiotaste
                                       Lauf zeigt Ihnen den gesamten Lauf an.
2.50 / 01-2023




                 A+W Production Grobplanung                                                                   E-53
                 Grobplanung                       Tutorial
2.50 / 01-2023




                 E-54          A+W Production Grobplanung
Grobplanung                  E

                Softwarereferenz




              A+W Production
                 Softwarereferenz                                                                      Grobplanung




                                       Grobplanung
                                       In der Grobplanung bilden Sie Läufe, die Sie im Prozess der Produktionsvor-
                                       bereitung anschließend feinplanen und optimieren. Die Laufgröße und -zu-
                                       sammenstellung entscheidet maßgeblich über die Optimierungsergebnisse
                                       und die Produktionsauslastung.
                                       Nach der Einlastung der Aufträge finden Sie diese im Dialog Aufträge, der
                                       auch Pool genannt wird. Von dort aus können Sie die Aufträge in Töpfen vor-
                                       sortieren oder direkt Läufe bilden. Mit den unterschiedlichen Ansichten ver-
                                       schaffen Sie sich einen Überblick über die Auftragsdaten und -details. Aus den
                                       Ansichten heraus bilden Sie Läufe und übergeben diese an den nächsten Pro-
                                       zessschritt in der Arbeitsvorbereitung: die Feinplanung.
                                       Sie können die Ansichten der Grobplanung Ihren Bedürfnissen anpassen, da-
                                       mit diese genau die Informationen anzeigen, die Sie benötigen.
2.50 / 01-2023




                 A+W Production Grobplanung                                                                    E-57
                 Aufträge in der Grobplanung                                                        Softwarereferenz




                                         Aufträge in der Grobplanung
                                         In diesem Kapitel finden Sie Informationen zu allen Dialogen, mit denen Sie
                                         sich einen Überblick zu Aufträgen bzw. Auftragsdaten verschaffen können. Sie
                                         können Füllaufträge verwalten und Übermengen bearbeiten.
2.50 / 01-2023




                 E-58                                                                 A+W Production Grobplanung
                 Softwarereferenz                                                          Aufträge in der Grobplanung




                                          Aufträge
                                          Anzeigen > Aufträge




                 Abb. E-38   Aufträge – Summen (Beispiel)


                                          Im Dialog Aufträge haben Sie eine Übersicht über alle eingelasteten Aufträge,
                                          die noch nicht weiter verarbeitet wurden. Von dieser Ansicht aus können Sie
                                          die Aufträge im Prozess der Arbeitsvorbereitung weiter bearbeiten, z. B. Läufe
                                          und Töpfe bilden und Auftragsdetails aus verschiedenen Blickrichtungen an-
                                          zeigen. Der Dialog Aufträge wird auch Pool genannt.
                                          Folgende Bestandteile des Dialogs Aufträge können Sie frei konfigurieren:
                                          •   Register
                                          •   Spalten
                                          •   Summenzeile
                                          •   Filter
                                          Die Steuerung des Dialogs erfolgt zum größten Teil über Kontextmenüs.
                                          Das Register Summen enthält z. B. folgende Spalten:
2.50 / 01-2023




                                          Liefertermin Liefertermin für den Auftrag.

                                          ESG Stk Anzahl der im Auftrag enthaltenen ESG.


                 A+W Production Grobplanung                                                                       E-59
                 Aufträge in der Grobplanung                                                            Softwarereferenz




                                         Mod Stk Anzahl der im Auftrag enthaltenen Modelle.

                                         Spr Stk Anzahl der im Auftrag enthaltenen Sprossen.

                                         Sprossen produziert Anzahl der bereits für den Auftrag produzierten Spros-
                                         sen.

                                         Sprossen bestellt Anzahl der bereits für den Auftrag bestellten Sprossen.

                                         3-fach Anzahl der im Auftrag enthaltenen 3-fach-ISO.

                                         Stufen Anzahl der im Auftrag enthaltenen Stufen-ISO.

                                               Datenbank-Informationen von Spalten
                                               Mit einem Rechtsklick auf eine Spalte und der Option Definition anzeigen
                                               öffnen Sie den Dialog Spaltendefinition. Im Dialog Spaltendefinition finden
                                               Sie die jeweiligen Datenbank-Informationen einer Spalte.

                                                “Spaltendefinition” auf Seite E-129

                                         Summenzeile

                                         Stück Endprodukt Stückzahl der markierten Endprodukte, z. B. ISO oder
                                         VSG.

                                         ISO Stk Anzahl der markierten ISO bei Mehrfachauswahl.

                                         nur Zuschnitt Summe aller Scheiben, die geschnitten werden müssen.

                                         Filter

                                         [Filter hinzufügen] Fügt einen Filter ein.

                                         Dropdown-Menü Sie haben im Dropdown-Menü des Filters folgende Optio-
                                         nen:
                                         • Klick: Öffnet das Dropdown-Menü, aus dem Sie einen Filter wählen.
                                         • Rechtsklick: Öffnet den Dialog (Filter Name). Mit der Schaltfläche Verwal-
                                            ten gelangen Sie in den Dialog Filter-Definition, in dem Sie den jeweiligen
                                            Filter bearbeiten.
                                          “Filter-Definition” auf Seite E-131

                                         Kontextmenüs
                                         In folgenden Bereichen des Dialogs Aufträge werden Kontextmenüs angebo-
                                         ten:
                                         •     Register
                                         •     Spalten
                                         •     Liste
2.50 / 01-2023




                                         •     Summenzeile
                                         •     Filter



                 E-60                                                                      A+W Production Grobplanung
                 Softwarereferenz                                                          Aufträge in der Grobplanung




                                        Kontextmenüs, die im gesamten Bereich der Arbeitsvorbereitung vorkommen,
                                        sind im Kapitel Übergreifende Kontextmenüs gelistet.
                                         “Übergreifende Kontextmenüs” auf Seite E-136


                                        Gruppe       Pfad               Bemerkung

                                        Liste        Arbeitsplan >      Öffnet den Dialog Umlastung zur
                                                     Maschinen-         Maschinenumlastung.
                                                     Umlastung
                                                                         Kapazitätsplanung: Softwarereferenz, “Ma-
                                                                          schinenumlastung” auf Seite E-175
                                                                        Die Ergebnisse der Maschinenzuordnung im
                                                                        Rahmen der Einlastung werden überschrieben.

                                                     Arbeitsplan >      Führt die Maschinenzuordnung für markierte
                                                     Maschinen-         Aufträge erneut durch.
                                                     Zuordnung
                                                                        Die Ergebnisse der Maschinenzuordnung im
                                                                        Rahmen der Einlastung werden überschrieben.

                                                     Arbeitsplan >      Zur Zeit nicht genutzt.
                                                     Arbeitsplan neu
                                                     berechnen

                                                     Beschaffungsart    Öffnet den Dialog Änderung der
                                                     ändern             Beschaffungsart.
                                                                         “Änderung der Beschaffungsart” auf
                                                                          Seite E-70
                                                                        Die Option funktioniert ausschließlich bei ESG
                                                                        und VSG.

                 Tab. E-2   Aufträge, Kontextmenüs

                                        Schaltflächen

                                        [Lauf] Bildet aus den markierten Aufträgen, Positionen oder Teilen einen
                                        Lauf.

                                        [Glasarten] Zeigt die Glasarten der markierten Aufträge an.

                                        [Details] Zeigt die Details der markierten Aufträge an.
2.50 / 01-2023




                 A+W Production Grobplanung                                                                        E-61
                 Aufträge in der Grobplanung                                                         Softwarereferenz




                                          Auftragsübersicht
                                          Anzeigen > Aufträge > Kontextmenü – Liste > Bearbeitungen > Kontextmenü
                                          – Liste > Auftragsübersicht
                                          Anzeigen > Aufträge > Kontextmenü – Liste > Glasarten > Kontextmenü – Lis-
                                          te > Auftragsübersicht
                                          Anzeigen > Aufträge > Kontextmenü – Liste > Details > Kontextmenü – Liste
                                          > Auftragsübersicht
                                          Anzeigen > Töpfe > Kontextmenü – Liste > Auftragsübersicht
                                          Anzeigen > Läufe > Kontextmenü – Liste > Auftragsübersicht
                                          Anzeigen > Füllaufträge > Kontextmenü – Liste > Auftragsübersicht




                 Abb. E-39   Auftragsübersicht, geordnet nach Bearbeitungen (Beispiel)


                                          Im Dialog Auftragsübersicht haben Sie eine Übersicht über Details in Aufträ-
                                          gen. Sie können die Auftragsübersicht nach Positionen, Teilen oder Bearbei-
                                          tungen ordnen. Zudem können Sie Rahmen und Folien ein- oder ausblenden.
                                          Aus dem Dialog Auftragsübersicht heraus können Sie keine Läufe oder Töpfe
                                          erstellen.
                                          Sie können die Register und Spalten im Dialog Auftragsübersicht nach Ihren
                                          Bedürfnissen anpassen, sodass genau die Informationen angezeigt werden,
                                          die Sie benötigen.
2.50 / 01-2023




                                          Die Steuerung des Dialogs erfolgt zum größten Teil über Kontextmenüs.




                 E-62                                                                    A+W Production Grobplanung
                 Softwarereferenz                                                       Aufträge in der Grobplanung




                                       [Speicherautomatik] Aktiviert automatisches Speichern.

                                       [Speichern] Speichert die aktuellen Daten.

                                       [Systemweite Anzeige] Änderungen im Dialog Auftragsübersicht werden
                                       systemweit gespeichert.
                                       Der Dialog Auftragsübersicht enthält z. B. folgende Informationen:

                                       Auftrag Auftrag, zu dem Details angezeigt werden.

                                       [Positionen] Ordnet die Ansicht nach Positionen.

                                       [Teile] Ordnet die Ansicht nach Teilen.

                                       [Bearbeitungen] Ordnet die Ansicht nach Bearbeitungen.

                                       Rahmen, Folien anzeigen Checkbox mit folgenden Funktionen:
                                        Bearbeitungen, die Rahmen und Folien enthalten, werden nicht angezeigt.
                                        Bearbeitungen, die Rahmen und Folien enthalten, werden angezeigt.

                                       Position Positionsnummer der Auftragsposition.

                                       Name Artikel oder Auftragsposition.

                                       Größe Größe der Scheiben.

                                       Stückzahl Stückzahl der Artikel.

                                       Maschine Maschine, auf der die Bearbeitung durchgeführt wird.

                                       Prod.-Termin Datum, an dem die Bearbeitung durchgeführt wird.

                                       Prod. Stückzahl Zahl der bereits produzierten Scheiben.

                                       Lauf Lauf, dem die Bearbeitung zugeordnet wurde.

                                       Beschaffungsart Beschaffungsart, die dem Artikel zugeordnet wurde.

                                       Modellnummer Modellnummer der Scheibe.

                                       Bearbeitungstext Anmerkungen zur Bearbeitung.

                                          Datenbank-Informationen von Spalten
                                          Mit einem Rechtsklick auf eine Spalte und der Option Definition anzeigen
                                          öffnen Sie den Dialog Spaltendefinition. Im Dialog Spaltendefinition finden
                                          Sie die jeweiligen Datenbank-Informationen einer Spalte.

                                           “Spaltendefinition” auf Seite E-129
2.50 / 01-2023




                 A+W Production Grobplanung                                                                     E-63
                 Aufträge in der Grobplanung                                                                   Softwarereferenz




                                          Kontextmenüs
                                          In folgenden Bereichen des Dialogs Auftragsübersicht werden Kontextmenüs
                                          angeboten:
                                          •    Schaltflächen-Leiste
                                          •    Kopfzeile
                                          •    Spalten
                                          Kontextmenüs, die im gesamten Bereich der Arbeitsvorbereitung vorkommen,
                                          sind im Kapitel Übergreifende Kontextmenüs gelistet.
                                           “Übergreifende Kontextmenüs” auf Seite E-136


                                          Gruppe        Pfad                 Bemerkung

                                          Kopfzeile     Formatieren          Format oder Einheit für die Spalten in der
                                                                             Kopfzeile auswählen, z. B. Datumsformate oder
                                                                             Längen-Einheiten.

                                                        Einfügen             Fügt eine neue Spalte in die Kopfzeile ein.
                                                                             Verschiedene Kategorien stehen zur Verfügung.

                                                        Entfernen            Entfernt eine markierte Spalte.

                                                        Definition anzeigen Öffnet den Dialog Spaltendefinition.
                                                                              “Spaltendefinition” auf Seite E-129

                                          Spalten       Formatieren          Format oder Einheit für die Spalten in der Liste
                                                                             auswählen, z. B. Datumsformate oder Längen-
                                                                             Einheiten.

                                                        Einfügen >           Fügt eine neue Spalte mit Bearbeitungsdaten
                                                        Bearbeitungsdaten    ein. Verschiedene Kategorien stehen zur
                                                                             Verfügung.

                                                        Einfügen >           Fügt eine neue Spalte mit Stücklistendaten ein.
                                                        Stücklistendaten     Verschiedene Kategorien stehen zur Verfügung.

                                                        Entfernen            Löscht eine markierte Spalte.

                                                        Definition anzeigen Öffnet den Dialog Spaltendefinition, in dem
                                                                            Details zur jeweiligen Spalte angezeigt werden.
                                                                              “Spaltendefinition” auf Seite E-129

                 Tab. E-3    Auftragsübersicht, Kontextmenüs
2.50 / 01-2023




                 E-64                                                                        A+W Production Grobplanung
                 Softwarereferenz                                                           Aufträge in der Grobplanung




                                           Füllaufträge
                                           Anzeigen > Füllaufträge




                 Abb. E-40   Füllaufträge (Beispiel)


                                           Im Dialog Füllaufträge haben Sie eine Übersicht über alle Füllaufträge. Sie
                                           können sich z. B. anzeigen lassen, wie viele Positionen der Füllaufträge be-
                                           reits produziert sind und wie viele noch produziert werden müssen.
                                           Folgende Bestandteile des Dialogs Füllaufträge können Sie frei konfigurieren:
                                           •   Register
                                           •   Spalten
                                           •   Summenzeile
                                           •   Filter
                                           Die Steuerung des Dialogs erfolgt zum größten Teil über Kontextmenüs.
                                           Der Dialog Füllaufträge enthält z. B. folgende Spalten:

                                           Auftrag Auftragsnummer des jeweiligen Auftrags.

                                           Pos (int Pos) Interne A+W Production Sub-Position, die z. B. nach einem
                                           Positionssplit vergeben wurde.
2.50 / 01-2023




                                           Artikelbezeichnung Bezeichnung des im Auftrag enthaltenen Artikels.

                                           Produzierte Menge Anzahl der bereits produzierten Positionen des jeweili-
                                           gen Auftrags.


                 A+W Production Grobplanung                                                                       E-65
                 Aufträge in der Grobplanung                                                            Softwarereferenz




                                               Datenbank-Informationen von Spalten
                                               Mit einem Rechtsklick auf eine Spalte und der Option Definition anzeigen
                                               öffnen Sie den Dialog Spaltendefinition. Im Dialog Spaltendefinition finden
                                               Sie die jeweiligen Datenbank-Informationen einer Spalte.

                                                “Spaltendefinition” auf Seite E-129

                                         Summenzeile

                                         Stück Endprodukt Anzahl der markierten Endprodukte, z. B. ISO oder VSG.

                                         ISO Stk Anzahl der markierten ISO.

                                         nur Zuschnitt Anzahl der markierten Scheiben, die geschnitten werden müs-
                                         sen.

                                         Filter

                                         [Filter hinzufügen] Fügt einen Filter ein.

                                         Dropdown-Menü Sie haben im Dropdown-Menü des Filters folgende Optio-
                                         nen:
                                         • Klick: Öffnet das Dropdown-Menü, aus dem Sie einen Filter wählen.
                                         • Rechtsklick: Öffnet den Dialog (Filter Name). Mit der Schaltfläche Verwal-
                                            ten gelangen Sie in den Dialog Filter-Definition, in dem Sie den jeweiligen
                                            Filter bearbeiten.
                                          “Filter-Definition” auf Seite E-131

                                         Kontextmenüs
                                         In folgenden Bereichen des Dialogs Füllaufträge werden Kontextmenüs ange-
                                         boten:
                                         •     Register
                                         •     Spalten
                                         •     Liste
                                         •     Summenzeile
                                         •     Filter
                                         Kontextmenüs, die im gesamten Bereich der Arbeitsvorbereitung vorkommen,
                                         sind im Kapitel Übergreifende Kontextmenüs gelistet.
                                          “Übergreifende Kontextmenüs” auf Seite E-136
2.50 / 01-2023




                 E-66                                                                      A+W Production Grobplanung
                 Softwarereferenz                                                              Aufträge in der Grobplanung




                                         Gruppe          Pfad               Bemerkung

                                         Liste           Arbeitsplan >      Öffnet den Dialog Umlastung zur
                                                         Maschinen-Umlas-   Maschinenumlastung.
                                                         tung
                                                                             Kapazitätsplanung: Softwarereferenz, “Ma-
                                                                              schinenumlastung” auf Seite E-175
                                                                            Die Ergebnisse der Maschinenzuordnung im
                                                                            Rahmen der Einlastung werden überschrieben.

                                                         Arbeitsplan >      Führt die Maschinenzuordnung für markierte
                                                         Maschinen-         Aufträge bzw. Positionen erneut durch.
                                                         Zuordnung
                                                                            Die Ergebnisse der Maschinenzuordnung im
                                                                            Rahmen der Einlastung werden überschrieben.

                                                         Arbeitsplan >      Zur Zeit nicht genutzt.
                                                         Arbeitsplan neu
                                                         berechnen

                                                         Beschaffungsart    Öffnet den Dialog Änderung der
                                                         ändern             Beschaffungsart.
                                                                             “Änderung der Beschaffungsart” auf
                                                                              Seite E-70
                                                                            Die Option funktioniert ausschließlich bei ESG
                                                                            und VSG.

                 Tab. E-4   Füllaufträge, Kontextmenüs

                                         Schaltflächen

                                         [Lauf] Bildet aus den markierten Aufträgen, Positionen oder Teilen einen
                                         Lauf.

                                         [Glasarten] Zeigt die Glasarten der markierten Aufträge an.

                                         [Details] Zeigt die Details der markierten Aufträge an.
2.50 / 01-2023




                 A+W Production Grobplanung                                                                            E-67
                 Aufträge in der Grobplanung                                                    Softwarereferenz




                                         Übermengen-Editor
                                         Anzeigen > Aufträge > Kontextmenü – Liste > Nacherfassung > Übermengen




                 Abb. E-41   Übermengen-Editor


                                         Im Dialog Übermengen-Editor können Sie kaufmännische und produktions-
                                         technische Übermengen in Aufträgen bearbeiten.

                                         Auftragspositionen

                                         Auftrag Nummer des Auftrags.

                                         Pos Anzahl der im Auftrag enthaltenen Positionen.

                                         Produkt Produktbezeichnung aus den Produktstammdaten.

                                         Menge laut Auftrag Menge, die in der Bestellung angegeben wurde.

                                         Übermenge Kaufmännische Übermenge, die Sie ändern können.
2.50 / 01-2023




                                         Mehrmenge Produktionstechnische Mehrmenge, die Sie ändern können.




                 E-68                                                                A+W Production Grobplanung
                 Softwarereferenz                                                   Aufträge in der Grobplanung




                                       Gesamtmenge Gesamtmenge der Positionen, nachdem Sie die Übermen-
                                       gen und Mehrmengen geändert haben.

                                       Übersicht
                                       Anzeige des Scheibenaufbaus.

                                       Modell
                                       Anzeige der Form des markierten Produkts.

                                       Schaltflächen

                                       [Speichern] Speichert die Daten.

                                       [Beenden] Schließt den Dialog, ohne die Daten zu speichern.
2.50 / 01-2023




                 A+W Production Grobplanung                                                              E-69
                 Aufträge in der Grobplanung                                                          Softwarereferenz




                                          Änderung der Beschaffungsart
                                          Anzeigen > Aufträge > Kontextmenü – Liste > Beschaffungsart ändern
                                          Anzeigen > Füllauftr. > Kontextmenü – Liste > Beschaffungsart ändern




                 Abb. E-42   Änderung der Beschaffungsart


                                          Im Dialog Änderung der Beschaffungsart können Sie die Beschaffungsart von
                                          ESG und VSG ändern.

                                          Änderbare Teile

                                          Liste der Teile, deren Beschaffungsart Sie ändern können.

                                          Details

                                          Auftragsnummer Auftragsnummer des markierten Teils.

                                          Positionsnummer Positionsnummer des markierten Teils.
2.50 / 01-2023




                                          Artikelbezeichnung Bezeichnung des markierten Teils.

                                          Stück Anzahl der enthaltenen Teile.


                 E-70                                                                  A+W Production Grobplanung
                 Softwarereferenz                                                    Aufträge in der Grobplanung




                                       Produktionsdatum Produktionsbeginn der Teile.

                                       Aktuelle Beschaffungsart Aktuell definierte Beschaffungsart.

                                       Aufbau Enthaltene Scheiben, für die Sie die Beschaffungsart ändern kön-
                                       nen.

                                       [Pfeil nach unten] Bewegt markierte Teile ins Feld Ausgewählte Teile.

                                       [Pfeil nach oben] Bewegt markierte Teile zurück ins Feld Änderbare Teile.

                                       Ausgewählte Teile
                                       Liste der ausgewählten Teile.

                                       Auswahl der neuen Beschaffungsart
                                       Auswahl der neuen Beschaffungsart, Sie wählen zwischen Zuschnitt, Produk-
                                       tion, Bestellung oder Lagerentnahme.

                                       [Ausführen] Führt die Änderung der Beschaffungsart durch.

                                       [Schließen] Schließt den Dialog, ohne die Daten zu speichern.
2.50 / 01-2023




                 A+W Production Grobplanung                                                                    E-71
                 Töpfe in der Grobplanung                                                         Softwarereferenz




                                        Töpfe in der Grobplanung
                                        In diesem Kapitel finden Sie Informationen zu allen Dialogen, mit denen Sie
                                        sich zu Töpfen einen Überblick verschaffen. Sie können Töpfe bilden und be-
                                        arbeiten und Reservierungsaufträge verwalten.
2.50 / 01-2023




                 E-72                                                                A+W Production Grobplanung
                 Softwarereferenz                                                               Töpfe in der Grobplanung




                                           Töpfe
                                           Anzeigen > Töpfe




                 Abb. E-43   Töpfe – Töpfe (Beispiel)


                                           Im Dialog Töpfe haben Sie eine Übersicht über die Töpfe in A+W Production.
                                           Sie können die Töpfe nach unterschiedlichen Kriterien sortieren und bearbei-
                                           ten.
                                           Folgende Bestandteile des Dialogs Töpfe können Sie frei konfigurieren:
                                           •   Register
                                           •   Spalten
                                           •   Summenzeile
                                           •   Filter
                                           Die Steuerung des Dialogs erfolgt zum größten Teil über Kontextmenüs.
                                           Das Register Töpfe enthält z. B. folgende Spalten:

                                           Topf Bezeichnung des Topfs.

                                           Beschreibung Beschreibung des Topfs.

                                           Aufträge Anzahl der enthaltenen Aufträge im jeweiligen Topf.

                                           Positionen Anzahl der enthaltenen Positionen im jeweiligen Topf.
2.50 / 01-2023




                                           ISO Anzahl der enthaltenen ISO im jeweiligen Topf.

                                           VSG Anzahl der enthaltenen VSG im jeweiligen Topf.


                 A+W Production Grobplanung                                                                         E-73
                 Töpfe in der Grobplanung                                                                 Softwarereferenz




                                        ESG Anzahl der enthaltenen ESG im jeweiligen Topf.

                                        Modelle Anzahl der enthaltenen Modelle im jeweiligen Topf.

                                            Datenbank-Informationen von Spalten
                                            Mit einem Rechtsklick auf eine Spalte und der Option Definition anzeigen
                                            öffnen Sie den Dialog Spaltendefinition. Im Dialog Spaltendefinition finden
                                            Sie die jeweiligen Datenbank-Informationen einer Spalte.

                                             “Spaltendefinition” auf Seite E-129

                                        Summenzeile

                                        Summe Fläche Gesamtfläche aller Positionen.

                                        Summe ISO Anzahl der enthaltenen ISO.

                                        Summe ESG Anzahl der enthaltenen ESG.

                                        Filter

                                        [Filter hinzufügen] Fügt einen Filter ein.

                                        Dropdown-Menü Sie haben im Dropdown-Menü des Filters folgende Optio-
                                        nen:
                                        • Klick: Öffnet das Dropdown-Menü, aus dem Sie einen Filter wählen.
                                        • Rechtsklick: Öffnet den Dialog (Filter Name). Mit der Schaltfläche Verwal-
                                           ten gelangen Sie in den Dialog Filter-Definition, in dem Sie den jeweiligen
                                           Filter bearbeiten.
                                         “Filter-Definition” auf Seite E-131

                                        Kontextmenüs
                                        In folgenden Bereichen des Dialogs Töpfe werden Kontextmenüs angeboten:
                                        •   Register
                                        •   Spalten
                                        •   Liste
                                        •   Summenzeile
                                        •   Filter
                                        Kontextmenüs, die im gesamten Bereich der Arbeitsvorbereitung vorkommen,
                                        sind im Kapitel Übergreifende Kontextmenüs gelistet.
                                         “Übergreifende Kontextmenüs” auf Seite E-136


                                        Gruppe        Pfad                  Bemerkung

                                        Liste         Topf auflösen         Löst die markierten Töpfe auf und schiebt die
                                                                            enthaltenen Aufträge zurück in den Dialog
2.50 / 01-2023




                                                                            Aufträge.

                 Tab. E-5   Töpfe, Kontextmenüs



                 E-74                                                                      A+W Production Grobplanung
                 Softwarereferenz                                                         Töpfe in der Grobplanung




                                       Schaltflächen

                                       [Lauf] Bildet aus den markierten Aufträgen, Positionen oder Teilen einen
                                       Lauf.

                                       [Glasarten] Zeigt die Glasarten der markierten Töpfe an.

                                       [Details] Zeigt die Details der markierten Töpfe an.
2.50 / 01-2023




                 A+W Production Grobplanung                                                                  E-75
                 Töpfe in der Grobplanung                                                              Softwarereferenz




                                          Reservierungsaufträge-Topf
                                          Anzeigen > Reservierungsaufträge-Topf




                 Abb. E-44   Reservierungsaufträge-Topf (Beispiel)


                                          Im Dialog Reservierungsaufträge-Topf können Sie sich Reservierungsaufträ-
                                          ge anzeigen lassen. Der Dialog dient lediglich als Übersicht über die einge-
                                          planten Kapazitäten, sie können aus dem Dialog heraus keine Läufe oder
                                          Töpfe bilden.
                                          Der Dialog Reservierungsaufträge-Topf ist in A+W Production nicht standard-
                                          mäßig freigeschaltet, Sie müssen die Ansicht des Dialogs zuerst aktivieren.
                                          Sie können die Register und Spalten im Dialog Reservierungsaufträge-Topf
                                          nach Ihren Bedürfnissen anpassen, sodass genau die Informationen ange-
                                          zeigt werden, die Sie benötigen.
                                          Der Dialog Reservierungsaufträge-Topf enthält z. B. folgende Spalten:

                                          Auftragsnummer Angabe der Auftragsnummer.

                                          Laufnummer Angabe der Laufnummer.

                                          Liefertermin Angabe des Liefertermins.

                                              Datenbank-Informationen von Spalten
                                              Mit einem Rechtsklick auf eine Spalte und der Option Definition anzeigen
                                              öffnen Sie den Dialog Spaltendefinition. Im Dialog Spaltendefinition finden
                                              Sie die jeweiligen Datenbank-Informationen einer Spalte.
2.50 / 01-2023




                                               “Spaltendefinition” auf Seite E-129




                 E-76                                                                     A+W Production Grobplanung
                 Softwarereferenz                                                                 Töpfe in der Grobplanung




                                         Summenzeile

                                         Stück Anzahl der Positionen, der im Dialog angezeigten Aufträge.

                                         Filter

                                         [Filter hinzufügen] Fügt einen Filter ein.

                                         Dropdown-Menü Sie haben im Dropdown-Menü des Filters folgende Optio-
                                         nen:
                                         • Klick: Öffnet das Dropdown-Menü, aus dem Sie einen Filter wählen.
                                         • Rechtsklick: Öffnet den Dialog (Filter Name). Mit der Schaltfläche Verwal-
                                            ten gelangen Sie in den Dialog Filter-Definition, in dem Sie den jeweiligen
                                            Filter bearbeiten.
                                          “Filter-Definition” auf Seite E-131

                                         Kontextmenüs
                                         In folgenden Bereichen des Dialogs Glasarten werden Kontextmenüs angebo-
                                         ten:
                                         •   Spalten
                                         •   Liste
                                         •   Summenzeile
                                         •   Filter
                                         Kontextmenüs, die im gesamten Bereich der Arbeitsvorbereitung vorkommen,
                                         sind im Kapitel Übergreifende Kontextmenüs gelistet.
                                          “Übergreifende Kontextmenüs” auf Seite E-136


                                         Gruppe        Pfad                  Bemerkung

                                         Spalten       Umsortieren           Spalte aufsteigend oder absteigend sortieren.
                                                                             Wirkt sich auf die ersten drei Spalten im Dialog
                                                                             aus.

                                                       Formatieren           Format oder Einheit für die Spalten auswählen,
                                                                             z. B. Datumsformate oder Längen-Einheiten.

                                                       Einfügen              Fügt eine neue Spalte ein. Verschiedene
                                                                             Kategorien stehen zur Verfügung.

                                                       Einfügen >            Öffnet den Dialog Felddefinition, in dem Sie
                                                       Felddefinitionen >    Abfragen auf Datenbank-Tabellen und -Felder
                                                       Editieren             formulieren können. Diese Abfragen können Sie
                                                                             dann z. B. teile-, positions- oder
                                                                             auftragsbezogen als Spalte einfügen.
                                                                              “Felddefinition” auf Seite E-101

                                                       Einfügen >            Öffnet den Dialog Importieren von
                                                       Felddefinitionen >    Felddefinitionen.
2.50 / 01-2023




                                                       Importieren

                 Tab. E-6   Reservierungsaufträge-Topf, Kontextmenüs (Abschnitt 1 von 2)




                 A+W Production Grobplanung                                                                              E-77
                 Töpfe in der Grobplanung                                                                  Softwarereferenz




                                         Gruppe       Pfad                 Bemerkung

                                                      Einfügen >           Öffnet den Dialog Exportieren von
                                                      Felddefinitionen >   Felddefinitionen, mit dem Sie Felddefinitionen
                                                      Exportieren          exportieren können.

                                                      Entfernen            Löscht die markierte Spalte.

                                                      Ändern               Derzeit nicht genutzt.

                                                      Definition anzeigen Öffnet den Dialog Spaltendefinition, in dem
                                                                          Details zur jeweiligen Spalte angezeigt werden.
                                                                            “Spaltendefinition” auf Seite E-129

                                         Liste        Auftragsübersicht    Öffnet den Dialog Auftragsübersicht.
                                                                            “Auftragsübersicht” auf Seite E-62


                                                      Positionen           Öffnet den Dialog Positionen.
                                                                            “Positionen” auf Seite E-95

                                         Summen-      Umsortieren          Zur Zeit nicht genutzt.
                                         zeile

                                                      Formatieren          Format oder Einheit für die Spalten auswählen,
                                                                           z. B. Datumsformate oder Längen-Einheiten.

                                                      Einfügen             Fügt ein neues Feld in die Summenzeile ein.
                                                                           Verschiedene Kategorien stehen zur Verfügung.

                                                      Einfügen >           Öffnet den Dialog Felddefinition, in dem Sie
                                                      Felddefinitionen >   Abfragen auf Datenbank-Tabellen und -Felder
                                                      Editieren            formulieren können. Diese Abfragen können Sie
                                                                           dann z. B. teile-, positions- oder
                                                                           auftragsbezogen einfügen.
                                                                            “Felddefinition” auf Seite E-101

                                                      Einfügen >           Öffnet den Dialog Importieren von
                                                      Felddefinitionen >   Felddefinitionen.
                                                      Importieren

                                                      Einfügen >           Öffnet den Dialog Exportieren von
                                                      Felddefinitionen >   Felddefinitionen, mit dem Sie Felddefinitionen
                                                      Exportieren          exportieren können.

                                         Filter                            Öffnet den Dialog (Filter Name). Mit der
                                                                           Schaltfläche [Verwalten] gelangen Sie zum
                                                                           Dialog Filter-Definition, in dem Sie Filter
                                                                           bearbeiten können.
                                                                            “Filter-Definition” auf Seite E-131

                 Tab. E-6   Reservierungsaufträge-Topf, Kontextmenüs (Abschnitt 2 von 2)
2.50 / 01-2023




                 E-78                                                                      A+W Production Grobplanung
                 Softwarereferenz                                            Töpfe in der Grobplanung




                                       Schaltflächen

                                       [Laufbildung] Zur Zeit nicht aktiv.

                                       [Glasarten] Zur Zeit nicht aktiv.

                                       [Details] Zur Zeit nicht aktiv.
2.50 / 01-2023




                 A+W Production Grobplanung                                                    E-79
                 Töpfe in der Grobplanung                                                                  Softwarereferenz




                                            Bestellteile-Topf
                                            Anzeigen > Bestellteile-Topf




                 Abb. E-45   Bestellteile-Topf (Beispiel)


                                            Im Dialog Bestellteile-Topf haben Sie eine Übersicht über Töpfe, die mit Be-
                                            stellteilen erstellt wurden.
                                            Sie können die Register und Spalten im Dialog Bestellteile-Topf nach Ihren Be-
                                            dürfnissen anpassen, sodass genau die Informationen angezeigt werden, die
                                            Sie benötigen.
                                            Die Steuerung des Dialogs erfolgt zum größten Teil über Kontextmenüs.
                                            Der Dialog Bestellteile-Topf enthält z. B. folgende Spalten:

                                            Auftrag Nummer des Auftrags.

                                            Artikel Nummer des Artikels.

                                            Liefertermin Termin, an dem ausgeliefert wird.

                                            Artikelbezeichnung Bezeichnung des Artikels.

                                            Liefername Name des Kunden.
2.50 / 01-2023




                 E-80                                                                      A+W Production Grobplanung
                 Softwarereferenz                                                                  Töpfe in der Grobplanung




                                              Datenbank-Informationen von Spalten
                                              Mit einem Rechtsklick auf eine Spalte und der Option Definition anzeigen
                                              öffnen Sie den Dialog Spaltendefinition. Im Dialog Spaltendefinition finden
                                              Sie die jeweiligen Datenbank-Informationen einer Spalte.

                                               “Spaltendefinition” auf Seite E-129

                                          Summenzeile

                                          Summe Stück Summe der Teile in den markierten Aufträgen bzw. Positio-
                                          nen.

                                          Dauer gesamt Gesamte Bearbeitungsdauer der markierten Aufträge bzw.
                                          Positionen. Einheit: Stunden.

                                          Filter

                                          [Filter hinzufügen] Fügt einen Filter ein.

                                          Dropdown-Menü Sie haben im Dropdown-Menü des Filters folgende Optio-
                                          nen:
                                          • Klick: Öffnet das Dropdown-Menü, aus dem Sie einen Filter wählen.
                                          • Rechtsklick: Öffnet den Dialog (Filter Name). Mit der Schaltfläche Verwal-
                                             ten gelangen Sie in den Dialog Filter-Definition, in dem Sie den jeweiligen
                                             Filter bearbeiten.
                                           “Filter-Definition” auf Seite E-131

                                          Kontextmenüs
                                          In folgenden Bereichen des Dialogs Bestellteile-Topf werden Kontextmenüs
                                          angeboten:
                                          •   Register
                                          •   Spalten
                                          •   Liste
                                          •   Summenzeile
                                          •   Filter
                                          Kontextmenüs, die im gesamten Bereich der Arbeitsvorbereitung vorkommen,
                                          sind im Kapitel Übergreifende Kontextmenüs gelistet.
                                           “Übergreifende Kontextmenüs” auf Seite E-136


                                          Gruppe        Pfad                  Bemerkung

                                          Liste         Verschieben in        Schiebt die ausgewählten Aufträge zurück in
                                                        Pool                  den Dialog Aufträge und damit in den Status vor
                                                                              der Grobplanung.
                                                                               “Aufträge” auf Seite E-59
2.50 / 01-2023




                 Tab. E-7   Bestellteiletopf, Kontextmenüs (Abschnitt 1 von 2)




                 A+W Production Grobplanung                                                                              E-81
                 Töpfe in der Grobplanung                                                                 Softwarereferenz




                                          Gruppe        Pfad                 Bemerkung

                                                        Arbeitsplan >        Führt die Maschinenzuordnung für markierte
                                                        Maschinen-           Aufträge erneut durch.
                                                        Zuordnung
                                                                             Die Ergebnisse der Maschinenzuordnung im
                                                                             Rahmen der Einlastung werden überschrieben.

                                                        Arbeitsplan >        Zur Zeit nicht aktiv.
                                                        Arbeitsplan neu
                                                        berechnen

                                                        Nachläufer-          Zur Zeit nicht aktiv.
                                                        bestellungen >
                                                        Auslösen

                                                        Nachläufer-          Zur Zeit nicht aktiv.
                                                        bestellungen >
                                                        Nicht auslösen



                 Tab. E-7   Bestellteiletopf, Kontextmenüs (Abschnitt 2 von 2)

                                          Schaltflächen

                                          [Lauf] Bildet aus den markierten Bestellteilen einen Lauf.

                                          [Glasarten] Zur Zeit nicht aktiv.

                                          [Details] Zur Zeit nicht aktiv.
2.50 / 01-2023




                 E-82                                                                         A+W Production Grobplanung
                 Softwarereferenz                                                        Töpfe in der Grobplanung




                                       Topf-Bildung
                                       Anzeigen > Aufträge > Kontextmenü – Liste > Topf bilden
                                       Anzeigen > Töpfe > Kontextmenü – Liste > Topf bilden
                                       Anzeigen > Läufe > Kontextmenü – Liste > Topf bilden
                                       Anzeigen > Füllaufträge > Kontextmenü – Liste > Topf bilden
                                       Glasarten > Kontextmenü – Liste > Topf bilden
                                       Bearbeitungen > Kontextmenü – Liste > Topf bilden
                                       Details > Kontextmenü – Liste > Topf bilden




                                       Abb. E-46   Topf-Bildung


                                       Mit dem Dialog Topf-Bildung können Sie einen Topf bilden. Dieser wird im Di-
                                       alog Töpfe angezeigt. Sie können Töpfe als Zwischenspeicher nutzen, z. B.
                                       wenn nicht genug Aufträge des gleichen Typs vorhanden sind.

                                       Topf-Typ Auswahl des Topf-Typs:
                                       • Normal
                                       • Bestellteiltopf

                                       Topf Sie können einen neuen Topf bilden oder den Auftrag einem bestehen-
                                       den Topf hinzufügen.
                                       • Wenn Sie keine Änderungen vornehmen, wird ein neuer Topf gebildet.
                                       • Wenn Sie einen Topf aus der Auswahl-Liste wählen, wird der Auftrag einem
                                          bestehenden Topf hinzugefügt.

                                       Bezeichnung Bezeichnung des Topfs.

                                       Produktionstermin Auswahl des Produktionstermins für den Lauf.
2.50 / 01-2023




                                       Produktionsschicht Angabe der Schicht, in der der Lauf gestartet werden
                                       soll.




                 A+W Production Grobplanung                                                                  E-83
                 Töpfe in der Grobplanung                                                            Softwarereferenz




                                        Artikeltyp-Filter Auswahl, für welche Teile Sie den Topf bilden. Zur Auswahl
                                        stehen: Sprossen, Folie, Rahmen oder Sonstige Nicht-Glas-Artikel.
                                        Die Teile müssen für die weitere Bearbeitung als Freigabeteile in den Artikel-
                                        stammdaten angelegt sein.

                                        Auftrag zusammenhalten Sie können die Positionen des Auftrags zusam-
                                        men halten. Das heißt, alle Positionen – also auch die, die Sie nicht explizit
                                        ausgewählt haben, werden gemeinsam durch die Produktion geführt. Damit
                                        stellen Sie sicher, dass keine Positionen des Auftrags vergessen werden.
                                         Die Positionen des Auftrags werden nicht zusammen gehalten.
                                         Die Positionen des Auftrags werden zusammen gehalten.

                                        [OK] Speichert die Daten.

                                        [Abbrechen] Schließt den Dialog, ohne die Daten zu speichern.
2.50 / 01-2023




                 E-84                                                                  A+W Production Grobplanung
                 Softwarereferenz                                                      Töpfe in der Grobplanung




                                       Topfbezeichnung ändern
                                       Anzeigen > Töpfe > Kontextmenü – Liste > Text ändern




                                       Abb. E-47   Topfbezeichnung ändern


                                       Mit dem Dialog Topfbezeichnung ändern können Sie die Bezeichnung, den
                                       Produktionstermin und die Produktionsschicht eines Topfs ändern.

                                       Topf Bezeichnung des Topfs.

                                       Bezeichnung Bezeichnung des Topfs.

                                       Produktionstermin Auswahl des Produktionsstarts für den Topf.

                                       Produktionsschicht Angabe der Schicht, in der der Topf gestartet werden
                                       soll.

                                       [OK] Speichert die Daten.

                                       [Abbrechen] Schließt den Dialog, ohne die Daten zu speichern.
2.50 / 01-2023




                 A+W Production Grobplanung                                                               E-85
                 Läufe in der Grobplanung                                                              Softwarereferenz




                                            Läufe in der Grobplanung
                                            In diesem Kapitel finden Sie Informationen zu allen Dialogen, mit denen Sie
                                            sich zu Läufen einen Überblick verschaffen. Sie können Läufe bilden und be-
                                            arbeiten, Sonderglas-Läufe bilden und Läufe freigeben, die somit für die Pro-
                                            duktion freigegeben werden.
2.50 / 01-2023




                 E-86                                                                     A+W Production Grobplanung
                 Softwarereferenz                                                               Läufe in der Grobplanung




                                           Läufe
                                           Anzeigen > Läufe




                 Abb. E-48   Läufe (Beispiel)


                                           Im Dialog Läufe haben Sie eine Übersicht über die erstellten Läufe. Läufe sind
                                           eine Gruppierung von Aufträgen bzw. Positionen, die im Prozess der Produk-
                                           tionsvorbereitung und Produktionsfreigabe gemeinsam bearbeitet werden sol-
                                           len. Auf Basis der Läufe werden die Grobplanung, die Feinplanung, die
                                           Optimierung und die Lauffreigabe durchgeführt.
                                           Sie können die Läufe nach unterschiedlichen Kriterien sortieren und bearbei-
                                           ten. Die Steuerung des Dialogs Läufe erfolgt vorrangig über Kontextmenüs.
                                           Folgende Bestandteile des Dialogs Läufe können Sie frei konfigurieren:
                                           •    Register
                                           •    Spalten
                                           •    Summenzeile
                                           •    Filter
                                           Das Register Läufe enthält z. B. folgende Spalten:

                                           Lauf Bezeichnung des Laufs.

                                           Status Status des Laufs.
2.50 / 01-2023




                                           Anzahl Anzahl der enthaltenen Aufträge im jeweiligen Lauf.



                 A+W Production Grobplanung                                                                        E-87
                 Läufe in der Grobplanung                                                                Softwarereferenz




                                            Modelle Anzahl der enthaltenen Modelle im jeweiligen Lauf.

                                            Beschreibung Beschreibung des Laufs.

                                                Datenbank-Informationen von Spalten
                                                Mit einem Rechtsklick auf eine Spalte und der Option Definition anzeigen
                                                öffnen Sie den Dialog Spaltendefinition. Im Dialog Spaltendefinition finden
                                                Sie die jeweiligen Datenbank-Informationen einer Spalte.

                                                 “Spaltendefinition” auf Seite E-129

                                            Summenzeile
                                            In der Summenzeile können Sie sich verschiedene Summen anzeigen lassen,
                                            Sie bekommen z. B. folgende Informationen angezeigt:

                                            Modelle Summe der Modelle in den Aufträgen bzw. Positionen.

                                            Dauer gesamt Gesamte Bearbeitungsdauer der markierten Aufträge bzw.
                                            Positionen. Einheit: Stunden.

                                            Summe Stück Summe der Teile in den markierten Aufträgen bzw. Positio-
                                            nen.

                                            Filter

                                            [Filter hinzufügen] Fügt einen Filter ein.

                                            Dropdown-Menü Sie haben im Dropdown-Menü des Filters folgende Optio-
                                            nen:
                                            • Klick: Öffnet das Dropdown-Menü, aus dem Sie einen Filter wählen.
                                            • Rechtsklick: Öffnet den Dialog (Filter Name). Mit der Schaltfläche Verwal-
                                               ten gelangen Sie in den Dialog Filter-Definition, in dem Sie den jeweiligen
                                               Filter bearbeiten.
                                             “Filter-Definition” auf Seite E-131

                                            Kontextmenüs
                                            In folgenden Bereichen des Dialogs Läufe werden Kontextmenüs angeboten:
                                            •   Register
                                            •   Spalten
                                            •   Liste
                                            •   Summenzeile
                                            •   Filter
                                            Kontextmenüs, die im gesamten Bereich der Arbeitsvorbereitung vorkommen,
                                            sind im Kapitel Übergreifende Kontextmenüs gelistet.
                                             “Übergreifende Kontextmenüs” auf Seite E-136
2.50 / 01-2023




                 E-88                                                                        A+W Production Grobplanung
                 Softwarereferenz                                                             Läufe in der Grobplanung




                                        Gruppe      Pfad                Bemerkung

                                        Liste       Lauf freigeben      Markierte Läufe zur Produktion freigeben.




                                                    Lauf verwalten >    Der Laufstatus wird zurückgesetzt.
                                                    Lauf rücksetzen

                                                    Lauf verwalten >    Der Lauf wird aufgelöst. Die Auftragsdaten
                                                    Lauf auflösen       gehen wieder in den Pool.

                                                    Lauf verwalten >    Der Lauf wird archiviert.
                                                    Lauf archivieren
                                                                        Die Erstellung der Archiv-Ansicht erfolgt durch
                                                                        den Service der A+W Software GmbH.

                                                    Lauf verwalten >    Öffnet den Dialog Status setzen, in dem Sie den
                                                    Status setzen       Status des Laufs wählen:
                                                                        •   in Produktion
                                                                        •   produziert
                                                                        •   versandfertig
                                                                        •   ausgeliefert

                                                    Feinplanung         Übergibt den Lauf an die Feinplanung und
                                                                        öffnet den Dialog Feinplanung für Lauf (Name)

                                                    Sprossen-Druck      Startet den Druck von Produktionspapieren für
                                                                        Sprossen.

                                                    Sprossen            Übergibt die Produktionsdaten für Sprossen an
                                                    Maschinen-          die jeweiligen Maschinen.
                                                    Ansteuerung

                                                    Maschinen-          Öffnet den Dialog Umlastung zur
                                                    Umlastung           Maschinenumlastung.
                                                                         Kapazitätsplanung: Softwarereferenz, “Ma-
                                                                          schinenumlastung” auf Seite E-175
                                                                        Die Ergebnisse der Maschinenzuordnung im
                                                                        Rahmen der Einlastung werden überschrieben.

                 Tab. E-8   Läufe, Kontextmenüs

                                        Schaltflächen

                                        [Freigabe] Gibt die markierten Läufe zur Produktion frei.

                                        [Feinplan.] Übergibt den markierten Lauf an die Feinplanung und öffnet den
                                        Dialog Feinplanung für Lauf (Name).

                                        [Glasarten] Zeigt die Glasarten der markierten Läufe an.

                                        [Details] Zeigt die Details der markierten Läufe an.
2.50 / 01-2023




                 A+W Production Grobplanung                                                                          E-89
                 Läufe in der Grobplanung                                                            Softwarereferenz




                                            Lauf-Bildung
                                            Anzeigen > Aufträge > [Lauf]
                                            Anzeigen > Töpfe > [Lauf]
                                            Anzeigen > Läufe > Kontextmenü – Liste > Lauf bilden
                                            Anzeigen > Füllaufträge > [Lauf]
                                            Glasarten > [Lauf]
                                            Bearbeitungen > [Lauf]
                                            Details > [Lauf]
                                            Lose > [Lauf]
                                            BDE > [Lauf]
                                            Sie können den Dialog Lauf-Bildung jeweils auch über das Kontextmenü öff-
                                            nen.




                                            Abb. E-49    Lauf-Bildung


                                            Mit dem Dialog Lauf-Bildung können Sie einen Lauf bilden, oder Aufträge zu
                                            einem bestehenden Lauf hinzufügen. Der Lauf erscheint dann im Dialog Läu-
                                            fe.
                                             “Läufe” auf Seite E-87

                                            Lauf Sie können einen neuen Lauf bilden, oder den Auftrag einem bestehen-
                                            den Lauf hinzufügen.
                                            • Wenn Sie keine Änderungen vornehmen, wird ein neuer Lauf gebildet.
                                            • Wenn Sie einen Lauf aus der Auswahl-Liste wählen, wird der Auftrag ei-
                                               nem bestehenden Lauf hinzugefügt.

                                            Bezeichnung Bezeichnung des Laufs.
2.50 / 01-2023




                 E-90                                                                   A+W Production Grobplanung
                 Softwarereferenz                                                          Läufe in der Grobplanung




                                       Feinplanungs-Orga Definiert, welche Abstellplatz-Organisation für die Opti-
                                       mierung des Laufs verwendet wird. Sie können diese Voreinstellung beim Ar-
                                       beitsschritt Feinplanung ändern.

                                       Ausgewählte Orga zur Standardvorgabe machen Im Feld Feinplanungs-
                                       Orga gewählte Abstellplatz-Organisation zum Standard machen.
                                        Gewählte Abstellplatz-Organisation wird nicht Standard.
                                        Gewählte Abstellplatz-Organisation wird Standard.

                                       Produktionstermin Hier wählen Sie einen Produktions-Starttermin für den
                                       Lauf.
                                       Wenn Sie mit dem A+W Capacity Planner arbeiten, können Sie hier den er-
                                       rechneten Starttermin bestätigen oder diesen bewusst ändern.

                                       Produktionsschicht Angabe, in welcher Schicht die Produktion des Laufs
                                       gestartet wird.

                                       Artikeltyp-Filter Sie können spezielle Läufe für Sprossen, ISO-Rahmen,
                                       VSG-Folie und sonstige Nicht-Glasartikel bilden. Die Läufe werden nur aus
                                       den gewählten Artikeltypen gebildet.
                                       Für diese Option müssen die Artikeltypen in den Artikelstammdaten als Frei-
                                       gabeteile definiert werden.

                                       Auftrag zusammenhalten Sie können die Positionen des Auftrags zusam-
                                       menhalten. Das heißt, alle Positionen – also auch die, die Sie nicht explizit
                                       ausgewählt haben, werden gemeinsam durch die Produktion geführt. Damit
                                       stellen Sie sicher, dass keine Positionen des Auftrags vergessen werden.
                                        Die Positionen des Auftrags werden nicht zusammen gehalten.
                                        Die Positionen des Auftrags werden zusammen gehalten.

                                       [OK] Speichert die Daten.

                                       [Abbrechen] Schließt den Dialog, ohne die Daten zu speichern.
2.50 / 01-2023




                 A+W Production Grobplanung                                                                    E-91
                 Läufe in der Grobplanung                                                            Softwarereferenz




                                            Sonderglas-Lauf bilden
                                            Glasarten > Kontextmenü – Liste > Sonderglas > Hinzufügen




                                            Abb. E-50   Sonderglas-Lauf bilden


                                            Im Dialog Sonderglas-Lauf bilden können Sie Läufe speziell für Sonderglas
                                            bilden.

                                            Sonderglas-Lauf Sie können entweder einen neuen Sonderglas-Lauf bilden
                                            oder den Auftrag einem bestehenden Sonderglas-Lauf hinzufügen.
                                            • Wenn Sie keine Änderungen vornehmen, wird ein neuer Sonderglas-Lauf
                                               gebildet.
                                            • Wenn Sie einen Sonderglas-Lauf aus der Auswahl-Liste wählen, wird der
                                               Auftrag einem bestehenden Lauf hinzugefügt.

                                            Bezeichnung Angabe der Bezeichnung des neuen Sonderglas-Laufs.

                                            Feinplanungs-Orga Auswahl der Gestelle für den Sonderglas-Lauf.

                                            Produktionstermin Auswahl des Produktionstermins für den Lauf.

                                            Produktionsschicht Angabe der Schicht, in der der Lauf gestartet werden
                                            soll.

                                            [OK] Speichert die Daten.

                                            [Abbrechen] Schließt den Dialog, ohne die Daten zu speichern.
2.50 / 01-2023




                 E-92                                                                   A+W Production Grobplanung
                 Softwarereferenz                                                      Läufe in der Grobplanung




                                       Laufbezeichnung ändern
                                       Anzeigen > Läufe > Kontextmenü – Liste > Text ändern




                                       Abb. E-51   Laufbezeichnung ändern


                                       Mit dem Dialog Laufbezeichnung ändern können Sie die Bezeichnung, den
                                       Produktionstermin und die Produktionsschicht eines Laufs ändern.

                                       Lauf Ausgewählter Lauf.

                                       Bezeichnung Bezeichnung des Laufs.

                                       Produktionstermin Auswahl des Produktionstermins für den Lauf.

                                       Produktionsschicht Auswahl der Schicht, in der der Lauf gestartet werden
                                       soll.

                                       [OK] Speichert die Daten.

                                       [Abbrechen] Schließt den Dialog, ohne die Daten zu speichern.
2.50 / 01-2023




                 A+W Production Grobplanung                                                               E-93
                 Positionen in der Grobplanung                                                      Softwarereferenz




                                         Positionen in der Grobpla-
                                         nung
                                         In diesem Kapitel finden Sie Informationen zu allen Dialogen, mit denen Sie
                                         sich zu Positionen einen Überblick verschaffen oder diese weiter bearbeiten
                                         können. Sie können Positionen überwachen, Positionen splitten und Positi-
                                         onsansichten importieren bzw. exportieren.
2.50 / 01-2023




                 E-94                                                                 A+W Production Grobplanung
                 Softwarereferenz                                                         Positionen in der Grobplanung




                                           Positionen
                                           Anzeigen > Aufträge > Kontextmenü – Liste > Positionen
                                           Anzeigen > Töpfe > Kontextmenü – Liste > Positionen
                                           Anzeigen > Läufe > Kontextmenü – Liste > Positionen
                                           Anzeigen > Füllaufträge > Kontextmenü – Liste > Positionen
                                           Glasarten > Kontextmenü – Liste > Positionen
                                           Bearbeitungen > Kontextmenü – Liste > Positionen
                                           Details > Kontextmenü – Liste > Positionen
                                           Lose > Kontextmenü – Liste > Positionen
                                           BDE > Kontextmenü – Liste > Positionen




                 A




                 B




                 C




                 A Navigation                                     C Liste
                 B Datenbankspalten
                 Abb. E-52   Positionen (Beispiel)


                                           Im Dialog Positionen haben Sie eine Übersicht über die Positionen in den Auf-
                                           trägen.
                                           Sie können die Register und Spalten im Dialog Positionen nach Ihren Bedürf-
                                           nissen anpassen, sodass genau die Informationen angezeigt werden, die Sie
                                           benötigen.
                                           Die Steuerung des Dialogs erfolgt zum größten Teil über Kontextmenüs.
                                           Der Dialog Positionen enthält z. B. folgende Informationen:
2.50 / 01-2023




                 A+W Production Grobplanung                                                                       E-95
                 Positionen in der Grobplanung                                                      Softwarereferenz




                                         Navigation
                                         Im Navigationsbereich wählen Sie, welche Details angezeigt werden sollen.

                                         Auftrag (Auftragsnummer) Auftragsnummer des gewählten Auftrags:
                                         • Pos. (Positionsnummer): Die einzelnen Positionen werden gelistet.
                                         • Teil (Teilenummer): Die einzelnen Teilenummern werden gelistet.
                                         • Geometrie: Zeigt Details zur Geometrie der Scheibe an.
                                         • Texte: Zeigt zum Auftrag hinterlegte Texte.
                                         • Bearbeitungen: Zeigt enthaltene Bearbeitungen an.

                                         Datenbankspalten

                                         Datenbankspalte Liste der zugehörigen Datenbankspalten zum Element,
                                         das Sie in der Navigation markiert haben.

                                         Wert Wert der jeweiligen Datenbankspalte.

                                         Liste
                                         In der Liste werden Details zum Element angezeigt, das Sie in der Navigation
                                         markiert haben.

                                         Freigabeteil Angabe, ob es sich um ein Freigabteil handelt.

                                         Teile-Nr Angabe der Teilenummer.

                                         Typ Angabe des Typs des Artikels bzw. des Teils.

                                         Beschaffungsart Beschaffungsart des Artikels bzw. des Teils, z. B. Zukauf.

                                         Artikel Nr. Artikelnummer des Artikels.

                                         Artikelbezeichnung Bezeichnung des Artikels.

                                         Prodtermin Produktionstermin des Kopfteils. Bei mehrteiligen Aufträgen ist
                                         das der Zusammenbautermin. Bei einteiligen Aufträgen sind Produktionster-
                                         min und Starttermin identisch.

                                         SchichtPos Angabe, ob die Schicht zur Sonnenseite oder zur Innenseite
                                         zeigt. Die Angabe gilt pro Scheibe, Sie geben z. B. bei einem ISO mehrere
                                         Scheiben in der Zeile an. Die Angabe erfolgt folgendermaßen:
                                         • 0: keine Beschichtung
                                         • 1: Sonnenseite
                                         • 2: Innenseite
2.50 / 01-2023




                 E-96                                                                 A+W Production Grobplanung
                 Softwarereferenz                                                          Positionen in der Grobplanung




                                         Struktpos Angabe, ob die Struktur zur Sonnenseite oder zur Innenseite
                                         zeigt. Die Angabe gilt pro Scheibe, Sie geben z. B. bei einem ISO mehrere
                                         Scheiben in der Zeile an. Die Angabe erfolgt folgendermaßen:
                                         • 0: keine Beschichtung
                                         • 1: Sonnenseite
                                         • 2: Innenseite

                                         Stufe Angabe, ob es sich um ein Stufen-ISO oder VSG handelt.

                                         Mod-Nr Nummer des verwendeten Modells.

                                             Datenbank-Informationen von Spalten
                                             Mit einem Rechtsklick auf eine Spalte und der Option Definition anzeigen
                                             öffnen Sie den Dialog Spaltendefinition. Im Dialog Spaltendefinition finden
                                             Sie die jeweiligen Datenbank-Informationen einer Spalte.

                                              “Spaltendefinition” auf Seite E-129

                                         Kontextmenüs
                                         In folgenden Bereichen des Dialogs Positionen werden Kontextmenüs ange-
                                         boten:
                                         •   Navigation
                                         •   Datenbankspalten
                                         •   Liste
                                         Die Kontextmenüs variieren, je nachdem, welche Elemente Sie in der Naviga-
                                         tion markiert haben.
                                         Kontextmenüs, die im gesamten Bereich der Arbeitsvorbereitung vorkommen,
                                         sind im Kapitel Übergreifende Kontextmenüs gelistet.
                                          “Übergreifende Kontextmenüs” auf Seite E-136


                                         Gruppe        Pfad                 Bemerkung

                                         Navigation    Auftrag hinzufügen   Öffnet den Dialog Auftrag zu Positionen
                                                                            hinzufügen, mit dem Sie der jeweiligen Position
                                                                            einen Auftrag hinzufügen können.


                                                       Ansicht exportieren Öffnet den Dialog Export/Import
                                                                           Positionsansicht.

                                                       Ansicht importieren Öffnet den Dialog Export/Import
                                                                           Positionsansicht.

                                         Datenbank     Einfügen > Auftrag   Fügt ein neues Feld in die Liste ein.
                                         -spalten                           Verschiedene Kategorien zu Aufträgen stehen
                                                                            zur Verfügung.

                 Tab. E-9   Positionen, Kontextmenüs (Abschnitt 1 von 2)
2.50 / 01-2023




                 A+W Production Grobplanung                                                                            E-97
                 Positionen in der Grobplanung                                                            Softwarereferenz




                                          Gruppe        Pfad                Bemerkung

                                          Liste         Einfügen >          Fügt eine neue Spalte ein. Verschiedene
                                                        Position            Kategorien stehen zur Verfügung.



                                                        Einfügen > Teile    Fügt eine neue Spalte ein. Verschiedene
                                                                            Kategorien stehen zur Verfügung.

                                                        Einfügen > Teile    Fügt eine neue Spalte ein. Verschiedene
                                                        kumuliert           Kategorien stehen zur Verfügung.
                                                                            Die kumulierte Anzeige ist die gleichzeitige
                                                                            Abfrage mehrerer Datenbank-Tabellen und -
                                                                            Felder, z. B. Summen.

                 Tab. E-9    Positionen, Kontextmenüs (Abschnitt 2 von 2)



                                          Auftrag zu Positionen hinzufügen
                                          Positionen > Navigation > Kontextmenü > Auftrag hinzufügen




                                          Abb. E-53     Auftrag zu Positionen hinzufügen


                                          Im Dialog Auftrag zu Positionen hinzufügen können Sie weitere Aufträge in die
                                          Ansicht Positionen laden.

                                          Auftragsnummer Angabe der Nummer des Auftrags, der hinzugefügt wer-
                                          den soll.

                                          Auswahl vorher löschen Checkbox mit folgenden Optionen:
                                           Die bisher angezeigten Aufträge werden vor dem Hinzufügen nicht ge-
                                          löscht.
                                           Die bisher angezeigten Aufträge werden vor dem Hinzufügen gelöscht.

                                          [OK] Speichert die Daten.

                                          [Abbrechen] Schließt den Dialog, ohne die Daten zu speichern.
2.50 / 01-2023




                 E-98                                                                      A+W Production Grobplanung
                 Softwarereferenz                                                     Positionen in der Grobplanung




                                       Positionssplit
                                       Anzeigen > Aufträge > Kontextmenü – Liste > Positionen splitten
                                       Bearbeitungen > Kontextmenü – Liste > Positionen splitten
                                       Details > Kontextmenü – Liste > Positionen splitten




                                       Abb. E-54    Positionssplit


                                       Im Dialog Positionssplit können Sie Positionen aus Aufträgen aufsplitten. Der
                                       Positionssplit kann auch für mehrere Aufträge gleichzeitig durchgeführt wer-
                                       den.

                                       Markierte Positionen
                                       In der Liste werden die Bearbeitungen angezeigt, die Sie im Dialog Bearbei-
                                       tungen ausgewählt haben.
                                        “Bearbeitungen” auf Seite E-105

                                       Auftrag Aufträge, die Sie zum Splitten ausgewählt haben.

                                       Pos. Anzahl der Positionen in den Aufträgen.

                                       UPos. Zur Zeit nicht genutzt.

                                       Menge Anzahl der Teile in den Aufträgen.

                                       Neue Positionen
                                       In der Liste werden die gesplitteten Positionen angezeigt.

                                       Auftrag Gesplittete Aufträge.

                                       Pos. Anzahl der Positionen in den Aufträgen.
2.50 / 01-2023




                                       UPos. Zur Zeit nicht genutzt.

                                       Neue Position Neue Position nach dem Split.



                 A+W Production Grobplanung                                                                    E-99
                 Positionen in der Grobplanung                                                    Softwarereferenz




                                         Menge Anzahl der Scheiben in den Aufträgen.

                                         [Entfernen] Löscht eine markierte Position.

                                         Je Position in … Positionen aufteilen Angabe, in wie viele neue Positio-
                                         nen aufgeteilt wird.

                                         Positionen mit maximal … Scheiben erzeugen Angabe, wie viele Schei-
                                         ben eine neue Position maximal enthalten darf.

                                         Je Pos. eine Pos. mit … Scheiben erzeugen Angabe, dass je Position
                                         eine neue Position mit einer bestimmten Anzahl an Scheiben erzeugt wird.

                                         Teilung gemäß PMO Ergebnis Mit diesem Optionsschalter legen Sie fest,
                                         dass die Positionen passend zur Packmitteloptimierung gesplittet werden.

                                         [Splitten] Splittet die Positionen.

                                         [Schließen] Schließt den Dialog.
2.50 / 01-2023




                 E-100                                                                 A+W Production Grobplanung
                 Softwarereferenz                                                     Positionen in der Grobplanung




                                       Felddefinition
                                       Positionen > Kontextmenü – Datenbankspalten > Einfügen > Felddefinitionen
                                       > Editieren
                                       Positionen > Kontextmenü – Datenbankspalten > Einfügen > Felddefinitionen
                                       > Editieren




                                       Abb. E-55    Felddefinition


                                       Im Dialog Felddefinition können Sie die Definitionen der jeweiligen Felder be-
                                       arbeiten.

                                       Menü-Gruppe Auswahl der Menü-Gruppe, der das Feld zugeordnet wird.

                                       Menü-Eintrag Auswahl einer Beschreibung für die gewählte Menü-Gruppe.

                                       Spaltenüberschrift Angabe des Spaltennamens. Wenn Sie keine Spalten-
                                       überschrift angeben, wird der Eintrag aus dem Feld Menü-Eintrag als Spalten-
                                       überschrift übernommen.

                                       Beschreibung Angabe der Feldbeschreibung. Wenn Sie keine Beschrei-
                                       bung angeben, wird der Eintrag aus dem Feld Menü-Eintrag als Beschreibung
                                       übernommen.

                                       Format Angabe des Format des Feldes, z. B, ob es sich um Datums-, Län-
                                       gen-, oder Flächenangaben handelt.

                                       Datenbankfeld Angabe der Datenbanktabelle und des entsprechenden Fel-
                                       des, auf das die neue Abfrage bzw. Spalte zugreift.

                                       Optionen
                                       Sie können wählen, nach welchen Kriterien die angezeigten Daten sortiert
2.50 / 01-2023




                                       werden:
                                       •   Sortierung aufsteigend: Die angezeigten Daten werden aufsteigend sor-
                                           tiert.


                 A+W Production Grobplanung                                                                   E-101
                 Positionen in der Grobplanung                                                     Softwarereferenz




                                         •   Sortierreihenfolge absteigend: Die angezeigten Daten werden absteigend
                                             sortiert.
                                         •   Kumulieren: Die angezeigten Daten werden kumuliert.

                                         Anzeigeoptionen
                                         Sie haben verschiedene Optionen, wie die Felder angezeigt werden sollen:

                                         Gleiche Inhalte in Folgezeilen ausblenden Wenn aufeinanderfolgende
                                         Felder gleiche Inhalte haben, können Sie diese in Folgezeilen ausblenden.
                                          Gleiche Inhalte werden in Folgezeilen angezeigt.
                                          Gleiche Inhalte werden in Folgezeilen ausgeblendet.

                                         Wert änderbar (nur Positionsanzeige) Angabe, ob die Werte in den jewei-
                                         ligen Feldern geändert werden können.
                                          Die Werte können nicht geändert werden.
                                          Die Werte können geändert werden.

                                         Aufklappkriterium (nur Teileanzeige) Auswahl, ob es ein Aufklappkriterium
                                         gibt.
                                          Es gibt kein Aufklappkriterium.
                                          Es gibt ein Aufklappkriterium.

                                         [Speichern] Speichert den Menüeintrag.

                                         [Löschen] Löscht den gesamten Menüeintrag.

                                         [Schließen] Schließt den Dialog.
2.50 / 01-2023




                 E-102                                                                A+W Production Grobplanung
                 Softwarereferenz                                                    Positionen in der Grobplanung




                                       Export/Import Positionsansicht
                                       Positionen > Navigation > Kontextmenü > Ansicht exportieren
                                       Positionen > Navigation > Kontextmenü > Ansicht importieren




                                       Abb. E-56    Export/Import Positionsansicht


                                       Im Dialog Export/Import Positionsansicht können Sie geänderte oder neue er-
                                       stellte Ansichten des Dialogs Positionen importieren oder exportieren. Sie
                                       wählen dabei, ob der Export bzw. Import global oder lokal durchgeführt wird.
                                        “Positionen” auf Seite E-95

                                       Ansichtentyp

                                       Nur global Speichert die neue Ansicht systemweit, für alle Anwender.

                                       Nur lokal Speichert die neue Ansicht nur für den aktuell angemeldeten An-
                                       wender.

                                       [OK] Speichert die Daten.

                                       [Abbrechen] Schließt den Dialog, ohne die Daten zu speichern.
2.50 / 01-2023




                 A+W Production Grobplanung                                                                   E-103
                 Bearbeitungen in der Grobplanung                                                  Softwarereferenz




                                        Bearbeitungen in der Grob-
                                        planung
                                        In diesem Kapitel finden Sie Informationen zu allen Dialogen, mit denen Sie
                                        sich zu Bearbeitungen einen Überblick verschaffen. Sie können Bearbeitun-
                                        gen überwachen und Vorgabezeiten ändern.
2.50 / 01-2023




                 E-104                                                               A+W Production Grobplanung
                 Softwarereferenz                                                  Bearbeitungen in der Grobplanung




                                          Bearbeitungen
                                          Anzeigen > Aufträge > Kontextmenü – Liste > Bearbeitungen
                                          Anzeigen > Töpfe > Kontextmenü – Liste > Bearbeitungen
                                          Anzeigen > Läufe > Kontextmenü – Liste > Bearbeitungen
                                          Anzeigen > Füllaufträge > Kontextmenü – Liste > Bearbeitungen
                                          Glasarten > Kontextmenü – Liste > Bearbeitungen
                                          Details > Kontextmenü – Liste > Bearbeitungen
                                          BDE > Kontextmenü – Liste > Bearbeitungen
                                          Lose > Kontextmenü – Liste > Bearbeitungen




                 Abb. E-57   Bearbeitungen (Beispiel)


                                          Im Dialog Bearbeitungen haben Sie eine Übersicht über die Bearbeitungen in
                                          den Aufträgen.
                                          Sie können die Register und Spalten im Dialog Bearbeitungen nach Ihren Be-
                                          dürfnissen anpassen, sodass genau die Informationen angezeigt werden, die
                                          Sie benötigen.
                                          Die Steuerung des Dialogs erfolgt zum größten Teil über Kontextmenüs.
                                          Der Dialog Bearbeitungen enthält z. B. folgende Spalten:

                                          Termin Termin, an dem die Bearbeitung durchgeführt wird.

                                          Schicht Schicht, in der die Bearbeitung durchgeführt wird.

                                          Sequenz Sequenznummer der Bearbeitung.
2.50 / 01-2023




                                          Typ Nummer des Bearbeitungstyps.

                                          ArtikNr Artikelnummer.


                 A+W Production Grobplanung                                                                   E-105
                 Bearbeitungen in der Grobplanung                                                    Softwarereferenz




                                        Bezeichnung Bezeichnung der Bearbeitung.

                                        MZO-Maschine Maschine, auf der die Bearbeitung durchgeführt wird.

                                        Menge Anzahl der zu fertigenden Teile bzw. durchzuführenden Bearbeitun-
                                        gen.

                                        Erfassungsstelle Erfassungsstelle der zugewiesenen Maschine.

                                        Dauer gesamt Gesamte Bearbeitungsdauer der markierten Aufträge bzw.
                                        Positionen. Einheit: Stunden.

                                            Datenbank-Informationen von Spalten
                                            Mit einem Rechtsklick auf eine Spalte und der Option Definition anzeigen
                                            öffnen Sie den Dialog Spaltendefinition. Im Dialog Spaltendefinition finden
                                            Sie die jeweiligen Datenbank-Informationen einer Spalte.

                                             “Spaltendefinition” auf Seite E-129

                                        Summenzeile

                                        Dauer gesamt Gesamte Bearbeitungsdauer der markierten Aufträge bzw.
                                        Positionen. Einheit: Stunden.

                                        Summe Stück Summe der Teile in den markierten Aufträgen bzw. Positio-
                                        nen.

                                        Filter

                                        [Filter hinzufügen] Fügt einen Filter ein.

                                        Dropdown-Menü Sie haben im Dropdown-Menü des Filters folgende Optio-
                                        nen:
                                        • Klick: Öffnet das Dropdown-Menü, aus dem Sie einen Filter wählen.
                                        • Rechtsklick: Öffnet den Dialog (Filter Name). Mit der Schaltfläche Verwal-
                                           ten gelangen Sie in den Dialog Filter-Definition, in dem Sie den jeweiligen
                                           Filter bearbeiten.
                                         “Filter-Definition” auf Seite E-131

                                        Kontextmenüs
                                        In folgenden Bereichen des Dialogs Bearbeitungen werden Kontextmenüs an-
                                        geboten:
                                        •   Register
                                        •   Spalten
                                        •   Liste
                                        •   Summenzeile
                                        •   Filter
2.50 / 01-2023




                 E-106                                                                  A+W Production Grobplanung
                 Softwarereferenz                                                    Bearbeitungen in der Grobplanung




                                         Kontextmenüs, die im gesamten Bereich der Arbeitsvorbereitung vorkommen,
                                         sind im Kapitel Übergreifende Kontextmenüs gelistet.
                                          “Übergreifende Kontextmenüs” auf Seite E-136


                                         Gruppe       Pfad               Bemerkung

                                         Liste        Status setzen      Öffnet den Dialog Status setzen, in dem Sie den
                                                                         Status der Glasart wählen:
                                                                         •   in Produktion
                                                                         •   produziert
                                                                         •   versandfertig
                                                                         •   ausgeliefert

                                                      Arbeitsplan >      Öffnet den Dialog Umlastung zur
                                                      Maschinen-         Maschinenumlastung.
                                                      Umlastung
                                                                          Kapazitätsplanung: Softwarereferenz, “Ma-
                                                                           schinenumlastung” auf Seite E-175
                                                                         Die Ergebnisse der Maschinenzuordnung im
                                                                         Rahmen der Einlastung werden überschrieben.

                                                      Arbeitsplan >      Öffnet den Dialog Umlastung zur
                                                      Terminumlastung    Terminumlastung.
                                                                          Kapazitätsplanung: Softwarereferenz, “Um-
                                                                           lastung” auf Seite E-171
                                                                         Die Ergebnisse der Maschinenzuordnung im
                                                                         Rahmen der Einlastung werden überschrieben.

                                                      Arbeitsplan >      Öffnet den Dialog Vorgabezeiten ändern, in
                                                      Vorgabezeiten      dem Sie Vorgabezeiten ändern können.
                                                      ändern
                                                                          “Vorgabezeiten ändern” auf Seite E-108
                                                                         Die Ergebnisse der Kapazitätsplanung im
                                                                         Rahmen der Einlastung werden überschrieben.

                                                      Arbeitsplan >      Schützt den Bearbeitungstermin für die
                                                      Bearbeitungs-      markierten Bearbeitungen.
                                                      Termin schützen
                                                                         Die Ergebnisse der Kapazitätsplanung im
                                                                         Rahmen der Einlastung werden überschrieben.

                                                      Arbeitsplan >      Hebt den Bearbeitungstermin-Schutz für die
                                                      Bearbeitungs-      markierten Bearbeitungen auf.
                                                      Termin Schutz
                                                                         Die Ergebnisse der Kapazitätsplanung im
                                                      aufheben
                                                                         Rahmen der Einlastung werden überschrieben.

                 Tab. E-10   Bearbeitungen, Kontextmenüs
2.50 / 01-2023




                 A+W Production Grobplanung                                                                        E-107
                 Bearbeitungen in der Grobplanung                                                 Softwarereferenz




                                        Schaltflächen

                                        [Lauf] Bildet aus den markierten Aufträgen, Positionen oder Teilen einen
                                        Lauf.

                                        [Glasarten] Zeigt die Glasarten der markierten Aufträge an.

                                        [Details] Zeigt die Details der markierten Aufträge an.


                                        Vorgabezeiten ändern
                                        Bearbeitungen > Kontextmenü – Liste > Arbeitsplan > Vorgabezeiten ändern




                                        Abb. E-58   Vorgabezeiten ändern


                                        Im Dialog Vorgabezeiten ändern können Sie Vorgabezeiten für Bearbeitungen
                                        ändern.

                                           Vorgabezeiten ändern
                                           Die errechneten Vorgabezeiten des A+W Capacity Planner werden für die
                                           jeweilige Auswahl überschrieben, wenn Sie im Dialog Vorgabezeiten än-
                                           dern einen Wert festlegen.
                                           Die hinterlegten Vorgabezeitformeln in den Stammdaten der Kapazitätspla-
                                           nung sind von dieser Änderung nicht betroffen.

                                        Faktor Der Faktor, um den die Vorgabezeit verändert werden soll.

                                        [OK] Speichert die Daten.

                                        [Abbrechen] Schließt den Dialog, ohne die Daten zu speichern.
2.50 / 01-2023




                 E-108                                                                A+W Production Grobplanung
                 Softwarereferenz                                                Glasarten, Details, BDE und Lose




                                       Glasarten, Details, BDE und
                                       Lose
                                       In diesem Kapitel finden Sie Informationen zu allen Dialogen, mit denen Sie
                                       sich zu Glasarten, Details, BDE und Losen einen Überblick verschaffen.
2.50 / 01-2023




                 A+W Production Grobplanung                                                                 E-109
                 Glasarten, Details, BDE und Lose                                                      Softwarereferenz




                                           Glasarten
                                           Anzeigen > Aufträge > Kontextmenü – Liste > Glasarten
                                           Anzeigen > Töpfe > Kontextmenü – Liste > Glasarten
                                           Anzeigen > Läufe > Kontextmenü – Liste > Glasarten
                                           Anzeigen > Füllaufträge > Kontextmenü – Liste > Glasarten
                                           Bearbeitungen > Kontextmenü – Liste > Glasarten
                                           Details > Kontextmenü – Liste > Glasarten
                                           Lose > Kontextmenü – Liste > Glasarten
                                           BDE > Kontextmenü – Liste > Glasarten




                 Abb. E-59   Glasarten – Typen (Beispiel)


                                           Mit dem Dialog Glasarten können Sie sich in einer Übersicht die enthaltenen
                                           Glasarten ausgewählter Aufträge bzw. Positionen anzeigen lassen und einen
                                           Lauf bilden. Dieser erscheint dann im Dialog Läufe.
                                           Sie können die Register und Spalten im Dialog Glasarten nach Ihren Bedürf-
                                           nissen anpassen, sodass genau die Informationen angezeigt werden, die Sie
                                           benötigen.
                                           Die Steuerung des Dialogs erfolgt zum größten Teil über Kontextmenüs.
                                           Das Register Typen enthält z. B. folgende Spalten:

                                           Lauf Nummer des Laufs.

                                           Glasart Bezeichnung der Glasart, die im Auftrag bzw. der Position enthalten
                                           ist.

                                           Dicke Dicke der Scheiben.
2.50 / 01-2023




                                           Menge Anzahl der jeweiligen Glasart.

                                           im ISO Anzahl der Scheiben, die für ISO verwendet werden.



                 E-110                                                                  A+W Production Grobplanung
                 Softwarereferenz                                                   Glasarten, Details, BDE und Lose




                                       im ESG Anzahl der Scheiben, die für ESG verwendet werden.

                                       im VSG Anzahl der Scheiben, die für VSG verwendet werden.

                                           Datenbank-Informationen von Spalten
                                           Mit einem Rechtsklick auf eine Spalte und der Option Definition anzeigen
                                           öffnen Sie den Dialog Spaltendefinition. Im Dialog Spaltendefinition finden
                                           Sie die jeweiligen Datenbank-Informationen einer Spalte.

                                            “Spaltendefinition” auf Seite E-129

                                       Summenzeile

                                       Stück Anzahl der Scheiben in den markierten Aufträgen bzw. Positionen.

                                       Dauer gesamt Gesamte Bearbeitungsdauer der markierten Aufträge bzw.
                                       Positionen. Einheit: Stunden.

                                       Fläche Gesamtfläche aller markierten Aufträge bzw. Positionen. Einheit:
                                       Quadratmeter.

                                       Filter

                                       [Filter hinzufügen] Fügt einen Filter ein.

                                       Dropdown-Menü Sie haben im Dropdown-Menü des Filters folgende Optio-
                                       nen:
                                       • Klick: Öffnet das Dropdown-Menü, aus dem Sie einen Filter wählen.
                                       • Rechtsklick: Öffnet den Dialog (Filter Name). Mit der Schaltfläche Verwal-
                                          ten gelangen Sie in den Dialog Filter-Definition, in dem Sie den jeweiligen
                                          Filter bearbeiten.
                                        “Filter-Definition” auf Seite E-131

                                       Kontextmenüs
                                       In folgenden Bereichen des Dialogs Glasarten werden Kontextmenüs angebo-
                                       ten:
                                       •   Register
                                       •   Spalten
                                       •   Liste
                                       •   Summenzeile
                                       •   Filter
                                       Kontextmenüs, die im gesamten Bereich der Arbeitsvorbereitung vorkommen,
                                       sind im Kapitel Übergreifende Kontextmenüs gelistet.
                                        “Übergreifende Kontextmenüs” auf Seite E-136
2.50 / 01-2023




                 A+W Production Grobplanung                                                                     E-111
                 Glasarten, Details, BDE und Lose                                                      Softwarereferenz




                                         Gruppe        Pfad              Bemerkung

                                         Liste         Sonderglas >      Öffnet den Dialog Sonderglas-Lauf bilden.
                                                       Hinzufügen
                                                                          “Sonderglas-Lauf bilden” auf Seite E-92


                                                       Sonderglas >      Derzeit nicht genutzt.
                                                       Entfernen

                                                       Status setzen     Öffnet den Dialog Status setzen, in dem Sie den
                                                                         Status der Glasart wählen:
                                                                         •   in Produktion
                                                                         •   produziert
                                                                         •   versandfertig
                                                                         •   ausgeliefert

                                                       Freie Formen      Öffnet den A+W CAD Designer (Shapes) zur
                                                                         Nachbearbeitung der Modell-Daten.

                                                       Maschinen-        Öffnet den Dialog Maschinenumlastung aus der
                                                       Umlastung         Kapazitätsplanung.
                                                                          Kapazitätsplanung: Softwarereferenz, “Ma-
                                                                           schinenumlastung” auf Seite E-175
                                                                         Die Ergebnisse der Maschinenzuordnung im
                                                                         Rahmen der Einlastung werden überschrieben.

                 Tab. E-11   Glasarten, Kontextmenüs

                                         Schaltflächen

                                         [Lauf] Bildet aus den markierten Aufträgen, Positionen oder Teilen einen
                                         Lauf.

                                         [Glasarten] Zeigt die Glasarten der markierten Aufträge bzw. Positionen an.

                                         [Details] Zeigt die Details der markierten Aufträge bzw. Positionen an.
2.50 / 01-2023




                 E-112                                                                   A+W Production Grobplanung
                 Softwarereferenz                                                       Glasarten, Details, BDE und Lose




                                            Details
                                            Anzeigen > Aufträge > Details
                                            Anzeigen > Töpfe > Kontextmenü – Liste > Details
                                            Anzeigen > Läufe > Kontextmenü – Liste > Details
                                            Anzeigen > Füllaufträge > Kontextmenü – Liste > Details
                                            Glasarten > Kontextmenü – Liste > Details
                                            Bearbeitungen > Kontextmenü – Liste > Details
                                            BDE > Kontextmenü – Liste > Details
                                            Lose > Kontextmenü – Liste > Details




                 Abb. E-60   Details (Beispiel)


                                            Mit dem Dialog Details können Sie sich Details zu ausgewählten Aufträgen,
                                            Positionen, Teilen, Läufen oder Töpfen anzeigen lassen. Sie können den Dia-
                                            log Details aus jeder Ansicht in der Grobplanung öffnen.
                                            Sie können die Register und Spalten im Dialog Details nach Ihren Bedürfnis-
                                            sen anpassen, sodass genau die Informationen angezeigt werden, die Sie be-
                                            nötigen.
                                            Die Steuerung des Dialogs erfolgt zum größten Teil über Kontextmenüs.
                                            Der Dialog Details enthält z. B. folgende Spalten:

                                            SN Info Zeigt den Modellstatus und die damit verbundene Geometrieberech-
                                            nung im Rahmen der Einlastung. Folgende Anzeigen sind möglich:
                                            • 0: Status ok.
2.50 / 01-2023




                                            • Nummer: Es liegt ein Fehler vor.

                                            Storno Angabe, ob der Auftrag im ERP-System storniert wurde.



                 A+W Production Grobplanung                                                                      E-113
                 Glasarten, Details, BDE und Lose                                                    Softwarereferenz




                                         Auftrag Nummer des Auftrags.

                                         Lauf Nummer des Laufs.

                                         Liefertermin Liefertermin des Auftrags.

                                         Produktionstermin Produktionstermin des Auftrags, der Position, der Ein-
                                         heit oder des Teils.

                                         Summe ISO Anzahl der ISO-Scheiben, die der Auftrag enthält.

                                         Summe [teil] mattiert Anzahl der Scheiben, die mattiert oder teilmattiert
                                         werden.

                                         Summe VSG Anzahl der VSG-Scheiben im Auftrag bzw. in der Position.

                                         Summe ESG Anzahl der ESG-Scheiben im Auftrag bzw. in der Position.

                                         Summe Sprossen Anzahl der Sprossen im Auftrag.

                                         Summe Modelle Anzahl der Modelle im Auftrag.

                                         Summe 3-Fach-ISO Anzahl der 3-fach-ISO-Scheiben im Auftrag.

                                         Summe Stufen Anzahl der Stufen-ISO oder Stufen-VSG im Auftrag.

                                            Datenbank-Informationen von Spalten
                                            Mit einem Rechtsklick auf eine Spalte und der Option Definition anzeigen
                                            öffnen Sie den Dialog Spaltendefinition. Im Dialog Spaltendefinition finden
                                            Sie die jeweiligen Datenbank-Informationen einer Spalte.

                                             “Spaltendefinition” auf Seite E-129

                                         Summenzeile

                                         Summe Stück Summe der Teile in den markierten Aufträgen bzw. Positio-
                                         nen.

                                         Modelle Anzahl der in den markierten Aufträgen bzw. Positionen enthaltenen
                                         Modelle.

                                         Fläche Mod Gesamtfläche der Modelle in den markierten Aufträgen bzw. Po-
                                         sitionen. Einheit: Quadratmeter.
2.50 / 01-2023




                 E-114                                                                  A+W Production Grobplanung
                 Softwarereferenz                                                          Glasarten, Details, BDE und Lose




                                          Filter

                                          [Filter hinzufügen] Fügt einen Filter ein.

                                          Dropdown-Menü Sie haben im Dropdown-Menü des Filters folgende Optio-
                                          nen:
                                          • Klick: Öffnet das Dropdown-Menü, aus dem Sie einen Filter wählen.
                                          • Rechtsklick: Öffnet den Dialog (Filter Name). Mit der Schaltfläche Verwal-
                                             ten gelangen Sie in den Dialog Filter-Definition, in dem Sie den jeweiligen
                                             Filter bearbeiten.
                                           “Filter-Definition” auf Seite E-131

                                          Kontextmenüs
                                          In folgenden Bereichen des Dialogs Details werden Kontextmenüs angebo-
                                          ten:
                                          •   Register
                                          •   Spalten
                                          •   Liste
                                          •   Summenzeile
                                          •   Filter
                                          Kontextmenüs, die im gesamten Bereich der Arbeitsvorbereitung vorkommen,
                                          sind im Kapitel Übergreifende Kontextmenüs gelistet.
                                           “Übergreifende Kontextmenüs” auf Seite E-136


                                          Gruppe        Pfad                  Bemerkung

                                          Liste         Zurück in den Pool    Gibt die ausgewählten Aufträge zurück in den
                                                                              Dialog Aufträge.
                                                                               “Aufträge” auf Seite E-59

                                                        Status setzen         Öffnet den Dialog Status setzen, in dem Sie den
                                                                              Status des Laufs wählen:
                                                                              •   in Produktion
                                                                              •   produziert
                                                                              •   versandfertig
                                                                              •   ausgeliefert

                                                        Arbeitsplan >         Öffnet den Dialog Umlastung zur
                                                        Maschinen-            Maschinenumlastung.
                                                        Umlastung
                                                                               Kapazitätsplanung: Softwarereferenz, “Ma-
                                                                                schinenumlastung” auf Seite E-175
                                                                              Die Ergebnisse der Maschinenzuordnung im
                                                                              Rahmen der Einlastung werden überschrieben.

                                                        Arbeitsplan >         Führt die Maschinenzuordnung für markierte
                                                        Maschinen-            Aufträge bzw. Positionen erneut durch.
                                                        Zuordnung
2.50 / 01-2023




                                                                              Die Ergebnisse der Maschinenzuordnung im
                                                                              Rahmen der Einlastung werden überschrieben.

                 Tab. E-12   Details, Kontextmenüs (Abschnitt 1 von 2)



                 A+W Production Grobplanung                                                                             E-115
                 Glasarten, Details, BDE und Lose                                                      Softwarereferenz




                                          Gruppe        Pfad              Bemerkung

                                                        Arbeitsplan >     Zur Zeit nicht genutzt
                                                        Arbeitsplan neu
                                                        berechnen

                                                        Sprossen-Druck    Startet den Druck von Produktionspapieren für
                                                                          die Sprossenproduktion bzw. -bearbeitung.

                                                        Vorgabezeiten     Öffnet den Dialog Vorgabezeiten ändern, in
                                                        ändern            dem Sie Vorgabezeiten ändern können.
                                                                           “Vorgabezeiten ändern” auf Seite E-108
                                                                          Die Ergebnisse der Kapazitätsplanung im
                                                                          Rahmen der Einlastung werden überschrieben.

                 Tab. E-12   Details, Kontextmenüs (Abschnitt 2 von 2)

                                          Schaltflächen

                                          [Lauf] Bildet aus den markierten Aufträgen, Positionen oder Teilen einen
                                          Lauf.

                                          [Glasarten] Zeigt die Glasarten der markierten Aufträge bzw. Positionen an.

                                          [Details] Zeigt die Details der markierten Aufträge bzw. Positionen an.
2.50 / 01-2023




                 E-116                                                                    A+W Production Grobplanung
                 Softwarereferenz                                                   Glasarten, Details, BDE und Lose




                                          BDE
                                          Anzeigen > Aufträge > Kontextmenü – Liste > Bearbeitungen > Kontextmenü
                                          – Liste > BDE
                                          Anzeigen > Töpfe > Kontextmenü – Liste > Bearbeitungen > Kontextmenü –
                                          Liste > BDE
                                          Anzeigen > Läufe > Kontextmenü – Liste > BDE
                                          Glasarten > Kontextmenü – Liste > BDE
                                          Details > Kontextmenü – Liste > BDE




                 Abb. E-61   BDE – Produkt (Beispiel)


                                          Im Dialog BDE bekommen Sie einen Überblick über Informationen, die sich
                                          auf die Betriebsdatenerfassung beziehen.
                                          Sie können die Aufträge nach unterschiedlichen Kriterien sortieren und bear-
                                          beiten. Folgende Bestandteile des Dialogs BDE können Sie frei konfigurieren:
2.50 / 01-2023




                 A+W Production Grobplanung                                                                    E-117
                 Glasarten, Details, BDE und Lose                                                     Softwarereferenz




                                         •   Register
                                         •   Spalten
                                         •   Summenzeile
                                         •   Filter
                                         Die Steuerung des Dialogs erfolgt zum größten Teil über Kontextmenüs.
                                         Das Register Produkt enthält z. B. folgende Spalten:

                                         Auftrag Nummer des Auftrags.

                                         Pos (int Pos) Interne Positionsnummer aus der Auftragserfassung.

                                         Teile-Nr. Teilenummer des jeweiligen Teils.

                                         Artikelbezeichnung Bezeichnung des jeweiligen Artikels.

                                         Etikett-Nr. Etikettnummer des jeweiligen Teils.

                                             Datenbank-Informationen von Spalten
                                             Mit einem Rechtsklick auf eine Spalte und der Option Definition anzeigen
                                             öffnen Sie den Dialog Spaltendefinition. Im Dialog Spaltendefinition finden
                                             Sie die jeweiligen Datenbank-Informationen einer Spalte.

                                              “Spaltendefinition” auf Seite E-129

                                         Summenzeile
                                         In der Summenzeile können Sie sich verschiedene Summen anzeigen lassen,
                                         Sie bekommen z. B. folgende Informationen angezeigt:

                                         Dauer gesamt Gesamte Bearbeitungsdauer der markierten Aufträge bzw.
                                         Positionen. Einheit: Stunden.

                                         Summe Stück Summe der Teile in den markierten Aufträgen bzw. Positio-
                                         nen.

                                         Filter

                                         [Filter hinzufügen] Fügt einen Filter ein.

                                         Dropdown-Menü Sie haben im Dropdown-Menü des Filters folgende Optio-
                                         nen:
                                         • Klick: Öffnet das Dropdown-Menü, aus dem Sie einen Filter wählen.
                                         • Rechtsklick: Öffnet den Dialog (Filter Name). Mit der Schaltfläche Verwal-
                                            ten gelangen Sie in den Dialog Filter-Definition, in dem Sie den jeweiligen
                                            Filter bearbeiten.
                                          “Filter-Definition” auf Seite E-131
2.50 / 01-2023




                 E-118                                                                   A+W Production Grobplanung
                 Softwarereferenz                                                     Glasarten, Details, BDE und Lose




                                        Kontextmenüs
                                        In folgenden Bereichen des Dialogs BDE werden Kontextmenüs angeboten:
                                        •   Register
                                        •   Spalten
                                        •   Liste
                                        •   Summenzeile
                                        •   Filter
                                        Kontextmenüs, die im gesamten Bereich der Arbeitsvorbereitung vorkommen,
                                        sind im Kapitel Übergreifende Kontextmenüs gelistet.
                                         “Übergreifende Kontextmenüs” auf Seite E-136


                                        Gruppe      Pfad                 Bemerkung

                                        Liste       Zurück in den Pool   Gibt die ausgewählten Aufträge bzw. Positionen
                                                                         zurück in den Dialog Aufträge.



                                                    Status setzen        Öffnet den Dialog Status setzen, in dem Sie den
                                                                         Status des Laufs wählen:
                                                                         •   in Produktion
                                                                         •   produziert
                                                                         •   versandfertig
                                                                         •   ausgeliefert

                                                    Arbeitsplan >        Öffnet den Dialog Umlastung zur
                                                    Maschinen-           Maschinenumlastung.
                                                    Umlastung
                                                                          Kapazitätsplanung: Softwarereferenz, “Ma-
                                                                           schinenumlastung” auf Seite E-175
                                                                         Die Ergebnisse der Maschinenzuordnung im
                                                                         Rahmen der Einlastung werden überschrieben.

                                                    Arbeitsplan >        Führt die Maschinenzuordnung für markierte
                                                    Maschinen-           Aufträge bzw. Positionen erneut durch.
                                                    Zuordnung
                                                                         Die Ergebnisse der Maschinenzuordnung im
                                                                         Rahmen der Einlastung werden überschrieben.

                                                    Arbeitsplan >        Zur Zeit nicht genutzt.
                                                    Arbeitsplan neu
                                                    berechnen

                                                    Vorgabezeiten        Öffnet den Dialog Vorgabezeiten ändern, in
                                                    ändern               dem Sie Vorgabezeiten ändern können.
                                                                          “Vorgabezeiten ändern” auf Seite E-108
                                                                         Die Ergebnisse der Kapazitätsplanung im
                                                                         Rahmen der Einlastung werden überschrieben.

                 Tab. E-13   BDE, Kontextmenüs
2.50 / 01-2023




                 A+W Production Grobplanung                                                                        E-119
                 Glasarten, Details, BDE und Lose                                                   Softwarereferenz




                                         Schaltflächen

                                         [Lauf] Zur Zeit nicht aktiv.

                                         [Glasarten] Zeigt die Glasarten der markierten Aufträge bzw. Positionen an.

                                         [Details] Zeigt die Details der markierten Aufträge bzw. Positionen an.
2.50 / 01-2023




                 E-120                                                                 A+W Production Grobplanung
                 Softwarereferenz                                                    Glasarten, Details, BDE und Lose




                                           Lose
                                           Anzeigen > Läufe > Kontextmenü – Liste > Lose
                                           Details > Kontextmenü – Liste > Lose




                 Abb. E-62   Lose – Zuschnitt (Beispiel)


                                           Im Dialog Lose bekommen Sie einen Überblick über die erstellten Lose der
                                           ausgewählten Läufe.
                                           Sie können die Lose nach unterschiedlichen Kriterien sortieren und bearbei-
                                           ten. Die Steuerung des Dialogs Lose erfolgt vorrangig über Kontextmenüs.
                                           Folgende Bestandteile des Dialogs Lose können Sie frei konfigurieren:
                                           •   Register
                                           •   Spalten
                                           •   Summenzeile
                                           •   Filter
2.50 / 01-2023




                 A+W Production Grobplanung                                                                     E-121
                 Glasarten, Details, BDE und Lose                                                    Softwarereferenz




                                         Das Register Zuschnitt enthält z. B. folgende Spalten:

                                         Lostyp Gibt den Typ des Loses an.

                                         Los Bezeichnung des Loses.

                                         Bock Gestell, auf das das Los geplant wird.

                                         Glasart Nummer der Glasart.

                                         Glasart-Bez. Bezeichnung der Glasart des Loses.

                                         Stück Anzahl der Positionen bzw. Teile im Los.

                                            Datenbank-Informationen von Spalten
                                            Mit einem Rechtsklick auf eine Spalte und der Option Definition anzeigen
                                            öffnen Sie den Dialog Spaltendefinition. Im Dialog Spaltendefinition finden
                                            Sie die jeweiligen Datenbank-Informationen einer Spalte.

                                             “Spaltendefinition” auf Seite E-129

                                         Summenzeile
                                         In der Summenzeile können Sie sich verschiedene Summen anzeigen lassen,
                                         Sie bekommen z. B. folgende Informationen angezeigt:

                                         Dauer gesamt Gesamte Bearbeitungsdauer der markierten Aufträge bzw.
                                         Positionen. Einheit: Stunden.

                                         Stück Anzahl der Einzelscheiben oder Stückartikel in den markierten Aufträ-
                                         gen bzw. Positionen.

                                         Filter

                                         [Filter hinzufügen] Fügt einen Filter ein.

                                         Dropdown-Menü Sie haben im Dropdown-Menü des Filters folgende Optio-
                                         nen:
                                         • Klick: Öffnet das Dropdown-Menü, aus dem Sie einen Filter wählen.
                                         • Rechtsklick: Öffnet den Dialog (Filter Name). Mit der Schaltfläche Verwal-
                                            ten gelangen Sie in den Dialog Filter-Definition, in dem Sie den jeweiligen
                                            Filter bearbeiten.
                                          “Filter-Definition” auf Seite E-131
2.50 / 01-2023




                 E-122                                                                  A+W Production Grobplanung
                 Softwarereferenz                                                     Glasarten, Details, BDE und Lose




                                         Kontextmenüs
                                         In folgenden Bereichen des Dialogs Lose werden Kontextmenüs angeboten:
                                         •   Register
                                         •   Spalten
                                         •   Liste
                                         •   Summenzeile
                                         •   Filter
                                         Kontextmenüs, die im gesamten Bereich der Arbeitsvorbereitung vorkommen,
                                         sind im Kapitel Übergreifende Kontextmenüs gelistet.
                                          “Übergreifende Kontextmenüs” auf Seite E-136


                                         Gruppe       Pfad               Bemerkung

                                         Liste        Status setzen      Öffnet den Dialog Status setzen, in dem Sie den
                                                                         Status des Laufs wählen:
                                                                         •   in Produktion
                                                                         •   produziert
                                                                         •   versandfertig
                                                                         •   ausgeliefert

                 Tab. E-14   Lose, Kontextmenüs

                                         Schaltflächen

                                         [Lauf] Zur Zeit nicht aktiv.

                                         [Glasarten] Zeigt die Glasarten der markierten Lose an.

                                         [Details] Zeigt die Details der markierten Lose an.
2.50 / 01-2023




                 A+W Production Grobplanung                                                                        E-123
                 Übergreifende Dialoge                                                                Softwarereferenz




                                         Übergreifende Dialoge
                                         In diesem Kapitel finden Sie Informationen zu allen Dialogen, die Sie übergrei-
                                         fend in der gesamten Arbeitsvorbereitung finden. Sie können Eigenschaften
                                         von Dialogen bearbeiten, Dokumentenverknüpfungen verwalten und Ent-
                                         schichtungsflächen bearbeiten.
                                         Das Kapitel enthält folgende Themen:
                                         •   “Eigenschaften von (Register)” auf Seite E-128
                                         •   “Spaltendefinition” auf Seite E-129
                                         •   “(Filter Name)” auf Seite E-130
                                         •   “Filter-Definition” auf Seite E-131
                                         •   “Dokumentenverknüpfungen” auf Seite E-133
                                         •   “Entschichtungsflächen” auf Seite E-134
2.50 / 01-2023




                 E-124                                                                  A+W Production Grobplanung
                 Softwarereferenz                                                                 Übergreifende Dialoge




                                           Arbeitsplan
                                           Produktionsmonitor > Kontextmenü – Schicht > Arbeitsplan




                 Abb. E-63   Arbeitsplan (Beispiel)


                                           Mit dem Dialog Arbeitsplan können Sie sich aus dem Produktionsmonitor he-
                                           raus einen Überblick verschaffen. Der Arbeitsplan zeigt die geplanten Läufe
                                           auf einer Maschine, bzw. in einer Schicht.
                                           Sie können die Register und Spalten im Dialog Arbeitsplan nach Ihren Bedürf-
                                           nissen anpassen, sodass genau die Informationen angezeigt werden, die Sie
                                           benötigen.
                                           Die Steuerung des Dialogs erfolgt zum größten Teil über Kontextmenüs.
                                           Das Register Details enthält z. B. folgende Spalten:

                                           Lauf Angabe des Laufs.

                                           Auftrag Angabe des Auftrags.

                                           Pos (int Pos) Angabe der Positionsnummer.

                                           Teile-Nr Angabe der Teilenummer.

                                           Sequenz Sequenznummer der Bearbeitung.
2.50 / 01-2023




                 A+W Production Grobplanung                                                                     E-125
                 Übergreifende Dialoge                                                                Softwarereferenz




                                         Bearbnr Nummer der Bearbeitung.

                                         MZO-Maschine Logische Maschine, auf der die Bearbeitung durchgeführt
                                         wird.

                                             Datenbank-Informationen von Spalten
                                             Mit einem Rechtsklick auf eine Spalte und der Option Definition anzeigen
                                             öffnen Sie den Dialog Spaltendefinition. Im Dialog Spaltendefinition finden
                                             Sie die jeweiligen Datenbank-Informationen einer Spalte.

                                              “Spaltendefinition” auf Seite E-129

                                         Summenzeile
                                         In der Summenzeile können Sie sich verschiedene Summen anzeigen lassen,
                                         Sie bekommen z. B. folgende Informationen angezeigt:

                                         Summe Stück Summe der Teile in den markierten Aufträgen bzw. Positio-
                                         nen.

                                         Dauer gesamt Gesamte Bearbeitungsdauer der markierten Aufträge bzw.
                                         Positionen. Einheit: Stunden.

                                         Filter

                                         [Filter hinzufügen] Fügt einen Filter ein.

                                         Dropdown-Menü Sie haben im Dropdown-Menü des Filters folgende Optio-
                                         nen:
                                         • Klick: Öffnet das Dropdown-Menü, aus dem Sie einen Filter wählen.
                                         • Rechtsklick: Öffnet den Dialog (Filter Name). Mit der Schaltfläche Verwal-
                                            ten gelangen Sie in den Dialog Filter-Definition, in dem Sie den jeweiligen
                                            Filter bearbeiten.
                                          “Filter-Definition” auf Seite E-131

                                         Kontextmenüs
                                         In folgenden Bereichen des Dialogs Arbeitsplan werden Kontextmenüs ange-
                                         boten:
                                         •   Register
                                         •   Spalten
                                         •   Liste
                                         •   Summenzeile
                                         •   Filter
                                         Kontextmenüs, die im gesamten Bereich der Arbeitsvorbereitung vorkommen,
                                         sind im Kapitel Übergreifende Kontextmenüs gelistet.
                                          “Übergreifende Kontextmenüs” auf Seite E-136
2.50 / 01-2023




                 E-126                                                                    A+W Production Grobplanung
                 Softwarereferenz                                                                  Übergreifende Dialoge




                                          Gruppe         Pfad              Bemerkung

                                          Liste          Status setzen     Öffnet den Dialog Status setzen, in dem Sie den
                                                                           Status des Laufs wählen:
                                                                           •   in Produktion
                                                                           •   produziert
                                                                           •   versandfertig
                                                                           •   ausgeliefert

                                                         Arbeitsplan >     Öffnet den Dialog Umlastung zur
                                                         Maschinen-        Maschinenumlastung.
                                                         Umlastung
                                                                            Kapazitätsplanung: Softwarereferenz, “Ma-
                                                                             schinenumlastung” auf Seite E-175
                                                                           Die Ergebnisse der Maschinenzuordnung im
                                                                           Rahmen der Einlastung werden überschrieben.

                                                         Arbeitsplan >     Öffnet den Dialog Umlastung zur
                                                         Terminumlastung   Terminumlastung.
                                                                            Kapazitätsplanung: Softwarereferenz, “Ma-
                                                                             schinenumlastung” auf Seite E-175
                                                                           Die Ergebnisse der Maschinenzuordnung im
                                                                           Rahmen der Einlastung werden überschrieben.

                                                         Arbeitsplan >     Öffnet den Dialog Vorgabezeiten ändern, in
                                                         Vorgabezeiten     dem Sie Vorgabezeiten ändern können.
                                                         ändern
                                                                            “Vorgabezeiten ändern” auf Seite E-108
                                                                           Die Ergebnisse der Kapazitätsplanung im
                                                                           Rahmen der Einlastung werden überschrieben.

                                                         Arbeitsplan >     Schützt den Bearbeitungstermin für die
                                                         Bearbeitungs-     markierten Bearbeitungen.
                                                         Termin schützen
                                                                           Die Ergebnisse der Kapazitätsplanung im
                                                                           Rahmen der Einlastung werden überschrieben.

                                                         Arbeitsplan >     Hebt den Bearbeitungstermin-Schutz für die
                                                         Bearbeitungs-     markierten Bearbeitungen auf.
                                                         Termin Schutz
                                                                           Die Ergebnisse der Kapazitätsplanung im
                                                         aufheben
                                                                           Rahmen der Einlastung werden überschrieben.

                                                         Fertigmelden      Die Läufe, Aufträge oder Positionen werden auf
                                                                           den Status Fertig gesetzt.

                 Tab. E-15   Arbeitsplan, Kontextmenüs
2.50 / 01-2023




                 A+W Production Grobplanung                                                                          E-127
                 Übergreifende Dialoge                                                               Softwarereferenz




                                         Schaltflächen

                                         [Lauf] Bildet aus den markierten Läufen, Aufträgen oder Positionen einen
                                         Lauf.

                                         [Glasarten] Zeigt die Glasarten der markierten Läufe, Aufträge oder Positio-
                                         nen an.

                                         [Details] Zeigt die Details der markierten Läufe, Aufträge oder Positionen an.


                                         Eigenschaften von (Register)
                                         Anzeigen > Aufträge > Kontextmenü – Register > Einfügen
                                         Anzeigen > Aufträge > Kontextmenü – Register > Eigenschaften




                                         Abb. E-64    Eigenschaften von (Register)


                                         Im Dialog Eigenschaften von (Register) können Sie neue Register anlegen
                                         oder bestehende Register ändern.

                                         Registertext Titel des Registers.

                                         Beschreibung Beschreibung des Registers.

                                         Systemweite Anzeige Checkbox mit folgenden Funktionen:
                                          Das Register wird nur in diesem Dialog angezeigt.
                                          Das Register wird systemweit angezeigt.

                                         [OK] Speichert die Daten.

                                         [Abbrechen] Schließt den Dialog, ohne die Daten zu speichern.
2.50 / 01-2023




                 E-128                                                                 A+W Production Grobplanung
                 Softwarereferenz                                                           Übergreifende Dialoge




                                       Spaltendefinition
                                       Anzeigen > Aufträge > Kontextmenü – Spalten > Definition anzeigen
                                       Anzeigen > Töpfe > Kontextmenü – Spalten > Definition anzeigen
                                       Anzeigen > Läufe > Kontextmenü – Spalten > Definition anzeigen
                                       Auftragsübersicht > Kontextmenü – Spalten > Definition anzeigen
                                       Glasarten > Kontextmenü – Spalten > Definition anzeigen
                                       Bearbeitungen > Kontextmenü – Spalten > Definition anzeigen
                                       Lose > Kontextmenü – Spalten > Definition anzeigen
                                       BDE > Kontextmenü – Spalten > Definition anzeigen
                                       Details > Kontextmenü – Spalten > Definition anzeigen




                                       Abb. E-65   Spaltendefinition


                                       Im Dialog Spaltendefinition werden die Eigenschaften einer Spalte angezeigt.

                                       Titel Name der Spalte.

                                       Format Format der Spalte, z. B. das Datums-Format.

                                       Menü Gibt an, in welchem Bereich des Kontextmenüs die jeweilige Auswahl
                                       hinterlegt ist.

                                       SQL-Def. Name der Datenbank-Tabelle und des Datenbank-Felds. Diese
                                       werden ausführlich in der A+W Datenbank-Dokumentation beschrieben.
2.50 / 01-2023




                 A+W Production Grobplanung                                                                 E-129
                 Übergreifende Dialoge                                                               Softwarereferenz




                                         SQL-Definition Teile Name der Datenbank-Tabelle und des Datenbank-
                                         Felds, wenn Sie im Dialog Auftragsübersicht die Anzeige-Option Teile gewählt
                                         haben. Die Datenbanktabellen und -felder sind ausführlich in der A+W Daten-
                                         bank-Dokumentation beschrieben.

                                         SQL-Definition Bearbeitungen Name der Datenbank-Tabelle und des Da-
                                         tenbank-Felds, wenn Sie im Dialog Auftragsübersicht die Anzeige-Option Be-
                                         arbeitungen gewählt haben. Die Datenbanktabellen und -felder sind
                                         ausführlich in der A+W Datenbank-Dokumentation beschrieben.

                                         [OK] Schließt den Dialog.


                                         (Filter Name)
                                         Anzeigen > Aufträge > Kontextmenü – Filter




                                         Abb. E-66     (Filter Name)


                                         Im Dialog (Filter Name) gelangen Sie zur Filter-Definition und Sie können Fil-
                                         ter löschen.

                                         Verwalten Öffnet den Dialog Filter-Definition, in dem Sie Filter bearbeiten.
                                          “Filter-Definition” auf Seite E-131

                                         Entfernen Löscht den ausgewählten Filter.

                                         [OK] Schließt den Dialog.

                                         [Abbrechen] Schließt den Dialog, ohne die Daten zu speichern.
2.50 / 01-2023




                 E-130                                                                  A+W Production Grobplanung
                 Softwarereferenz                                                              Übergreifende Dialoge




                                       Filter-Definition
                                       Anzeigen > Aufträge > Kontextmenü – Filter > (Filter Name) > [Verwalten]




                                       Abb. E-67    Filter-Definition


                                       Im Dialog Filter-Definition können Sie Filter definieren und bearbeiten.

                                       Definierte Filter Liste der definierten Filter.

                                       Name Bezeichnung des jeweiligen Filters.

                                       Beschreibung Beschreibung des jeweiligen Filters.

                                       SQL-Bedingung Hinterlegte Formel bzw. Bedingung mit Referenz auf die
                                       entsprechenden Datenbanktabellen und -felder.

                                       Standard-Parameter Angabe eines Standard-Werts, z. B. ein Standard-Da-
                                       tum, auf das zurückgegriffen wird, wenn die entsprechenden Datenbanktabel-
                                       len bzw. -felder keinen Wert ermitteln.

                                       Zulässig für Ansicht Auswahl, in welchem Dialog der Filter zur Verfügung
                                       steht. Zur Auswahl stehen:
                                       • Pool-Ansicht
                                       • Topf-Ansicht
                                       • Lauf-Ansicht
                                       • Füllauftrags-Ansicht
                                       • Details
                                       • Vorauswahl BDE-Ansicht
                                       • Bestellteile-Topf
                                       • Glasarten-Ansicht
                                       • Produktionslos-Ansicht
                                       • Bearbeitungs-Ansicht
2.50 / 01-2023




                                       • BDE
                                       • Packmittel




                 A+W Production Grobplanung                                                                       E-131
                 Übergreifende Dialoge                                                              Softwarereferenz




                                         •   Bruchstatistik
                                         •   Produktionsstatistik
                                         •   Produktionsübersicht

                                         Speichern Speichert die Daten.

                                         Löschen Löscht den markierten Filter.

                                         Exportieren Öffnet den Dialog Speichern unter, in dem Sie den jeweiligen Fil-
                                         ter speichern können.

                                         Importieren Öffnet den Dialog Öffnen, in dem Sie Filter zum Importieren aus-
                                         wählen.

                                         [Schließen] Schließt den Dialog, ohne die Daten zu speichern.
2.50 / 01-2023




                 E-132                                                                 A+W Production Grobplanung
                 Softwarereferenz                                                           Übergreifende Dialoge




                                       Dokumentenverknüpfungen
                                       Anzeigen > Aufträge > Kontextmenü – Liste > Zugehörige Dokumente
                                       Anzeigen > Töpfe > Kontextmenü – Liste > Zugehörige Dokumente
                                       Anzeigen > Läufe > Kontextmenü – Liste > Zugehörige Dokumente
                                       Anzeigen > Füllaufträge > Kontextmenü – Liste > Zugehörige Dokumente
                                       Glasarten > Kontextmenü – Liste > Zugehörige Dokumente
                                       Bearbeitungen > Kontextmenü – Liste > Zugehörige Dokumente
                                       BDE > Kontextmenü – Liste > Zugehörige Dokumente
                                       Lose > Kontextmenü – Liste > Zugehörige Dokumente




                                       Abb. E-68   Dokumentenverknüpfungen


                                       Im Dialog Dokumentenverknüpfungen können Sie Aufträge mit Dokumenten,
                                       wie z. B. speziellen Lieferbedingungen, verknüpfen und sehen, mit welchen
                                       Dokumenten ein Auftrag bzw. eine Position verknüpft ist.

                                       Auftrag Ausgewählte Aufträge.

                                       Position Anzahl der Positionen pro Auftrag.

                                       Typ Typ des verknüpften Dokuments. Sie geben den Dokumententyp mit ei-
                                       ner frei wählbaren Zahl an. Sie legen auch fest, welcher Dokumententyp einer
                                       Zahl zugeordnet ist, z. B 3 für Textdokumente.

                                       Dokument Pfad des verknüpften Dokuments.

                                       [Öffnen] Öffnet ein angehängtes Dokument.

                                       [Löschen] Löscht die Dokumentenverknüpfung.

                                       [Neu] Erstellt eine neue Dokumentenverknüpfung.

                                       [Ändern] Öffnet den Dialog Dokumentenverknüpfung (Auftragsnummer), um
2.50 / 01-2023




                                       die Daten zu ändern.

                                       [Schließen] Schließt den Dialog.


                 A+W Production Grobplanung                                                                 E-133
                 Übergreifende Dialoge                                                              Softwarereferenz




                                         Entschichtungsflächen
                                         Anzeigen > Aufträge > Kontextmenü – Liste > Nacherfassung > Entschichtung
                                         Anzeigen > Töpfe > Kontextmenü – Liste > Nacherfassung > Entschichtung
                                         Anzeigen > Läufe > Kontextmenü – Liste > Nacherfassung > Entschichtung
                                         Anzeigen > Füllauftr. > Kontextmenü – Liste > Nacherfassung > Entschichtung
                                         Details > Kontextmenü – Liste > Nacherfassung > Entschichtung
                                         BDE > Kontextmenü – Liste > Nacherfassung > Entschichtung




                                         Abb. E-69    Entschichtungsflächen


                                         Im Dialog Entschichtungsflächen können Sie nachträglich die Flächen ange-
                                         ben, die entschichtet werden sollen.

                                         Kopfzeile
                                         In der Kopfzeile werden folgende Informationen zur jeweiligen Position ange-
                                         zeigt:
                                         •   Auftrag
                                         •   Position
                                         •   Unterposition
                                         •   Teilenummer
                                         •   Glasart
                                         •   Modell
2.50 / 01-2023




                                         Navigationsfenster
                                         Im Navigationsfenster bekommen Sie die markierten Entschichtungsflächen
                                         angezeigt.


                 E-134                                                                A+W Production Grobplanung
                 Softwarereferenz                                                           Übergreifende Dialoge




                                       Navigation

                                       1 Abstand der Entschichtungsfläche von Ecke 1. Einheit: Millimeter.

                                       2 Abstand der Entschichtungsfläche von Ecke 2. Einheit: Millimeter.

                                       [Pfeil nach links] Ändert die Lage der Ecken 1 und 2 auf der Scheibe.

                                       [Pfeil nach rechts] Ändert die Lage der Ecken 1 und 2 auf der Scheibe.

                                       Schaltflächen

                                       [OK] Speichert die Daten.

                                       [Abbrechen] Schließt den Dialog, ohne die Daten zu speichern.
2.50 / 01-2023




                 A+W Production Grobplanung                                                                  E-135
                 Übergreifende Kontextmenüs                                                                 Softwarereferenz




                                         Übergreifende Kontextmenüs
                                         In diesem Kapitel finden Sie Informationen zu allen Kontextmenüs, die über-
                                         greifend im gesamten Bereich der Arbeitsvorbereitung vorkommen.
                                         Die Kontextmenüs finden Sie in folgenden Dialogbereichen:
                                         •   Register
                                         •   Spalten
                                         •   Liste
                                         •   Summenzeile
                                         •   Filter


                                         Gruppe       Pfad                 Bemerkung

                                         Register     Speicherautomatik    Änderungen am Register werden automatisch
                                                                           gespeichert.

                                                      Speichern            Manuelles Speichern von Änderungen am
                                                                           Register.

                                                      Einfügen             Öffnet den Dialog Eigenschaften von (Register).
                                                                            “Eigenschaften von (Register)” auf
                                                                             Seite E-128

                                                      Löschen              Löscht das markierte Register.

                                                      Eigenschaften        Öffnet den Dialog Eigenschaften von (Register),
                                                                           in dem Sie die Eigenschaften des Registers
                                                                           ändern.
                                                                            “Eigenschaften von (Register)” auf
                                                                             Seite E-128

                                                      Import               Öffnet den Dialog Importieren eines Registers.

                                                      Export               Öffnet den Dialog Exportieren eines Registers.

                                         Spalten      Umsortieren          Spalte aufsteigend oder absteigend sortieren.
                                                                           Wirkt sich auf die ersten drei Spalten im Dialog
                                                                           aus.

                                                      Formatieren          Format oder Einheit für die Spalten auswählen,
                                                                           z. B. Datumsformate oder Längen-Einheiten.

                                                      Einfügen             Fügt eine neue Spalte ein. Verschiedene
                                                                           Kategorien stehen zur Verfügung.

                                                      Einfügen >           Öffnet den Dialog Felddefinition, in dem Sie
                                                      Felddefinitionen >   Abfragen auf Datenbank-Tabellen und -Felder
                                                      Editieren            formulieren können. Diese Abfragen können Sie
                                                                           dann z. B. teile-, positions- oder
                                                                           auftragsbezogen als Spalte einfügen.
                                                                            “Felddefinition” auf Seite E-101
2.50 / 01-2023




                 Tab. E-16   Übergreifende Kontextmenüs




                 E-136                                                                     A+W Production Grobplanung
                 Softwarereferenz                                                           Übergreifende Kontextmenüs




                                         Gruppe       Pfad                 Bemerkung

                                                      Einfügen >           Öffnet den Dialog Importieren von
                                                      Felddefinitionen >   Felddefinitionen.
                                                      Importieren

                                                      Einfügen >           Öffnet den Dialog Exportieren von
                                                      Felddefinitionen >   Felddefinitionen.
                                                      Exportieren

                                                      Entfernen            Löscht die markierte Spalte.

                                                      Ändern               Derzeit nicht genutzt.

                                                      Definition anzeigen Öffnet den Dialog Spaltendefinition, in dem
                                                                          Details zur jeweiligen Spalte angezeigt werden.
                                                                            “Spaltendefinition” auf Seite E-129

                                         Liste        Lauf bilden          Öffnet den Dialog Lauf-Bildung.
                                                                            “Lauf-Bildung” auf Seite E-90


                                                      Topf bilden          Öffnet den Dialog Topf-Bildung.
                                                                            “Topf-Bildung” auf Seite E-83

                                                      Füllauftrag          Ändert den ausgewählten Auftrag zu einem
                                                                           Füllauftrag.
                                                                            “Füllaufträge” auf Seite E-65

                                                      Packmittelgruppe     Öffnet den Dialog Packmittelgruppen.
                                                      bilden

                                                      Automatisch          Bildet automatisch Packmittelgruppen.
                                                      Packmittelgruppen
                                                      bilden

                                                      Auftragsübersicht    Öffnet den Dialog Auftragsübersicht.
                                                                            “Auftragsübersicht” auf Seite E-62

                                                      Positionen           Öffnet den Dialog Positionen.
                                                                            “Positionen” auf Seite E-95

                                                      Glasarten            Öffnet den Dialog Glasarten.
                                                                            “Glasarten” auf Seite E-110

                                                      Bearbeitungen        Öffnet den Dialog Bearbeitungen.
                                                                            “Bearbeitungen” auf Seite E-105

                                                      Lose                 Öffnet den Dialog Lose.
                                                                            “Lose” auf Seite E-121

                                                      BDE                  Öffnet den Dialog BDE.
                                                                            “BDE” auf Seite E-117
2.50 / 01-2023




                 Tab. E-16   Übergreifende Kontextmenüs




                 A+W Production Grobplanung                                                                         E-137
                 Übergreifende Kontextmenüs                                                                Softwarereferenz




                                         Gruppe       Pfad                  Bemerkung

                                                      Details               Öffnet den Dialog Details.
                                                                             “Details” auf Seite E-113

                                                      Nacherfassung >       Öffnet den Dialog Entschichtungsflächen.
                                                      Entschichtung
                                                                             “Entschichtungsflächen” auf Seite E-134

                                                      Nacherfassung >       Öffnet den A+W CAD Designer (Shapes) zur
                                                      Sprossen              Nacherfassung von Sprossen.

                                                      Nacherfassung >       Öffnet denA+W CAD Designer (Bars) zur
                                                      Freie Formen          Nachbearbeitung der Modell-Daten.

                                                      Nacherfassung >       Öffnet den Dialog Übermengen-Editor zur
                                                      Übermengen            Nacherfassung von kaufmännischen und
                                                                            produktionstechnischen Übermengen.
                                                                             “Übermengen-Editor” auf Seite E-68

                                                      Arbeitsplan >         Öffnet den Dialog Umlastung zur
                                                      Maschinen-            Maschinenumlastung.
                                                      Umlastung
                                                                             Kapazitätsplanung: Softwarereferenz, “Ma-
                                                                              schinenumlastung” auf Seite E-175
                                                                            Die Ergebnisse der Maschinenzuordnung im
                                                                            Rahmen der Einlastung werden überschrieben.

                                                      Arbeitsplan >         Führt die Maschinenzuordnung für markierte
                                                      Maschinen-            Aufträge bzw. Positionen erneut durch.
                                                      Zuordnung
                                                                            Die Ergebnisse der Maschinenzuordnung im
                                                                            Rahmen der Einlastung werden überschrieben.

                                                      Arbeitsplan >         Zur Zeit nicht genutzt.
                                                      Arbeitsplan neu
                                                      berechnen

                                                      Positionen splitten   Öffnet den Dialog Positionssplit.
                                                                             “Positionssplit” auf Seite E-99

                                                      Beschaffungsart       Öffnet den Dialog Änderung der
                                                      ändern                Beschaffungsart.
                                                                             “Änderung der Beschaffungsart” auf
                                                                              Seite E-70
                                                                            Die Option funktioniert ausschließlich bei ESG
                                                                            und VSG.

                                                      Zugehörige            Öffnet den Dialog Dokumentenverknüpfungen.
                                                      Dokumente
                                                                             “Dokumentenverknüpfungen” auf
                                                                              Seite E-133

                                         Summen-      Umsortieren           Zur Zeit nicht genutzt.
                                         zeile
2.50 / 01-2023




                                                      Formatieren           Format oder Einheit für die Spalten auswählen,
                                                                            z. B. Datumsformate oder Längen-Einheiten.

                 Tab. E-16   Übergreifende Kontextmenüs



                 E-138                                                                      A+W Production Grobplanung
                 Softwarereferenz                                                           Übergreifende Kontextmenüs




                                         Gruppe       Pfad                 Bemerkung

                                                      Einfügen             Fügt ein neues Feld in die Summenzeile ein.
                                                                           Verschiedene Kategorien stehen zur Verfügung.

                                                      Einfügen >           Öffnet den Dialog Felddefinition, in dem Sie
                                                      Felddefinitionen >   Abfragen auf Datenbank-Tabellen und -Felder
                                                      Editieren            formulieren können. Diese Abfragen können Sie
                                                                           dann z. B. teile-, positions- oder
                                                                           auftragsbezogen einfügen.
                                                                            “Felddefinition” auf Seite E-101

                                                      Einfügen >           Öffnet den Dialog Importieren von
                                                      Felddefinitionen >   Felddefinitionen.
                                                      Importieren

                                                      Einfügen >           Öffnet den Dialog Exportieren von
                                                      Felddefinitionen >   Felddefinitionen.
                                                      Exportieren

                                         Filter                            Öffnet den Dialog (Filter Name). Mit der
                                                                           Schaltfläche [Verwalten] gelangen Sie zum
                                                                           Dialog Filter-Definition, in dem Sie Filter
                                                                           bearbeiten können.
                                                                            “Filter-Definition” auf Seite E-131

                 Tab. E-16   Übergreifende Kontextmenüs
2.50 / 01-2023




                 A+W Production Grobplanung                                                                          E-139
                 Übergreifende Kontextmenüs              Softwarereferenz
2.50 / 01-2023




                 E-140                        A+W Production Grobplanung
Grobplanung                E

                     Partindex




              A+W Production
                 Partindex                                                                 Index




                 Index
                 A                                       Filter konfigurieren E-29
                 Änderung der Beschaffungsart E-70       Filter-Definition E-131
                 Ansichten E-16                          Füllaufträge E-65
                 – Arbeiten mit der Liste E-23
                 – Filter konfigurieren E-29             G
                 – konfigurierbare Bestandteile E-17     Glasarten E-110
                 – konfigurieren E-19                    Grobplanung
                 – Register konfigurieren E-19           – Begriffe E-14
                 – Spalte definieren E-26
                 – Spalten konfigurieren E-21
                                                         K
                 – Summenzeile definieren E-26
                                                         Kapazitätsplanung E-14
                 – Summenzeile konfigurieren E-24
                                                         Kontextmenüs E-136
                 – Übungen E-33
                 – Weißer Screen E-32
                 Arbeitsplan E-125                       L
                 Arbeitsvorbereitung E-13                Laufbezeichnung ändern E-93
                 Auftrag zu Positionen hinzufügen E-98   Lauf-Bildung E-90
                 Aufträge E-34, E-59                     Läufe E-43, E-87
                 – fehlerhafte Angaben E-36              – auflösen E-49
                 – Kapazitätsplanung E-36                – Auftrag hinzufügen E-48
                 Auftragsübersicht E-62                  – Bezeichnung ändern E-93
                                                         – bilden E-46, E-90
                                                         – Laufstrategien E-45
                 B
                                                         – Sonderglas-Lauf E-92
                 BDE E-117
                                                         – verwalten E-49
                 Bearbeitungen E-105
                                                         Läufe auflösen E-49
                 – Vorgabezeiten ändern E-108
                                                         Läufe bilden E-46
                 Begriffe in der Grobplanung E-14
                                                         Läufe verwalten E-49
                 Beschaffungsart ändern E-70
                                                         Laufstrategien E-45
                 Bestellteile E-80
                                                         Liste E-23
                 Bestellteile-Topf E-80
                                                         Lose E-121
                 Betriebsdatenerfassung E-117

                                                         P
                 D
                                                         Pool E-34
                 Details E-113
                                                         Positionen E-50, E-95
                 Dokumente
                                                         – Auftrag hinzufügen E-98
                 – verknüpfen E-133
                                                         – Felddefinition E-101
                 Dokumentenverknüpfungen    E-133
                                                         – Import/Export Ansicht E-103
                                                         – splitten E-52, E-99
                 E                                       Positionssplit E-99
                 Eigenschaften von Register E-128
                 Entschichtungsflächen E-134
                                                         R
                 Export/Import Positionsansicht E-103
                                                         Rechtsklick E-136
                                                         Register
                 F                                       – Eigenschaften E-128
2.50 / 01-2023




                 Felddefinition E-101                    Register konfigurieren E-19
                 Filter                                  Reservierungsaufträge E-76
                 – bearbeiten E-130                      Reservierungsaufträge-Topf E-76
                 – definieren E-131


                 A+W Production Grobplanung                                                E-143
                 Index                                              Partindex




                 S
                 Sonderglas-Lauf bilden E-92
                 Spalte definieren E-26
                 Spalten
                 – Definition E-129
                 Spalten konfigurieren E-21
                 Spaltendefinition E-129
                 Status setzen E-14
                 Summenzeile definieren E-26
                 Summenzeile konfigurieren E-24

                 T
                 Topfbezeichnung ändern E-85
                 Topf-Bildung E-83
                 Töpfe E-37, E-73
                 – auflösen E-42
                 – Aufträge hinzufügen E-40
                 – Bestellteile E-80
                 – Bezeichnung ändern E-85
                 – bilden E-83
                 – erstellen E-39
                 – Reservierungsaufträge E-76
                 Töpfe auflösen E-42
                 Töpfe erstellen E-39

                 U
                 Übergreifende Dialoge E-124
                 Übermengen-Editor E-68
                 Übersichtsdialoge E-16
                 Übungen
                 – Ansichten E-33

                 V
                 Vorgabezeiten ändern E-108
                 Vorgang suchen E-53

                 W
                 Weißer Screen   E-32
2.50 / 01-2023




                 E-144                            A+W Production Grobplanung

