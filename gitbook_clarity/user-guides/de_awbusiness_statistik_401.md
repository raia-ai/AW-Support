---
description: "DE AWBusiness Statistik 4.01"
---



# DE AWBusiness Statistik 4.01

Statistik             F




                     deutsch




            A+W Business
                                                                                                             Vorspann




                                          Vorspann
                                          In diesem Teil der Dokumentation finden Sie editorische Notizen.


                                          Revisionsübersicht
                                          Part             Beschreibung
                                          Version/Datum

                                          1.00/03-1998     Ersterstellung

                                          2.00/08-2000     Überarbeitung Statistik

                                          3.00/12-2003     Struktureller Umbau auf Programmstruktur 4.0

                                          3.01/08-2008     Rechtschreibkorrekturen

                                          3.02/09-2008     Abbildungen und Part-Nummer angepasst.

                                          3.03/09-2010     Layout an Doku-Konzept 2010 angepasst.

                                          3.04/01-2013     Layout an A+W Business angepasst.

                                          4.00/06-2016     Vollständige Überarbeitung

                                          4.01/01-2017     Produkt- und Firmennamen angepasst.



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
                                          nen Fehler nicht vollständig ausgeschlossen werden. A+W Software GmbH
                                          übernimmt keine Haftung für Fehler oder Ungenauigkeiten, es sei denn, diese
                                          beruhen auf vorsätzlichem oder grobfahrlässigem Handeln.
4.01 / 01-2017




                                          Dieses Dokument beschreibt die volle Ausbaustufe von A+W Business.




                 A+W Business Statistik                                                                          F-3
                 Vorspann




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

                               +49 6404 205 10

                               +49 6404 205 1877

                            Zentrale@a-w.com

                            http://www.a-w.com
4.01 / 01-2017




                 F-4                                                             A+W Business Statistik
                                                                                                                                                               Inhalt




                                          Inhalt
                                          Vorspann ................................................................................................................ F-3
                                           Revisionsübersicht .............................................................................................. F-3
                                           Editorial ............................................................................................................... F-3

                                          Softwarereferenz                                                                                                     F-7
                                          Übersicht ................................................................................................................. F-9
                                          Verkaufsstatistiken ................................................................................................ F-10
                                            Auftragsinformation ........................................................................................... F-10
                                               Menü Drucken ................................................................................................ F-11
                                               Auftragsinfo – Optionen ................................................................................. F-11
                                               Auftragsinfo – Erfasst ..................................................................................... F-15
                                               Auftragsinfo – Produziert ............................................................................... F-16
                                               Auftragsinfo – Fakturiert ................................................................................. F-17
                                               Auftragsinfo – Offen ....................................................................................... F-18
                                               Auftragsinfo – Grafik ...................................................................................... F-19
                                            Auswahl ............................................................................................................. F-20
                                            Umsatz Verkauf ................................................................................................. F-21
                                               Menü Optionen .............................................................................................. F-21
                                               Menü Superstatistik ....................................................................................... F-22
                                               Umsatz Verkauf – Auswahl ............................................................................ F-23
                                               Umsatz Verkauf – Restriktionen .................................................................... F-28
                                               Umsatz Verkauf – Tabelle .............................................................................. F-29
                                               Umsatzstatistik – Grafik ................................................................................. F-30
                                               Umsatz Verkauf – SQL .................................................................................. F-31
                                            Superstatistik ..................................................................................................... F-32
                                            Superstatistik – Export ...................................................................................... F-34
                                            Superstatistik – Import ....................................................................................... F-35
                                            Reklamationsstatistik Verkauf ........................................................................... F-36
                                            Statistik nach Aufbau ......................................................................................... F-37
                                               Statistik nach Aufbau – Auswahl .................................................................... F-37
                                               Statistik nach Aufbau – Tabelle ..................................................................... F-40
                                            Kunden nach AV-Bereich .................................................................................. F-42
                                          Einkaufsstatistiken ................................................................................................ F-44
                                            Umsatzstatistik Einkauf ..................................................................................... F-44
                                            Reklamationsstatistik Einkauf ............................................................................ F-45
                                            Liefertreue ......................................................................................................... F-46
                                            Analyse Verbrauch ............................................................................................ F-48
                                               Analyse Verbrauch – Auswahl ....................................................................... F-48
                                               Analyse Verbrauch – Restriktionen ................................................................ F-51
                                               Analyse Verbrauch – Tabelle ......................................................................... F-53
                                          Provisionsstatistik ................................................................................................. F-54
                                          Intrastat Meldung .................................................................................................. F-56

                                          Partindex                                                                                                          F-59
                                          Index Statistik ....................................................................................................... F-61
4.01 / 01-2017




                 A+W Business Statistik                                                                                                                           F-5
                 Inhalt
4.01 / 01-2017




                 F-6      A+W Business Statistik
Statistik                F

            Softwarereferenz




            A+W Business
                 Softwarereferenz                                                                               Übersicht




                                          Übersicht
                                          A+W Business verfügt über verschiedene Auswertungsmöglichkeiten. Dabei
                                          wird, wie nachfolgend beschrieben, zwischen aktueller Auftragsbestandsaus-
                                          wertung, Umsatz-, Reklamations- und Provisionsstatistik unterschieden.
                                          •   “Verkaufsstatistiken” auf Seite F-10
                                          •   “Einkaufsstatistiken” auf Seite F-44
                                          •   “Provisionsstatistik” auf Seite F-54
                                          •   “Intrastat Meldung” auf Seite F-56

                                              Systemeinstellungen
                                              In den Firmendaten können Sie Details für die Übergabe der Aufträge und
                                              Bestellungen in die Statistik festlegen. Eine ausführliche Beschreibung fin-
                                              den Sie im Part Stammdaten.

                                               Stammdaten, “Firmendaten – Archiv” auf Seite B-948
4.01 / 01-2017




                 A+W Business Statistik                                                                              F-9
                 Verkaufsstatistiken                                                              Softwarereferenz




                                       Verkaufsstatistiken
                                       Die Statistik in A+W Business ist ein wichtiges Instrument für die Unterneh-
                                       mensanalyse. Sie erhalten Auswertungen über Ihre Kunden, Branchen, Pro-
                                       dukte, Geschäftsbereiche, Vertreter, etc. Dazu wählen Sie aus, ob die Daten
                                       jahresweise oder monatsweise ausgewertet werden sollen.
                                       In diesem Kapitel finden Sie Informationen zu folgenden Themen:
                                       •   “Auftragsinformation” auf Seite F-10
                                       •   “Auswahl” auf Seite F-20
                                       •   “Umsatz Verkauf” auf Seite F-21
                                       •   “Superstatistik” auf Seite F-32
                                       •   “Superstatistik – Export” auf Seite F-34
                                       •   “Superstatistik – Import” auf Seite F-35
                                       •   “Reklamationsstatistik Verkauf” auf Seite F-36
                                       •   “Statistik nach Aufbau” auf Seite F-37
                                       •   “Kunden nach AV-Bereich” auf Seite F-42


                                       Auftragsinformation
                                       Statistik > Auftragsinfo
                                       In diesem Dialog werten Sie Ihren Auftragsbestand aus. Dabei können Sie
                                       zwischen den neuen Aufträgen, den an die Produktion übergebenen Aufträ-
                                       gen und den fakturierten Aufträgen unterscheiden.
                                       In diesem Dialog finden Sie folgende Register:
                                       •   “Auftragsinfo – Optionen” auf Seite F-11
                                       •   “Auftragsinfo – Erfasst” auf Seite F-15
                                       •   “Auftragsinfo – Produziert” auf Seite F-16
                                       •   “Auftragsinfo – Fakturiert” auf Seite F-17
                                       •   “Auftragsinfo – Offen” auf Seite F-18
                                       •   “Auftragsinfo – Grafik” auf Seite F-19
4.01 / 01-2017




                 F-10                                                                       A+W Business Statistik
                 Softwarereferenz                                                                  Verkaufsstatistiken




                                          Menü Drucken
                                          Statistik > Auftragsinfo
                                          Über dieses Menü starten Sie den Druck der Auswertung auf dem Bildschirm
                                          oder dem Drucker:
                                          •   Standard:
                                              Öffnet den Dialog Auswahl, um festzulegen, welche Daten gedruckt wer-
                                              den sollen.
                                               “Auswahl” auf Seite F-20
                                          •   Umsatz:
                                              Startet den Druck der Umsatzdaten und der Vergleichdaten des Vorjahres.
                                              In der tabellarischen Gegenüberstellung werden die Arbeitstage pro Monat
                                              angegeben. Die Aufstellung schließt mit den Werten für den durchschnitt-
                                              lichen Umsatz pro Arbeitstag.


                                          Auftragsinfo – Optionen
                                          Statistik > Auftragsinfo > Register Optionen




                                          Abb. F-1     Auftragsinfo - Optionen


                                          In diesem Register legen Sie die Auswahlkriterien und die Ausgabeeinstellun-
                                          gen fest. Das Ergebnis der Suche wird in den Registern Erfasst, Produziert,
                                          Fakturiert und Offen ausgegeben.
