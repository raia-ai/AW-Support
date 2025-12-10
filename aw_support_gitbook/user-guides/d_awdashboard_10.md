---
title: "D AWDashboard 1.0"
category: "user_manuals"
product: "Unknown"
doc_type: "Unknown"
language: "EN"
tags: ["D_AWDashboard_1.0"]
version: "1.0"
last_updated: "2025-12-10"
description: "Dashboard                           Deutsch                 A+W Dashboard                  Vorspann                                 Vorspann                             In diesem Teil der Dokumentation finden Sie editorische Notizen.                               Revisionsübersicht                             A+W Dashboard            Beschreibung                             Version / Datum                              1.00 / 04-2014           Ersterstellung                                Editor"
source_file: "D_AWDashboard_1.0.pdf"
---


# D AWDashboard 1.0

Dashboard




                      Deutsch




            A+W Dashboard
                 Vorspann




                            Vorspann
                            In diesem Teil der Dokumentation finden Sie editorische Notizen.


                            Revisionsübersicht
                            A+W Dashboard            Beschreibung
                            Version / Datum

                            1.00 / 04-2014           Ersterstellung



                            Editorial
                            Das Editorial enthält Informationen zu folgenden Themen:
                            •   Anmerkungen zu diesem Dokument
                            •   Urheberrechte
                            •   Warenzeichen
                            •   Kontakte

                            Anmerkungen zu diesem Dokument
                            Diese Veröffentlichung ist ausschließlich für Endanwender von
                            A+W Dashboard gedacht. Das Produkt A+W Production Cockpit ist in einem
                            separaten Dokument beschrieben.
                            Diese Dokumentation und die darin beschriebene Software werden nur in Li-
                            zenz vergeben und dürfen nur gemäß dieser Lizenz verwendet und kopiert
                            werden. Der Inhalt der Dokumentation dient nur der Information und kann je-
                            derzeit ohne Vorankündigung geändert werden. Bei der Zusammenstellung
                            von Texten und Abbildungen wurde mit größter Sorgfalt vorgegangen. Trotz-
                            dem können Fehler nicht vollständig ausgeschlossen werden. A+W Software
                            GmbH übernimmt keine Haftung für Fehler oder Ungenauigkeiten, es sei
                            denn, diese beruhen auf vorsätzlichem oder grobfahrlässigem Handeln.
                            Dieses Dokument beschreibt A+W Dashboard anhand von Beispielen.

                            Urheberrechte
                            © 2014, A+W Software GmbH, alle Rechte, auch des Nachdrucks, der Her-
                            stellung von Kopien und der Übersetzung, bleiben vorbehalten.
                            Die Dokumentation darf nur gemäß dem Lizenzvertrag ganz oder in Teilen ko-
                            piert, in einem Archivierungssystem gespeichert oder in irgendeiner anderen
                            Form übertragen werden. Ohne die vorherige schriftliche Genehmigung von
                            A+W Software GmbH darf die Dokumentation weder elektronisch, noch me-
                            chanisch, per Aufzeichnung oder in sonstiger Form übertragen werden.
1.00 / 04-2014




                 2                                                                     A+W Dashboard
                                                                                                     Vorspann




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

                                 Zentrale@a-w.com

                                 http://www.a-w.com
1.00 / 04-2014




                 A+W Dashboard                                                                               3
                 Inhalt




                          Inhalt
                          Vorspann ................................................................................................................... 2
                           Revisionsübersicht ................................................................................................. 2
                           Editorial .................................................................................................................. 2

                          Tutorial                                                                                                                  5
                          Dokumentation ........................................................................................................... 6
                          A+W Dashboard ........................................................................................................ 7
                          Darstellung der Daten .............................................................................................. 10
                          Programm bedienen ................................................................................................ 12
                            Dashboard ............................................................................................................ 13
                            Einstellungen ........................................................................................................ 14
                          Aufbau der Anzeigen ............................................................................................... 15
                            Struktur ................................................................................................................. 15
                            Control Editor ....................................................................................................... 18
                            Page Editor ........................................................................................................... 25
                            View Editor ........................................................................................................... 26
                          Anzeige erstellen ..................................................................................................... 27
                            Zusammenfassung ............................................................................................... 27
                            Vorbereitungen ..................................................................................................... 28
                            Control anlegen .................................................................................................... 29
                            Seite zusammenstellen ........................................................................................ 32
                            Ansicht konfigurieren ............................................................................................ 37

                          Index                                                                                                                  41
1.00 / 04-2014




                 4                                                                                                          A+W Dashboard
        Tutorial




A+W Dashboard
                 Dokumentation                                                                                Tutorial




                                 Dokumentation
                                 Das Tutorial zu A+W Dashboard zeigt Ihnen, wie Sie mit den Ansichten zu den
                                 Produktions-Snapshots arbeiten und wie Sie diese einrichten.

                                 Themenblöcke
                                 In diesem Tutorial finden Sie folgende Themenblöcke:
                                 •    A+W Dashboard
                                 •    Darstellung der Daten
                                 •    Programm bedienen
                                 •    Aufbau der Anzeigen
                                 •    Anzeige erstellen

                                 Vorausgesetzte Kenntnisse
                                 Das Tutorial richtet sich an Mitarbeiter, die die Produktionsabläufe kennen und
                                 steuern. Kenntnisse zur Bedienung eines Touchscreens werden vorausge-
                                 setzt. Im Einzelnen sind das folgende Gesten: Tippen, Wischen, Vergrößern
                                 und Verkleinern.
                                 Das Programm kann auch mit einer Maus bedient werden. Auf die Verwen-
                                 dung einer Maus wird nur eingegangen, wenn sie sich erheblich von der Be-
                                 dienung des Touchscreens unterscheidet.

                                 Lesehinweis
                                 Der Inhalt einer Lerneinheit baut auf den Kenntnissen auf, die in der voraus-
                                 gegangenen Einheit vermittelt wurden. Es ist daher sinnvoll, keine Lerneinhei-
                                 ten zu überspringen.

                                 Darstellungskonventionen
                                 Einzelne Satzteile werden in besonderer Form dargestellt. Diese haben fol-
                                 gende Bedeutung:

                                 Kursiv                       sind Zeichenfolgen ausgezeichnet, die Elemente der
                                                              Software bezeichnen, z. B. die Auswahl Status.

                                 Fett                         sind Zeichenfolgen ausgezeichnet, die Sie über die Tas-
                                                              tatur eingeben, z. B.: Geben Sie den Wert 0 ein.

                                 >                            Mit dem sogenannten Brotkrumenpfad ist der Weg
                                                              kennzeichnet, auf dem Sie eine Ansicht öffnen, z. B.
                                                              Dashboard > Menüleiste > Editor.

                                 []                           Eckige Klammern bezeichnen Schaltflächen im Dialog,
                                                              z. B.: Mit [Einstellungen] legen Sie die Sprache fest.

                                 <>                           Spitze Klammern bezeichnen Tasten oder Tastenkombi-
                                                              nationen auf der Tastatur, z. B.: Mit <F5> aktualisieren
1.00 / 04-2014




                                                              Sie den Browser.




                 6                                                                                 A+W Dashboard
                 Tutorial                                                                             A+W Dashboard




                                         A+W Dashboard
                                         Das A+W Dashboard ist ein Service mit einer Web-basierten Oberfläche, um
                                         KPI-Daten aus der Produktion und aus ERP-Systemen, z. B. A+W Enterprise,
                                         A+W Business, anzuzeigen.
                                         A+W Dashboard kann in jedem Browser der neuesten Version gestartet wer-
                                         den. Dazu kann die Adresse auf den gewünschten Server als Favorit oder als
                                         Link auf dem Desktop hinterlegt werden – wie alle Internet-Adressen.

                                         Ziel des Programms
                                         A+W Dashboard ist ein Tool zur Visualisierung der Produktion. Es zeigt die ak-
                                         tuelle Leistung der Maschinen und Mitarbeiter in grafischer Form.




                 Abb. 1     Monitor-Anzeige (Beispiele)


                                         Zur Auswertung werden die Datenbanktabellen mit den BDE-Buchungen her-
                                         angezogen. Dabei wird in der Regel ein Zeitraum von max. 24 Stunden be-
                                         rücksichtigt. Damit grenzt sich A+W Dashboard von A+W Discovery ab, das
                                         statistische Auswertungen über längere Zeiträume ermöglicht.

                                             Korrekte Darstellung nur mit korrekten BDE-Buchungen
                                             Voraussetzung für aussagekräftige Anzeigen sind lückenlose BDE-Bu-
                                             chungen.
1.00 / 04-2014




                 A+W Dashboard                                                                                       7
                 A+W Dashboard                                                                       Tutorial




                                        A+W Dashboard verbindet die Produktions-Software A+W Production und
                                        das A+W Production Terminal. Die BDE-Daten werden über den PPS-Web-
                                        service ausgelesen.




                 Abb. 2    Systemportfolio der A+W Software GmbH für den Bereich Flachglas
1.00 / 04-2014




                 8                                                                           A+W Dashboard
                 Tutorial                                                                       A+W Dashboard




                                 Leistungsmerkmale
                                 A+W Dashboard zeigt wichtige Kennzahlen an den entscheidenden Stellen
                                 der Produktion an und sorgt damit für hohe Transparenz.
                                 In Echtzeit erhalten Sie Auskunft über einzelne Produktionsbereiche wie Zu-
                                 schnitt, ISO-Linien, Bearbeitungen, ESG-Fertigung: Sie sehen z. B. den aktu-
                                 ellen Nutzungsgrad, den Status jeder Maschine, den Verlauf der Produktivität.
                                 Das Programm kann sowohl auf großen Monitoren in den verschiedenen Ab-
                                 teilungen der Fertigung eingesetzt werden als auch auf mobilen Endgeräten
                                 wie Smartphones, Tablet-Computern oder PDAs. Voraussetzung ist ein Inter-
                                 net-Browser und ein Zugang zum Programm (Adresse, Benutzer-Account).
                                 Damit dient die Anzeige als Online-Monitoring-Tool und Entscheidungsmittel,
                                 wenn sich im Laufe einer Schicht Maschinenzustände ändern oder die zu fer-
                                 tigenden Stückzahlen nicht eingehalten werden können.
                                 Bei Störungen können die Mitarbeiter die Situation exakt kommunizieren und
                                 in vielen Fällen bereits eigene Lösungsansätze vorschlagen.
                                 A+W Dashboard enthält vordefinierte Anzeigen, kann aber auch individuell
                                 auf die jeweilige Maschine oder Abteilung angepasst werden. Damit können
                                 Sie die kritischen Stellen Ihrer Produktion im Auge behalten und notfalls sofort
                                 eingreifen.
1.00 / 04-2014




                 A+W Dashboard                                                                                 9
                 Darstellung der Daten                                                                           Tutorial




                                            Darstellung der Daten
                                            Die Auswertungen der BDE-Buchungen werden auf verschiedene Arten visu-
                                            alisiert. Sie können in die Anzeigen hinein- und herauszoomen und mit Wi-
                                            schen die Seiten wechseln.




                          A                B                         C                 D                  E
                 A Ampel                              C Punktediagramm                E Tacho
                 B Kreis (Kuchen)                     D Balkendiagramm
                 Abb. 3       Arten der Visualisierung (Beispiele)


                                            Jede dieser Darstellungsarten können Sie so einrichten, wie es den Erforder-
                                            nissen des betrachteten Produktionsbereichs und der Überwachung ent-
                                            spricht.

                                            Ampel (A)
                                            Die Ampel zeigt den aktuellen Status einer Erfassungsstelle an. Die Bedeu-
                                            tung der Farben können Sie selbst festlegen. Diese Anzeige ist für Statusan-
                                            zeigen über sehr kurze Zeiträume sinnvoll, z. B. um darzustellen, ob eine
                                            Maschine in Betrieb oder ausgefallen ist.

                                            Kreisdiagramm (B)
                                            Das Kreisdiagramm zeigt die Anteile der gemeldeten Maschinenstatus über
                                            einen selbst definierten Zeitraum an. Standardmäßig sind das die letzten
                                            24 Stunden. Damit wird die Summe der Ausfallzeiten über alle Schichten im
                                            Zeitraum sichtbar.
                                            Diese Anzeige ist geeignet, den Betrieb ähnlicher Maschinen miteinander zu
                                            vergleichen.
                                            In der Anzeige können einzelne Farben ausgeblendet werden, damit das Ver-
                                            hältnis der anderen beiden Farbanteile zueinander deutlicher wird.

                                            Punktediagramm (C)
                                            Die Linie zeigt die Buchungen eines vergangenen Zeitraums verteilt auf einen
                                            Anzeigezeitraum an, z. B. die Buchungen der letzten Stunde verteilt auf den
                                            Anzeigezeitraum. Ein Punkt zeigt die Summe pro Gruppierung, z. B. pro Mi-
                                            nute, pro Stunde, pro Tag.