4.01 / 01-2017




                 A+W Business Statistik                                                                          F-11
                 Verkaufsstatistiken                                                                   Softwarereferenz




                                       Spalten
                                       Über die Checkboxen legen Sie die Spalten fest, die in den Registern ange-
                                       zeigt werden sollen.
                                       •   Menge:
                                           Gesamtmenge aller Aufträgspositionen im gewählten Zeitraum.
                                       •   Fläche:
                                           Gesamtfläche aller Auftragspositionen.
                                       •   LFM:
                                           Gesamtlänge aller Kanten.
                                       •   VK:
                                           Gesamtsumme VK.
                                       •   EK:
                                           Gesamtsumme EK.
                                       •   Deckungsbeitrag:
                                           Gesamtsumme des Deckungsbeitrags. Im Bereich Selektionskriterien wer-
                                           den die Optionen für den Deckungsbeitrag freigeschaltet.
                                        Die Spalte wird nicht angezeigt.
                                        Die Spalte wird angezeigt.

                                       Selektionskriterien
                                       In diesem Bereich legen Sie die Auswahlkriterien fest.
                                       •   Tag, Monat, Jahr, Kalenderwoche, Quartal:
                                           Mit der Wahl einer Option legen Sie den Betrachtungszeitraum fest.
                                           Die Optionen Jahr und Quartal sind gesperrt, wenn Sie im Bereich Auf-
                                           schlüsselung nach die Checkbox Aufträge markiert haben.
                                           Wenn Sie die Auflistung nach Zeitraum wählen, wird die Auswahl entspre-
                                           chend eingeschränkt.
                                       •   Auswahl Datum:
                                           Mit dieser Einstellung schränken Sie den Betrachtungszeitraum auf ein be-
                                           stimmtes Datum ein.

                                       Klassifikator Nur die Klassifikatoren stehen zur Wahl, die übergreifend für
                                       alle Partner und/oder Kunden gelten.
                                        Stammdaten, “Klassifikatoren” auf Seite B-745

                                       Wert von, Wert bis Eingrenzung auf Klassifikatorenwerte.
                                        Stammdaten, “Klassifikatoren Wertzuordnung” auf Seite B-790

                                       Deckungsbeitrag Mit der Wahl der Option legen Sie fest, ob der Deckungs-
                                       beitrag als Betrag oder prozentual angezeigt werden soll. Die Felder sind nur
                                       freigeschaltet, wenn im Bereich Spalten die Checkbox Deckungsbeitrag mar-
                                       kiert ist.
                                        Stammdaten, “Klassifikatoren” auf Seite B-745

                                       Wert von, Wert bis Eingrenzung auf einen Wert oder eine Spanne von Wer-
4.01 / 01-2017




                                       ten. Sie können auch negative Zahlenwerte eintragen.




                 F-12                                                                        A+W Business Statistik
                 Softwarereferenz                                                                        Verkaufsstatistiken




                                              Beispiele

                                              Eingabe              Ergebnis

                                              Negativer Wert:      Alle Aufträge, deren Kosten größer sind als der VK,
                                                                   z. B. von -99999 bis 0,00

                                              Null                 Alle Aufträge, deren Kosten durch den VK gedeckt
                                                                   sind, z. B. von 0,00 bis 0,00

                                              Größer null          Alle Aufträge, deren Kosten kleiner sind als der VK,
                                                                   z. B. von 1,00 bis 1000


                                          Auflistung nach
                                          Mit der Wahl der Option legen Sie fest, wie die Werte der Trefferliste gegliedert
                                          werden:
                                          •   Zeitraum:
                                              Im Bereich Aufschlüsseln nach können Sie die Ausgabe zusätzlich nach
                                              AV-Bereichen, Warengruppen oder Aufträgen auflösen.
                                              Bei der Auswertung eines Jahres werden die Daten z. B. nach Monaten
                                              summiert. Wenn Sie z. B. die Auswahl auf einen Monat eingeschränkt ha-
                                              ben, können Sie das Ergebnis zusätzlich nach Aufträgen aufschlüsseln.
                                          •   Warengruppen:
                                              Im Bereich Summieren nach werden die Felder freigeschaltet. Im Bereich
                                              Aufschlüsseln nach wird die Checkbox Warengruppen gesperrt.
                                          •   AV-Bereiche:
                                              Im Bereich Aufschlüsseln nach können Sie die Ausgabe zusätzlich nach
                                              Warengruppen oder Aufträgen auflösen.
                                          •   Kunden:
                                              Im Bereich Aufschlüsseln nach können Sie die Ausgabe zusätzlich nach
                                              AV-Bereichen, Warengruppen oder Aufträgen auflösen.

                                          Summieren nach
                                          Mit der Wahl der Option legen Sie fest, wie die Werte für Warengruppen sum-
                                          miert werden sollen. Die Felder sind nur freigeschaltet, wenn Sie im Bereich
                                          Auflistung nach die Option Warengruppen gewählt haben.
                                          •   Warenhauptgruppen, Warenobergruppen, Warengruppen:
                                              Die Werte des Betrachtungszeitraums werden nach der gewählten Option
                                              summiert.
                                          •   Top-Warengruppen:
                                              Die Werte werden nach Top-Warengruppen summiert. Dazu müssen Top-
                                              Warengruppen in den Stammdaten angelegt sein.
4.01 / 01-2017




                 A+W Business Statistik                                                                                   F-13
                 Verkaufsstatistiken                                                               Softwarereferenz




                                       Aufschlüsselung nach
                                       Mit der Wahl der Option legen Sie fest, wie die Werte aufgelöst werden sollen.
                                       Damit wird die Gesamtmenge pro AV-Bereich, pro Warengruppe oder pro Auf-
                                       trag angezeigt.
                                       Sie können nur eine der angezeigten Checkboxen markieren. Wenn Sie keine
                                       Checkbox markieren, werden die Werte nach den Selektionskriterien grup-
                                       piert.
                                       •   AV-Bereiche:
                                           Die Checkbox ist gesperrt, wenn Sie im Bereich Aufschlüsseln nach die
                                           Option AV-Bereiche gewählt haben.
                                       •   Warengruppen:
                                           Die Checkbox ist gesperrt, wenn Sie im Bereich Aufschlüsseln nach die
                                           Option Warengruppen gewählt haben.
                                           Wenn Sie die Checkbox markieren, wird im Bereich Optionen die Check-
                                           box Vergleich mit Vorjahreswerten freigeschaltet.
                                       •   Aufträge:
                                           Die Werte werden nach Aufträgen aufgelöst.

                                       Optionen

                                       Vergleich mit Vorjahreswerten In den Registern können die Vergleichs-
                                       werte des Vorjahres angezeigt werden.
                                        Die Vergleichswerte werden nicht ausgegeben.
                                        Die Vergleichswerte werden ausgegeben. Diese Einstellung wird auch in
                                       den Standard-Druck übernommen.
                                       Im Umsatzdruck werden die Vergleichswerte immer angezeigt.
4.01 / 01-2017




                 F-14                                                                       A+W Business Statistik
                 Softwarereferenz                                                                  Verkaufsstatistiken




                                          Auftragsinfo – Erfasst
                                          Statistik > Auftragsinfo > Register Erfasst




                                          Abb. F-2     Auftragsinfo – Erfasst


                                          In diesem Register werden alle Aufträge angezeigt, die noch nicht weiter be-
                                          arbeitet wurden. Zur Auswahl wird das Erfassungsdatum herangezogen.
                                          Die Ausgabe kann mit der Ausgabe im Register Offen übereinstimmen, wenn
                                          die Selektionskriterien nicht weiter eingegrenzt wurden.
                                          Die Anzeige der Spalten wird im Register Optionen ausgewählt.
                                           “Auftragsinfo – Optionen” auf Seite F-11
4.01 / 01-2017




                 A+W Business Statistik                                                                          F-15
                 Verkaufsstatistiken                                                               Softwarereferenz




                                       Auftragsinfo – Produziert
                                       Statistik > Auftragsinfo > Register Produziert




                                       Abb. F-3     Auftragsinfo – Produziert


                                       In diesem Register werden alle Aufträge angezeigt, die aus der Produktion als
                                       fertig gemeldet sind.
                                       Die Anzeige der Spalten wird im Register Optionen ausgewählt.
                                        “Auftragsinfo – Optionen” auf Seite F-11
4.01 / 01-2017




                 F-16                                                                       A+W Business Statistik
                 Softwarereferenz                                                                  Verkaufsstatistiken




                                          Auftragsinfo – Fakturiert
                                          Statistik > Auftragsinfo > Register Fakturiert




                                          Abb. F-4     Auftragsinfo – Fakturiert


                                          In diesem Register werden alle Aufträge angezeigt, für die eine Rechnung ge-
                                          schrieben wurde. Dazu wird das Rechnungsdatum herangezogen.
                                          Die Anzeige der Spalten wird im Register Optionen ausgewählt.
                                           “Auftragsinfo – Optionen” auf Seite F-11
4.01 / 01-2017




                 A+W Business Statistik                                                                         F-17
                 Verkaufsstatistiken                                                               Softwarereferenz




                                       Auftragsinfo – Offen
                                       Statistik > Auftragsinfo > Register Offen




                                       Abb. F-5     Auftragsinfo – Offen


                                       In diesem Register werden alle Aufträge angezeigt, die vor dem aktuellen Da-
                                       tum erfasst, aber noch nicht produziert wurden. Das sind alle Aufträge, zu de-
                                       nen weder ein Rechnungsdatum noch eine Laufnummer existiert.
                                       Die Anzeige der Spalten wird im Register Optionen ausgewählt.
                                        “Auftragsinfo – Optionen” auf Seite F-11
4.01 / 01-2017




                 F-18                                                                       A+W Business Statistik
                 Softwarereferenz                                                                 Verkaufsstatistiken




                                          Auftragsinfo – Grafik
                                          Statistik > Auftragsinfo > Register Grafik




                 Abb. F-6    Auftragsinfo – Grafik und Legende


                                          in diesem Register werden die Daten der Auswahl grafisch dargestellt.
                                          Die Anzeige der Daten wird im Register Optionen ausgewählt.
                                           “Auftragsinfo – Optionen” auf Seite F-11

                                          Anzeige
                                          Mit der Wahl der Option können Sie die Daten der Register einzeln anzeigen
                                          lassen.
4.01 / 01-2017




                 A+W Business Statistik                                                                           F-19
                 Verkaufsstatistiken                                                               Softwarereferenz




                                       Auswahl
                                       Statistik > Auftragsinfo > Menü Druck




                                       Abb. F-7     Druckeinstellung


                                       In diesem Dialog legen Sie fest, wie die Auftragsinformationen im Druck aus-
                                       gegeben werden sollen.

                                       Auswahl Report
                                       Mit der Wahl der Option legen Sie fest, welches Register gedruckt werden soll.

                                       Auswahl Spalten (max. 3)
                                       In diesem Bereich wird für jede Spalte aus dem Register Offen eine Checkbox
                                       angezeigt. Wenn Sie im Bereich Auswahl Report die Option Alle ausgewählt
                                       haben, können Sie nur maximal drei Spalten drucken.
                                        Die Spalte wird nicht gedruckt.
                                        Die Spalte wird gedruckt.
4.01 / 01-2017




                 F-20                                                                       A+W Business Statistik
                 Softwarereferenz                                                                   Verkaufsstatistiken




                                          Umsatz Verkauf
                                          Statistik > Umsatz Verkauf
                                          Neben dem Druck der Umsatzinformationen aus dem Dialog Auftragsinfo ste-
                                          hen in diesem Dialog detaillierte Auswertungen für die Verkaufszahlen zur
                                          Verfügung.
                                          In diesem Dialog finden Sie folgende Register:
                                          •   “Umsatz Verkauf – Auswahl” auf Seite F-23
                                          •   “Umsatz Verkauf – Restriktionen” auf Seite F-28
                                          •   “Umsatz Verkauf – Tabelle” auf Seite F-29
                                          •   “Umsatzstatistik – Grafik” auf Seite F-30
                                          •   “Umsatz Verkauf – SQL” auf Seite F-31
                                          In den Registern Auswahl und Restriktionen legen Sie die Kriterien für die
                                          Auswertung der Daten fest.
                                          In den Registern Tabelle und Grafik wird das Ergebnis der Auswertung ange-
                                          zeigt.


                                          Menü Optionen
                                          Statistik > Umsatz Verkauf
                                          Über dieses Menü können Sie die Standardeinstellung des Dialogs bestim-
                                          men. Sie können die Optionen aktivieren oder deaktivieren. Die Einstellung
                                          wird nicht zurückgesetzt, wenn Sie den Dialog schließen.

                                              Aktivierte Optionen nach dem Öffnen des Dialogs
                                              Bitte beachten Sie, dass geänderte Optionen erst beim nächsten Öffnen
                                              des Dialogs wirksam werden.
                                              Die folgenden Beschreibungen stellen die aktivierte Option dar.

                                          Gruppe Einstellungen
                                          •   Mengen inklusive Stückliste:
                                              Die Mengen aus der Stückliste werden in die Angabe der Menge aufge-
                                              nommen.
                                          •   Nur Positionsmengen:
                                              Nur die Stückzahl der Positionen wird angezeigt, z. B. 5 Stk. ISO.
                                          •   Nur Stücklistenmengen:
                                              Nur die Stückzahlen der Stückliste werden angezeigt. Diese Einstellung
                                              eignet sich z. B. für Bearbeitungen.
4.01 / 01-2017




                 A+W Business Statistik                                                                           F-21
                 Verkaufsstatistiken                                                                  Softwarereferenz




                                       •   Abweichendes Wirtschaftsjahr aktiv:
                                           Bei Jahresauswertungen soll nicht das Kalenderjahr sondern das Wirt-
                                           schaftsjahr betrachtet werden.
                                       •   Statistiknamen drucken:
                                           Im Druck soll die Bezeichnung der Statistik mit angegeben werden. Der
                                           Name wird aus der gespeicherten Datei entnommen.

                                       Gruppe Automatischer Seitenvorschub beim Druck
                                       •   Nach Zwischensumme 1 bis 5:
                                           Nach den ausgewählten Zwischensummen wird im Druck ein Seitenum-
                                           bruch eingefügt.
                                       •   Vor Endsumme:
                                           Vor der Endsumme wird ein Seitenumbruch eingefügt.


                                       Menü Superstatistik
                                       Statistik > Umsatz Verkauf
                                       Über dieses Menü erstellen Sie eine Superstatistik.
                                       •   Einstellungen:
                                           Öffnet den Dialog Statistik, um die Einstellungen für die Superstatistik fest-
                                           zulegen.
                                            “Superstatistik” auf Seite F-32
                                       •   Exportieren, Importieren:
                                           Öffnet die Dialoge für manuellen Export oder Import einer Superstatistik.
                                            “Superstatistik – Export” auf Seite F-34
4.01 / 01-2017




                 F-22                                                                          A+W Business Statistik
                 Softwarereferenz                                                                   Verkaufsstatistiken




                                          Umsatz Verkauf – Auswahl
                                          Statistik > Umsatz Verkauf > Register Auswahl




                                          Abb. F-8     Umsatzstatistik Verkauf


                                          in diesem Register legen Sie die Kriterien für die Auswertung der Umsatzzah-
                                          len fest. Die Einstellungen können Sie als Datei speichern, um eine gleichwer-
                                          tige Statistik später wieder erstellen zu können.

                                          Auswahl Statistik
                                          Wenn Sie bestimmte Einstellungen sehr häufig benutzen, können Sie diese
                                          als Datei speichern und wieder auswählen.
                                          Wenn Sie eine der gespeicherten Einstellungen wieder auswählen, müssen
                                          Sie im Bereich Auswertungszeitraum nur den Zeitraum angeben.

                                          Ausgabe / Summenbildung / Sortierung

                                          Ausgabe Im linken Feld sind alle Ausgabekriterien aufgeführt, auf die sich
                                          die statistischen Auswertungen beziehen können.
                                          Für die Auswertung verschieben Sie alle die Ausgabekriterien, deren Werte
                                          herangezogen werden sollen.
                                          Von den folgenden Checkboxen muss mindestens eine markiert sein, damit
                                          Daten ausgewertet werden.
4.01 / 01-2017




                 A+W Business Statistik                                                                           F-23
                 Verkaufsstatistiken                                                                   Softwarereferenz




                                       Statistik gesamt bilden Sie können den Gesamtumsatz des Unternehmens
                                       anzeigen lassen.
                                        Die Statistik wird nur über die ausgewählten Kriterien gebildet.
                                        Die Statistik wird über den Gesamtumsatz gebildet. Diese Form dient ins-
                                       besondere Vergleichszwecken.

                                          Beispiel

                                          Wenn im Bereich Ausgabe/Summenbildung/Sortierung das Merkmal
                                          Produkte/Artikel gewählt ist, wird der Umsatz der Produkte im Vergleich zum
                                          Gesamtumsatz des Unternehmens dargestellt, z. B. EUR 800.000 gegenüber
                                          EUR 20.000.000.

                                          Performance
                                          Diese Auswertung dauert einige Zeit, da alle Daten des gesamten Unter-
                                          nehmens eingelesen werden müssen.

                                       Summe Selektion bilden Sie können im Ergebnis Zwischensummen anzei-
                                       gen lassen.
                                        Eine Zwischensumme wird nicht gebildet.
                                        Pro Ausgabekriterium wird die Zwischensumme gebildet. Dazu werden die
                                       Einstellungen im Register Restriktionen berücksichtigt, z. B. die angegebenen
                                       Warengruppen.

                                       Jahresauswertung Sie können die Ausgabe für ein ganzes Jahr zusam-
                                       menfassen.
                                        Das Ergebnis wird nicht pro Jahr angezeigt. Bei dieser Einstellung sollten
                                       Sie eine Monatsauswertung starten.
                                        Das Ergebnis wird pro Jahr angezeigt. Betrachtet werden die Jahre, die im
                                       Bereich Auswertungszeitraum angegeben sind.

                                       Monatsauswertung Sie können die Ausgabe pro Monat zusammenfassen.
                                        Das Ergebnis wird nicht pro Monat angezeigt. Bei dieser Einstellung sollten
                                       Sie eine Jahresauswertung starten.
                                        Das Ergebnis wird pro Monat angezeigt. Betrachtet werden die Jahre und
                                       Monate, die im Bereich Auswertungszeitraum angegeben sind.
4.01 / 01-2017




                 F-24                                                                           A+W Business Statistik
                 Softwarereferenz                                                                      Verkaufsstatistiken




                                          Direkte Gegenüberstellung Sie können die Auswertung von mehreren
                                          Jahren monatsweise gegenüberstellen.
                                           Die Auswertung über mehrere Jahre wird Jahr für Jahr dargestellt.
                                           Die Auswertung über mehrere Jahre wird Monat für Monat über die ange-
                                          gebenen Jahre dargestellt.

                                             Beispiele für drei Jahre und Monat 1 bis 3

                                             Einstellung        Ausgabe

                                                               Jahr 1        Januar, Februar, März
                                                                Jahr 2        Januar, Februar, März
                                                                Jahr 3        Januar, Februar, März

                                                               Januar        Jahr 1, Jahr 2, Jahr 3
                                                                Februar       Jahr 1, Jahr 2, Jahr 3
                                                                März          Jahr 1, Jahr 2, Jahr 3


                                          Superstatistik Sie können Statistiken als Gegenüberstellung der Umsatz-
                                          zahlen für Filialen und/oder Mandanten erstellen.
                                           Die Superstatistik wird nicht erstellt.
                                           Die Daten werden nach den Vorgaben erstellt, die im Dialog Statistik fest-
                                          gelegt wurden. Im Register Tabelle wird kein Ergebnis angezeigt.
                                          Eine Beschreibung dieser Superstatistik finden Sie in einem separaten Ab-
                                          schnitt.
                                           “Superstatistik” auf Seite F-32

                                          Top-10-Modus Sie können die Ausgabe der Statistik auf die besten Ergeb-
                                          nisse einschränken.
                                           Die Auswertung wird nicht auf die besten Ergebnisse eingeschränkt.
                                           In der Auswertung sollen nur die besten Ergebnisse angezeigt werden.
                                          Dazu müssen Sie im Bereich Top 10 - Auswertung / Sortierung die Darstellung
                                          der Daten festlegen.

                                          Startmonat Wirtschaftsjahr Bei Auswertungen soll nicht das Kalenderjahr
                                          sondern das Wirtschaftsjahr betrachtet werden. Das Feld zur Eingabe des ers-
                                          ten Monats ist nur freigeschaltet, wenn im Menü Optionen > Gruppe Einstel-
                                          lungen > Abweichendes Wirtschaftsjahr aktiv aktiviert wurde.