1.00 / 04-2014




                                            Die Ziel-Stückzahl und der Durchschnitt können durch durchgehende waage-
                                            rechte Linien angezeigt werden, so dass die Über- oder Untermengen der tat-
                                            sächlichen Stückzahlen deutlich wird.


                 10                                                                                    A+W Dashboard
                 Tutorial                                                               Darstellung der Daten




                                 Diese Anzeige ist geeignet, längere Zeiträume darzustellen, jedoch max.
                                 24 Stunden. Ein rapider Abfall der Kurve könnte bei einer ISO-Linie z. B. be-
                                 deuten, dass die dass die Einzelgläser sehr groß waren und daher weniger
                                 Einheiten produziert werden konnten.

                                 Balkendiagramm (D)
                                 Das Balkendiagramm stellt statistische Daten dar, die über SQL-Abfragen er-
                                 hoben wurden. Für eine Konfiguration der Ansicht müssen diese Statistiken
                                 vorhanden sein.

                                 Tacho (E)
                                 Der Tacho zeigt die aktuelle Auslastung an. Dazu wird die Anzahl der gebuch-
                                 ten Stückzahlen der letzten Stunde betrachtet. Die rot-gelb-grün-Markierung
                                 zeigt an, wie die Stückzahlen bewertet sind.
                                 Die Anzeige ist geeignet für kurze Zeiträume mit einem relativ hohen Durch-
                                 satz.
1.00 / 04-2014




                 A+W Dashboard                                                                             11
                 Programm bedienen                                                                                        Tutorial




                                            Programm bedienen
                                            A+W Dashboard kann sowohl über den Touchscreen als auch mit der Maus
                                            bedient werden.
                                            Auf der Startseite (Monitor) werden die verschiedenen definierten Ansichten
                                            (Views) angezeigt.


                                            A




                                            B


                                                                                                                         C
                                            A Zurück zur Startseite (Monitor)              C Einstellungen
                                            B Menüleiste
                                            Abb. 4        Schaltflächen auf dem Monitor


                                            Die folgenden Funktionen gelten in allen Anzeigen in A+W Dashboard.


                 Funktion                            Bedienung

                 Menüleiste (B) anzeigen oder verber- Nach unten wischen (Rechtsklick).
                 gen

                 Zur Startseite (Monitor)            Auf den Pfeil (A) tippen (klicken).

                 Ansicht aktivieren                  Mit einmal tippen (Linksklick) fährt die Ansicht etwas hoch und die konfigu-
                                                     rierten Seiten schalten nacheinander durch.
                                                     Nochmal tippen (klicken) öffnet die Ansicht.
                                                      “Dashboard” auf Seite 13

                 Bearbeiten oder anlegen             Auf die entsprechende Editor-Schaltfläche in der Menüleiste (B) tippen (kli-
                                                     cken).

                 Einstellungen der Benutzerober-     Auf die Schaltfläche (C) tippen (klicken).
                 fläche (GUI) bearbeiten
                                                      “Einstellungen” auf Seite 14
1.00 / 04-2014




                 12                                                                                           A+W Dashboard
                 Tutorial                                                                                  Programm bedienen




                                             Dashboard
                                             Im sogenannten Dashboard (Armaturenbrett, Instrumententafel) werden die
                                             Informationen in verdichteter, grafischer Form visualisiert.
                                             Die Daten werden zyklisch aktualisiert und können damit die aktuelle Produk-
                                             tion abbilden.




                                                                                                                             A




                                                                                                                             B




                                                                                                                             C


                 A Anzeige der konfigurierten Seiten      B Ausgewählte View (Ansicht)      C Menüleiste mit Schaltflächen
                 Abb. 5        Dashboard und Menüleisten


                 Funktion                              Bedienung

                 Menüleisten (A + C) anzeigen oder     Nach unten wischen (oder Rechtsklick).
                 verbergen

                 Konfigurierte Seite in das Dashboard Im Monitor auf die gewünschte Ansicht tippen (klicken).
                 laden
                                                       “Dashboard” auf Seite 13

                 Ansicht vergrößern oder verkleinern Mit zwei Fingern auseinanderziehen oder zusammenschieben.
                 (Zoom)                              Auf Bildschirmen, die mit der Maus bedient werden können, wird diese
1.00 / 04-2014




                                                     Funktion nicht genutzt.

                 Seiten wechseln (durchschalten)       Über ein Control wischen (oder Doppelklick).



                 A+W Dashboard                                                                                               13
                 Programm bedienen                                                                                      Tutorial




                 Funktion                             Bedienung

                 Werte als Zahlen anzeigen            Im Kreis- oder im Balkendiagramm auf einen Bereich tippen (Maus darüber
                                                      halten).

                 Farbbereich ausblenden               Auf einen Farbbereich tippen. Damit können Sie das Verhältnis der verblei-
                                                      benden beiden Farbbereiche zu einander besser erkennen.

                 Schaltflächen                        • Automatik ein/aus:
                                                        Seiten werden zyklisch gewechselt (durchgeschaltet).

                                                      • Control Editor:
                                                        Controls anlegen oder bearbeiten.
                                                          “Control Editor” auf Seite 18
                                                      • Page Editor:
                                                        Controls zu einer Seite (Page) zusammenstellen.
                                                          “Page Editor” auf Seite 25
                                                      • View Editor:
                                                        Seiten zu einer Ansicht (View) zusammenstellen.
                                                          “View Editor” auf Seite 26
                                                      • Einstellungen
                                                        Sprache und Farbe der Bedienoberfläche (GUI) einstellen




                                             Einstellungen
                                             Die Einstellungen können aus jeder Anzeige heraus geöffnet werden. Sie gel-
                                             ten nur für den angeschlossenen Monitor.


                                             A


                                             B

                                             C

                                             D




                                             A Dialog Einstellungen schließen         C Sprache
                                             B Mandant                                D Farbschema
                                             Abb. 6       Einstellungen der Bedienoberfläche


                                             Mit der Einstellung des Farbschemas können Sie die Darstellung an die Um-
                                             gebung anpassen, in der der Monitor steht. Ein helles Farbschema eignet sich
                                             z. B. für Orte mit schlechteren Lichtverhältnissen.
1.00 / 04-2014




                 14                                                                                            A+W Dashboard
                 Tutorial                                                                                Aufbau der Anzeigen




                                         Aufbau der Anzeigen
                                         Sie können alle Anzeigen nach Ihren Erfordernissen erstellen und nachträg-
                                         lich bearbeiten.


                                         Struktur
                                         Die Anzeige in A+W Dashboard ist aus verschiedenen Elementen aufgebaut,
                                         die in einem hierarchischen Verhältnis zueinander stehen.




                      A           B      A                                                      C
                 A Control                                            C View (Ansicht)
                 B Page (Seite)
                 Abb. 7        Monitor


                 Ebene                   Definition

                 Control (A)             Ein Control ist die kleinste Einheit einer Ansicht. Es ist das Anzeigeelement, das die
                                         Daten visualisiert.
                                         Das Control wird z. B. als Ampel, Kreisdiagramm, Punktdiagramm oder Tacho ange-
                                         legt.

                 Page (B)                Eine Page (Seite) ist aus verschiedenen Controls zusammengesetzte.

                 View (C)                Die View (Ansicht) stellt mindestens eine Seite dar.
                                         In der Ansicht können mehrere Seiten hinter einander liegen. Die View kann durchge-
                                         schaltet werden, damit die Seiten abwechselnd in den Vordergrund geholt werden.
1.00 / 04-2014




                 A+W Dashboard                                                                                               15
                 Aufbau der Anzeigen                                                                                                                      Tutorial




                                                                        In einer Ansicht können hinter der sichtbaren Seite weitere Seiten liegen, auf
                                                                        die durchgeschaltet werden kann.



                                                                                  40              60




                                                                            20                         80


                                                         40             60




                           40             60
                                                    20                           80
                                                                                        0   100
                                                                                                                                            ISO-Linie 1

                      20                       80             0   100
                                                                                                                                  ISO-Linie 2
                                0   100
                                                                                                                    ISO-Linie 3

                 Abb. 8                        Aufbau einer Ansicht mit drei Seiten


                                                                        In diesem Beispiel sind drei Seiten für die drei ISO-Linien eingerichtet. Diese
                                                                        Seiten liegen in der Ansicht neben einander. Im Beispiel wird die Seite der
                                                                        ISO-Linie 3 angezeigt.
                                                                        •              Die Seiten der Linien 2 und 3 werden durch Wischen angezeigt.
                                                                        •              Der statische Zustand kann in einen automatischen Wechsel umgeschaltet
                                                                                       werden.
                                                                        Die Umschaltung ist in den Kurzbeschreibungen für das Dashboard erklärt.
                                                                         “Dashboard” auf Seite 13
1.00 / 04-2014




                 16                                                                                                                             A+W Dashboard
                 Tutorial                                                                                        Aufbau der Anzeigen




                                               Programmtechnisch sieht der Aufbau eine Ansicht (View) so aus:


                                                                View                              View




                                            Page                                 Page                              Page




                                            Pane                                 Pane                              Pane




                                   Pane                  Pane             Pane           Pane             Pane             Pane




                           Pane            Pane




                        Control           Control               Control                         Control                   Control


                 Abb. 9           Konzept der Struktur


                 Ebene                         Definition

                 Control                       Ein Control ist die kleinste Einheit einer Ansicht. Das Control wird als z. B. Ampel,
                                               Kreisdiagramm, Punktdiagramm oder Tacho angelegt.
                                               Ein Control kann mehreren Panes zugeordnet werden.

                 Pane                          Panes bilden die Aufteilung einer Seite. In einem Pane wird jeweils ein Control plat-
                                               ziert.
                                               Panes können weitere Panes enthalten, um die Seite weiter zu gliedern.

                 Page                          Eine Page (Seite) ist in Panes unterteilt, in denen die Controls platziert sind.
                                               Eine Page kann mehreren Views zugeordnet werden.

                 View                          Die View (Ansicht) fasst verschiedene Pages zusammen.
                                               Eine Page kann in mehrere Views aufgenommen werden, aber in einer View nicht
                                               doppelt.

                                               Um eine View einzurichten, muss der Baum von unten nach oben aufgebaut
                                               werden.
                                                “Seite zusammenstellen” auf Seite 32
1.00 / 04-2014




                 A+W Dashboard                                                                                                         17
                 Aufbau der Anzeigen                                                                              Tutorial




                                            Control Editor
                                            Im Control Editor verwalten Sie die Controls. Dabei werden aktuelle Daten ge-
                                            holt und angezeigt. Dadurch können Sie prüfen, ob die gewählten Einstellun-
                                            gen sinnvoll sind.




                                                                                                              A




                                                                                                              B
                                                                                                                   C




                           D




                           E


                 A Control Editor – Ebene 1                           C Control Editor – Ebene 2
                 B Schaltfläche zur Ebene 2                           D Schaltfläche zurück zur Ebene 1
                                                                      E Menüleiste mit Schaltflächen
                 Abb. 10       Control Editor – Ebene 1 und 2


                                            Alle Editoren sind nach demselben Prinzip aufgebaut:
                                            •   Auf der Ebene 1 wählen Sie ein Control aus, um es zu bearbeiten, oder le-
                                                gen ein neues an.
1.00 / 04-2014




                                            •   Auf der Ebene 2 bearbeiten Sie ein Control.
                                            •   Die Menüleisten öffnen Sie mit schnellem vertikalem Wischen (Rechts-
                                                klick).


                 18                                                                                       A+W Dashboard
                 Tutorial                                                                      Aufbau der Anzeigen




                                 Die Einstellungsmöglichkeiten eines Controls hängen vom Controltyp ab:
                                 •   “Tacho” auf Seite 20
                                 •   “Punktdiagramm (Graph)” auf Seite 21
                                 •   “Balkendiagramm” auf Seite 22
                                 •   “Kreis (Kuchen)” auf Seite 23
                                 •   “Ampel” auf Seite 24

                                 Datenquellen
                                 A+W Dashboard wertet zur Berechnung die BDE-Meldungen von Stammda-
                                 ten und Fließ-Daten aus. Dabei werden immer die Stückzahlen ausgelesen,
                                 auch wenn Auftragspositionen insgesamt fertig gemeldet werden.
                                 Voraussetzung für aussagekräftige Anzeigen sind lückenlose BDE-Buchun-
                                 gen. Für die Berechnung der Daten werden in der Regel die Buchungen der
                                 letzten 24 Stunden des eingestellten Zeitraums berücksichtigt.
                                 In Einzelnen werden die folgenden Datenquellen ausgelesen:
                                 •   Stammdaten:
                                     – awbar_stellen
                                     – awbar_status

                                 •   Fließdaten:
                                     – awbar_booking
                                        Diese Daten werden vorzugsweise als Punktdiagramm und als Tacho
                                        angezeigt.
                                     – bde_stat_es
                                        Diese Daten werden vorzugsweise als Ampel und als Kuchen ange-
                                        zeigt.
                                 •   KPI-Daten: (zur Zeit nur CANTOR)
                                     – SQL-Abfragen
                                     Diese Daten werden vorzugsweise als Punkt- oder Balkendiagramm ange-
                                     zeigt.


                 Datenquelle     Zur Auswahl stehen Buchung, Status und KPI.

                 Controltyp      Die Auswahl der verfügbaren Controltypen hängt von der eingestellten Datenquelle
                                 ab (Beispiele):
                                 • Buchung: Tacho oder Punktediagramm
                                 • BDE-Status: Ampel oder Kuchen
                                 • KPI: Balken, Punkte, Tacho, Kuchen
                                 (KPI: Key Performance Indikator - Kritischer Erfolgsfaktor (= Leistungskennzahl))