4.01 / 01-2017




                 A+W Business Statistik                                                                             F-25
                 Verkaufsstatistiken                                                               Softwarereferenz




                                       Auswahl Rubriken
                                       Mit der Wahl der Rubriken entscheiden Sie, welche Werte im Einzelnen im Re-
                                       gister Tabelle ausgegeben werden.

                                           Tipp
                                           Beachten Sie bei der Auswahl der Rubriken, dass die Übersichtlichkeit ver-
                                           loren gehen kann, wenn Sie zu viele Checkboxen markieren. Wenn Sie
                                           viele Detaildaten brauchen, erstellen Sie mehrere Statistiken mit unter-
                                           schiedlichen Einstellungen, die Sie im Feld Auswahl Statistik jeweils (mit
                                           einem sprechenden Namen) speichern.

                                       •   Umsatz:
                                           Wird in der Spalte Rubrik als Umsatz dargestellt.
                                       •   Eigenkosten:
                                           Wird in der Spalte Rubrik als Kosten dargestellt.
                                       •   Deckungsbeitrag:
                                           Wird in der Spalte Rubrik als DB dargestellt.
                                       •   Deckungsbeitrag in %:
                                           Wird in der Spalte Rubrik als DB % dargestellt.
                                       •   Durchschnittspreis:
                                           Wird in der Spalte Rubrik als D.Preis dargestellt.
                                       •   Umsatz %:
                                           Wird in der Spalte Rubrik als % U. dargestellt.
                                       •   Separate Deckungsbeiträge:
                                           Wird in der Spalte Rubrik als DB Material und DB Material % dargestellt.
                                       •   Stück:
                                           Wird in der Spalte Rubrik als Stück dargestellt.
                                       •   Fläche:
                                           Wird in der Spalte Rubrik als Fläche dargestellt.
                                       •   Umfang:
                                           Gesamte Kantenlänge. Wird in der Spalte Rubrik als Umfang dargestellt.
                                       •   Gewicht:
                                           Wird in der Spalte Rubrik als Gewicht dargestellt.
                                       •   Umsatz Reklamation:
                                           Nur im Dialog Reklamation Verkauf freigeschaltet. Wird in der Spalte Rub-
                                           rik angezeigt.
                                       •   Separate Kosten:
                                           Wird in der Spalte Rubrik als Materialkosten und Zeitkosten dargestellt.
                                        Die Werte werden nicht angezeigt.
                                        Die Werte werden angezeigt.
4.01 / 01-2017




                 F-26                                                                        A+W Business Statistik
                 Softwarereferenz                                                                       Verkaufsstatistiken




                                          TOP10 - Auswertung / Sortierung
                                          Die Felder in diesem Bereich sind nur freigeschaltet, wenn die Checkbox
                                          Top10 Modus markiert ist. In diesem Modus werden jeweils nur die besten Er-
                                          gebnisse angezeigt.

                                          Sortierung nach Die Sortierungskriterien sind von der A+W Software
                                          GmbH vorgegeben: DB (Deckungsbeitrag), Fläche, Kosten, Stück, Umfang,
                                          Umsatz.
                                          Mit der Wahl der Option legen Sie fest, welcher Wert zuerst aufgeführt wird:
                                          • Absteigend:
                                             Bei den Tops wird der höchste Wert zuerst angezeigt.
                                          • Aufsteigend:
                                             Bei den Flops wird niedrigste Wert zuerst angezeigt.

                                          Zeilen maximal Anzahl der auszuwertenden Tops oder Flops. Damit können
                                          Sie die Anzeige z. B. auf die 3 umsatzstärksten Tops einschränken.
                                          In der Tabelle ist das die Anzahl der Zeilen. In der Grafik ist das die Anzahl der
                                          Balken.

                                          Auswertungszeitraum

                                          Jahr von, bis Jahr oder Spanne von Jahren, die ausgewertet werden sollen.

                                          Monat von, bis Monat oder Spanne von Monaten, die ausgewertet werden
                                          sollen.

                                          Anzeige Beträge

                                          Beträge Sie können die Geldbeträge durch 1000 geteilt darstellen lassen.
                                           Die Geldbeträge werden unverändert angezeigt.
                                           Die Geldbeträge werden durch 1000 geteilt angezeigt. Bei dieser Einstel-
                                          lung sollten Sie angeben, wie viele Nachkommastellen angezeigt werden sol-
                                          len.

                                          Nachkommastellen Anzahl der Nachkommastellen, wenn die Geldbeträge
                                          geteilt durch 1000 angezeigt werden.
4.01 / 01-2017




                 A+W Business Statistik                                                                               F-27
                 Verkaufsstatistiken                                                                   Softwarereferenz




                                       Umsatz Verkauf – Restriktionen
                                       Statistik > Umsatz Verkauf > Register Restriktionen




                                       Abb. F-9      Umsatzstatistik – Restriktionen


                                       In diesem Register können Sie die Auswertungen auf bestimmte Bereiche ein-
                                       grenzen oder diese Bereiche ausschließen.

                                          Beispiel

                                          Register Auswahl:                 Register Restriktionen:
                                          •   Vertreter                     •   Vertreter 1
                                          •   Kundengruppe                  •   Kundengruppe 3 - 7
                                          •   Kunde                         •   Nicht Kunde 4000
                                          •   Produkt                       •   Produkt 103 - 106


                                       Auswahl der Restriktionen

                                       Nicht Sie können die in den Feldern von und bis angegebenen Bereiche ein-
                                       oder ausschließen.
                                        Die Statistik wird auf die angegebenen Restriktionen eingeschränkt.
                                        Die angegebenen Restriktionen werden nicht in die Statistik aufgenommen.

                                       Von, bis Restriktion, die in die Statistik aufgenommen oder aus ihr ausge-
                                       schlossen werden soll.
4.01 / 01-2017




                 F-28                                                                            A+W Business Statistik
                 Softwarereferenz                                                                 Verkaufsstatistiken




                                          Mindestumsatz für Auswertung Angabe des Mindestumsatzes, ab dem
                                          die Werte in die Auswertungen mit einbezogen werden.
                                          Mit der Wahl der Option legen Sie fest, ob sich der angegebene Mindestum-
                                          satz auf ein Jahr oder einen Monat bezieht.


                                          Umsatz Verkauf – Tabelle
                                          Statistik > Umsatz Verkauf > Register Tabelle




                                          Abb. F-10   Umsatzstatistik – Tabelle


                                          In diesem Register wird das Ergebnis der Auswertung als Tabelle angezeigt.
                                          Über das Menü Druck können Sie das Ergebnis in tabellarischer Form dru-
                                          cken.
4.01 / 01-2017




                 A+W Business Statistik                                                                        F-29
                 Verkaufsstatistiken                                                            Softwarereferenz




                                       Umsatzstatistik – Grafik
                                       Statistik > Umsatz Verkauf > Register Grafik




                                       Abb. F-11   Umsatzstatistik – Grafik


                                       In diesem Register werden die Daten der Auswertung grafisch angezeigt.
4.01 / 01-2017




                 F-30                                                                    A+W Business Statistik
                 Softwarereferenz                                                                Verkaufsstatistiken




                                          Umsatz Verkauf – SQL
                                          Statistik > Umsatz Verkauf > Register SQL




                                          Abb. F-12   Umsatzstatistik – Grafik


                                          In diesem Register können Sie eigene SQL-Abfragen erstellen.
4.01 / 01-2017




                 A+W Business Statistik                                                                       F-31
                 Verkaufsstatistiken                                                               Softwarereferenz




                                       Superstatistik
                                       Statistik > Umsatz Verkauf > Menü Superstatistik > Einstellungen




                                       Abb. F-13   Gruppenstatistik Verwalten


                                       Über diesen Dialog werden die Daten für die Superstatistiken exportiert oder
                                       importiert.

                                       Voraussetzung und Ziel der Superstatistik
                                       Superstatistiken können nur von Hauptfirmen mit Filialen erstellt werden. Die
                                       Hauptfirma/Zentrale und die Filialen müssen per Datenaustausch miteinander
                                       kommunizieren können.
                                       In der Superstatistik werden die Umsatzdaten der Hauptfirma/Zentrale und der
                                       Filialen einander gegenüber gestellt.
                                       Die Filialen werden durch die Zuordnung in einer Superstatistik der Zentrale/
                                       Hauptfirma zu Mandanten.
4.01 / 01-2017




                 F-32                                                                       A+W Business Statistik
                 Softwarereferenz                                                                           Verkaufsstatistiken




                                                   Zentrale              Filialen

                                                                                         Folgende Verschiebung findet statt:
                                                Zentrale 1

                                                Filiale 2             Filiale 1          Filiale 1              Filiale 1
                  Mandanten                     Filiale 3             Filiale 2          Filiale 2              Filiale 2

                                                Filiale 4             Filiale 3          Filiale 3              Filiale 3



                 Abb. F-14    Superstatistik


                                               Die Zentrale legt fest, in welchen Abständen die Filialen ASCII-Dateien erstel-
                                               len und exportieren müssen. In der Zentrale werden alle gesammelten Filial-
                                               Daten in die Superstatistik importiert.
                                               Die Zentrale selbst kann auch eine Filiale sein und muss ihre eigenen Statistik-
                                               Daten ebenfalls exportieren.

                                               Dialogbeschreibung

                                               Mandant ID der Filiale oder des Mandanten, an den die Daten exportiert
                                               werden.

                                               Statistik Statistik, für die die Daten erstellt werden.

                                               Export Mandant ID des Mandanten, an den die Daten exportiert werden.
                                               Über diese ID liest das Importsystem die Daten beim (Ziel-)Mandanten ein.

                                               Import Pfad Verzeichnis, in dem die exportierten Daten liegen. Sie werden
                                               beim Ziel-Mandanten in einer Schleife nacheinander eingelesen.

                                               Protokoll Pfad Daten, die nicht importiert werden können, werden in einer
                                               Protokolldatei gespeichert. Der Administrator muss die fehlenden Stammda-
                                               ten anlegen und/oder die falschen Stammdaten korrigieren. Beim nächsten
                                               Import wird erneut versucht, den entsprechenden Datensatz einzulesen.

                                               Definition Import
                                               In diesem Bereich legt die importierende Zentrale fest, wie eingehende Daten
                                               standardmäßig gebucht werden sollen:
                                               • Integration immer auf default
                                               • Integration 1:1 oder auf default
                                               • Integration 1:1 zwingend

                                               Auswahl default In diesen Feldern legen Sie den Default-Satz fest, in den
                                               die importierten Daten geschrieben werden.