1.00 / 04-2014




                 A+W Dashboard                                                                                       19
                 Aufbau der Anzeigen                                                                                      Tutorial




                                            Tacho

                                                      A                                       B




                                            A Datenquelle                                B Controltyp
                                            Abb. 11         Definition Tacho


                 Feld                       Beschreibung

                 Datenquelle                Die Auswahl der Datenquelle legt fest, ob Fließdaten, Stammdaten oder KPI-Daten
                                            ausgewertet werden sollen.

                 Controltyp                 Die Auswahl des Controltyps legt fest, welche Felder für die Definition angezeigt wer-
                                            den.

                 Gruppierung Modus          Minute, Stunde, Tag, Woche, Monat, Quartal, Jahr:
                                            Die Gruppierung legt fest, welche Daten zu einer Gruppe zusammengefasst werden.
                                            Die Gruppen werden im Tacho als Werte zwischen 0 und dem Maximalwert ange-
                                            zeigt. Die Angaben werden aus dem Zeitstempel der BDE-Meldung gelesen.
                                            Durchschnitt, aufsummieren, niedrigster Wert, höchster Wert:
                                            Der Modus legt fest, wie die Werte der Gruppe betrachtet werden sollen.

                 Maximalwert                Endwert der Anzeige.

                 Endwert gelber Bereich     Endwert des gelben Bereichs.

                 Endwert roter Bereich      Endwert des roten Bereichs.


                      Berechnungsbeispiele Tacho

                      Gruppierung                                                     Modus
1.00 / 04-2014




                                     Gemeldete Stück      Durchschnitt     Aufsummiert     höchster Wert    niedrigster Wert

                      Monat          10, 30, 20, 50            27,5             110               50              10




                 20                                                                                            A+W Dashboard
                 Tutorial                                                                          Aufbau der Anzeigen




                                    Punktdiagramm (Graph)




                                    Abb. 12       Definition Punktediagramm



                 Feld               Beschreibung

                 Erfassungsstelle   Erfassungsstelle, deren Stückzahlen angezeigt werden sollen.

                 Zielmarke          Horizontale Linie im Diagramm, die anzeigt, ob der Sollwert erreicht wurde.

                 Durchschnitt       Horizontale Linie im Diagramm, die den Durchschnitt über den ausgewerteten Zeit-
                                    raum anzeigt.

                 On, Off            Funktion kann aktiviert oder deaktiviert werden.

                                    Die übrigen Felder sind ausführlich zum Tacho beschrieben.
                                     “Tacho” auf Seite 20
1.00 / 04-2014




                 A+W Dashboard                                                                                     21
                 Aufbau der Anzeigen                                                                   Tutorial




                                       Balkendiagramm




                                       Abb. 13        Definition Balkendiagramm



                 Feld                  Beschreibung

                 Statistik             SQL-Abfrage, deren Daten angezeigt werden sollen.

                 Zeitspanne            Zeitraum, der in die Anzeige einfließen soll.

                                       Die übrigen Felder sind ausführlich zum Tacho beschrieben.
                                        “Tacho” auf Seite 20
1.00 / 04-2014




                 22                                                                             A+W Dashboard
                 Tutorial                                                                         Aufbau der Anzeigen




                                    Kreis (Kuchen)




                                    Abb. 14        Definition Kreis



                 Feld               Beschreibung

                 Erfassungsstelle   Erfassungsstelle, deren Verteilung der Statuszeiten angezeigt werden soll.

                 Grüner Status      Gemeldeter Status, für den ein grüner Bereich angezeigt werden soll. In der Regel ist
                                    das die Meldung für betriebsbereit (in Betrieb).

                 Gelber Status      Gemeldeter Status, für den ein gelber Bereich angezeigt werden soll.
                                    Sie können beliebig viele Status auswählen, jedoch lässt die Anzeige dann immer
                                    mehrere Interpretationen (durch den Betrachter) zu.
                                    Alle nicht eingestellten Status werden rot angezeigt.

                 Zeitraum           Zeitraum, auf den zurückgeschaut werden soll in hh:mm:ss (maximal 24 Std). Alle Sta-
                                    tus innerhalb des Zeitraums werden berücksichtigt. Das Feld wird nicht angezeigt,
                                    wenn Statusmeldungen ausgewertet werden.
1.00 / 04-2014




                 A+W Dashboard                                                                                        23
                 Aufbau der Anzeigen                                                                               Tutorial




                                       Ampel




                                       Abb. 15       Definition Ampel



                 Feld                  Beschreibung

                 Erfassungsstelle      Erfassungsstelle, deren Status angezeigt werden soll.

                 Grüner Status         Gemeldeter Status, bei dem die Ampel grün anzeigen soll. In der Regel ist das die
                                       Meldung für betriebsbereit (in Betrieb).

                 Gelber Status         Gemeldeter Status, bei dem die Ampel gelb anzeigen soll. In der Regel sind das die
                                       Meldungen für Pause und Wartung.
                                       Sie können beliebig viele Status auswählen, jedoch lässt die Anzeige dann immer
                                       mehrere Interpretationen (durch den Betrachter) zu.
                                       Alle nicht eingestellten Status werden rot angezeigt.

                                          Status mehrfach vergeben
                                          Wenn Sie den Status betriebsbereit für den grünen Bereich und Wartung
                                          für den gelben Bereich ausgewählt haben, dann ist die Zuordnung eindeu-
                                          tig.
                                          Wenn Sie versehentlich z. B. den Status betriebsbereit zusätzlich auch für
                                          den gelben Bereich ausgewählt haben, dann wird der gelbe Bereich auch
                                          dann angezeigt, wenn die Maschine betriebsbereit ist. Der niedrigere Sta-
                                          tus ist also immer ausschlaggeben.
1.00 / 04-2014




                 24                                                                                     A+W Dashboard
                 Tutorial                                                                              Aufbau der Anzeigen




                                            Page Editor
                                            Im Page Editor verwalten Sie die Seiten. Auf einer Seite sind die Controls zu-
                                            sammengefasst, die gemeinsam angezeigt werden sollen.




                 A

                 B




                                    C                                                     D
                 A Listen der Controls Listen nach Buchungstypen        C Einstellung der Trenner (Magnet-Raster)
                 B Trenner zur Aufteilung in Panes                      D Controls, die der Page zugewiesen sind
                 Abb. 16      Page Editor


                                            Panes geben die Aufteilung der Seite vor. Für die schnelle Platzierung der Pa-
                                            nes steht ein Magnet-Raster zur Verfügung, das Sie selbst skalieren können.

                                            Rasterlinien




                                            Die Anzahl der waagerechten und senkrechten Reihen können Sie über die
1.00 / 04-2014




                                            Pfeil-Schalter erhöhen oder verringern.
                                            Siehe dazu auch die Beschreibung zum Control Editor:
                                             “Control Editor” auf Seite 18


                 A+W Dashboard                                                                                         25
                 Aufbau der Anzeigen                                                                                    Tutorial




                                            View Editor
                                            Im View Editor verwalten Sie die Ansichten. In einer Ansicht sind die Seiten
                                            zusammengefasst, die nacheinander angezeigt werden sollen.




                 A




                                             B                                            C
                 A Liste der angelegten Views (Ansichten)               C Liste der Seiten, die der aktuellen Ansicht zugeordnet
                 B Liste der angelegten Pages (Seiten)                    sind

                 Abb. 17      View Editor


                                            Siehe dazu auch die Beschreibung zum Control Editor:
                                             “Control Editor” auf Seite 18
1.00 / 04-2014




                 26                                                                                          A+W Dashboard
                 Tutorial                                                                           Anzeige erstellen




                                 Anzeige erstellen
                                 In diesem Abschnitt lernen Sie, wie Sie eine vollständige Ansicht (View) Schritt
                                 für Schritt aufbauen.


                                 Zusammenfassung
                                 Lernziele

                                 • Aspekte der Planung kennenlernen.
                                 • Arbeitsschritte aus der Aufgabenstellung entwickeln.
                                 • Eine Ansicht vom Control bis zur View aufbauen.


                                 Nutzen

                                 • Mit der Kenntnis der Einstellungen wird deutlich, wozu welche Anzeigen geeignet
                                   sind.
                                 • Mit dem Verständnis der Funktionsweise werden die Anzeigen besser zu
                                   analysieren.


                                 Merke

                                 Control                    Ein Control ist die kleinste Einheit einer Ansicht. Es ist
                                                            das Anzeigeelement, das die Daten visualisiert.
                                                            Das Control wird als Ampel, Kreisdiagramm,
                                                            Punktdiagramm oder Tacho angelegt.

                                 Datenquelle                Die Auswahl der Datenquelle legt fest, ob Fließdaten,
                                                            Stammdaten oder KPI-Daten ausgewertet werden.

                                 Controltyp                 Die Auswahl des Controltyps legt fest, welche Felder für
                                                            die Definition angezeigt werden.

                                 Page                       Eine Page (Seite) ist aus verschiedenen Controls
                                                            zusammengesetzt.

                                 Pane                       Ein Pane ist der selbst definierte Bereich einer Page, in
                                                            den ein Control platziert wird. Panes werden durch
                                                            Trenner festgelegt.
                                                            Eine Page kann in mehrere Panes unterteilt werden.

                                 Magnet-Raster              Das Magnet-Raster ist ein Hilfsmittel, mit dem die
                                                            Trenner ausgerichtet werden. Die Trenner müssen nicht
                                                            zwingend auf eine Rasterlinie gelegt werden.

                                 View                       Die View (Ansicht) stellt die Seiten im Dashboard dar. In
                                                            der Ansicht können mehrere Seiten hinter einander lie-
                                                            gen.
                                                            Die Seiten können durchgeschaltet werden, damit sie
1.00 / 04-2014




                                                            abwechselnd in den Vordergrund geholt werden.




                 A+W Dashboard                                                                                       27
                 Anzeige erstellen                                                                        Tutorial




                                     Vorbereitungen
                                     Grundsätzlich können für jede Maschine bis zu vier Controls angelegt werden.
                                     Bei z. B. 10 Maschinen wären das 40 Controls. Bedenken Sie aber, dass die
                                     Überwachung der Ansichten eine gewisse Aufmerksamkeit erfordert. Gleich-
                                     zeitig wird die Performance langsamer und senkt damit die Aktualität der An-
                                     zeige.

                                     Planung
                                     Bevor Sie neue Ansichten definieren, müssen Sie folgende Ziele festlegen:
                                     •   Welche Produktionsbereiche oder Maschinen (Erfassungsstellen) sollen
                                         überwacht werden.
                                     •   Was wollen Sie sehen: Status oder Stückzahlen.
                                     •   Welcher Zeitraum soll überwacht werden.
                                     •   Welche Art der Anzeige ist dafür geeignet.
                                     •   Wie soll die Seite/Ansicht aufgebaut werden.

                                     Aufgabe
                                     In den folgenden Lerneinheiten wird gezeigt, wie eine einfache Ansicht aufge-
                                     baut wird. In dieser Ansicht sollen folgende Daten angezeigt werden:
                                     •   Produktionslinie 1
                                         – Status der Maschinen in der Linie: Zuschnitt 1, CNC
                                         – Anzahl der gefertigten Stück: ISO-Linie 1
                                     •   Produktionslinie 2
                                         – Status der Maschinen in der Linie: Zuschnitt 2,
                                         – Anzahl der gefertigten Stück: Kantenbearbeitung, ISO-Linie 2

                                         Voraussetzungen für die Anzeige
                                         Wenn Sie die Anzeige aus dieser Anleitung in Ihrem Betrieb einsetzen wol-
                                         len, müssen Sie sicherstellen, dass die angesprochenen Maschinen als Er-
                                         fassungsstellen eingerichtet sind und dass die Daten korrekt erfasst
                                         werden.

                                     Abfolge der Arbeitsschritte
                                     •   Grafische Form der Anzeige pro Maschine festlegen.
                                     •   Control pro Maschine anlegen.
                                     •   Panes (Seitenaufbau) planen und festlegen.
                                     •   Controls zu Seite (Page) zusammenstellen
                                     •   Pages zu Ansicht (View) zusammenstellen
                                     In allen Editoren arbeiten Sie auf zwei Ebenen:
                                     •   Auf der ersten Ebene legen Sie den Namen und die Beschreibung fest.
                                     •   Auf der zweiten Ebene legen Sie die Details fest:
1.00 / 04-2014




                                         – Control Editor: Controltyp und Werte für die Anzeige.
                                         – Page Editor: Panes (Aufteilung der Seite) und Controls.
                                         – View Editor: Seiten, die nacheinander angezeigt werden.



                 28                                                                             A+W Dashboard
                 Tutorial                                                                         Anzeige erstellen




                                        Control anlegen
                                        Für die Anzeige der Produktionslinie 1 und 2 müssen Sie pro Maschine ein
                                        Control anlegen. In diesem Beispiel wird das für den Zuschnitt 1 gezeigt.


                                         So legen Sie ein neues Control an
                                        1 Öffnen Sie im Monitor oder im Dashboard die Menüleiste und tippen Sie
                                          auf [Control Editor].
                                        2 Öffnen Sie im Control Editor die Menüleiste.




                    Abb. 18   Control Editor – Ebene 1


                                        3 Tippen Sie auf [Einfügen], um eine neue Zeile freizuschalten.
1.00 / 04-2014




                 A+W Dashboard                                                                                  29
                 Anzeige erstellen                                                                              Tutorial




                      Abb. 19   Zeile für neues Control freigeschaltet


                                           4 Tragen Sie folgende Daten ein:
                                              •   den Namen, z. B. Tisch 1,
                                              •   eine Beschreibung dazu, was angezeigt werden soll, z. B. aktueller Ma-
                                                  schinenstatus.
                                           5 Schließen Sie die Menüleiste und tippen Sie auf [Editieren].




                      Abb. 20   Control Editor – Ebene 2


                                           6 Wählen Sie die Datenquelle und den Controltyp aus.
                                              Die Auswahl des Controltyps hängt davon ab, welche Datenquelle Sie aus-
                                              gewählt haben. in diesem Beispiel wird Status und Ampel gewählt.