4.01 / 01-2017




                 A+W Business Statistik                                                                                     F-33
                 Verkaufsstatistiken                                                               Softwarereferenz




                                       Superstatistik – Export
                                       Statistik > Umsatz Verkauf > Menü Superstatistik > Exportieren




                                       Abb. F-15   Superstatistik – Export manuell


                                       In diesem Dialog exportieren Sie die ASCII-Dateien für die Superstatistik ma-
                                       nuell. Der manuelle Export stellt in der Praxis die Ausnahme dar. Normaler-
                                       weise werden die Einstellungen einmal in der Filiale vorgenommen, die
                                       Mandanten-Nummer wird eingestellt, und der Rest erfolgt automatisch.
                                       In der Regel werden die Daten bei der Archivübergabe auch an die Statistik
                                       übergeben: Dokumente > Auftrag > Übergabe Archiv > Checkbox Umsatzsta-
                                       tistik.

                                       Export

                                       Mandant (lokal) Mandant, der die Daten exportiert.

                                       Auswahl Datum von, bis Angabe der Zeitspanne, in der die Datei(en) mit
                                       den Umsatzdaten erzeugt wurden.

                                       Zieldatei überschreiben Im Exportverzeichnis kann bereits eine gleichna-
                                       mige Datei liegen. Wenn Sie sicher sind, dass diese bereits in die Auswertung
                                       der Superstatistik eingeflossen ist, können Sie die alte Datei überschreiben.
                                        Die alte Datei wird nicht überschrieben. Die neue Datei unterscheidet sich
                                       durch Datum und Zeitstempel.
                                        Die alte Datei wird überschrieben.

                                       Export Mandant ID der Filiale oder des Mandanten, an den die Daten ex-
                                       portiert werden, d. h. der Ziel-Mandant.

                                       Exportierte Sätze Anzahl der exportierten Datensätze in der Datei.

                                       Export Pfad Pfad und Dateiname,
                                       z. B. C:\Superstat\Export\0001_20140506.asc.
4.01 / 01-2017




                 F-34                                                                       A+W Business Statistik
                 Softwarereferenz                                                                   Verkaufsstatistiken




                                          Superstatistik – Import
                                          Statistik > Umsatz Verkauf > Menü Superstatistik > Importieren




                                          Abb. F-16   Superstatistik – Import manuell


                                          In diesem Dialog importieren Sie die ASCII-Dateien für die Superstatistik.
                                          Die aufgelaufenen Fehler werden im Systemlogbuch angezeigt und können
                                          über Protokoll-Dateien identifiziert werden.
                                          Protokolle werden mit der Endung .sav gespeichert.
4.01 / 01-2017




                 A+W Business Statistik                                                                           F-35
                 Verkaufsstatistiken                                                              Softwarereferenz




                                       Reklamationsstatistik Verkauf
                                       Statistik > Reklamation Verkauf




                                       Abb. F-17    Reklamationsstatistik Verkauf


                                       In diesem Dialog erstellen Sie Statistiken über die Reklamationen im Verkauf.
                                       Zu dieser Statistik werden alle Dokumente vom Typ Reklamationen herange-
                                       zogen.
                                       Die Felder sind ausführlich zum Dialog Umsatz Verkauf beschrieben.
                                        “Umsatz Verkauf” auf Seite F-21
                                       Für die Reklamationsstatistik müssen Sie eine Monatsauswertung erstellen.
                                       Auswertungen über den Reklamationsgrund, Verursacher und Reklamations-
                                       ort können nur erstellt werden, wenn Reklamationsgründe und Reklamations-
                                       verursacher in den Stammdaten angelegt sind.
4.01 / 01-2017




                 F-36                                                                       A+W Business Statistik
                 Softwarereferenz                                                                  Verkaufsstatistiken




                                          Statistik nach Aufbau
                                          Statistik > Statistik nach Aufbau
                                          In diesem Dialog erstellen Sie Auswertungen über den Aufbau Scheiben mit
                                          Stücklisten. Dabei werden nur fakturierte Aufträge ausgewertet.
                                          Das Ergebnis der Auswertung wird im Register Tabelle angezeigt und kann
                                          gedruckt werden.
                                          In diesem Dialog finden Sie folgende Register:
                                          •   “Statistik nach Aufbau – Auswahl” auf Seite F-37
                                          •   “Statistik nach Aufbau – Tabelle” auf Seite F-40


                                          Statistik nach Aufbau – Auswahl
                                          Statistik > Statistik nach Aufbau > Register Auswahl




                 Abb. F-18   Statistik nach Aufbau – Auswahl


                                          In diesem Register legen Sie die Auswertungskriterien fest.

                                          Menü Sperre aufheben
                                          Sie können die Datensätze für die Dauer der Auswertung sperren, damit wäh-
                                          rend der Auswertung keine Datensätze ergänzt oder verändert werden. Diese
                                          Funktion ist sinnvoll, wenn die Auswertung längere Zeit in Anspruch nimmt.
4.01 / 01-2017




                 A+W Business Statistik                                                                         F-37
                 Verkaufsstatistiken                                                              Softwarereferenz




                                       Auswertungszeitraum

                                       Jahr, Monat von, bis Angabe des Zeitraums, der ausgewertet werden soll.

                                       Abstandhalter
                                       Mit der Wahl der Option legen Sie für die Auswertung von ISO fest, welche Ab-
                                       standhalter berücksichtigt werden sollen:
                                       •   Gesamt:
                                           Alle ISO-Scheiben werden ausgewertet.
                                       •   TPS:
                                           Nur ISO-Scheiben mit TPS werden ausgewertet.
                                       •   ISO normal:
                                           Nur ISO-Scheiben ohne TPS werden ausgewertet.

                                       Typ
                                       Mit der Wahl der Option legen Sie den Typ der Produkte fest, die ausgewertet
                                       werden sollen:
                                       •   Isolierglas:
                                           Nur ISO wird ausgewertet. Mit dieser Option können Sie zusätzlich auch
                                           ISO mit Zusatzarbeiten auswerten lassen.
                                       •   Zusatzarbeiten:
                                           Nur Zusatzarbeiten werden ausgewertet.
                                       •   Glasarten:
                                           Nur die Glasarten werden ausgewertet. Die Checkbox Mit Zusatzarbeiten
                                           ist gesperrt.

                                       Mit Zusatzarbeiten Wenn Sie ISO auswerten wollen, können Sie zusätzlich
                                       das ISO mit Zusatzarbeiten auswerten.
                                        ISO-Scheiben werden ohne Zusatzarbeiten ausgewertet.
                                        Zusätzlich zu den ISO-Scheiben werden ISO-Scheiben mit Zusatzarbeiten
                                       ausgewertet.

                                       Auswahl von Restriktionen

                                       Vertreter von, bis Vertreter, auf die die Auswertung eingegrenzt werden
                                       soll.

                                       Kunde von, bis Kunden, auf die die Auswertung eingegrenzt werden soll.
4.01 / 01-2017




                 F-38                                                                       A+W Business Statistik
                 Softwarereferenz                                                                   Verkaufsstatistiken




                                          Trennung nach
                                          Sie können die Auswertung weiter auflösen. Die Daten werden dann z. B. pro
                                          Kunde und Produkt ausgegeben.
                                           Im Druck wird kein zusätzlicher Seitenumbruch eingefügt.
                                           Im Druck wird der zusätzliche Seitenumbruch eingefügt.

                                              Freigeschaltete Checkboxen
                                              • Die Checkboxen Modell, SZR, Absth.-Typ und Gas sind nur freigeschal-
                                                 tet, wenn Sie den Typ ISO gewählt haben.
                                              • Die Checkbox Dicke wird gesperrt, wenn Sie die Checkbox Produkte
                                                 markieren.

                                          Sortierung nach
                                          Mit der Wahl der Option legen Sie die Sortierung der Ausgabe fest:
                                          •   Kunde-Umsatz:
                                              Die Daten werden pro Kunde nach Umsatz absteigend sortiert.
                                          •   Umsatz-Kunde:
                                              Die Daten werden pro Umsatz nach Kunden sortiert.
                                          •   Kunde-Fläche:
                                              Die Daten werden pro Kunde nach Fläche absteigend sortiert.
                                          •   Kunde-Aufbau:
                                              Die Daten werden pro Kunde nach Aufbau sortiert.

                                          Summen

                                          Anzahl Einzel-Zeilen Anzahl der Zeilen, nach der eine Zwischensumme an-
                                          gezeigt werden soll. Wenn Sie 0 eintragen, werden keine Zwischensummen
                                          angezeigt.

                                          Zeilen insgesamt Anzahl der Zeilen, die angezeigt werden sollen.

                                          Sonstiges

                                          Mit Firmensummen Sie können die Summen der beteiligten Firmen anzei-
                                          gen lassen. Im Register Tabelle sind das die Spalten Stück Firma, Fläche Fir-
                                          ma, Umsatz Firma, Wert/Fläche Firma.
                                           Die Firmensummen werden nicht angezeigt.
                                           Die Firmensummen werden angezeigt.

                                          Spalten immer füllen Sie können die Anzeige von Namen und Kundennum-
                                          mern unterdrücken, wenn die gewählte Sortierung das übersichtlicher macht.
                                           Die Spalten werden nur gefüllt, wenn die Daten für den nächsten Kunden
                                          angezeigt werden.
                                           Die Spalten werden immer gefüllt.