1.00 / 04-2014




                 30                                                                                   A+W Dashboard
                 Tutorial                                                                           Anzeige erstellen




                    Abb. 21   Details für das Control festlegen


                                        7 Wählen Sie die Erfassungsstelle aus.
                                        8 Legen Sie die Werte für den grünen und den gelben Status fest, z. B.:
                                            •   grün: Produktion
                                            •   gelb: Pause, Wartung.
                                            Sie können jeder Farbe mehr als einen Status zuweisen. Allerdings ist es
                                            sinnvoll, dem grünen Status nur Produktion zuzuweisen.
                                            Alle Status, die nicht zugewiesen wurden, gelten automatisch für den roten
                                            Status.
                                        9 Tippen Sie auf [Zurück], um die erste Ebene des Control Editors wieder an-
                                          zuzeigen.
                                        10 Öffnen Sie die Menüleiste, um die Schaltflächen anzuzeigen.
                                        11 Tippen Sie auf Speichern.
                                            Das neue Control wird gespeichert und im Control Editor angezeigt.
                                        12 Wiederholen Sie die Schritte für alle Controls, die Sie anlegen müssen.
                                            Für das Beispiel Produktionslinie 1 wären das folgende Controls:
                                            – Status der Maschine: CNC
                                            – Anzahl der gefertigten Stück: ISO-Linie 1
                                            Beachten Sie für die Controltypen Tacho und Punktediagramm die Einstel-
                                            lung zur Berechnung der Werte:
                                             “Tacho” auf Seite 20
1.00 / 04-2014




                 A+W Dashboard                                                                                     31
                 Anzeige erstellen                                                                               Tutorial




                                         Seite zusammenstellen
                                         Planen Sie die Zusammenstellung einer Seite für die Produktionslinie 1.
                                         Beachten Sie dazu das (optische) Format der Controls, z. B. braucht ein Punk-
                                         tediagramm ein langes Feld, ein Kreisdiagramm oder ein Tacho eher ein qua-
                                         dratisches Feld.
                                         In diesem Beispiel werden drei Controls in eine unsymmetrische Aufteilung
                                         eingefügt.
                                         Zu dieser Anleitung gehören folgende Handlungssequenzen:
                                         •   “So richten Sie die Panes auf einer neuen Seite ein” auf Seite 32
                                         •   “So stellen Sie die Controls auf der Seite zusammen” auf Seite 35

                                             Voraussetzung
                                             Im Folgenden wird vorausgesetzt, dass Sie die Handlungsschritte zum
                                             Anlegen eines Control kennen. Dazu gehört, dass Sie wissen, wie Sie die
                                             Menüleiste ein- und ausblenden.


                                          So richten Sie die Panes auf einer neuen Seite ein
                                         1 Öffnen Sie den Page Editor und lassen Sie sich die Menüleiste anzeigen.




                      Abb. 22   Page Editor – Ebene 1


                                         2 Tippen Sie auf [Einfügen], um eine neue Zeile freizuschalten.
1.00 / 04-2014




                 32                                                                                 A+W Dashboard
                 Tutorial                                                                                Anzeige erstellen




                                           3 Tragen Sie folgende Daten ein:
                                                 •   den Namen, z. B. Produktionslinie 1,
                                                 •   eine Beschreibung dazu, was angezeigt werden soll, z. B. Sonderschei-
                                                     ben.
                                           4 Tippen Sie auf [Editieren], um in die Ebene 2 des Page Editors zu wech-
                                             seln.




                                A    B               C                   D
                    A Trenner (für Panes)                                 C Listen der Controls nach Buchungstypen
                    B Einstellung Rasterlinien                            D Rasterlinien mit Magnet-Funktion
                    Abb. 23      Page Editor – Ebene 2


                                           5 Öffnen Sie die Liste der Trennlinien (A) und ziehen Sie die gewünschte(n)
                                             Linie(n) auf das Raster.

                                                 Panes nachträglich ändern
                                                 Sie können die Größe der Panes nicht mehr ändern, wenn Sie die Controls
                                                 eingefügt haben. Wenn Sie mehr Panes eingerichtet haben, als Sie benö-
1.00 / 04-2014




                                                 tigen, können Sie nach dem Einfügen der Controls die nicht benötigten
                                                 Trenner löschen. Das Programm verteilt dann die Controls auf der zur Ver-
                                                 fügung stehenden Fläche.



                 A+W Dashboard                                                                                        33
                 Anzeige erstellen                                                                                       Tutorial




                                A                                     B                         B             C
                      A Zwei vertikale Trenner einfügen                   B Eingefügte Trenner
                                                                          C Pane (Feld, in das ein Control positioniert wird)
                      Abb. 24       Panes festlegen


                                                 Die Trennlinien werden eingefügt. Sie können diese Linien an die ge-
                                                 wünschte Position verschieben. Das Raster hat Magnetfunktion: wenn Sie
                                                 die Trennlinie in der Nähe einer Rasterlinie loslassen, wird sie automatisch
                                                 auf die Rasterlinie gezogen.
                                                 Wenn Sie die Panes eingerichtet haben, können Sie die Controls einfügen.
1.00 / 04-2014




                 34                                                                                           A+W Dashboard
                 Tutorial                                                                           Anzeige erstellen




                                          So stellen Sie die Controls auf der Seite zusammen
                                         1 Öffnen Sie die Liste des gewünschten Controltyps und ziehen Sie das Con-
                                           trol in das zugehörige Pane.
                                             Wenn Sie das Control in ein anderes Pane versetzen oder ganz entfernen
                                             wollen, müssen Sie das Kontextmenü öffnen.




                                              A                  B     C                           D
                                             A Schaltfläche (Menü B Control löschen      D Ausgeschnittenes
                                               öffnen)            C Control ausschneiden   Control einfügen

                                             Abb. 25        Kontextmenü


                                         2 Tippen Sie auf das Control (rechte Maustaste), um das Kontextmenü zu
                                           öffnen.
                                         3 Tippen Sie im Kontextmenü auf die Schaltfläche [Menü] (A).
                                             Im Kontextmenü können Sie das Control löschen (B) oder
                                             ausschneiden (C).
                                             Wenn Sie das Kontextmenü an der neuen Position öffnen, können Sie das
                                             ausgeschnittene Control einfügen (D).
                                         4 Positionieren Sie die Controls, die zur Produktionslinie 1 gehören.
1.00 / 04-2014




                    Abb. 26   Beispiel: Seite für Produktionslinie 1



                 A+W Dashboard                                                                                   35
                 Anzeige erstellen                                                                       Tutorial




                                     5 Tippen Sie auf [Zurück], um die erste Ebene des Pages Editors wieder an-
                                       zuzeigen.
                                     6 Öffnen Sie die Menüleiste und speichern Sie die Seite.
                                        Sie können jetzt eine weitere Seite zusammenstellen, z. B. mit den Cont-
                                        rols für die Produktionslinie 2.
1.00 / 04-2014




                 36                                                                             A+W Dashboard
                 Tutorial                                                                          Anzeige erstellen




                                         Ansicht konfigurieren
                                         Die verfügbaren Seiten stellen Sie zu einer Ansicht (View) zusammen. Alle
                                         Seiten, die Sie in die neue Ansicht verschieben, werden im Dashboard hinter-
                                         einander gestellt. Mit den Funktionen zum Durchschalten werden sie in den
                                         Vordergrund geholt und über die aktuelle Seite gelegt.
                                          “Programm bedienen” auf Seite 12

                                            Voraussetzung
                                            Im Folgenden wird vorausgesetzt, dass Sie die Handlungsschritte zum An-
                                            legen eines Controls kennen. Dazu gehört, dass Sie die Handlungsschritte
                                            über die Menüleiste kennen.


                                          So stellen Sie die Seiten zu einer View zusammen
                                         1 Öffnen Sie den View Editor und lassen Sie sich die Menüleiste anzeigen.




                    Abb. 27   View Editor – Ebene 1


                                         2 Tippen Sie auf [Einfügen], um eine neue Zeile freizuschalten.




                    Abb. 28   Zeile für neue Seite freigeschaltet
1.00 / 04-2014




                                         3 Tragen Sie folgende Daten ein:
                                            •   den Namen, z. B. Demo-View.
                                            •   eine Beschreibung dazu, z. B. Training.


                 A+W Dashboard                                                                                   37
                 Anzeige erstellen                                                                           Tutorial




                                          4 Tippen Sie auf [Editieren], um in die Ebene 2 des View Editors zu wech-
                                            seln.




                      Abb. 29   View Editor – Ebene 2


                                          5 Ziehen Sie die gewünschte Seite aus dem linken Bereich in den rechten
                                            Bereich (neue View).




                      Abb. 30   Neuen View mit zugeordneter Seite


                                             Beachten Sie dabei Folgendes:
                                             •   Jede Seite kann durch Verschieben wieder aus der Ansicht entfernt
                                                 werden.
                                             •   Die Reihenfolge der Seiten kann durch Verschieben innerhalb der An-
                                                 sicht geändert werden.
1.00 / 04-2014




                                             •   Die Reihenfolge entscheidet, wie die Seiten nacheinander durchge-
                                                 schaltet werden.



                 38                                                                                 A+W Dashboard
                 Tutorial                                                                        Anzeige erstellen




                                      6 Tippen Sie auf [Zurück], um die erste Ebene des View- Editors wieder an-
                                        zuzeigen.
                                      7 Öffnen Sie die Menüleiste und speichern Sie die Seite.
                                      8 Wechseln Sie zum Monitor, um die View zu prüfen.




                    Abb. 31   Neue View


                                      9 Aktualisieren Sie ggf. die Browser-Ansicht (<F5>), damit die Seite neu ge-
                                        laden wird.
                                      10 Wechseln Sie zum Dashboard, um die aktuellen Daten anzuzeigen.
                                      11 Testen Sie das Durchschalten.
1.00 / 04-2014




                 A+W Dashboard                                                                                39
                 Anzeige erstellen          Tutorial
1.00 / 04-2014




                 40                  A+W Dashboard
         Index




A+W Dashboard
                 Index                                                                 Index




                 Index
                 A                              Datenquelle
                 Ampel 24                       – auswählen 30
                 Ansicht                        – Datenbank-Tabellen 19
                 – Editor 26                    Definition
                 – konfigurieren 37             – Ampel 24
                 – planen 28                    – Balkendiagramm 22
                 – siehe auch View              – Kreis 23
                 Anzeige                        – Punktediagram 21
                 – aktuelle Daten 13            – Tacho 20
                 – Aufbau 15                    Durchschnittswert 21
                 – Control Editor 18
                 – Controls 10                  E
                 – Page Editor 25               Editor
                 – View Editor 26               – Ansicht 26
                                                – Control 18
                 B                              – Page 25
                 Balkendiagramm 22              – Rasterlinien 25
                 BDE-Buchungen                  – Schaltflächen 18
                 – Datenquelle 19               – View 26
                 – lückenlose Buchung 7         Einstellungen 14
                 Bedienoberfläche 14            Erfassungsstelle auswählen   31
                 Bedienung
                 – allgemeine Funktionen 12     G
                 – Dashboard 13                 Gruppierung 20
                 – Editor 18                    Gruppierungsmodus    20
                 – Schaltflächen 12, 13, 18
                 Berechnung der Daten 20
                                                K
                                                Korrekte Daten   7
                 C                              Kreis 23
                 Control
                 – anlegen 29
                                                M
                 – auf Seite stellen 35
                                                Monitor
                 – auf Seite verschieben   35
                                                – Aufbau 15
                 – Erfassungsstelle 31
                                                – Bedienfunktionen 12
                 Controltyp 19
                                                – Dummy-Daten 12
                 – auswählen 30
                 – Datenquelle 19
                                                P
                                                Page
                 D
                                                – anlegen 32
                 Darstellungskonventionen 6
                                                – siehe auch Seite 32
                 Dashboard
                                                Page-Editor
                 – Bedienung 13
                                                – Rasterlinien 25
                 – sktuelle Daten 13
                                                Pane
                 Daten
                                                – festlegen 32
                 – aktuell (Dashboard) 13
1.00 / 04-2014




                                                Programm
                 – Berechnung 20
                                                – Leistungsmerkmale 9
                 – Darstellung 10
                                                – Ziel 7
                 – Dummy-Daten (Monitor) 12
                                                Punktediagramm 21

                 42                                                           A+W Dashboard
                 Index                               Index




                 R
                 Rasterlinien    25

                 S
                 Schaltflächen 12, 13, 18
                 Seite
                 – anlegen 32
                 – Control einfügen 35
                 – in Ansicht einfügen 37
                 – Panes festlegen 32
                 Seite
                 – siehe auch Page 32
                 Struktur
                 – Konzept 17
                 – Seiten im Dashboard 16
                 Struktur der Anzeigen 15

                 T
                 Tacho   20

                 V
                 View 26
                 – siehe auch Ansicht
                 – zusammenstellen 37

                 Z
                 Zielmarke      21
1.00 / 04-2014




                 43                         A+W Dashboard
1.00 / 04-2014   Index           Index




                 A+W Dashboard     44