4.01 / 01-2017




                                          Getr. n. Monaten Die Summen können nach Monaten gruppiert werden.
                                           Die Summen werden chronologisch angezeigt.
                                           Die Summen werden getrennt nach Monaten angezeigt.


                 A+W Business Statistik                                                                          F-39
                 Verkaufsstatistiken                                                                    Softwarereferenz




                                           Statistik nach Aufbau – Tabelle
                                           Statistik > Statistik nach Aufbau > Register Tabelle




                 Abb. F-19   Statistik nach Aufbau – Tabelle


                                           In diesem Register wird das Ergebnis der Auswertung angezeigt.
                                           Abhängig von den Filterkriterien im Register Auswahl werden zusätzlich fol-
                                           gende Spalten angezeigt:
                                           •   Modell:
                                               Anzeige, ob Modelle enthalten sind.
                                           •   SZR:
                                               Dicke des Abstandhalters (Rahmen).
                                           •   Rahmen Typ:
                                               Nummer der Produktgruppe, zu der der Abstandhalter (Rahmen) gehört.
                                           •   Gas:
                                               Produktnummer des Gases.
                                           Standardmäßig können folgende Spalten angezeigt werden:
                                           •   Vertreter, Kunde:
                                               Wenn Sie keine Eingrenzung im Bereich Auswahl von Restriktionen einge-
                                               stellt haben, werden die Namen nicht angezeigt.
                                           •   Aufbau:
                                               Scheibenaufbau, z. B. Float 5 mm + Therm 6 mm, wenn Produkte ange-
                                               zeigt werden, oder 4 + 4 + 8 mm, wenn die Dicke angezeigt wird.
                                           •   Stück.:
4.01 / 01-2017




                                               Stückzahl.
                                           •   Fläche:
                                               Gesamtfläche.


                 F-40                                                                             A+W Business Statistik
                 Softwarereferenz                                                                 Verkaufsstatistiken




                                          •   Lfm:
                                              Kantenlänge insgesamt.
                                          •   Sprossenfelder:
                                              Anzahle der Sprossenfelder. Die Anzahl wird nur angezeigt, wenn im Be-
                                              reich Typ die Option Isolierglas ausgewählt ist.
                                          •   Umsatz:
                                              Gesamtumsatz
                                          •   Fläche pro Stück:
                                              Durchschnittliche Fläche pro Stück.
                                          •   Wert pro Fläche:
                                              Wert der Fläche in Eigenwährung. z. B. €/qm.
                                          •   Wert Reklamationen:
                                              Gesamtwert aller Reklamationen pro Kunde in Eigenwährung.
                                          •   Wert Gutschriften:
                                              Gesamtwert aller Gutschriften pro Kunde in Eigenwährung.
                                          •   Stück Firma, Fläche Firma, Umsatz Firma, Wert/Fläche Firma:
                                              Anzeige der Gesamtsummen. Werden nur angezeigt, wenn im Bereich
                                              Sonstiges die Checkbox mit Firmensummen ausgewählt ist.
                                          •   Faktor:
                                              Verhältnis von Wert/Fläche Firma zu Wert pro Fläche.
                                          •   Zusatzarbeiten:
                                              Anzahl der Zusatzarbeiten. Wird nur angezeigt, wenn im Bereich Typ die
                                              Checkbox mit Zusatzarbeiten ausgewählt ist.
4.01 / 01-2017




                 A+W Business Statistik                                                                        F-41
                 Verkaufsstatistiken                                                                Softwarereferenz




                                       Kunden nach AV-Bereich
                                       Statistik > Kunden nach AV-Bereichen




                                       Abb. F-20    AV-Bereiche


                                       In diesem Dialog erstellen Sie Auswertungen über die AV-Bereiche. Sie kön-
                                       nen die Auswertung über alle AV-Bereiche starten oder auf einzelne eingren-
                                       zen. Ausgegeben werden jeweils die Umsatzwerte des angegebenen Jahres
                                       pro Kunde und Monat.

                                       Auswahl
                                       Mit der Wahl der Option legen Sie fest, welche AV-Bereiche betrachtet werden
                                       sollen:
                                       •   AV-Bereich auswählen:
                                           Der Bereich Auswahl der AV-Bereiche wird freigeschaltet. Die Statistik wird
                                           über alle AV-Bereiche erstellt, die in dieser Auswahl markiert sind.
                                       •   Alle AV-Bereiche mit Umsatz:
                                           Die Statistik wird über alle AV-Bereiche erstellt, in denen Umsatzwerte ge-
                                           funden wurden. Der Bereich Auswahl der AV-Bereiche wird gesperrt.

                                       Jahr Jahr, das betrachtet werden soll.
4.01 / 01-2017




                 F-42                                                                        A+W Business Statistik
                 Softwarereferenz                                                                     Verkaufsstatistiken




                                          Druck-Modus
                                          Mit der Wahl der Option legen Sie fest, ob die Statistik auf dem Bildschirm oder
                                          einem Drucker ausgegeben werden soll.

                                          Auswahl der AV-Bereiche
                                          In diesem Bereich sind alle AV-Bereiche aufgelistet. Die Auswahl ist nur frei-
                                          geschaltet, wenn die Option AV-Bereiche auswählen markiert ist. Die Statistik
                                          wird zu allen AV-Bereichen erstellt, deren Checkbox markiert ist.
4.01 / 01-2017




                 A+W Business Statistik                                                                             F-43
                 Einkaufsstatistiken                                                              Softwarereferenz




                                       Einkaufsstatistiken
                                       Neben den Umsatzinformationen stehen auch detaillierte Auswertungen für
                                       die Einkaufszahlen zur Verfügung.
                                       In diesem Kapitel finden Sie Informationen zu folgenden Themen:
                                       •   “Umsatzstatistik Einkauf” auf Seite F-44
                                       •   “Reklamationsstatistik Einkauf” auf Seite F-45
                                       •   “Liefertreue” auf Seite F-46
                                       •   “Analyse Verbrauch” auf Seite F-48


                                       Umsatzstatistik Einkauf
                                       Statistik > Umsatz Einkauf




                                       Abb. F-21    Umsatzstatistik Einkauf


                                       In diesem Dialog erstellen Sie Statistiken zum Einkauf. Dazu werden die Be-
                                       stellungen ausgewertet.
                                       Die Felder sind ausführlich zum Dialog Umsatz Verkauf beschrieben.
                                        “Umsatz Verkauf” auf Seite F-21
4.01 / 01-2017




                 F-44                                                                       A+W Business Statistik
                 Softwarereferenz                                                                   Einkaufsstatistiken




                                          Reklamationsstatistik Einkauf
                                          Statistik > Reklamation Einkauf




                                          Abb. F-22    Reklamationsstatistik Einkauf


                                          In diesem Dialog erstellen Sie Statistiken über die Reklamationen im Einkauf.
                                          Zu dieser Statistik werden alle fakturierten Bestellungen herangezogen.
                                          Die Felder sind ausführlich zum Dialog Umsatz Verkauf beschrieben.
                                           “Umsatz Verkauf” auf Seite F-21
4.01 / 01-2017




                 A+W Business Statistik                                                                           F-45
                 Einkaufsstatistiken                                                                     Softwarereferenz




                                            Liefertreue
                                            Statistik > Liefertreue




                 Abb. F-23    Liefertreue


                                            In diesem Dialog erstellen Sie Statistiken über die Verzögerungen, die bei Lie-
                                            ferungen oder Aufträgen aufgetreten sind. Für die Auswertung werden die Ter-
                                            minverschiebungen herangezogen.

                                            Auswahl

                                            Modus Mit der Wahl der Option legen Sie fest, nach welchen Partnern aus-
                                            gewertet werden soll:
                                            • Kunden:
                                              Die Lieferterminverschiebungen werden ausgewertet. Diese Verschiebun-
                                              gen können z. B. durch verspätete Lieferungen von Bestellteilen oder
                                              durch Produktionstermine entstanden sein.
                                            • Lieferanten:
                                              Verspätete Lieferungen durch die Lieferanten werden ausgewertet.

                                            Datenbank Mit der Wahl der Option legen Sie fest, welcher Datenumfang
                                            ausgewertet werden soll:
                                            • Hauptdatenbank + aktuelles Archiv:
                                               Die Hauptdatenbank und das aktuell Archivjahr werden ausgewertet.
                                            • Archivjahr:
                                               Nur ein bestimmtes Archiv wird ausgewertet. Das Feld für die Auswahl des
                                               Archives wird freigeschaltet. Bei dieser Einstellung werden keine Doku-
4.01 / 01-2017




                                               mente berücksichtigt, die in der Hauptdatenbank liegen.




                 F-46                                                                             A+W Business Statistik
                 Softwarereferenz                                                                 Einkaufsstatistiken




                                          Einschränkungen

                                          Zeitraum von, bis Zeitraum, der ausgewertet werden soll.

                                          Auswertungsgrenze 1, 2 Anzahl von Verspätungstagen. Mit der Auswahl
                                          ändert sich die Anzeige in den Tabellenspalten.

                                          Kundennummer von, bis Kunden oder Folge von Kunden, zu denen Verzö-
                                          gerungen ausgewertet werden sollen.

                                          Kundengruppe Kundengruppe, zu der Verzögerungen ausgewertet werden
                                          sollen.

                                          Nicht einschränken Alle Kunden sollen ausgewertet werden.

                                          Tabelle
                                          In der Übersicht wird das Ergebnis der Auswertung pro Kunde oder Lieferant
                                          angezeigt.
                                          •  Ø Tage früher, Ø Tage später:
                                             Durchschnitt aus beiden Auswertungsgrenzen in Tagen.
                                          • > n Tage früher:
                                             Anzahl der Aufträge pro Auswertungsgrenze, die über der Grenze lagen.
                                             Bei Lieferanten sind das die Bestellungen, die über der Grenze lagen.
                                          • < n Tage später:
                                             Anzahl der Aufträge pro Auswertungsgrenze, die unter der Grenze lagen.
                                          • Pünktlich:
                                             Anzahl der Aufträge, die zum vereinbarten Termin geliefert wurden.
                                          Die Anzeige schließt mit einer Summenzeile.
4.01 / 01-2017




                 A+W Business Statistik                                                                        F-47
                 Einkaufsstatistiken                                                                  Softwarereferenz




                                          Analyse Verbrauch
                                          Statistik > Analyse Verbrauch
                                          Sie können den Materialverbrauch nach selbst gewählten Kriterien auswerten.
                                          In diesem Dialog finden Sie folgende Register:
                                          •   “Analyse Verbrauch – Auswahl” auf Seite F-48
                                          •   “Analyse Verbrauch – Restriktionen” auf Seite F-51
                                          •   “Analyse Verbrauch – Tabelle” auf Seite F-53

                                          Menü Optionen
                                          •   Automatischer Seitenvorschub aktiv:
                                              Im Druck wird automatisch ein Seitenumbruch eingefügt.


                                          Analyse Verbrauch – Auswahl
                                          Statistik > Analyse Verbrauch > Register Auswahl




                 Abb. F-24    Analyse Verbrauch – Auswahl


                                          In diesem Register legen Sie die Kriterien für die Auswertung fest.
4.01 / 01-2017




                 F-48                                                                          A+W Business Statistik
                 Softwarereferenz                                                                  Einkaufsstatistiken




                                          Quelle

                                          Nummer Auftrag, der ausgewertet werden soll.

                                          Archiv Die Archive können in die Suche nach einem einzelnen Auftrag ein-
                                          geschlossen werden.
                                           Nur in der Hauptdatenbank wird nach dem Auftrag gesucht.
                                           In der Hauptdatenbank und in den Archiven wird nach dem Auftrag gesucht.

                                          Nummernverwalter Auswahl des Nummernverwalters. Mit dieser Option
                                          werden die Felder im Bereich Auswertungszeitraum gesperrt.

                                          Mandant Mandant, auf den die Auswertung eingeschränkt werden soll.

                                          AV-Bereich AV-Bereich, auf den die Auswertung eingeschränkt werden soll.

                                          Auswertungszeitraum
                                          Die Felder in diesem Bereich sind gesperrt, wenn die Option Nummernverwal-
                                          ter gewählt ist.

                                          Nach Liefertermin von, bis Zeitraum von Lieferterminen, der ausgewertet
                                          werden soll.

                                          Nach Produktionstermin von, bis Zeitraum von Produktionsterminen, der
                                          ausgewertet werden soll.

                                          Auswahl Statusbereich

                                          Von, bis Statusbereich der Dokumente, die ausgewertet werden sollen.

                                          Auswahl Produkt

                                          Produktart Produktart, die ausgewertet werden soll. Sie können die Stan-
                                          dardauswahl <k.A.> löschen.

                                          Produktgruppe Produktgruppe, die ausgewertet werden soll.

                                          Artikel Produkt, das ausgewertet werden soll.

                                          Sortierung / Summenbildung
                                          Sie können festlegen, nach welchen Kriterien das Ergebnis sortiert werden
                                          soll. Pro ausgewähltem Kriterium wird eine Summe gebildet.

                                          Auswahlfelder Die ausgewählten Kriterien werden im rechten Feld ange-
                                          zeigt und können dort mit den Pfeil-Schaltflächen in die gewünschte Reihen-
                                          folge verschoben werden.
4.01 / 01-2017




                 A+W Business Statistik                                                                         F-49
                 Einkaufsstatistiken                                                               Softwarereferenz




                                       Auflösung pro Auftrag Das Ergebnis kann detailliert nach Aufträgen ange-
                                       zeigt werden.
                                        Pro Sortierkriterium wird eine Zeile angezeigt.
                                        Pro Sortierkriterium und Auftrag wird eine Zeile angezeigt.

                                       Auflösung pro Position Das Ergebnis kann nach Positionen angezeigt
                                       werden.
                                        Pro Sortierkriterium wird eine Zeile angezeigt. Wenn nach Aufträgen aufge-
                                       löst wird, werden die Auftragspositionen nicht einzeln aufgeführt.
                                        Pro Sortierkriterium und Auftragsposition wird eine Zeile angezeigt.

                                       Auswahl Produktbereich
                                       Sie können die Statistik auf einzelne Produktbereiche folgender Glasarten ein-
                                       schränken: EFG (Einfachglas), ESG, VSG, ISO.
                                        Die Daten aus diesem Produktbereich werden nicht in der Statistik ausge-
                                       geben.
                                        Die Daten aus diesem Produktbereich werden in der Statistik ausgegeben.

                                       Optionen

                                       Gasberechnung individuell Zur Zeit nicht genutzt.

                                       Mengeneinheit Mengeneinheit, in der Gas angegeben werden soll.
4.01 / 01-2017




                 F-50                                                                       A+W Business Statistik
                 Softwarereferenz                                                                  Einkaufsstatistiken




                                          Analyse Verbrauch – Restriktionen
                                          Statistik > Analyse Verbrauch > Register Restriktionen




                 Abb. F-25   Analyse Verbrauch – Restriktionen


                                          In diesem Register können Sie die Auswahl der Analyse nach Verbrauch wei-
                                          ter einschränken.

                                          Quelle
                                          Mit der Wahl der Option legen Sie fest, welche Dokumente ausgewertet wer-
                                          den sollen:
                                          •   Nummer:
                                              Ein einzelner Auftrag soll ausgewertet werden. Das Feld zur Eingabe der
                                              Auftragsnummer und die Checkbox Archiv werden freigeschaltet.
                                          •   Nummernverwalter:
                                              Die Aufträge eines Nummernverwalters sollen ausgewertet werden.

                                          Archiv Das angegebene Dokument kann auch im Archiv gesucht werden.
                                           Die Archive werden nicht durchsucht.
                                           Das Dokument soll im Archiv gesucht werden, wenn es nicht in der Haupt-
                                          datenbank gefunden wurde. Diese Einstellung ist sinnvoll, wenn Sie Doku-
                                          mente in kurzen Zeiträumen archivieren.

                                          Mandant Mandant, auf den die Auswertung eingeschränkt werden soll.
4.01 / 01-2017




                                          AV-Bereich AV-Bereich, der ausgewertet werden soll.




                 A+W Business Statistik                                                                         F-51
                 Einkaufsstatistiken                                                            Softwarereferenz




                                       Auswertungszeitraum
                                       Mit der Wahl der Option legen Sie fest, aus welchem Zeitraum Dokumente
                                       ausgewertet werden sollen:
                                       •   Nach Lieferdatum:
                                           Der angegebene Zeitraum bezieht sich auf das Lieferdatum.
                                       •   Nach Produktionstermin:
                                           Der angegebene Zeitraum bezieht sich auf den Termin, an dem die Pro-
                                           duktion begonnen wurde.

                                       Von, bis Zeitraum, der ausgewertet werden soll.

                                       Auswahl Statusbereich

                                       Von, bis Statusbereich der Dokumente, die ausgewertet werden sollen.

                                       Auswahl Produkt

                                       Produktart Produktart, die ausgewertet werden soll.

                                       Produktgruppe Produktgruppe, die ausgewertet werden soll.

                                       Artikel Produkt, das ausgewertet werden soll.

                                       Auswahl Beschaffungsarten
                                       Die Auswertung kann zusätzlich auf Beschaffungsarten eingegrenzt werden.
                                        Die Beschaffungsart wird nicht berücksichtigt.
                                        Nur Produkte mit dieser Beschaffungsart sollen ausgewertet werden.

                                       Auswahl Produktarten
                                       Die Auswertung kann zusätzlich auf Produktarten eingegrenzt werden.
                                        Die Produktart wird nicht berücksichtigt.
                                        Nur Produkte dieser Produktart sollen ausgewertet werden.
4.01 / 01-2017




                 F-52                                                                     A+W Business Statistik
                 Softwarereferenz                                                                     Einkaufsstatistiken




                                          Analyse Verbrauch – Tabelle
                                          Statistik > Analyse Verbrauch > Register Tabelle




                 Abb. F-26   Analyse Verbrauch – Tabelle


                                          In diesem Register wird das Ergebnis der Auswertung angezeigt. Die Anzeige
                                          der Spalten und Zeilen richtet sich nach den Einstellungen, die Sie im Register
                                          Auswahl festgelegt haben.
4.01 / 01-2017




                 A+W Business Statistik                                                                             F-53
                 Provisionsstatistik                                                                     Softwarereferenz




                                             Provisionsstatistik
                                             Statistik > Provisionsstatistik




                 Abb. F-27    Provisionsstatistik


                                             In diesem Dialog werten Sie die Vertreterprovisionen aus.

                                             Auswahl

                                             Vertreter Vertreter, wenn die Auswertung auf einen einzelnen Vertreter ein-
                                             geschränkt werden soll.

                                             Von, bis Zeitraum, der ausgewertet werden soll.
                                             Mit der Wahl der Option legen Sie fest, worauf sich der Zeitraum bezieht:
                                             • Nach Rechnungsdatum:
                                                Mit dieser Einstellung werten Sie nur fakturierte Dokumente aus.
                                             • Nach Erfassungsdatum:
                                                Mit dieser Einstellung werten Sie alle Dokumente im angegebenen Zeit-
                                                raum aus.
                                             • Nach Übergabedatum:
                                                Mit dieser Einstellung werten Sie die Dokumente aus, die im angegebenen
                                                Zeitraum an die Statistik übergeben wurden.
4.01 / 01-2017




                 F-54                                                                            A+W Business Statistik
                 Softwarereferenz                                                                    Provisionsstatistik




                                          Zwischensumme
                                          Sie können einstellen, ob und wo Zwischensummen gebildet werden sollen.

                                          Pro Vertreter Wenn Sie die Dokumente für alle Vertreter auswerten, können
                                          Sie pro Vertreter eine Zwischensumme bilden lassen.
                                           Zwischensummen werden nicht gebildet. Diese Einstellung ist dann sinn-
                                          voll, wenn Sie die Auswertung für einen bestimmten Vertreter erstellen lassen.
                                           Nach jedem Vertreter wird eine Zwischensumme eingefügt.

                                          Pro Kunde Wenn Sie die Dokumente über einen längeren Zeitraum aus-
                                          werten, können Sie pro Kunde eine Zwischensumme bilden lassen.
                                           Zwischensummen werden nicht gebildet.
                                           Pro Kunde wird eine Zwischensumme eingefügt.

                                          Ergebnis
                                          In der Übersicht werden folgende Spalten angezeigt.
                                          •   Vertreter:
                                              Name des Vertreters.
                                          •   Nr. Rechnung, Datum Rechnung:
                                              Nummer und Datum der Rechnung.
                                          •   Nr. Auftrag:
                                              Auftragsnummer.
                                          •   Datum Erfassung:
                                              Erfassungsdatum.
                                          •   Summe Umsatz:
                                              Gesamtsumme des Auftrags.
                                          •   % Provision:
                                              Provisionssatz im Auftrag.
                                          •   Summe Provision:
                                              Betrag der Provision.
                                          •   ID Kunde, Name Kunde:
                                              Nummer und Name des Kunden.
                                          •   Datum Übergabe:
                                              Übergabe an die Statistik.
                                          •   Land:
                                              Land, in dem der Kunde ansässig ist.
4.01 / 01-2017




                 A+W Business Statistik                                                                           F-55
                 Intrastat Meldung                                                                  Softwarereferenz




                                          Intrastat Meldung
                                          Statistik > Intrastat Meldungen




                 Abb. F-28   Intrastat Meldung


                                          In diesem Dialog erstellen Sie Auswertungen zu den Intrastat-Meldungen.

                                          Indentifikation

                                          Mandant Mandant, für dessen Dokumente die Statistik erstellt wird.

                                          Mitarbeiter Angemeldeter Mitarbeiter.

                                          NV Aufträge Nummernverwalter, in dem die Aufträge gesammelt sind.

                                          NV Gutschriften Nummernverwalter, in dem die Gutschriften gesammelt
                                          sind.

                                          Vorgabe

                                          Archiv Archiv, dessen Dokumente ausgewertet werden sollen.

                                          Neuen NV anlegen
                                          Die Felder in diesem Bereich sind nur freigeschaltet, wenn Sie einen neuen
                                          Nummernverwalter anlegen. Wählen Sie dazu Menü Start > [Neu].
4.01 / 01-2017




                                          Rechnungsdatum von, bis Zeitraum, in dem die Aufträge fakturiert wur-
                                          den.


                 F-56                                                                         A+W Business Statistik
                 Softwarereferenz                                                                 Intrastat Meldung




                                          Länderkennzeichen Land, zu dem Sie die Statistik erstellen wollen. Zur
                                          Wahl stehen nur die Länderkennzeichen, die in den Stammdaten angelegt
                                          sind.

                                          Name NV Aufträge Eingabe des Namens. Wählen Sie einen sprechenden
                                          Namen, damit Sie erkennen können, welche Dokumente in diesem Nummern-
                                          verwalter gesammelt sind.

                                          Name NV Gutschriften Eingabe des Namens. Wählen Sie einen sprechen-
                                          den Namen, damit Sie erkennen können, welche Gutschriften in diesem Num-
                                          mernverwalter gesammelt sind.

                                          Zu meldende Dokumente
                                          In der Übersicht werden alle Dokumente angezeigt, die im gewählten Num-
                                          mernverwalter zusammengestellt sind.
                                          •   Best. Land:
                                              Land aus dem die Ware eingeführt wurde.
                                          •   Nummer:
                                              Auftragsnummer.
                                          •   Bestell-Nr.:
                                              Bestellnummer.
                                          •   AB-Lieferant:
                                              Nummer der Auftragsbestätigung durch den Lieferanten.
                                          •   Rechnung:
                                              Nummer der Rechnungsnummer zum Kundenautrag.
                                          •   Datum Anlief. Lief.:
                                              Datum der Anlieferung durch den Lieferanten.
                                          •   Auftrags-Nummer:
                                              Auftragsnummer.
                                          •   Datum Auslieferung:
                                              Lieferdatum ab Werk.
                                          •   Kunde/Lieferant:
                                              Kunden- oder Lieferantennummer.
                                          •   Name, Matchcode:
                                              Name und Matchcode des Kunden oder Lieferanten.
                                          •   Status:
                                              Dokumentenstatus.
                                          •   Datum Erfass.:
                                              Erfassungsdatum des Dokumentes.
                                          •   Datum AB:
                                              Datum der Auftragsbestätigung.
                                          •   Datum Prod. ISO, VSG, ESG:
                                              Produktionsdatum für die Glasart.
                                          •   Lauf-Nr. Prod. ISO, VSG, ESG:
                                              Nummer des Produktionslaufs.
                                          •   Anlieferdatum:
4.01 / 01-2017




                                              Lieferdatum beim Kunden.
                                          •   Lieferschein:
                                              Lieferscheinnummer.


                 A+W Business Statistik                                                                      F-57
                 Intrastat Meldung                                                           Softwarereferenz




                                     •   Datum Lieferung:
                                         Lieferdatum.
                                     •   Rechnung, Datum Rechnung:
                                         Nummer und Datum der Rechnung.
                                     •   Stück gesamt:
                                         Gesamtstückzahl.
                                     •   Qm real:
                                         Fläche insgesamt.
                                     •   LFM real:
                                         Tatsächliche Laufmeter der Kantenlänge.
                                     •   Gewicht gesamt:
                                         Gesamtgewicht.
                                     •   Qm fakturiert:
                                         Fakturierte Gesamtfläche.
                                     •   LFM fakturiert:
                                         Fakturierte Kantenlänge.
                                     •   Betrag Netto:
                                         Rechnungsbetrag netto.
                                     •   Tour:
                                         Name der Liefertour.
                                     •   Geschäftsart:
                                         Bezeichnung der Geschäftsart.
                                     •   AV-Bereich:
                                         Bezeichnung des AV-Bereichs.
                                     •   Vertreter 1, Vertreter 2:
                                         Namen der beteiligten Vertreter.
                                     •   Sperr-KZ:
                                         Sperrkennzeichen aus den Zusatzinformationen zum Auftrag.
4.01 / 01-2017




                 F-58                                                                  A+W Business Statistik
Statistik              F

                 Partindex




            A+W Business
                 Partindex                                                                 Index Statistik




                 Index Statistik
                 A                                    K
                 Analyse                              Kunden
                 – Verbrauch F-48                     – nach AV-Bereichen     F-42
                 Anzeige Beträge F-27
                 Aufbau                               L
                 – Auswahl der Statistik F-37         Liefertreue   F-46
                 – Ergebnis der Statistik F-40
                 – Statistik F-37
                 Auflistung nach F-13                 O
                 Auftragsinformation F-10             Optionen
                 – Druckeinstellung F-20              – Auftragsinfo F-11
                 – Erfasst F-15
                 – Fakturiert F-17                    P
                 – Grafik F-19                        Provision
                 – Offen F-18                         – Statistik F-54
                 – Optionen F-11                      – Statistik nach Vertretern   F-54
                 – Produziert F-16
                 Auswahl                              R
                 – Rubriken in Umsatzstatistik F-26   Reklamationsstatistik
                 – Umsatz VK, EK F-23                 – Einkauf F-45
                 – Verbrauchsanalyse F-48             – Verkauf F-36
                 AV-Bereich                           Restriktionen
                 – Kundenstatistik F-42               – Umsatz VK, EK F-28
                                                      – Verbrausanalyse F-51
                 D
                 Druck                                S
                 – Auftragsinfo     F-20              SQL
                                                      – Umsatz VK, EK F-31
                 E                                    Statistik
                 Einkauf                              – Liefertreue F-46
                 – Reklamationsstatistik F-45         – Umsatz VK, EK F-29
                 – Umsatz F-44                        Superstatistik
                 Einstellung                          – Einstellungen F-32
                 – Superstatistik F-32                – Export F-34
                 Ergebnis                             – Import F-35
                 – Verbrauchsanalyse F-53             – Menü F-22
                 Export                               – Ziel, Voraussetzung F-32
                 – Superstatistik F-34
                                                      T
                 G                                    TOP10-Statistik F-25
                 Grafik                               – Auswertung, Sortierung      F-27
                 – Auftragsinfo F-19
                 – Umsatz VK, EK F-30                 U
                 – Umsatzstatistik F-30               Übersicht
4.01 / 01-2017




                                                      – erfasste Aufträge F-15
                 I                                    – fakturierte Aufträge F-17
                 Import                               – offene Aufträge F-18
                 – Superstatistik    F-35             – produzierte Aufträge F-16


                 A+W Business Statistik                                                             F-61
                 Index Statistik                                            Partindex




                 Umsatz
                 – Ausgabe, Summenbildung, Sortierung   F-23
                 – Auswahl F-23
                 – Einkauf F-44
                 – Ergebnis F-29
                 – Grafik F-30
                 – Restriktionen F-28
                 – SQL-Abfrage F-31
                 – Verkauf F-21

                 V
                 Verbrauch
                 – Analyse F-48
                 Verbrauchsanalyse
                 – Ergebnis F-53
                 – Restriktionen F-51
                 Vergleich mit Vorjahreswerten   F-14
                 Verkauf
                 – Grafik F-30
                 – Reklamationsstatistik F-36
                 – Umsatz F-21
4.01 / 01-2017




                 F-62                                          A+W Business Statistik

