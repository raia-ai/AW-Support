---
title: "DE AWEnterprise Versandsteuerung"
category: "user_manuals"
product: "Unknown"
doc_type: "Unknown"
language: "EN"
tags: ["DE_AWEnterprise_Versandsteuerung"]
version: "1.0"
last_updated: "2025-12-10"
description: "Versandsteuerung              G                                   deutsch                        A+W Enterprise                                                                                                           Vorspann                                            Vorspann                                        In diesem Teil der Dokumentation finden Sie editorische Notizen.                                          Revisionsübersicht                                        Part"
source_file: "DE_AWEnterprise_Versandsteuerung.pdf"
---


# DE AWEnterprise Versandsteuerung

Versandsteuerung              G




                              deutsch




                   A+W Enterprise
                                                                                                          Vorspann




                                       Vorspann
                                       In diesem Teil der Dokumentation finden Sie editorische Notizen.


                                       Revisionsübersicht
                                       Part             Software   Beschreibung
                                       Version/Datum    Version

                                       2.00/ 04-2022    6          Aktualisierung der Softwarereferenz.

                                       1.03 / 01-2017   5.2.4      Produkt- und Firmennamen angepasst.

                                       1.02 / 02-2014   5.2.4      Produktnamen aktualisiert

                                       1.01 / 01-2013   5.2.4      Layout an CI 2013 angepasst

                                       1.00 / 11-2012   5.2.4      Ersterstellung



                                       Editorial
                                       Das Editorial enthält Informationen zu folgenden Themen:
                                       •   Anmerkungen zu diesem Dokument
                                       •   Urheberrechte
                                       •   Warenzeichen
                                       •   Kontakte

                                       Anmerkungen zu diesem Dokument
                                       Diese Veröffentlichung ist ausschließlich für Endanwender von A+W Enterpri-
                                       se gedacht.
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
                                       stufe von A+W Enterprise.

                                       Urheberrechte
2.00 / 04-2022




                                       © 2022, A+W Software GmbH, alle Rechte, auch des Nachdrucks, der Her-
                                       stellung von Kopien und der Übersetzung, bleiben vorbehalten.




                 A+W Enterprise Versandsteuerung                                                              G-3
                 Vorspann




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
                            35415 Pohlheim
                            +49 6404 2051-0
                            +49 6404 2051 877
                            Zentrale@a-w.com
                            http://www.a-w.com
2.00 / 04-2022




                 G-4                                                  A+W Enterprise Versandsteuerung
                                                                                                                                                           Inhalt




                                       Inhalt
                                       Vorspann ............................................................................................................... G-3
                                        Revisionsübersicht ............................................................................................. G-3
                                        Editorial .............................................................................................................. G-3

                                       Softwarereferenz                                                                                                    G-7
                                       Übersicht ................................................................................................................ G-9
                                       Startfunktionen ..................................................................................................... G-10
                                         Programmstart .................................................................................................. G-11
                                         Auftragssuche .................................................................................................. G-13
                                         Marktpartnersuche ........................................................................................... G-14
                                       Versand-Explorer ................................................................................................. G-15
                                         Explorer – Baumstruktur ................................................................................... G-16
                                           Übersicht für die Lieferdatumsebene ............................................................ G-17
                                           Übersicht für die Tourenebene ..................................................................... G-19
                                           Übersicht für die Auftragsebene ................................................................... G-20
                                           Übersicht für die Positionsebene .................................................................. G-21
                                       Versandsteuerung – Menüs ................................................................................. G-22
                                         Zusatzmenü ...................................................................................................... G-22
                                         Infomenü .......................................................................................................... G-25
                                         Schaltflächen .................................................................................................... G-27
                                       Touren ................................................................................................................. G-28
                                         Register – TourenInfo ....................................................................................... G-29
                                         Register – GestellInfo ....................................................................................... G-32
                                         Register – FahrzeugInfo ................................................................................... G-34
                                         Register – Optimierung .................................................................................... G-36
                                       Auftragsebene ..................................................................................................... G-38
                                         Register – AuftragsInfo ..................................................................................... G-39
                                         Register– AuftragsInfo/Gestell ......................................................................... G-44
                                         Register– Lieferanschrift .................................................................................. G-46
                                         Register – VersandInfo I ................................................................................... G-48
                                         Register – VersandInfo II .................................................................................. G-51
                                         Register – ZusatzInfo ....................................................................................... G-53
                                       Positionsebene .................................................................................................... G-56
                                         Register – PositionsInfo I ................................................................................. G-57
                                         Register – PositionsInfo II ................................................................................ G-60
                                       Funktionen im Versand ........................................................................................ G-62
                                         Suchen ............................................................................................................. G-63
                                         Springen ........................................................................................................... G-64
                                         Verschieben ..................................................................................................... G-66
                                         Verschieben mehrerer Pos. - Auswahl ............................................................. G-69
                                         Verschiebung mehrerer Pos. - Aktion .............................................................. G-70
                                         Auftragsinfo ...................................................................................................... G-72
                                           Informationen zum Auftrag ............................................................................ G-73
                                         Liefereingang buchen ....................................................................................... G-76
                                         Storno des Liefereingangs ............................................................................... G-77
                                         Fehlmengenkontrolle - Auswahl ....................................................................... G-78
                                         Fehlmengenkontrolle - Aktion ........................................................................... G-80
                                         Buchen auf Transport ....................................................................................... G-82
                                         Transport zurückbuchen ................................................................................... G-83
                                         Barcode Gestellanzeige ................................................................................... G-84
2.00 / 04-2022




                                         Ergebnisse der Gestellplanung ........................................................................ G-85
                                         Packmittelplanung ............................................................................................ G-86
                                         Lieferanschrift suchen ...................................................................................... G-87
                                         Neue Lieferanschrift ......................................................................................... G-88


                 A+W Enterprise Versandsteuerung                                                                                                             G-5
                 Inhalt




                            Gestellinformationen ........................................................................................ G-89
                            Toursperre setzen/löschen ............................................................................... G-90
                            Alle Touren sperren .......................................................................................... G-91
                            Transportdaten ................................................................................................. G-92
                            Lagerkommissionierung ................................................................................... G-93
                          Storno .................................................................................................................. G-94
                            Lieferscheinstorno ............................................................................................ G-94
                            Auftragsstorno .................................................................................................. G-95
                            Wareneingangsstorno ...................................................................................... G-96
                            Storno des Versandstatus ................................................................................ G-97
                          Gestelle ................................................................................................................ G-98
                            Gestellzuordnung - Auswahl ............................................................................ G-99
                            Gestellzuordnung - Anzeige ........................................................................... G-100
                            Gestellauflösung - Auswahl ............................................................................ G-102
                            Gestellauflösung - Anzeige ............................................................................ G-102
                            Freie Gestelle (Übersicht) .............................................................................. G-104
                            Gebuchte Gestelle (Übersicht) ....................................................................... G-106
                            Alle Gestelle (Übersicht) ................................................................................. G-107
                            Einzelne Gestelle ........................................................................................... G-109
                            Gestelle zu Auftrag ......................................................................................... G-110
                            Scheibenzuordnung ....................................................................................... G-112
                            VK/EK Information .......................................................................................... G-115
                            VK/EK Info (Global) ........................................................................................ G-117
                            Versandsteuerung - Übersicht ........................................................................ G-119
                            Lieferterminänderungen ................................................................................. G-122
                            Versandinformationen .................................................................................... G-123
                            Via Details ...................................................................................................... G-124
                            Fertigwarenlager ............................................................................................ G-125
                              Fertigwarenlagerbestand ............................................................................ G-126
                              Fertigwarenlager Übersicht ......................................................................... G-127
                              Fertigwarenlager Inventur ........................................................................... G-128
                              Inventur abschließen ................................................................................... G-128
                              Protokoll ...................................................................................................... G-129
                            Grafische Tourenübersicht ............................................................................. G-131
                          Drucken ............................................................................................................. G-132
                            Drucken einer Ladeliste .................................................................................. G-133
                            Drucken aller Ladelisten ................................................................................. G-134
                            Drucken Ergänzungsladelisten ....................................................................... G-135
                            Listendruck ..................................................................................................... G-136
                            Vorablieferschein Druck ................................................................................. G-137
                            Lief./Wareneing. Freigabe + Druck ................................................................ G-139
                            Druckformat .................................................................................................... G-140
                            Druckerauswahl .............................................................................................. G-140

                          Partindex                                                                                                     G-141
                          Index .................................................................................................................. G-143
2.00 / 04-2022




                 G-6                                                                         A+W Enterprise Versandsteuerung
Versandsteuerung                G

                    Softwarereferenz




                   A+W Enterprise
                 Softwarereferenz                                                                               Übersicht




                                       Übersicht
                                       Alle Ansichten, Dialoge und Funktionen für die Versandsteuerung sind über
                                       das Modul Logistik erreichbar. Sie können das Modul auch direkt aus dem Fix-
                                       Win starten. In der Standard-Konfiguration starten Sie direkt mit dem Versand-
                                       Explorer:
                                        “Versand-Explorer” auf Seite G-15
                                       Mit der Versandsteuerung finden, planen, bearbeiten und versenden Sie ter-
                                       mingerecht Ihre Lieferaufträge. Die Versandsteuerung ist die Steuerzentrale
                                       für das Versandgeschäft und ermöglicht den einfachen und schnellen Zugriff
                                       auf alle Lieferaufträge. Sie erstellen z. B. eine Auflistung aller Liefertermine ei-
                                       nes Zeitraums oder springen direkt in den gesuchten Lieferauftrag. Für die
                                       Übersicht der Versandvorgänge ist jeder Lieferauftrag in die folgenden vier
                                       Ebenen eingeteilt:
                                       •   Liefertermine
                                       •   Touren mit Routen
                                       •   Aufträge
                                       •   Positionen
                                       Die Liefertermine sehen Sie in der ersten Ebene. Ein Liefertermin enthält die
                                       zugehörigen Touren oder Routen.
                                       Die Touren mit den Routen sehen Sie in der zweiten Ebene. Eine Tour enthält
                                       die zugehörigen Aufträge und kann aus einer oder mehreren Routen beste-
                                       hen. Eine Tour steht für mindestens eine Route, die zu einem bestimmten Lie-
                                       fertermin gefahren wird. Die Route steht für eine festgelegte Fahrstrecke. Die
                                       Routen können auf bestimmte Wochentage oder auf bestimmte Zeiten festge-
                                       legt werden. In der Tourenebene haben Sie eine Übersicht zu den vorhande-
                                       nen Versandpapieren.
                                       Die Aufträge sehen Sie in der dritten Ebene. Ein Auftrag enthält die zugehöri-
                                       gen Positionen und die Lieferanschrift. In der Auftragsebene haben Sie eine
                                       Übersicht zu den vorhandenen Versandpapieren.
                                       Die Positionen sehen Sie in der vierten Ebene. Eine Position enthält die zuge-
                                       hörigen Einheiten.
                                       Geöffnete Touren, Aufträge oder Positionen sind für andere Mitarbeiter zur Be-
                                       arbeitung gesperrt. sie werden dann nur mit Leserecht geöffnet.
2.00 / 04-2022




                 A+W Enterprise Versandsteuerung                                                                      G-9
                 Startfunktionen                                                            Softwarereferenz




                                   Startfunktionen
                                   In A+W Enterprise haben Sie die Möglichkeit, über verschiedene Suchfunkti-
                                   onen Ihre Liefertermine und Aufträge zu suchen.
                                   Zu diesem Thema finden Sie folgende Informationen:
                                    “Programmstart” auf Seite G-11
                                    “Auftragssuche” auf Seite G-13
                                    “Marktpartnersuche” auf Seite G-14
2.00 / 04-2022




                 G-10                                                      A+W Enterprise Versandsteuerung
                 Softwarereferenz                                                                     Startfunktionen




                                        Programmstart
                                        Logistik > Versandsteuerung




                 Abb. G-1   Suchmodus


                                        Sie starten die Versandsteuerung mit der Eingabe der folgenden Kriterien:
                                        •   Versandmodus (alle, VK-Ausgang, EK-Warenaus- und -eingang)
                                        •   Hausnummer bzw. Mandantennummer
                                        •   Liefertermin
                                        •   Lieferzeitraum
                                        Über die Felder in der Kopfzeile filtern Sie Ihre Suche und das System listet
                                        Ihnen anhand der eingegebenen Daten die Liefertermine auf.

                                        VK-Aus. Versandmodus. Standardmäßig werden in der Versandsteuerung
                                        nur die auszuliefernden Aufträge behandelt. Bei einer entsprechenden Konfi-
                                        guration können jedoch auch die Bestellungen, komplett oder nur mit bestell-
                                        ten Bearbeitungen, im Versand - Modul bearbeitet werden. Sprechen Sie
                                        einen zuständigen Mitarbeiter von A+W an, falls Sie nähere Informationen da-
                                        rüber benötigen. Wenn die Verkaufs- und Einkaufs-Vorgänge über den Ver-
                                        sand abgewickelt werden, können auch alle Aufträge für das gewählte Datum
                                        bzw., für den gewählten Zeitraum angezeigt werden, wie z. B., im Versand-Ex-
                                        plorer, oder auf einer Datenebene.
2.00 / 04-2022




                                        Technische Info: Toggle-Feld, DB-Feld: lapool.vmodus




                 A+W Enterprise Versandsteuerung                                                                G-11
                 Startfunktionen                                                               Softwarereferenz




                                   Haus Nummer des Hauses oder Mandanten.
                                   Technische Info: Numerisches Feld, DB-Feld: lapool.hausnr

                                   Lieferdatum Eingabefeld für das Lieferdatum eines bestimmten Tages.
                                   Technische Info: Datumsfeld, DB-Feld: lapool.ltplan

                                   bis Eingabefeld für das Lieferdatum eines bestimmten Zeitraums.
                                   Technische Info: Datumsfeld, DB-Feld: lapool.ltplan

                                      Lieferdatum
                                      Die Eingabe des Zeitraums ist nur möglich, wenn Sie mit dem Versandex-
                                      plorer arbeiten. Alternativ ist nur ein Lieferdatums-Feld aktiv.
                                      Wenn Sie in beiden Datumsfelder das gleiche Datum eingeben, startet die
                                      Versandsteuerung direkt mit der Tourenebene.
2.00 / 04-2022




                 G-12                                                     A+W Enterprise Versandsteuerung
                 Softwarereferenz                                                                    Startfunktionen




                                        Auftragssuche
                                        Versandsteuerung > [Suchen] > <F9>




                 Abb. G-2   Auftragssuche


                                        In der Versandsteuerung besteht die Möglichkeit, an vielen verschiedenen
                                        Stellen nach Aufträgen über die erweiterte Suche zu suchen. In den Eingabe-
                                        feldern des Dialogkopfs geben Sie die Kriterien für die Suche ein. Im unteren
                                        Bereich wird die Trefferliste angezeigt. Die Suchergebnisse werden in ver-
                                        schiedenen Registern zusammengefasst.
                                        Die Suchmöglichkeit nach bestimmten Vorgangsarten wurde im gesamten
                                        A+W Enterprise mit der Version 6 einheitlich gestaltet.
                                        Ausführliche Dokumentation darüber finden Sie im Part Verkauf:
                                         Verkauf, “Suche Aufträge” auf Seite D-23
                                         Verkauf, “Suche Aufträge – Trefferliste” auf Seite D-28
2.00 / 04-2022




                 A+W Enterprise Versandsteuerung                                                               G-13
                 Startfunktionen                                                                     Softwarereferenz




                                          Marktpartnersuche
                                          Versandsteuerung > [Suchen] > <F9> > Feld Kunde > <F9>




                 Abb. G-3    Marktpartner-Suchdialog


                                          Ausführliche Dokumentation über die Marktpartnersuche finden Sie im Part
                                          Verkauf:
                                           Verkauf, “Marktpartnersuche” auf Seite D-37
2.00 / 04-2022




                 G-14                                                                A+W Enterprise Versandsteuerung
                 Softwarereferenz                                                                      Versand-Explorer




                                              Versand-Explorer
                                              Logistik > Versandsteuerung > Eingabe einer Zeitspanne

                 A


                 B


                                                                                                                     E




                 C
                 D




                 A Kopfdaten: Eingabe der             B Explorer – Baumstruktur        C Detailinformation zu dem
                   Suchkriterien                                                         ausgewählten Liefertermin
                 D Detailinformation zu der           E Ausgewählte Datenebene
                   ausgewählten Route
                 Abb. G-4     Versandsteuerung – Ansicht Explorer


                                              In der Versandsteuerung sehen Sie die Lieferaufträge nach dem Lieferdatum
                                              aufgelistet, die anhand der Suchkriterien ermittelt wurden.

                                              VK-Aus. VK-Ausgang: ausgewählter Versandmodus.
                                              Technische Info: Toggle-Feld, DB-Feld: lapool.vmodus

                                              Haus Nummer des Hauses oder Mandanten.
                                              Technische Info: Numerisches FeldNumerisches Feld, DB-Feld: lapool.hausnr

                                              Lieferdatum Eingabefeld für das Lieferdatum eines bestimmten Tages.
                                              Technische Info: Datumsfeld, DB-Feld: lapool.ltplan

                                              bis Eingabefeld für das Lieferdatum eines bestimmten Zeitraums.
                                              Technische Info: Datumsfeld, DB-Feld: lapool.ltplan
2.00 / 04-2022




                 A+W Enterprise Versandsteuerung                                                                     G-15
                 Versand-Explorer                                                               Softwarereferenz




                                    Explorer – Baumstruktur
                                    Zur besseren Übersicht sind die Lieferaufträge in der Explorer-Struktur aufge-
                                    baut. Das Arbeiten mit dem Versand-Explorer muss zunächst entsprechend
                                    konfiguriert werden. Im Explorer werden die Versanddaten in mehreren Ebe-
                                    nen dargestellt:
                                    •   Datumsebene
                                    •   Routenebene
                                    •   Vorgangsebene
                                    •   Positionsebene
                                    Jede Ebene ist mit einem festgelegten Symbol gekennzeichnet. In der rechten
                                    Dialoghälfte wird eine kurze Übersicht über die vorhanden Lieferungen ange-
                                    zeigt.
                                    In der Baumstruktur wählen Sie die Ebene aus. Wenn das Ebenen-Feld blau
                                    hinterlegt ist, dann ist die Ebene ausgewählt.
                                    In den folgenden vier Ebenen werden Kurzinformationen als Schnellübersicht
                                    angezeigt:
                                     “Übersicht für die Lieferdatumsebene” auf Seite G-17
                                     “Übersicht für die Tourenebene” auf Seite G-19
                                     “Übersicht für die Auftragsebene” auf Seite G-20
                                     “Übersicht für die Positionsebene” auf Seite G-21
2.00 / 04-2022




                 G-16                                                          A+W Enterprise Versandsteuerung
                 Softwarereferenz                                                                Versand-Explorer




                                        Übersicht für die Lieferdatumsebene
                                        Logistik > Versandsteuerung > Eingabe einer Zeitspanne, Datum im Explorer




                 Abb. G-5   Datumsebene im Versand-Explorer


                                        Nach der Liefertermin-Auswahl im Explorer werden in der Übersicht folgende
                                        Felder angezeigt:

                                        Route Nummer der Route.
                                        Technische Info: Numerisches Feld, DB-Feld: lapool.routenr

                                        Haus Nummer des Hauses oder Mandanten.
                                        Technische Info: Numerisches Feld, DB-Feld: lapool.hausnr

                                        Typ Versandmodus: Aufgrund der begrenzten Platzmöglichkeit wird der
                                        Name des Feldes (Versandmodus=Typ) sowie auch die Anzeige des Versand-
                                        modus weitgehend gekürzt:
                                        • VK: VK-Ausgang
                                        • E1: EK-Wareneingang
                                        • E2: EK-Warenausgang
                                        Technische Info: Alphanumerisches Feld, DB-Feld: lapool.vmodus

                                        Name Routenbezeichnung aus den A+W Enterprise - Stammdaten.
2.00 / 04-2022




                                        Technische Info: Anzeigefeld, DB-Feld: route.routenname




                 A+W Enterprise Versandsteuerung                                                             G-17
                 Versand-Explorer                                                                Softwarereferenz




                                    Ges. Gesamte Stückzahl der Position, die für diese Route erfasst ist.
                                    Technische Info: Numerisches Feld, DB-Feld: lapool.gesstk

                                    Abruf Stückzahl der Position, die der Kunde für den Liefertermin anfordert.
                                    Technische Info: Numerisches Feld, DB-Feld: lapool.abrufstk

                                    Verf. Verfügbare Stückzahl der Position.
                                    Technische Info: Numerisches Feld, DB-Feld: lapool.sollstk

                                    Verp. Verpackte Stückzahl der Position.
                                    Technische Info: Numerisches Feld, DB-Feld: lapool.iststk

                                    kmp. Komplett gemeldete Route. Alle Aufträge sind verpackt.
                                     Alle Positionen sind zur Auslieferung bereit.
                                     Noch nicht alle Positionen sind zur Auslieferung bereit.
                                    Technische Info: Anzeigefeld
2.00 / 04-2022




                 G-18                                                        A+W Enterprise Versandsteuerung
                 Softwarereferenz                                                                Versand-Explorer




                                        Übersicht für die Tourenebene
                                        Logistik > Versandsteuerung > Eingabe einer Zeitspanne, Datum im Explorer




                 Abb. G-6   Tourenebene im Versand-Explorer


                                        Nach der Routen-Auswahl im Explorer werden in der Übersicht folgende Fel-
                                        der angezeigt:

                                        Auftrag/Bestellung Auftragsnummer oder Bestellnummer für die geplante
                                        Lieferung je nach Versandmodus. Es wird immer nach der Vorgangsart unter-
                                        schieden: 5=Auftrag, 2=Bestellung
                                        Technische Info: Numerisches Feld, DB-Feld: lapool.auftrnr, lapool.vorgang

                                        Kunde Kundenname bei Aufträgen bzw., Lieferantenname bei Bestellungen
                                        für die geplante Lieferung.
                                        Technische Info: Alphanumerisches Feld, DB-Feld: mp.name
                                        Die folgenden Felder sind von der vorhergehende Übersicht übernommen:
                                        •   Ges. (gesamt)
                                        •   Abruf
                                        •   Verf. (verfügbar)
                                        •   Verp. (verpackt)
                                        •   kmp. (komplett)
2.00 / 04-2022




                 A+W Enterprise Versandsteuerung                                                            G-19
                 Versand-Explorer                                                                  Softwarereferenz




                                         Übersicht für die Auftragsebene
                                         Logistik > Versandsteuerung > Eingabe einer Zeitspanne, Datum im Explorer




                 Abb. G-7   Auftragsebene im Versand-Explorer


                                         Nach der Auftrags-/Bestellungs-Auswahl im Explorer werden in der Übersicht
                                         folgende Felder angezeigt:

                                         Pos. Laufende Positionsnummer aus dem Auftrag bzw. der Bestellung.
                                         Technische Info: Numerisches Feld, DB-Feld: lapool.posnr

                                         Artikel Artikelbezeichnung des zu liefernden Artikels.
                                         Technische Info: Numerisches Feld, DB-Feld: artikel.artbez1
                                         Die folgenden Felder werden von der vorhergehende Übersicht übernommen:
                                         •   Ges. (gesamt)
                                         •   Abruf
                                         •   Verf. (verfügbar)
                                         •   Verp. (verpackt)
                                         •   kmp. (komplett)
2.00 / 04-2022




                 G-20                                                            A+W Enterprise Versandsteuerung
                 Softwarereferenz                                                                   Versand-Explorer




                                         Übersicht für die Positionsebene
                                         Logistik > Versandsteuerung > Eingabe einer Zeitspanne, Datum im Explorer




                 Abb. G-8   Positionsebene im Versand-Explorer


                                         Die Übersicht aus der Positionsebene listet alle Auftragspositionen bzw. alle
                                         Positionen aus dem Einkaufsvorgang mit den jeweiligen Feldern, wie auf Auf-
                                         tragsebene.
                                         Die Felder sind in den folgenden Kapitel beschrieben:
                                          “Übersicht für die Lieferdatumsebene” auf Seite G-17
                                          “Übersicht für die Auftragsebene” auf Seite G-20
2.00 / 04-2022




                 A+W Enterprise Versandsteuerung                                                                G-21
                 Versandsteuerung – Menüs                                                           Softwarereferenz




                                        Versandsteuerung – Menüs
                                        In der Versandsteuerung stehen Ihnen zusätzliche Funktionen zur Verfügung.
                                        Diese sind auf allen verfügbaren Ebenen unter Zusatz- und Infomenüs zusam-
                                        mengefasst. Ein detaillierter Überblick über die beiden Menüs sind in den fol-
                                        genden Kapiteln beschrieben:
                                         “Zusatzmenü” auf Seite G-22
                                         “Infomenü” auf Seite G-25



                                        Zusatzmenü
                                        Versandsteuerung – Übersichtsebenen > <F4>




                 Abb. G-9   Zusatzmenü auf der Tourenebene


                                        Auf allen Ebenen der Versandsteuerung haben Sie zusätzliche Funktionen,
                                        die über Zusatzmenü <F4> erreichbar sind. Die hier aufgelisteten Funktionen
                                        können je nach Konfiguration, Kontex und Datenbestand nur begrenzt oder
                                        sogar gar nicht zur Verfügung stehen.
                                         “Zusatzmenü auf der Tourenebene” auf Seite G-23
                                         “Zusatzmenü auf der Auftragsebene” auf Seite G-24
                                         “Zusatzmenü auf der Positionsebene” auf Seite G-24
2.00 / 04-2022




                 G-22                                                             A+W Enterprise Versandsteuerung
                 Softwarereferenz                                                               Versandsteuerung – Menüs




                                            Zusatzmenü auf der Tourenebene

                 Short Cut   Eintrag                              Beschreibung

                     a       Verschieben <F3>                      “Verschieben” auf Seite G-66

                     b       Springen zu <F5>                      “Springen” auf Seite G-64

                     c       Verschieben mehrere Pos. <Strg> +     “Verschieben mehrerer Pos. - Auswahl” auf Seite G-69
                             <E>

                     d       Auftragsinfo <Strg> + <K>             “Auftragsinfo” auf Seite G-72

                     e       Drucken einer Ladeliste <Strg> +      “Drucken einer Ladeliste” auf Seite G-133
                             <F8>

                      f      Drucken aller Ladeliste <Strg> +      “Drucken aller Ladelisten” auf Seite G-134
                             <F12>

                     g       Drucken Ergänzungsladelisten <Strg>  “Drucken Ergänzungsladelisten” auf Seite G-135
                             + <F10>

                     h       Listendruck                           “Listendruck” auf Seite G-136

                      i      Liefereingang buchen                  “Liefereingang buchen” auf Seite G-76

                      j      Storno des Liefereingangs             “Storno des Liefereingangs” auf Seite G-77

                     k       Fehlmengenkontrolle <Shift> + <F9>    “Fehlmengenkontrolle - Auswahl” auf Seite G-78

                      l      Vorablieferschein Druck <Strg> +      “Drucken einer Ladeliste” auf Seite G-133
                             <F11>

                     m       Buchen auf Transport                  “Buchen auf Transport” auf Seite G-82

                     n       Transport rückbuchen                  “Transport zurückbuchen” auf Seite G-83

                     o       Lief./Wareneing. Freigabe + Druck     “Lief./Wareneing. Freigabe + Druck” auf Seite G-139
                             <Strg> + <F9>
2.00 / 04-2022




                 A+W Enterprise Versandsteuerung                                                                      G-23
                 Versandsteuerung – Menüs                                                                      Softwarereferenz




                                            Zusatzmenü auf der Auftragsebene
                                            Zusätzlich zu einigen Funktionen, die auch auf der Tourenebene verfügbar
                                            sind, kommen folgende Menüeinträge auf der Auftragsebene dazu:


                 Short Cut   Eintrag                               Beschreibung

                        i    Barcode Gestellanzeige                 “Barcode Gestellanzeige” auf Seite G-84

                        j    Ergebnisse der Gestellplanung          “Ergebnisse der Gestellplanung” auf Seite G-85
                             <Shift> + <F12>

                     k       Packmittelplanung                      “Packmittelplanung” auf Seite G-86

                     oa      Lieferanschrift suchen                 “Lieferanschrift suchen” auf Seite G-87

                    ob       Neue Lieferanschrift                   “Neue Lieferanschrift” auf Seite G-88

                        t    Gestellinformationen                   “Gestellinformationen” auf Seite G-89


                                            Zusatzmenü auf der Positionsebene
                                            Zusätzlich zu einigen Funktionen, die auch auf der Touren- und Auftragsebene
                                            verfügbar sind, kommen folgende Menüeinträge auf der Positionsebene dazu:


                 Short Cut   Eintrag                               Beschreibung

                        j    Verpackte Menge korrigieren <Shift>   Über <F4> > Verpackte Menge korrigieren ändern Sie
                             + <F10>                               nachträglich den Wert in dem eingeblendeten Feld.

                     m       Übersicht                              “Versandsteuerung - Übersicht” auf Seite G-119

                     n       Lieferterminänderung                   “Lieferterminänderungen” auf Seite G-122
2.00 / 04-2022




                 G-24                                                                   A+W Enterprise Versandsteuerung
                 Softwarereferenz                                                              Versandsteuerung – Menüs




                                              Infomenü
                                              Versandsteuerung – Übersichtsebenen > <Shift> + <F4>




                 Abb. G-10   Infomenü auf der Auftragsebene


                                              Das Infomenü <Shift> + <F4> ist für alle Ebenen identisch. Über dieses Menü
                                              können Sie andere Dialoge öffnen und Funktionen starten. Folgende Einträge
                                              werden angezeigt:


                 Short Cut   Eintrag                                    Beschreibung

                     a       Toursperre setzen/löschen <Shift> + <F10>  “Toursperre setzen/löschen” auf Seite G-90

                     b       Alle Touren sperren <Shift> + <F12>         “Alle Touren sperren” auf Seite G-91

                      c      Transportdaten                              “Transportdaten” auf Seite G-92

                     d       Lagerkommissionierung                       “Lagerkommissionierung” auf Seite G-93

                     e       Storno                                     Öffnen das Untermenü
                                                                         “Storno” auf Seite G-94

                     ea      Lieferscheinstorno                          “Lieferscheinstorno” auf Seite G-94

                     eb      Auftragsstorno                              “Auftragsstorno” auf Seite G-95
2.00 / 04-2022




                     ec      Wareneingangsstorno                         “Wareneingangsstorno” auf Seite G-96

                     ed      Storno des Versandstatus                    “Storno des Versandstatus” auf Seite G-97



                 A+W Enterprise Versandsteuerung                                                                      G-25
                 Versandsteuerung – Menüs                                                                 Softwarereferenz




                 Short Cut   Eintrag                                   Beschreibung

                        f    Gestelle                                  Öffnen das Untermenü
                                                                        “Gestelle” auf Seite G-98

                     fa      Gestellzuordnung <Strg> + <G>              “Gestellzuordnung - Auswahl” auf Seite G-99

                     fb      Gestellauflösung <Strg> + <F>              “Gestellauflösung - Auswahl” auf Seite G-102

                     fc      Freie Gestelle (Übersicht) <Strg> + <L>    “Freie Gestelle (Übersicht)” auf Seite G-104

                     fd      Gebuchte Gestelle (Übersicht) <Alt> + <E>  “Gebuchte Gestelle (Übersicht)” auf Seite G-106

                     fe      Alle Gestelle (Übersicht) <Alt> + <G>      “Alle Gestelle (Übersicht)” auf Seite G-107

                     ff      Einzelne Gestelle <Alt> + <B>              “Einzelne Gestelle” auf Seite G-109

                     fg      Gestelle zu Auftrag <Alt> + <A>            “Gestellauflösung - Auswahl” auf Seite G-102

                     fh      Scheibenzuordnung <Alt> + <F>              “Scheibenzuordnung” auf Seite G-112

                        g    VK/EK Information <Strg> + <O>             “VK/EK Information” auf Seite G-115

                        h    VK/EK Info (Global)                        “VK/EK Info (Global)” auf Seite G-117

                        i    Übersicht                                  “Versandsteuerung - Übersicht” auf Seite G-119

                        j    Lieferterminänderungen                     “Lieferterminänderungen” auf Seite G-122

                        k    Versandinformationen <Alt> + <I>           “Versandinformationen” auf Seite G-123

                        l    Via Details                                “Via Details” auf Seite G-124

                     m       Fertigwarenlager                           “Fertigwarenlager” auf Seite G-125

                    ma       Fertigwarenlager                           “Fertigwarenlagerbestand” auf Seite G-126

                    mb       Fertigwarenlager Inventur                  “Fertigwarenlager Inventur” auf Seite G-128

                    mc       Inventur abschließen                       “Inventur abschließen” auf Seite G-128

                        d    Protokoll                                  “Protokoll” auf Seite G-129
2.00 / 04-2022




                 G-26                                                                 A+W Enterprise Versandsteuerung
                 Softwarereferenz                                                                Versandsteuerung – Menüs




                                           Schaltflächen
                                           In den Datenebenen der Versandsteuerung sind folgende Schaltflächen nutz-
                                           bar:


                 Schaltfläche       Eintrag                               Beschreibung

                      [Suchen]      Startet die Vorgangssuche              “Suchen” auf Seite G-63

                     [Übersicht]    Grafische Übersicht über die           “Grafische Tourenübersicht” auf Seite G-131
                                    Lieferungen

                     [Springen]     Wechseln zu einem bestimmten           “Springen” auf Seite G-64
                                    Vorgang

                   [Verschieben]    Startet den Verschiebungs-Dialog       “Verschieben” auf Seite G-66

                     [Auslösen]     Löst die gewählte Aktion aus          Mit dieser Schaltfläche, oder alternativ mit der Taste
                                                                          <F3>, starten Sie die gewählte Aktion.

                      [Details]     Startet die Tourenübersicht            “Register – TourenInfo” auf Seite G-29

                      [Touren]      Wechselt aus der niedrigen Ebenen      “Register – TourenInfo” auf Seite G-29
                                    in die Tourenebene

                     [Aufträge]     Wechselt aus der niedrigen oder        “Register – AuftragsInfo” auf Seite G-39
                                    oberen Ebenen in die Auftragsebene

                    [Positionen]    Wechselt aus der oberen Ebenen in      “Register – PositionsInfo I” auf Seite G-57
                                    die Positionsebene

                     [Explorer]     Wechselt aus der Datenebenen in        “Versand-Explorer” auf Seite G-15
                                    Explorer

                     [Beenden]      Beendet die Übersichts-Anzeige        Es ist eine erneute Datumseingabe möglich. Das
                                                                          nächste [Beenden] schließt die Versandsteuerung.

                 Tab. G-1     Übersicht über die Schaltflächen in der Versandsteuerung
2.00 / 04-2022




                 A+W Enterprise Versandsteuerung                                                                           G-27
                 Touren                                                                Softwarereferenz




                          Touren
                          Auf der Tourenebene sind alle Routen aufgelistet, die am ausgewählten Lie-
                          ferdatum gefahren werden. Für jede Route sind die Aufträge bzw. Bestellun-
                          gen mit zusätzlichen Details und dem Tourenstatus aufgelistet.
                          Die Suchfelder in der Kopfzeile sind im folgenden Kapitel erläutert:
                           “Versand-Explorer” auf Seite G-15

                             Technische Info im Versand
                             Einige wichtige Daten werden in der Datenbanktabelle lapool gespeichert.
                             Diese Daten sind jeweils pro Auftrags- bzw. Bestellposition, Route und Lie-
                             fertermin vorhanden. Diverse Anzeigen in den Dialogen werden zur Pro-
                             gramm-Laufzeit dynamisch gebildet oder errechnet. Daher sind die
                             Angaben zur technischen Info in der Regel nicht 1:1 möglich. In solchen
                             Fällen wird in diesem Dokument auf den Eintrag Technische Info verzich-
                             tet.
                             Die Feldinhalte, die programmintern (per SQL-Statements) ermittelt wer-
                             den, werden in diesem Dokument nicht aufgeführt. Im Bedarfsfall greifen
                             Sie auf die Datenbank-Dokumentation zurück.

                          Die Tourenebene besteht aus folgenden Registern:
                           “Register – TourenInfo” auf Seite G-29
                           “Register – GestellInfo” auf Seite G-32
                           “Register – FahrzeugInfo” auf Seite G-34
                           “Register – Optimierung” auf Seite G-36
2.00 / 04-2022




                 G-28                                                  A+W Enterprise Versandsteuerung
                 Softwarereferenz                                                                                           Touren




                                               Register – TourenInfo
                                               Versandsteuerung – Lieferdatum-Eingabe
                                               Versandsteuerung – Lieferdatumsebene > [Details] > Register TourenInfo




                 Abb. G-11      Versandsteuerung – Tourenebene – Register TourenInfo


                                               Im Register Toureninfo werden allgemeine Daten zu der Routen zusammen-
                                               gefasst.

                                               S Aktueller Routenstatus. Die Bedeutung einzelnen Symbole können Sie der
                                               nachfolgenden Tabelle entnehmen.
                                               Technische Info: Anzeige-Feld


                 S (Status)         Bedeutung               Information

                    weiß            Offen                   Für diese Route sind nicht alle Positionen komplett verpackt.

                    grün/gelb       Verfügbar               Für diese Route sind Positionen mit verfügbarer Menge vorhanden.

                    gelb            Verpackt                Für diese Route sind alle Positionen komplett verpackt.

                    blau/gelb       Auf Transport           Für diese Route befinden sich alle Positionen auf dem Transport.

                    blau            Lieferschein erstellt   Für diese Route sind alle Positionen komplett an den Kunden
                                                            ausgeliefert.
2.00 / 04-2022




                 Tab. G-2       Routenstatus




                 A+W Enterprise Versandsteuerung                                                                             G-29
                 Touren                                                                                      Softwarereferenz




                 S (Status)       Bedeutung                 Information

                    rot           gesperrt                  Für diese Route ist die Sperre gesetzt. Die Routensperre wird nur
                                                            gesetzt, wenn ein Auftrag der Route von einem anderen Haus oder
                                                            Mandanten auf Transport gebucht wird.
                                                             “Toursperre setzen/löschen” auf Seite G-90

                 Tab. G-2     Routenstatus

                                             Nr. Nummer der Route.
                                             Technische Info: Numerisches Feld, DB-Feld: lapooltou.routenr

                                             Route Routenbezeichnung aus den A+W Enterprise - Stammdaten.
                                             Technische Info: Anzeigefeld, DB-Feld: route.routenname

                                             Ges. Gesamte Stückzahl der Position, die für diese Route erfasst ist.
                                             Technische Info: Anzeigefeld, DB-Feld: lapooltou.gesstk

                                             Abruf Stückzahl der Position, die der Kunde für den Liefertermin anfordert.
                                             Technische Info: Anzeigefeld, DB-Feld: lapooltou.abrufstk

                                             Verp. Verpackte Stückzahl der Position. Über <F4> können Sie eine Fehl-
                                             mengenkontrolle durchführen.
                                             Technische Info: Anzeigefeld, DB-Feld: lapooltou.iststk
                                             Die verpackte Menge ist über folgende Dialoge änderbar:
                                              “Fehlmengenkontrolle - Auswahl” auf Seite G-78
                                              “Barcode Gestellanzeige” auf Seite G-84

                                             Rück. Rückstand. Positionsstückzahl, die zum gewünschten Tourentag nicht
                                             zur Verfügung steht.
                                             Wenn eine Tour mit der Begründung Rückstand verschoben ist, dann wird die-
                                             se Stückzahl übernommen.
                                             Technische Info: Anzeigefeld, DB-Feld: lapooltou.rueckstk
                                              “Funktionen im Versand” auf Seite G-62

                                             kg/N Nettogewicht in Kilogramm für diese Route. Das Nettogewicht ist das
                                             Gesamtgewicht der Position ohne Gestell oder Verpackung. Das Gewicht wird
                                             zur Laufzeit im Programm errechnet und in diesem Register gerundet ange-
                                             zeigt.
                                             Technische Info: Anzeigefeld, DB-Feld: lapooltou.gewicht

                                             qm Fläche der Position in Quadratmetern.
                                             Technische Info: Anzeigefeld, DB-Feld: lapooltou.qm

                                             LL Nummer der Ladeliste, wenn für diese Route eine Ladeliste gedruckt ist.
                                             Über <F4> können Sie die Ladelisten drucken.
                                             Technische Info: Anzeigefeld, DB-Feld: lapooltou.llnr
                                              “Drucken einer Ladeliste” auf Seite G-133
                                              “Drucken aller Ladelisten” auf Seite G-134
2.00 / 04-2022




                                             kmp. Komplett-Kennzeichen:
                                              Alle Positionen sind zur Auslieferung komplett verpackt.


                 G-30                                                                       A+W Enterprise Versandsteuerung
                 Softwarereferenz                                                                            Touren




                                        Noch nicht alle Positionen sind zur Auslieferung verpackt.
                                       Technische Info: Anzeigefeld, DB-Feld: lapooltou.liefkompl

                                       VL Vorablieferschein-Kennzeichen zeigt an, ob alle Vorablieferscheine für die
                                       Lieferungen dieser Tour gedruckt sind.
                                        Alle Vorablieferscheine sind gedruckt.
                                        Noch nicht alle Vorablieferscheine sind gedruckt.
                                       Über <F4> können Sie einen Vorablieferschein drucken.
                                       Technische Info: Anzeigefeld, DB-Feld: lapooltou.vlsdrukz
                                        “Drucken einer Ladeliste” auf Seite G-133

                                       LS Lieferschein-Kennzeichen zeigt an, ob alle Lieferscheine für die Lieferun-
                                       gen dieser Tour gedruckt sind.
                                        Mindestens ein Lieferschein ist gedruckt.
                                        Noch keine Lieferscheine sind gedruckt.
                                       Über <F4> können Sie einen Lieferschein drucken.
                                       Technische Info: Anzeigefeld, DB-Feld: lapooltou.lsdrukz
                                        “Gestellinformationen” auf Seite G-89

                                       I Versandinformation-Kennzeichen zeigt an, ob zu mindestens einem Aufträg
                                       auf dieser Tour eine Versandinformation exisitert.
                                        Mindestens ein Auftrag mit Versandinfo existiert.
                                        Keine Versandinfo ist verfügbar.
                                       Die Versandinformation kann in den Vorgängen bei der Erfassung hinterlegt
                                       werden.
                                       Technische Info: Anzeigefeld, DB-Feld: lapooltou.vlsdrukz
                                        Verkauf, “Fremdinformationen” auf Seite D-258

                                       TS Toursperr-Kennzeichen zeigt an, ob die aktuelle Tour gesperrt bzw., ver-
                                       bucht ist:
                                       • grau- die aktuelle Tour ist noch offen
                                       • gelb- die aktuelle Tour ist verbucht
                                       • rot- die aktuelle Tour ist gesperrt
                                       Über <F4> kann die Tour gesperrt oder verbucht werden.
                                       Technische Info: Anzeigefeld
                                        “Gestellinformationen” auf Seite G-89
                                        “Alle Touren sperren” auf Seite G-91


                                       Ergänzende Informationen
                                        “Zusatzmenü” auf Seite G-22
                                        “Infomenü” auf Seite G-25
                                        “Schaltflächen” auf Seite G-27
2.00 / 04-2022




                 A+W Enterprise Versandsteuerung                                                              G-31
                 Touren                                                                              Softwarereferenz




                                          Register – GestellInfo
                                          Versandsteuerung – Lieferdatum-Eingabe
                                          Versandsteuerung – Lieferdatumsebene > [Details] > Register GestellInfo




                 Abb. G-12   Versandsteuerung – Tourenebene – Register GestellInfo


                                          Im Register GestellInfo werden allgemeine Daten zu der Routen zusammen-
                                          gefasst und zusätzliche Gestellinformationen angezeigt. Die Anzeige dieses
                                          Registers ist dynamisch, d. h. es wird nur dann eingeblendet, wenn das Arbei-
                                          ten mit Gestellen in der Versandsteuerung konfiguriert ist.
                                          Die meisten Felder sind bereits im vorherigen Kapitel beschrieben:
                                           “Register – TourenInfo” auf Seite G-29
                                          Zusätzlich werden folgende Felder in dem Register Gestellinfo angezeigt:

                                          Auf Gest. Gestellnummer, auf dem sich die auszuliefernden Scheiben befin-
                                          den. Für die Konfiguration der freien Gestellen in der Versandsteuerung muss
                                          die Rücksprache mit einem A+W Mitarbeiter erfolgen.
                                          Technische Info: Anzeige-Feld, DB-Feld: lapooltou.freigeststk

                                          kg/N Nettogewicht in Kilogramm für diese Route. Das Gewicht wird zur Lauf-
                                          zeit im Programm errechnet und in diesem Register mit drei Dezimalstellen
                                          angezeigt.
2.00 / 04-2022




                                          Technische Info: Anzeigefeld, DB-Feld: lapooltou.gewicht




                 G-32                                                                A+W Enterprise Versandsteuerung
                 Softwarereferenz                                                                          Touren




                                       kg/Tara Leergewicht des Gestells (Taragewicht), in Kilogramm. Das Tarage-
                                       wicht wird in diesem Feld angezeigt, wenn dieses entsprechend in den
                                       Stammdaten hinterlegt ist und die Lieferware bereits auf den Gestellen ver-
                                       plant ist.
                                       Technische Info: Anzeige-Feld, DB-Feld: lapooltou.gewichttara

                                       kg/B Bruttogewicht in Kilogramm für diese Route. Das Gewicht wird zur Lauf-
                                       zeit im Programm errechnet und in diesem Register mit drei Dezimalstellen
                                       angezeigt. Das Bruttogewicht errechnet sich aus dem Nettogewicht und Tara-
                                       gewicht zusammen. Das Bruttogewicht wird in diesem Feld angezeigt, wenn
                                       die Lieferware bereits auf den Gestellen verplant ist.
                                       Technische Info: Anzeige-Feld, DB-Feld: lapooltou.gewichtbrutto


                                       Ergänzende Informationen
                                        “Zusatzmenü” auf Seite G-22
                                        “Infomenü” auf Seite G-25
                                        “Schaltflächen” auf Seite G-27
2.00 / 04-2022




                 A+W Enterprise Versandsteuerung                                                            G-33
                 Touren                                                                              Softwarereferenz




                                          Register – FahrzeugInfo
                                          Versandsteuerung – Lieferdatum-Eingabe
                                          Versandsteuerung – Lieferdatumsebene > [Details] > Register FahrzeugInfo




                 Abb. G-13   Versandsteuerung – Register FahrzeugInfo


                                          Im Register Fahrzeuginfo sind zusätzlich zu den Touren der Fahrer und die
                                          Fahrzeugdaten aufgelistet.
                                          Die meisten Felder sind bereits im vorherigen Kapitel beschrieben:
                                           “Register – TourenInfo” auf Seite G-29
                                          Zusätzlich werden folgende Felder in dem Register FahrzeugInfo angezeigt:

                                          Fahrer Personalnummer des Fahrers aus dem Mitarbeiterstamm. Der Fahrer
                                          für diese Route kann im Dialog Transportdaten ausgewählt werden.
                                          Technische Info: Numerisches Feld, DB-Feld: mitarb.manr
                                           “Transportdaten” auf Seite G-92

                                          Name Name des Fahrers. Wenn der Fahrer für diese Route im Dialog Trans-
                                          portdaten ausgewählt wird, wird der Name hier automatisch aus dem Mitarbei-
                                          terstamm übernommen.
                                          Technische Info: Anzeigefeld, mitarb.maname
2.00 / 04-2022




                                          Kfz Kraftfahrkennzeichen der Zugmaschine. Das Fahreug für diese Route
                                          wird im Dialog Transportdaten ausgewählt. Die Fahrzeuge müssen zunächst



                 G-34                                                                A+W Enterprise Versandsteuerung
                 Softwarereferenz                                                                         Touren




                                       in den Stammdaten hinterlegt werden.
                                       Technische Info: Numerisches Feld, DB-Feld: lkw.lkw.nr
                                        Stammdaten, “Fahrzeuge” auf Seite B-178

                                       Anhänger I/II Kennzeichen des verwendeten Anhängers oder Aufliegers.Es
                                       ist möglich, zwei Anhänger oder Auflieger im Dialog Transportdaten auszu-
                                       wählen. Die Anhänger müssen zunächst in den Stammdaten hinterlegt wer-
                                       den.
                                       Technische Info: Numerisches Feld, DB-Feld: lkw.lkw.nr
                                        Stammdaten, “Fahrzeuge” auf Seite B-178


                                       Ergänzende Informationen
                                        “Zusatzmenü” auf Seite G-22
                                        “Infomenü” auf Seite G-25
                                        “Schaltflächen” auf Seite G-27
2.00 / 04-2022




                 A+W Enterprise Versandsteuerung                                                           G-35
                 Touren                                                                                Softwarereferenz




                                          Register – Optimierung
                                          Versandsteuerung – Lieferdatum-Eingabe
                                          Versandsteuerung – Lieferdatumsebene > [Details] > Register Optimierung




                 Abb. G-14   Versandsteuerung – Tourenebene – Register Optimierung


                                          Im Register Optimierung werden allgemeine Daten zu der Routen zusammen-
                                          gefasst und zusätzliche Information über die Routenoptimierung angezeigt.
                                          Die Anzeige dieses Registers ist dynamisch, d. h, es wird nur dann eingeblen-
                                          det, wenn das Arbeiten mit A+W Logistics Optimizer in der Versandsteuerung
                                          konfiguriert ist.
                                          Die meisten Felder sind bereits in den vorherigen Kapiteln beschrieben:
                                           “Register – TourenInfo” auf Seite G-29
                                           “Register – GestellInfo” auf Seite G-32
                                           “Register – FahrzeugInfo” auf Seite G-34
                                          Zusätzlich werden folgende Felder in dem Register Gestellinfo angezeigt:

                                          OptiStatus Aktueller Status der Routenoptimierung im Klartext.
                                          Technische Info: Anzeige-Feld, DB-Feld: lapooltou.optistatus

                                          Opt Checkbox, um die Routen-Auswahl für die bevorstehende Optimierung
                                          zu treffen.
2.00 / 04-2022




                                           Aktuelle Route ist für die Optimierung ausgewählt.
                                           Die aktuelle Route ist nicht für die Optimierung ausgewählt.



                 G-36                                                                  A+W Enterprise Versandsteuerung
                 Softwarereferenz                                                                            Touren




                                       Über die Schaltfläche [StartOTR] starten Sie die Routenoptimierung.
                                       Technische Info: Anzeigefeld, DB-Feld: lapooltou.optkz

                                          Routenoptimierung in A+W Enterprise
                                          Die Routenoptimierung mit A+W Logistics Optimizer ist eine separat erhält-
                                          liche und konfigurierbare Erweiterung für A+W Enterprise. Bitte sprechen
                                          Sie bei bestehendem Interesse den zuständigen A+W - Mitarbeiter an.
                                          Die Dokumentation zu A+W Logistics Optimizer ist nicht Bestandteil dieses
                                          Dokumentes.


                                       Ergänzende Informationen
                                        “Zusatzmenü” auf Seite G-22
                                        “Infomenü” auf Seite G-25
                                        “Schaltflächen” auf Seite G-27
2.00 / 04-2022




                 A+W Enterprise Versandsteuerung                                                              G-37
                 Auftragsebene                                                               Softwarereferenz




                                 Auftragsebene
                                 Auf der Auftragsebene der Versandsteuerung sehen Sie die detaillierten Infor-
                                 mationen zu den angelegten Aufträgen wie Lieferanschriften, Versandinfor-
                                 mationen und Zusatzinformationen.
                                 Auf dieser Ebene finden Sie folgende Register:
                                     “Register – AuftragsInfo” auf Seite G-39
                                     “Register– AuftragsInfo/Gestell” auf Seite G-44
                                     “Register– Lieferanschrift” auf Seite G-46
                                     “Register – VersandInfo I” auf Seite G-48
                                     “Register – VersandInfo II” auf Seite G-51
                                     “Register – ZusatzInfo” auf Seite G-53
2.00 / 04-2022




                 G-38                                                        A+W Enterprise Versandsteuerung
                 Softwarereferenz                                                                        Auftragsebene




                                          Register – AuftragsInfo
                                          Versandsteuerung – Lieferdatumauswahl > Routenauswahl >
                                          Register AuftragsInfo




                 Abb. G-15   Versandsteuerung – Register Auftragsinfo


                                          Im Register AuftragsInfo sehen Sie für jede Tour die Informationen zu den Auf-
                                          trägen und den Status zum Versand.
                                          Die Suchfelder in der Kopfzeile sind im Dialog Versandsteuerung erklärt. Zu-
                                          sätzlich werden die Routennummer und der Routenname angezeigt.
                                           “Versand-Explorer” auf Seite G-15

                                          S Aktueller Auftragsstatus. Die Bedeutung der Ampelanzeige auf der Auf-
                                          tragsebene ist die Gleiche wie auf Tourenebene. Eine Erläuterung finden Sie
                                          hier:
                                           “Routenstatus” auf Seite G-29

                                          Modus Versandmodus. Das Feld ist wird nur dann angezeigt, wenn Sie die
                                          Versandsteuerung für die Einkaufsvorgänge nutzen und die entsprechende
2.00 / 04-2022




                                          Vorauswahl getroffen haben.
                                          Technische Info: Anzeige-Feld, DB-Feld: lapoolauf.vmodus




                 A+W Enterprise Versandsteuerung                                                                  G-39
                 Auftragsebene                                                                 Softwarereferenz




                                 Auftrag/Bestellung Auftragsnummer bzw. Bestellnummer. Es werden hier
                                 alle Vorgänge aufgelistet, die zum ausgewählten Datum für die Route geplant
                                 sind. Ob in diesem Feld ein Auftragsnummer oder ein Bestellnummer ange-
                                 zeigt wird, ist von dem gewählten Versandmodus abhängig.
                                 Technische Info: Numerisches Feld, DB-Feld: lapoolauf.auftrnr

                                 Nr. Subnummer des Lieferscheins. Falls zu einem Auftrag ein Komplettliefer-
                                 schein oder mehrere Teillieferscheine bereits erfasst wurden, wird hier die ent-
                                 sprechende Nummer anzeigt.
                                 • Ein Komplettlieferschein hat immer die Subnummer 1 und wird zusätzlich
                                    als komplett markiert (Checkbox Kmp).
                                 • Teillieferscheine haben die Subnummer größer gleich 1 und werden nicht
                                    als komplett markiert (Checkbox Kmp).
                                 Bei übertragenen Aufträgen aus einem anderen Haus, wird immer die Origi-
                                 nal-Auftragsnummer des sendenden Hauses angezeigt.
                                 Technische Info: Numerisches Feld, DB-Feld: lapoolauf.subnr

                                 Kunde Kunden- bzw. Lieferantenname aus dem Auftrag oder der Bestellung.
                                 Technische Info: Alphanumerisches Feld, DB-Feld: mp.name

                                 Ges. Gesamte Stückzahl im Auftrag bzw. in der Bestellung.
                                 Technische Info: Numerisches Feld, DB-Feld: lapoolauf.gesstk

                                 Abruf Abruf-Stückzahl, die der Kunde bzw. der Lieferant für den Liefertermin
                                 anfordert.
                                 Technische Info: Numerisches Feld, DB-Feld: lapoolauf.abrufstk

                                 Verf. Verfügbare Stückzahl der Position, die verpackt werden kann.
                                 Technische Info: Numerisches Feld, DB-Feld: lapoolauf.sollstk

                                 Verp. Verpackte Stückzahl der Position. Über <F4> können Sie eine Fehl-
                                 mengenkontrolle durchführen.
                                 Technische Info: Numerisches Feld, DB-Feld: lapoolauf.iststk
                                  “Fehlmengenkontrolle - Auswahl” auf Seite G-78

                                 Rück. Rückstand. Stückzahl der Position, die zum gewünschten Tourentag
                                 nicht zur Verfügung steht.
                                 Wenn eine Tour mit der Begründung Rückstand verschoben ist, dann wird die-
                                 se Stückzahl übernommen.
                                 Technische Info: Numerisches Feld, DB-Feld: lapoolauf.rueckstk
                                  “Funktionen im Versand” auf Seite G-62

                                 Nach. Nachlieferung. Stückzahl der Position, die für diesen Auftrag nachge-
                                 liefert werden muss. Nachlieferungen können z. B. durch Verschiebungen zu-
                                 stande kommen.
                                 Technische Info: Anzeige-Feld
                                  “Funktionen im Versand” auf Seite G-62
2.00 / 04-2022




                                 Über. Überlieferung. Stückzahl der Position, die für diesen Auftrag die ge-
                                 samte Stückzahl übersteigt. Eine Überlieferung kann durch die Verschiebung




                 G-40                                                       A+W Enterprise Versandsteuerung
                 Softwarereferenz                                                                                 Auftragsebene




                                              von Positionen zustande kommen.
                                              Technische Info: Anzeige-Feld
                                               “Funktionen im Versand” auf Seite G-62

                                              LL Ladelistennummer, wenn für diese Tour bereits Ladelisten gedruckt sind.
                                              Ladelisten können Sie über <F4> drucken.
                                              Technische Info: Numerisches Feld, DB-Feld: lapoolauf.llnr
                                               “Drucken einer Ladeliste” auf Seite G-133
                                               “Drucken aller Ladelisten” auf Seite G-134

                                              VL Vorablieferschein zeigt an, ob alle Vorablieferscheine für die Lieferungen
                                              dieser Route gedruckt sind.
                                               Alle Vorablieferscheine sind gedruckt.
                                               Noch nicht alle Vorablieferscheine sind gedruckt.
                                              Über <F4> können Sie einen Vorablieferschein drucken.
                                               Softwarereferenz, “Drucken einer Ladeliste” auf Seite G-133
                                              In folgenden Fällen markiert A+W Enterprise das Feld wieder als nicht ge-
                                              druckt:
                                              • Änderungen in der Route
                                              • Änderungen im Auftrag
                                              • Änderungen in der Auftragsposition
                                              Vorablieferscheine sind auch dann druckbar, wenn die Lieferung nicht kom-
                                              plett gemeldet ist. Wenn für einen Auftrag nur der Vorablieferschein gedruckt
                                              ist, dann ist der Auftrag in der Versandsteuerung noch änderbar. Wenn für ei-
                                              nen Auftrag ein Lieferschein gedruckt ist, dann ist der Auftrag in der Versand-
                                              steuerung nicht mehr änderbar.
                                              Ein Vorablieferschein ist kein eigener Vorgang in der Datenbank. Der Auf-
                                              tragsstatus ändert sich nicht durch den Vorablieferschein.
                                              Bei der Belieferung des Kunden muss die gelieferte Stückzahl auf dem Vorab-
                                              lieferschein korrigiert werden. Für den Druck des Lieferscheins müssen die
                                              korrigierten Werte übertragen werden.
                                              Technische Info: Anzeige-Feld, DB-Feld: lapoolauf.vlsdrukz

                                              LS Aktueller Status des Lieferscheins:


                 LS                 Bedeutung                Information

                      grau          Offen                    Noch kein Lieferschein erstellt.

                      gelb          Auf Transport gebucht     “Buchen auf Transport” auf Seite G-82.

                      blau          Lieferschein erstellt.   Vorgang ist bereits komplett geliefert.

                    rot-grau        Lieferstopp              Für den Kunden ist ein Lieferstopp festgelegt worden (diese Status-
                                                             Anzeige muss explizit konfiguriert werden).

                    grau-rot        Keine Teillieferung      Für diesen Auftrag sind keine Teillieferungen erwünscht (diese
                                                             Status-Anzeige muss explizit konfiguriert werden).
2.00 / 04-2022




                 Tab. G-3      Status des Lieferscheins




                 A+W Enterprise Versandsteuerung                                                                              G-41
                 Auftragsebene                                                                              Softwarereferenz




                 LS               Bedeutung               Information

                    rot-rot       Lieferstopp/Keine       Für diesen Kunden existiert ein Lieferstopp und für den aktuellen
                                  Teillieferung           Auftrag ist keine Teillieferung erwünscht (diese Status-Anzeige muss
                                                          explizit konfiguriert werden).

                 Tab. G-3     Status des Lieferscheins

                                           Über <F4> erstellen und drucken Sie den Lieferschein. Beim Druck des Lie-
                                           ferscheins wird der zugehörige Datensatz für die Finanzbuchhaltung erzeugt.
                                           Technische Info: Anzeige-Feld
                                            “Gestellinformationen” auf Seite G-89
                                           Über <Shift> + <F4> > Storno können Sie die Lieferscheine stornieren.
                                            “Lieferscheinstorno” auf Seite G-94

                                           Kmp. Komplett gemeldeter Auftrag. Alle Positionen sind verpackt.
                                            Alle Positionen sind zur Auslieferung bereit.
                                            Noch nicht alle Positionen sind zur Auslieferung bereit.
                                           Technische Info: Anzeigefeld, DB-Feld: lapoolauf.kompl

                                           Abr. Abrufauftrag. Der Auftrag wird auf Anforderung an den Kunden geliefert.
                                            Abrufauftrag durch den Kunden.
                                            Kein Abrufauftrag.
                                           Technische Info: Anzeigefeld, DB-Feld: lapoolauf.abruf

                                           F Fakturiert zeigt an, ob der Auftrag komplett fakturiert ist.
                                            Komplett fakturierter Auftrag.
                                            Noch nicht komplett fakturierter Auftrag.
                                           Technische Info: Anzeigefeld, DB-Feld: lapoolauf.fakturakz

                                           I Versandinformation zeigt an, ob zu diesem Auftrag eine Versandinformation
                                           vorliegt.
                                           Versandinformationen erfassen Sie im Verkauf oder Einkauf im Dialog Fremd-
                                           informationen. Über <Shift> + <F4> > VK/EK Information können Sie die Infor-
                                           mationen aufrufen.
                                            Zu diesem Auftrag bzw. Wareneingang liegt eine Versandinformation vor.
                                            Es liegt keine Versandinformation zu diesem Auftrag vor.
                                           Technische Info: Anzeigefeld, DB-Feld: lapoolauf.info

                                           Fußzeile
                                           In der Fußzeile des Registers sind für alle Positionen die Gesamtstückzahlen
                                           der folgenden Felder aufgelistet:
                                           •   Ges. (Gesamt)
                                           •   Abruf (Abrufwunsch)
                                           •   Verf. (Verfügbar)
                                           •   Verp. (Verpackt)
2.00 / 04-2022




                                           •   Rück. (Rückstand)
                                           •   Nach. (Nachlieferung)
                                           •   Über. (Überlieferte Stückzahl)


                 G-42                                                                   A+W Enterprise Versandsteuerung
                 Softwarereferenz                                         Auftragsebene




                                       Ergänzende Informationen
                                        “Zusatzmenü” auf Seite G-22
                                        “Infomenü” auf Seite G-25
                                        “Schaltflächen” auf Seite G-27
2.00 / 04-2022




                 A+W Enterprise Versandsteuerung                                 G-43
                 Auftragsebene                                                                         Softwarereferenz




                                          Register– AuftragsInfo/Gestell
                                          Versandsteuerung – Lieferdatumauswahl > Routenauswahl >
                                          Register AuftragsInfo/Gestell




                 Abb. G-16   Versandsteuerung – Register AuftragsInfo/Gestell


                                          Der Register AuftragsInfo/Gestell wird dynamisch angezeigt, wenn Sie in der
                                          Versandsteuerung mit dem Modul Gestelle arbeiten. Hier sehen Sie für jeden
                                          Auftrag zusätzlich die Gestell-Informationen.
                                          Die Suchfelder in der Kopfzeile sind im Dialog Versandsteuerung erklärt. Zu-
                                          sätzlich werden die Routennummer und der Routenname angezeigt.
                                           “Versand-Explorer” auf Seite G-15
                                          Die meisten Felder sind bereits im vorherigen Kapitel beschrieben:
                                           “Register – AuftragsInfo” auf Seite G-39
                                          Zusätzlich werden folgende Felder in dem Register AuftragsInfo/Gestell ange-
                                          zeigt:

                                          Auf Gest. Gestellnummer, auf dem sich die auszuliefernden Scheiben befin-
                                          den. Für die Konfiguration der freien Gestellen in der Versandsteuerung muss
                                          die Rücksprache mit einem A+W Mitarbeiter erfolgen.
                                          Technische Info: Numerisches Feld, DB-Feld: lapoolauf.freigeststk
2.00 / 04-2022




                 G-44                                                                  A+W Enterprise Versandsteuerung
                 Softwarereferenz                                                                   Auftragsebene




                                       Fußzeile
                                       In der Fußzeile des Registers sind für alle Positionen die Gesamtstückzahlen
                                       der folgenden Felder aufgelistet:
                                       •   Ges. (Gesamt)
                                       •   Abruf (Abrufwunsch)
                                       •   Verf. (Verfügbar)
                                       •   Verp. (Verpackt)
                                       •   Auf Gest. (Auf dem Gestell)


                                       Ergänzende Informationen
                                        “Zusatzmenü” auf Seite G-22
                                        “Infomenü” auf Seite G-25
                                        “Schaltflächen” auf Seite G-27
2.00 / 04-2022




                 A+W Enterprise Versandsteuerung                                                             G-45
                 Auftragsebene                                                                         Softwarereferenz




                                          Register– Lieferanschrift
                                          Versandsteuerung – Lieferdatumauswahl > Routenauswahl >
                                          Register Lieferanschrift




                 Abb. G-17   Versandsteuerung – Register Lieferanschrift


                                          Im Register Lieferanschrift sehen Sie für jeden Auftrag die Informationen zur
                                          Anlieferung, wie z. B. Anschrift, Fahrtdauer und Ladefolge im LKW oder An-
                                          hänger.
                                          Die Suchfelder in der Kopfzeile sind im Dialog Versandsteuerung erklärt. Zu-
                                          sätzlich werden die Routennummer und der Routenname angezeigt.
                                           “Versand-Explorer” auf Seite G-15
                                          Die meisten Felder sind bereits im vorherigen Kapitel beschrieben:
                                           “Register – AuftragsInfo” auf Seite G-39
                                          Zusätzlich werden folgende Felder in dem Register AuftragsInfo/Gestell ange-
                                          zeigt:

                                          LF Ladefolge der Aufträge im LKW. Die Reihenfolge der Kunden auf einer
                                          Tour oder Route bestimmt die Ladefolge der Aufträge. Wenn ein neuer Eintrag
                                          gemacht oder ein vorhandener Eintrag geändert wird, dann fragt A+W Enter-
                                          prise, ob die geänderte Ladefolge auf weitere Aufträge vererbt werden soll.
2.00 / 04-2022




                                          Technische Info: Numerisches Feld, DB-Feld: lapoolrouteposnr

                                          Anl. Datum Anlieferdatum für die geplante Lieferung zum Kunden.
                                          Technische Info: Datumsfeld, DB-Feld: lapool.ankunft


                 G-46                                                                  A+W Enterprise Versandsteuerung
                 Softwarereferenz                                                                     Auftragsebene




                                       A. Zeit Die Ankunftszeit wird aus dem Auftrag übernommen, wenn mit der
                                       via-Plant Auslieferung gearbeitet wird.
                                       Technische Info: Alphanumerisches Feld, DB-Feld: lapool.ankunftszeit
                                        “Versandinformationen” auf Seite G-123

                                       FD Fahrtdauer zum Kunden. Die geplante Fahrtdauer wird aus der Lieferad-
                                       resse des Vorgangs (Auftrag/Bestellung) ermittelt.
                                       Technische Info: Numerisches Feld, DB-Feld: lapool.fahrtzeit

                                       Lieferanschrift, Straße, PLZ, Ort Lieferanschrift des Kunden bzw. Liefe-
                                       rantes. Diese Felder werden aus der Lieferanschrift des Vorgangs übernom-
                                       men. Die Lieferanschrift kann in der Versandsteuerung geändert werden.
                                       Technische Info: Anzeige-Felder, DB-Feld: lapool.lname, lapool.lstr,
                                       lapoolauf.lplz, lapoolauf.lort.
                                        “Lieferanschrift suchen” auf Seite G-87
                                        “Neue Lieferanschrift” auf Seite G-88

                                       Spl Splitt. Eine Zahl-Eingabe im Feld Splitt führt zur Aufteilung der Gesamt-
                                       menge in die entsprechenden Anzahl der Lieferungen.
                                       Technische Info: Numerisches Feld, DB-Feld: lapool.splitt

                                       Fußzeile
                                       In der Fußzeile des Registers sind für alle Positionen die Gesamtstückzahlen
                                       der folgenden Felder aufgelistet:
                                       • Gewicht (des Auftrags) von (zu transportierende Gesamtgewicht)
                                       • Fläche (des Auftrags) von (gesamt zu transportierende Fläche)
                                       • Wunschtermin


                                       Ergänzende Informationen
                                        “Zusatzmenü” auf Seite G-22
                                        “Infomenü” auf Seite G-25
                                        “Schaltflächen” auf Seite G-27
2.00 / 04-2022




                 A+W Enterprise Versandsteuerung                                                               G-47
                 Auftragsebene                                                                         Softwarereferenz




                                          Register – VersandInfo I
                                          Versandsteuerung – Lieferdatumauswahl > Routenauswahl >
                                          Register Versandinfo I




                 Abb. G-18   Versandsteuerung – Register VersandInfo I


                                          Im Register VersandInfo I sehen Sie weitere Versandinformationen zum Auf-
                                          trag.
                                          Die Suchfelder in der Kopfzeile sind im Dialog Versandsteuerung erklärt. Zu-
                                          sätzlich werden die Routennummer und der Routenname angezeigt.
                                           “Versand-Explorer” auf Seite G-15
                                          Die meisten Felder sind bereits im vorherigen Kapitel beschrieben:
                                           “Register – AuftragsInfo” auf Seite G-39
                                          Zusätzlich werden folgende Felder in dem Register VersandInfo l angezeigt:

                                          Bezug Bezugsvorgang für Aufträge, die aus einem anderen Haus übertragen
                                          sind.
                                          Technische Info: Numerisches Feld, DB-Feld: kauf.parauftrnr

                                          Ex. Sender Externer Sender. Bei übertragenen Aufträgen wird die Mandan-
                                          tennummer des sendenden Hauses angezeigt.
2.00 / 04-2022




                                          Technische Info: nummerisches Feld, DB-Feld: kauf.parhausnr




                 G-48                                                                  A+W Enterprise Versandsteuerung
                 Softwarereferenz                                                                     Auftragsebene




                                       In. Sender Interner Sender. Bei übertragenen Aufträgen wird die Auftrags-
                                       nummer des empfangenen Hauses angezeigt.
                                       Technische Info: Numerisches Feld, DB-Feld: kauf.parhausnr

                                       Versandinformation Versandinformationen werden nur angezeigt, wenn
                                       diese in der Auftragserfassung hinterlegt sind.
                                       Sie können die Versandinformationen bearbeiten oder neue Versandinforma-
                                       tionen in das Feld schreiben. Mit <Strg> + <B> können Sie die Versandinfor-
                                       mation in den Auftrag übernehmen.
                                       Technische Info: Numerisches Feld, DB-Feld: lapool.exbez2

                                       VPA ID der Verpackungsart aus dem Auftrag. Die zugeordnete Verpackungs-
                                       art wird im Register Versandinfo II im Klartext angezeigt. Sie können eine
                                       neue Verpackungsart über die Schaltfläche <F9> dem Auftrag zuordnen. Die-
                                       se Änderung wird erst mit <Strg> + <B> in den Auftrag übernommen.
                                       Technische Info: Numerisches Feld, DB-Feld: lapool.verpackart

                                       VA ID der Versandart aus dem Auftrag. Die zugeordnete Versandart wird im
                                       Register Versandinfo II im Klartext angezeigt.
                                       Sie können eine neue Versandart über <F9> dem Auftrag zuordnen. Diese
                                       Änderung kann erst mit <Strg> + <B> in den Auftrag übernommen werden. Al-
                                       ternativ kann die Versandart über das Infomenü <Shift> + <F4> hinterlegt bzw.
                                       geändert werden:
                                        “Versandinformationen” auf Seite G-123
                                       Technische Info: Numerisches Feld, DB-Feld: lapool.versandart

                                       LA ID der Lieferart. Die zugeordnete Lieferart wird im Register Versandinfo II
                                       im Klartext angezeigt.
                                       Sie können eine neue Lieferart über die Schaltfläche <F9> dem Auftrag zuord-
                                       nen. Diese Änderung wird erst mit <Strg> + <B> in den Auftrag übernommen.
                                       Technische Info: Numerisches Feld, DB-Feld: lapool.lieferart

                                       A-Zoll Ausgangszoll. Nummer der Zollstelle des Ausgangslandes.
                                       Sie können eine andere Ausgangszollstelle angeben.
                                       Technische Info: Numerisches Feld, DB-Feld: lapool.azsnr

                                       B-Zoll Bestimmungszoll. Nummer der Zollstelle des Empfängerlandes.
                                       Sie können eine andere Bestimmungszollstelle angeben.
                                       Technische Info: Numerisches Feld, DB-Feld: lapool.bzsnr

                                       via H Nummer des Hauses, über das die Lieferung erfolgt. Das Feld ist nur
                                       bei der Nutzung des via-plant-Moduls belegt.
                                       Technische Info: Numerisches Feld, DB-Feld: lapool.viahaus

                                       Route Nummer der Route, über die die Lieferung erfolgt. Das Feld ist nur bei
                                       der Nutzung des via-plant-Moduls belegt.
                                       Technische Info: Numerisches Feld, DB-Feld: lapool.endroute
2.00 / 04-2022




                 A+W Enterprise Versandsteuerung                                                               G-49
                 Auftragsebene                                                      Softwarereferenz




                                 Ergänzende Informationen
                                  “Zusatzmenü” auf Seite G-22
                                  “Infomenü” auf Seite G-25
                                  “Schaltflächen” auf Seite G-27
2.00 / 04-2022




                 G-50                                               A+W Enterprise Versandsteuerung
                 Softwarereferenz                                                                       Auftragsebene




                                          Register – VersandInfo II
                                          Versandsteuerung – Lieferdatumauswahl > Routenauswahl >
                                          Register VersandInfo II




                 Abb. G-19   Versandsteuerung – Register Versandinfo II


                                          Im Register Versandinfo II sehen Sie die aufgeschlüsselten Informationen aus
                                          dem Register Versandinfo I.
                                          Die Suchfelder in der Kopfzeile sind im Dialog Versandsteuerung erklärt. Zu-
                                          sätzlich werden die Routennummer und der Routenname angezeigt.
                                           “Versand-Explorer” auf Seite G-15
                                          Die meisten Felder sind bereits im vorherigen Kapitel beschrieben:
                                           “Register – VersandInfo I” auf Seite G-48
                                          Zusätzlich werden folgende Felder in dem Register VersandInfo lI angezeigt:

                                          Versandinformation Gekürzte Versandinformation. Diese wird nur ange-
                                          zeigt, wenn sie im Auftrag oder der Bestellung hinterlegt ist. Sie können die
                                          Versandinformationen ändern oder eine neue Versandinformation in das Feld
                                          eingeben.
                                          Technische Info: Anzeige-Feld
2.00 / 04-2022




                                          Verpackungsart Bezeichnung der Verpackungsart. Die zugeordnete ID wird
                                          im Register Versandinfo I angezeigt.
                                          Technische Info: Anzeige-Feld



                 A+W Enterprise Versandsteuerung                                                                 G-51
                 Auftragsebene                                                              Softwarereferenz




                                 Versandart Bezeichnung der Versandart. Die zugeordnete ID wird im Regis-
                                 ter Versandinfo I angezeigt.
                                 Technische Info: Anzeige-Feld

                                 Lieferart Bezeichnung der Lieferart. Die zugeordnete ID wird im Register
                                 Versandinfo I angezeigt.
                                 Technische Info: Anzeige-Feld

                                 PL1, PL2 Private Long 1 und Private Long 2 dienen für kundenspezifische
                                 Zusatzinformationen. In der Auftragserfassung können Sie Informationen in
                                 Form von Ziffern speichern. Die Feldbezeichnungen PL1 und PL2 sind kun-
                                 denindividuell konfigurierbar. Über das Infomenü <Shift> + <F4> in der Ver-
                                 sandsteuerung können Sie diese Felder neue hinterlegen bzw. ändern.
                                  “Versandinformationen” auf Seite G-123
                                 Technische Info: Numerisches Feld, DB-Feld: lapool.private_long1, lapool.pri-
                                 vate_long2

                                 PC1, PC2 Private Char 1 und Private Char 2 dienen für kundenspezifische
                                 Zusatzinformationen. In der Auftragserfassung können Sie Informationstexte
                                 speichern. Die Feldbezeichnungen PC1 und PC2 sind kundenindividuell kon-
                                 figurierbar. Maximale Eingabe pro Feld ist 15 Zeichen. Über das Infomenü
                                 <Shift> + <F4> in der Versandsteuerung können Sie diese Felder neue hinter-
                                 legen bzw. ändern.
                                  “Versandinformationen” auf Seite G-123
                                 Technische Info: Alphanumerisches Feld, DB-Feld: lapool.private_char1, la-
                                 pool.private_char2

                                 Fußzeile
                                 In der Fußzeile des Registers wird keine weitere Information ausgegeben.


                                 Ergänzende Informationen
                                  “Zusatzmenü” auf Seite G-22
                                  “Infomenü” auf Seite G-25
                                  “Schaltflächen” auf Seite G-27
2.00 / 04-2022




                 G-52                                                       A+W Enterprise Versandsteuerung
                 Softwarereferenz                                                                       Auftragsebene




                                          Register – ZusatzInfo
                                          Versandsteuerung – Lieferdatumauswahl > Routenauswahl >
                                          Register ZusatzInfo




                 Abb. G-20   Versandsteuerung – Register Zusatzinfo


                                          Im Register Zusatzinfo sehen Sie die gelieferte Stückzahl mit weiterführenden
                                          Informationen zum Auftrag, Positionsgewichte, Verschiebungen und Informa-
                                          tionen zur Versandfreigabe durch den Kunden.
                                          Die Suchfelder in der Kopfzeile sind im Dialog Versandsteuerung erklärt. Zu-
                                          sätzlich werden die Routennummer und der Routenname angezeigt.
                                           “Versand-Explorer” auf Seite G-15
                                          Die meisten Felder sind bereits im vorherigen Kapitel beschrieben:
                                           “Register – VersandInfo I” auf Seite G-48
                                          Zusätzlich werden folgende Felder in dem Register ZusatzInfo angezeigt:

                                          Kunde Kundenname bzw. Lieferantenname aus dem Auftrag bzw. Bestel-
                                          lung.
                                          Technische Info: Anzeige-Feld, DB-Feld: mp.name

                                          G/Gel Gesamtstückzahl, die bereits an den Kunden geliefert ist.
2.00 / 04-2022




                                          Technische Info: Anzeige-Feld, DB-Feld: lapoolauf.geslief




                 A+W Enterprise Versandsteuerung                                                                 G-53
                 Auftragsebene                                                                 Softwarereferenz




                                 kg/N Nettogewicht in Kilogramm für diesen Auftrag. Das Nettogewicht ist das
                                 Gewicht aller Positionen ohne Gestelle oder Verpackung.
                                 Technische Info: Anzeige-Feld, DB-Feld: lapoolauf.gewicht

                                 kg/B Bruttogewicht in Kilogramm für diesen Auftrag. Das Bruttogewicht ist
                                 das Gewicht aller Positionen inkl. Gestell oder Verpackung.
                                 Technische Info: Anzeige-Feld, DB-Feld: lapoolauf.gewichtbrutto

                                 qm Quadratmeter der gesamten Glasfläche aus dem Auftrag.
                                 Technische Info: Anzeige-Feld, DB-Feld: lapoolauf.qm

                                 LS Ampelanzeige für den Lieferschein.
                                  “Status des Lieferscheins” auf Seite G-41

                                 Abr. Abrufkennzeichen für den Auftrag. Der Auftrag wird auf Anforderung an
                                 den Kunden geliefert.
                                 Technische Info: Anzeige-Feld, DB-Feld: DB-Feld: lapoolauf.abrufkz

                                 versch. Kennzeichen zum Markieren, um den Auftrag zu verschieben. Wenn
                                 Sie mehrere Aufträge auf einen anderen Versandtermin verschieben möch-
                                 ten, dann müssen Sie die Checkboxen der entsprechenden Aufträge ankli-
                                 cken. Die ausgewählten Aufträge sind dann mit einem Häkchen markiert. Über
                                 den Dialog Verschiebung (Versand) führen Sie die Verschiebung durch.
                                  Der Auftrag wird verschoben.
                                  Der Auftrag wird nicht verschoben.
                                 Technische Info: Anzeige-Feld
                                  “Funktionen im Versand” auf Seite G-62

                                 Anruf Kennzeichnung, ob der Kunde vor der Auslieferung telefonisch be-
                                 nachrichtigt wird.
                                  Der Kunde wird vor der Auslieferung angerufen.
                                  Der Kunde wird nicht angerufen.
                                 Wenn Sie das Feld aktivieren, dann wird die Anruf-Checkbox automatisch
                                 auch alle weiteren Aufträge für diesen Kunden mit aktivieren.
                                 Technische Info: Alphanumerisches Feld, DB-Feld: lapoolauf.anruf

                                 Druck Kennzeichen, ob ein Lieferschein gedruckt wurde.
                                  Der Lieferschein ist gedruckt.
                                  Der Lieferschein ist noch nicht gedruckt.
                                 Technische Info: Anzeige-Feld, DB-Feld: lapoolauf.druckkz

                                 Typ Der ausgewählte Lieferscheintyp für diesen Auftrag wird als Kürzel ange-
                                 zeigt.
                                 Folgende Kennzeichen stehen zur Verfügung:
                                 • E = Einzellieferschein
                                 • S = Sammellieferschein
2.00 / 04-2022




                                    Technische Info: Anzeige-Feld




                 G-54                                                          A+W Enterprise Versandsteuerung
                 Softwarereferenz                                                                   Auftragsebene




                                       Fußzeile
                                       In der Fußzeile des Registers sind für alle Positionen die Gesamtstückzahlen
                                       der folgenden Felder aufgelistet:
                                       • kg/N (Gewicht netto)
                                       • kg/B (Gewicht brutto)
                                       • qm (Gesamtfläche in Quadratmetern)
                                           Technische Info: Anzeige-Feld


                                       Ergänzende Informationen
                                        “Zusatzmenü” auf Seite G-22
                                        “Infomenü” auf Seite G-25
                                        “Schaltflächen” auf Seite G-27
2.00 / 04-2022




                 A+W Enterprise Versandsteuerung                                                             G-55
                 Positionsebene                                                                Softwarereferenz




                                  Positionsebene
                                  Auf der Positionsebene der Versandsteuerung sehen Sie die detaillierten In-
                                  formationen zu den einzelnen Positionen der Aufträge bzw. Bestellungen.
                                  Auf dieser Ebene finden Sie folgende Register:
                                      “Register – PositionsInfo I” auf Seite G-57
                                      “Register – PositionsInfo II” auf Seite G-60
                                  Aus der Positionsebene können Sie zurück zur Auftrags- oder Tourenebene
                                  wechseln. Wenn Sie mit dem Versand-Explorer arbeiten, haben Sie auch die
                                  Möglichkeit, direkt zu dem Versand-Explorer zu wechseln, um ein anderes Da-
                                  tum auszuwählen.
                                      “Versand-Explorer” auf Seite G-15
2.00 / 04-2022




                 G-56                                                          A+W Enterprise Versandsteuerung
                 Softwarereferenz                                                                      Positionsebene




                                          Register – PositionsInfo I
                                          Versandsteuerung – Lieferdatumauswahl > Routenauswahl > Auftrags-/Be-
                                          stellungs-Auswahl > Register PositionsInfo I




                 Abb. G-21   Versandsteuerung – Register PositionsInfo I


                                          Im Register PositionsInfo I sind Detailinformationen zu den Aufträgen aufge-
                                          listet.
                                          Die Suchfelder in der Kopfzeile sind im Dialog Versandsteuerung erklärt. Zu-
                                          sätzlich wird die Fahrtroute, Auftragsnummer und der Kundenname ange-
                                          zeigt.
                                           “Versand-Explorer” auf Seite G-15

                                          S Die Werte in der Spalte S (Status) sind aus den Registern TourenInfo und
                                          AuftragsInfo übernommen.
                                          Technische Info: Anzeige-Feld
                                           “Routenstatus” auf Seite G-29

                                          Pos. Laufende Positionsnummer aus dem Auftrag bzw. aus der Bestellung.
                                          Technische Info: Anzeige-Feld, DB-Feld: lapool.posnr

                                          Artikel Artikelbezeichnung des zu liefernden Artikels.
                                          Technische Info: Anzeige-Feld, DB-Feld: artikel.artbez1
2.00 / 04-2022




                                          Ges. Gesamte Stückzahl der zu liefernden Position.
                                          Technische Info: Anzeige-Feld, DB-Feld: lapoolpos.gesstk


                 A+W Enterprise Versandsteuerung                                                                 G-57
                 Positionsebene                                                                Softwarereferenz




                                  Abruf Stückzahl der Position, die der Kunde für den Liefertermin anfordert.
                                  Technische Info: Anzeige-Feld, DB-Feld: lapoolpos.abrufstk

                                  Gepl. Geplant. Stückzahl der Position, die zum Versand geplant sind.
                                  Technische Info: Anzeige-Feld, DB-Feld: lapoolpos.sollstk

                                  Verf. Verfügbare Stückzahl der Position.
                                  Technische Info: Anzeige-Feld, DB-Feld: lapoolpos.gefstk

                                  Verp. Verpackte Stückzahl der Position. Über <F4> führen Sie eine Fehlmen-
                                  genkontrolle durch. Über <F4> > Verpackte Menge korrigieren ändern Sie
                                  nachträglich den Wert in diesem Feld.
                                  Technische Info: Numerisches Feld, DB-Feld: lapoolpos.iststk
                                   “Fehlmengenkontrolle - Auswahl” auf Seite G-78
                                   “Barcode Gestellanzeige” auf Seite G-84

                                  Rück. Stückzahl der Position, die zum gewünschten Tourentag nicht zur Ver-
                                  fügung steht.
                                  Technische Info: Anzeige-Feld, DB-Feld: lapoolpos.rueckstk

                                  Nach. Stückzahl, die nachgeliefert werden muss. Nachlieferungen können
                                  durch Verschiebungen zustande kommen.
                                  Technische Info: Anzeige-Feld, DB-Feld: lapoolpos.nachstk
                                   “Verschieben” auf Seite G-66

                                  Über. Überlieferung. Stückzahl der Position, die für diesen Auftrag die ge-
                                  samte Stückzahl übersteigt. Überlieferung kann durch die Verschiebung von
                                  Positionen zustande kommen.
                                  Technische Info: Anzeige-Feld, DB-Feld: lapoolpos.ueberstk

                                  G/Gel Gesamtstückzahl, die bereits an den Kunden geliefert ist.
                                  Technische Info: Anzeige-Feld, DB-Feld: lapoolpos.gesliefstk

                                  kg Gewicht der Position in Kilogramm.
                                  Technische Info: Anzeige-Feld, DB-Feld: lapoolpos.gewicht

                                  qm Fläche der Position in Quadratmetern.
                                  Technische Info: Anzeige-Feld, DB-Feld: lapoolpos.qm

                                  kmp. Komplett verpackte Position.
                                   Alle Positionen sind zur Auslieferung bereit.
                                   Noch nicht alle Positionen sind zur Auslieferung bereit.
                                  Technische Info: Anzeige-Feld, DB-Feld: lapoolpos.kompl
                                   “Fehlmengenkontrolle - Auswahl” auf Seite G-78

                                  F (fakturiert) Komplett fakturierte Position.
                                   Die Auftragsposition ist fakturiert.
                                   Die Auftragsposition ist noch nicht fakturiert.
2.00 / 04-2022




                                  Technische Info: Anzeige-Feld, DB-Feld: lapoolpos.fakturakz




                 G-58                                                       A+W Enterprise Versandsteuerung
                 Softwarereferenz                                                                   Positionsebene




                                       Fußzeile
                                       In der Fußzeile des Registers sind für alle Positionen die Gesamtstückzahlen
                                       der folgenden Felder aufgelistet:
                                       • Ges. (gesamt)
                                       • Abruf (Abrufwunsch)
                                       • Gepl. (geplant)
                                       • Verf. (verfügbar)
                                       • Verp. (verpackt)
                                       • Rück. (Rückstand)
                                       • Nach. (Nachlieferung)
                                       • Über. (Überlieferung)
                                       • G/Gel. (gesamt geliefert)
                                       • kg
                                       • qm


                                       Ergänzende Informationen
                                        “Zusatzmenü” auf Seite G-22
                                        “Infomenü” auf Seite G-25
                                        “Schaltflächen” auf Seite G-27
2.00 / 04-2022




                 A+W Enterprise Versandsteuerung                                                             G-59
                 Positionsebene                                                                            Softwarereferenz




                                           Register – PositionsInfo II
                                           Versandsteuerung – Lieferdatumauswahl > Routenauswahl > Auftrags-/Be-
                                           stellungs-Auswahl > Register Positionsinfo II




                 Abb. G-22   Versandsteuerung – Register PositionsInfo II


                                           Im Register PositionsInfo II sind die Positionen zum Auftrag aufgelistet. Für
                                           jede Position sind weiterführende Informationen aufgelistet.
                                           Die Suchfelder in der Kopfzeile sind im Dialog Versandsteuerung erklärt. Zu-
                                           sätzlich wird die Fahrtroute, Auftragsnummer und der Kundenname ange-
                                           zeigt.
                                            “Versand-Explorer” auf Seite G-15
                                           Die meisten Felder sind bereits im vorherigen Kapitel beschrieben:
                                            “Register – PositionsInfo I” auf Seite G-57
                                           Zusätzlich werden folgende Felder in dem Register ZusatzInfo angezeigt:

                                           Verp./Verpackart Nummer und die Bezeichnung der Verpackungsart.
                                           Technische Info: Anzeige-Feld, DB-Feld: lapoolpos.verpackart

                                           Breite, Höhe Maße der Position.
                                           Technische Info: Anzeige-Feld, DB-Feld: lapoolpos.laenge, lapoolpos.breite
2.00 / 04-2022




                                           mm Dicke der Positionsscheibe in Millimeter.
                                           Technische Info: Anzeige-Feld, DB-Feld: lapoolpos.staerke



                 G-60                                                                      A+W Enterprise Versandsteuerung
                 Softwarereferenz                                                                   Positionsebene




                                       Fußzeile
                                       In der Fußzeile des Registers sind für alle Positionen die Gesamtstückzahlen
                                       der folgenden Felder aufgelistet:
                                       • Ges. (gesamt)
                                       • Gepl. (geplant)
                                       • Verp. (verpackt)
                                       • kg
                                       • qm


                                       Ergänzende Informationen
                                        “Zusatzmenü” auf Seite G-22
                                        “Infomenü” auf Seite G-25
                                        “Schaltflächen” auf Seite G-27
2.00 / 04-2022




                 A+W Enterprise Versandsteuerung                                                             G-61
                 Funktionen im Versand                                                              Softwarereferenz




                                         Funktionen im Versand
                                         In der Versandsteuerung haben Sie Möglichkeiten, die Positionsmenge manu-
                                         ell zu verpacken oder zu verschieben, Gestelle zu verwalten und die Versand-
                                         Dokumente zu drucken. Je nach Status der gewählten Daten auf der Positi-
                                         ons-, Auftrags- oder Tourenebene und verfügbarer Systemkonfiguration ha-
                                         ben Sie folgende Funktionen zur Verfügung:
                                          “Springen” auf Seite G-64
                                          “Verschieben mehrerer Pos. - Auswahl” auf Seite G-69
                                          “Fehlmengenkontrolle - Aktion” auf Seite G-80
                                          “Drucken einer Ladeliste” auf Seite G-133
                                          “Buchen auf Transport” auf Seite G-82
                                          “Barcode Gestellanzeige” auf Seite G-84
                                          “Gestellinformationen” auf Seite G-89
                                         Im Weiteren haben Sie viele Übersichtsmöglichkeiten und Informationsdialo-
                                         ge anhand der vorbestimmten Kriterien:
                                          “Transport zurückbuchen” auf Seite G-83
                                          “VK/EK Info (Global)” auf Seite G-117
                                          “Gebuchte Gestelle (Übersicht)” auf Seite G-106
                                          “Informationen zum Auftrag” auf Seite G-73
                                          “Fertigwarenlager Übersicht” auf Seite G-127
                                          “Versandinformationen” auf Seite G-123
                                          “Toursperre setzen/löschen” auf Seite G-90
                                          “Informationen zum Auftrag” auf Seite G-73
2.00 / 04-2022




                 G-62                                                               A+W Enterprise Versandsteuerung
                 Softwarereferenz                                                               Funktionen im Versand




                                       Suchen
                                       Versandsteuerung – [Suchen]




                                       Abb. G-23      Springe zu…


                                       Den Dialog Suchen erreichen Sie auf allen Datenebenen. Somit können Sie
                                       nach einem bestimmtem Vorgang suchen und direkt zu diesem Vorgang sprin-
                                       gen.
                                       Über die Tastenkombination <Strg> + <K> werden Sie ebenfalls zur Auftrags-
                                       info geleitet.

                                       Auftrag Auftragsnummer. Geben Sie in diesem Feld die Nummer ein, oder
                                       wählen Sie die Nummer über <F9 aus. Mit dieser Suche erhalten die ausführ-
                                       liche Information zu dem gewählten Vorgang.
                                       Technische Info: Numerisches Feld, Auswahl-Feld, <F9>
                                        “Informationen zum Auftrag” auf Seite G-73

                                       Modus Versandmodus. Wenn Sie direkt zu den Bestellvorgängen wechseln
                                       wollen, toggeln Sie im Feld Modus auf den entsprechenden Wert. Bei einem
                                       Einkaufsmodus können Sie anschließend nach einer Bestellung statt einen
                                       Auftrag suchen.
                                       Technische Info: Toggle-Feld


                                       Schaltfläche       Beschreibung

                                       [Auslösen]         Mit Auslösen starten Sie die Suche.
                                       [Abbrechen]        Mit Abbrechen verwerfen Sie die Suche.
2.00 / 04-2022




                 A+W Enterprise Versandsteuerung                                                               G-63
                 Funktionen im Versand                                                                   Softwarereferenz




                                         Springen
                                         Versandsteuerung – [Springen]




                                         Abb. G-24     Springe zu…


                                         Den Dialog Springen erreichen Sie auf allen Datenebenen. Somit können Sie
                                         nach bestimmten Aufträge suchen und direkt zu der Ebene springen. Die Fel-
                                         der Lieferdatum, Haus und Modus sind mit jeweils aktuellen Wert vorbelegt.
                                         Bei Bedarf können Sie die Suchkriterien verändern.

                                         Lieferdatum Lieferdatum der Aufträge. Das Feld wird mit dem tagesaktuellen
                                         Datum vorbelegt. Sie können den Wert ändern.
                                         Technische Info: Eingabe-Feld, Datumsformat.

                                         Haus Nummer des Hauses oder Mandanten, für den Sie Aufträge suchen.
                                         Das Feld wird mit dem Wert vorbelegt, der dem aktuellen Mitarbeiter in den
                                         Stammdaten standardmäßig zugewiesen ist.
                                         Technische Info: Auswahl-Feld, <F9>

                                         Route Routennummer. Wenn Sie das Feld Route leer lassen und sind für das
                                         Lieferdatum geplante Routen vorhanden, wird direkt in die TourenInfo ge-
                                         sprungen.
                                         Technische Info: Auswahl-Feld, <F9>
                                          “Register – TourenInfo” auf Seite G-29

                                         Auftrag Auftragsnummer. Wenn Sie das Feld Auftrag leer lassen und sind für
                                         das Lieferdatum und die gewählte Route Aufträge vorhanden, wird direkt in die
                                         AuftragsInfo gesprungen.
                                         Technische Info: Auswahl-Feld, <F9>
                                          “Register – AuftragsInfo” auf Seite G-39

                                         Position Laufende Positionsnummer aus dem Vorgang.Wenn Sie die Felder
                                         Lieferdatum, Route und Auftrag auswählen, startet direkt die PositionsInfo.
                                         Technische Info: Auswahl-Feld, <F9>
                                          “Register – PositionsInfo I” auf Seite G-57
2.00 / 04-2022




                                         Modus Versandmodus. Wenn Sie direkt zu den Bestellvorgängen wechseln
                                         wollen, toggeln Sie im Feld Modus auf den entsprechenden Wert. Bei Ein-


                 G-64                                                                    A+W Enterprise Versandsteuerung
                 Softwarereferenz                                                            Funktionen im Versand




                                       kaufsmodus können Sie anschließend nach einer Bestellung statt einen Auf-
                                       trag suchen.
                                       Technische Info: Toggle-Feld


                                       Schaltfläche    Beschreibung

                                       [Auslösen]      Mit Auslösen starten Sie die Suche.
                                       Inh. löschen    Mit Inh(alte) löschen leeren Sie die Dialogfelder.
                                       [Abbrechen]     Mit Abbrechen verwerfen Sie die Suche.
2.00 / 04-2022




                 A+W Enterprise Versandsteuerung                                                            G-65
                 Funktionen im Versand                                                               Softwarereferenz




                                         Verschieben
                                         Versandsteuerung – Datenebene > <F4> Verschieben




                                         Abb. G-25    Verschiebung (Versand)


                                         In diesem Dialog verschieben Sie Touren, Aufträge oder Einheiten auf einen
                                         anderen Tag oder auf eine andere Route. Im Feld Begründung geben Sie ei-
                                         nen Informationstext für den Grund der Verschiebung ein.
                                         Wenn Sie die Verschiebung auf der Tourenebene starten, kann die komplette
                                         Route verschoben werden. In diesen Fall sind die Felder Auftrag und Position
                                         im oberen Dialogteil leer. Starten Sie die Verschiebung auf der Auftrags- bzw.
                                         Positionsebene sind diese beiden Felder entsprechend vorbelegt.
                                         Die Felder im oberen Dialogteil geben an, was verschoben wird:

                                         Vom Tourtag Ursprünglich geplantes Versanddatum.

                                         Route Nummer der ursprünglich geplanten Versandroute.

                                         Einheiten Anzahl der Einheiten, die verschoben werden.

                                         Auftrag Nummer des Auftrags, der verschoben wird. Die Anzeige ist leer,
                                         wenn die gesamte Route verschoben wird.

                                         Position Laufende Auftragspositionsnummer, die verschoben wird. Die An-
                                         zeige ist leer, wenn die gesamte Route oder der gesamte Auftrag verschoben
                                         wird.
                                         Die Felder im mittleren Dialogbereich geben an, wohin und warum verscho-
                                         ben wird:

                                         Begründung Auswahl einer Begründung für das Verschieben. Im System
                                         kann konfiguriert werden, welche dieser Begründung als Standardwert im Di-
                                         alog erscheint. Folgende Gründe sind möglich:
                                         • Kundenwunsch:
                                            Der Kunde hat das Verschieben veranlasst.
                                         • Rückstand:
                                            Die Position ist noch nicht fertig gestellt oder noch nicht zum Versand be-
2.00 / 04-2022




                                            reit.
                                         • Kundenstorno:



                 G-66                                                              A+W Enterprise Versandsteuerung
                 Softwarereferenz                                                             Funktionen im Versand




                                           Der Kunde hat den Auftrag, die Position oder eine Teilstückzahl storniert.
                                           Bei der Verschiebung als Kundenstorno wird sowohl die Abrufmenge als
                                           auch die geplante Menge um die stornierte Stückzahl verringert.
                                       •   Betriebsstorno:
                                           Die Lieferung wird aus internen Gründen storniert, z. B. wenn das Produkt
                                           nicht mehr lieferbar ist. Bei Betriebsstorno wird nur die geplante Menge
                                           verringert. Die Verschiebung mit der Begründung Betriebsstorno ist sepa-
                                           rat konfigurierbar.
                                       •   Tourenplanung:
                                           Das Verschieben hat Gründe, die mit der Tourenplanung oder Disposition
                                           zusammenhängen. Die Verschiebung erfolgt analog der Verschiebung auf
                                           Kundenwunsch nur auf Tourenebene. Diese Möglichkeit kann separat kon-
                                           figuriert werden. Ebenso kann die Begründung Tourenplanung als Stan-
                                           dardgrund konfiguriert werden.
                                       Durch eine weitere Konfiguration können kundenindividuelle Gründe als ein
                                       Auswahlselo hinterlegt werden. Bei dieser Konfiguration kann das Feld Be-
                                       gründung leer gelassen werden oder ein freier Text eingegeben werden. Das
                                       System verschickt dabei eine E-Mail mit dem Verschiebegrund an den zustän-
                                       digen Mitarbeiter.

                                       Verschiebung Textfeld für die Begründung der Verschiebung. Dieser Text
                                       wird in das Versandprotokoll übernommen.

                                       Gestell Gestellnummer. Wenn Sie mit Gestellen in der Versandsteuerung ar-
                                       beiten, können unter Umständen auch komplette Gestelle verschoben wer-
                                       den. Diese Möglichkeit ist jedoch von anderen Kriterien abhängig, wie z.B.,
                                       verpackte und verfügbare Menge, Gestellplanung, Positionsstatus.

                                       Mehrere Sätze verschieben Toggle-Feld.

                                       Auf Tourtag Neues Lieferdatum. Nach dem Starten der Verschiebung wird
                                       geprüft, ob das eingegebene Datum ein gültiges Lieferdatum ist. Wenn das
                                       neue Datum kein gültiger Tourentag ist, dann kann die Tour bzw. die Lieferung
                                       nicht verschoben werden. Wenn Sie mit geplanten Touren arbeiten, können
                                       Sie in diesem Feld nach einer bestimmten Tour über <F9> suchen.
                                        Stammdaten: Softwarereferenz, “Tourenplan” auf Seite B-176

                                       Route Nummer der neuen Route, wenn durch die Verschiebung die Route
                                       angepasst werden muss.

                                       Einheiten Anzahl der Einheiten, die verschoben wird. Standardmäßig zeigt
                                       A+W Enterprise die komplette Anzahl an.
                                       Die Felder im unteren Dialogbereich geben an, wer und wann die Verschie-
                                       bung durchführt:

                                       Durchgeführt von Mitarbeiternummer, die die Verschiebung durchführt hat.
                                       Diese Information wird in das Protokoll geschrieben.
                                        “Versandinformationen” auf Seite G-123
2.00 / 04-2022




                 A+W Enterprise Versandsteuerung                                                               G-67
                 Funktionen im Versand                                                              Softwarereferenz




                                         am Datum, an dem die Verschiebung durchgeführt wurde. Diese Information
                                         wird in das Protokoll geschrieben.
                                          “Versandinformationen” auf Seite G-123
2.00 / 04-2022




                 G-68                                                               A+W Enterprise Versandsteuerung
                 Softwarereferenz                                                               Funktionen im Versand




                                       Verschieben mehrerer Pos. - Auswahl
                                       Versandsteuerung – Datenebene > <F4> > Verschieben mehrerer Pos.




                                       Abb. G-26    Verschieben mehrerer Positionen - Auswahldialog


                                       In diesem Dialog filtern Sie Ihre Lieferungen für die Verschiebung mehrerer
                                       Positionen eines Auftrags oder mehrere Aufträgen gleichzeitig. In dem nach-
                                       folgenden Dialog geben Sie pro Position die zu verschiebende Menge ein.
                                        “Verschiebung mehrerer Pos. - Aktion” auf Seite G-70

                                       Haus Hausnummer. Das Feld wird mit der aktuellen Hausnummer vorbelegt.
                                       Sie können den Wert nur ändern, wenn Sie im Mehrmandantensystem arbei-
                                       ten.
                                       Technische Info: Auswahl-Feld, <F9>, DB-Feld: lapool.hausnr

                                       Termin Datum der Lieferung. Das Feld wird mit dem Datum vorbelegt, das
                                       Sie sich auf der ursprünglichen Datenebene haben anzeigen lassen.
                                       Technische Info: Eingabe-Feld, Datumsformat, DB-Feld: lapool.ltplan

                                       Route Nummer der Route. Das Feld wird mit der Routennummer vorbelegt,
                                       die Sie sich auf der ursprünglichen Tourenebene haben anzeigen lassen.
                                       Technische Info: Auswahl-Feld, <F9>, DB-Feld: lapool.ltplan

                                       Auftrag Nummer des Auftrags. Das Feld wird mit der Auftragsnummer vor-
                                       belegt, die Sie sich auf der ursprünglichen Auftragsebene haben anzeigen las-
                                       sen.
                                       Technische Info: Auswahl-Feld, <F9>, DB-Feld: lapool.auftrnr

                                       Ladeliste Nummer der Ladeliste. Sie können hier nach einer bestimmten La-
                                       deliste suchen, falls diese bereits vergeben wurde.
                                       Technische Info: Auswahl-Feld, <F9>, DB-Feld: lapool.llnr
2.00 / 04-2022




                 A+W Enterprise Versandsteuerung                                                               G-69
                 Funktionen im Versand                                                                    Softwarereferenz




                                          Verschiebung mehrerer Pos. - Aktion
                                          Versandsteuerung – Datenebene > <F4> > Verschieben mehrerer Pos., Aus-
                                          wahl treffen




                 Abb. G-27   Verschiebung mehrere Positionen


                                          In diesem Dialog wählen Sie die Positionen für die Verschiebung aus. Außer-
                                          dem passen Sie die Menge pro Position an, die verschoben werden muss. Die
                                          Vorauswahl haben Sie bereits gemäß Angaben getroffen:
                                           “Verschieben mehrerer Pos. - Auswahl” auf Seite G-69
                                          Die meisten Felder sind bereits im folgenden Kapitel beschrieben:
                                           “Register – PositionsInfo I” auf Seite G-57
                                          Folgende Felder können Sie ändern, um die Verschiebung durchzuführen:

                                          Verschieben Das Feld Verschieben ist mit der Positionsmenge vorbelegt.
                                          Sie können diese Menge ändern, wenn nur ein Teil der Position verschoben
                                          werden soll. Es darf maximal die Positionsmenge verschoben werden. Das
                                          Programm prüft den eingegeben Wert auf die Plausibilität.
                                          Technische Info: Eingabe-Feld, Numerisches Feld.

                                          Buch. Checkbox für die Aktionsmarkierung der Buchung.
                                           Position wird zum Verschieben markiert.
2.00 / 04-2022




                                           Position wird nicht verschoben.
                                          Technische Info: Auswahl-Feld, Checkbox.



                 G-70                                                                     A+W Enterprise Versandsteuerung
                 Softwarereferenz                                                           Funktionen im Versand




                                       Über die Schaltfläche [Auslösen] starten Sie die Verschiebung. In dem darauf-
                                       folgenden Dialog geben Sie ein, wohin die markierten Positionen verschoben
                                       werden soll.
                                        “Verschieben” auf Seite G-66
2.00 / 04-2022




                 A+W Enterprise Versandsteuerung                                                              G-71
                 Funktionen im Versand                                                              Softwarereferenz




                                         Auftragsinfo
                                         Versandsteuerung – Datenebene> <F4> > Auftragsinfo.




                                         Abb. G-28    Verschieben mehrerer Positionen


                                         In diesem Dialog suchen Sie nach einem Auftrag (bei Versandmodus für Ver-
                                         kaufsvorgängen) oder nach einer Bestellung (bei Versandmodus mit Einkaufs-
                                         vorgängen) Über die Schaltfläche [Auslösen] gelangen Sie zur gesuchten
                                         Information.

                                         Auftrag/Bestellung Vorgangsnummer. Mit <F9> können Sie nach ge-
                                         wünschten Vorgangsnummer suchen.
                                         Technische Info: <F9>, Numerisches Feld, DB-Feld: lapool.auftrnr

                                         Modus Versandmodus. In diesem Feld wählen Sie den Versandmodus aus.
                                         Daraus resultiert auch, ob nach Aufträgen oder nach Bestellungen selektiert
                                         wird. Mit <F9> können Sie nach der gewünschten Vorgangsnummer suchen.
                                         Technische Info: Auswahl-Feld, <F9>, DB-Feld: lapool.vmodus
                                         Das Suchergebnis ist im folgenden Kapitel beschrieben:
                                          “Informationen zum Auftrag” auf Seite G-73
2.00 / 04-2022




                 G-72                                                               A+W Enterprise Versandsteuerung
                 Softwarereferenz                                                                           Funktionen im Versand




                                                 Informationen zum Auftrag
                                                 Versandsteuerung – Datenebene> <F4> > Auftragsinfo > [Auslösen]




                 Abb. G-29      Informationen zum Auftrag oder zur Bestellung


                                                 In diesem Dialog sehen Sie weitere Informationen zu dem gewählten Vor-
                                                 gang. Der Dialogtitel ist dynamisch, je nach gewählten Versandmodus wird die
                                                 Anzeige angepasst. Zusätzlich steht in dem Titel die entsprechende Vor-
                                                 gangsnummer.
                                                 Alle Felder in diesem Dialog sind informativ und nicht änderbar.

                                                 S Status aktueller Liefer-Position.


                 S (Status)          Bedeutung                 Information

                    weiß             Offen                     Für diese Position existiert noch keine Versandplanung.

                    grün/gelb        Verfügbar                 Ein Teil dieser Position ist als Verfügbar gemeldet.

                    gelb/weiß        Teil auf Gestell          Ein Teil dieser Position befindet sich bereits auf dem Gestell.

                    gelb             Verpackt                  Diese Position ist komplett verpackt.

                    halbblau         Auf Transport             Ein Teil dieser Position befindet sich bereits auf dem Transport.

                    blau             Geliefert                 Diese Position ist komplett ausgeliefert.
2.00 / 04-2022




                    rot              gesperrt                  Diese Position befindet sich auf einer gesperrten Tour.

                 Tab. G-4       Status zu Lieferpositionen



                 A+W Enterprise Versandsteuerung                                                                                   G-73
                 Funktionen im Versand                                                              Softwarereferenz




                                         Haus Nummer des Hauses oder Mandanten.
                                         Technische Info: Anzeige-Feld, DB-Feld: lapool.hausnr

                                         HZ Handlings-Zeit aus dem Auftrag bzw. Bestellung, um die Ware zu verla-
                                         den und zu entladen. Die Handlings-Zeit kann in den Marktpartner-Stammda-
                                         ten festgelegt werden.
                                         Technische Info: Anzeige-Feld, DB-Feld: lapool.hausnr

                                         Lieferdat. Lieferdatum, an dem der Auftrag zum Kunden geliefert wird.
                                         Technische Info: Anzeige-Feld, DB-Feld: lapool.ltplan, kauf.ltplan

                                         Ankunft Datum an dem die Lieferung beim Kunden ankommt. Das Ankunft-
                                         datum wird ausgehend vom Liefertermin - unter Berücksichtigung verschiede-
                                         ner weiterer Kriterien - wie Fahrdauer, Handlings-Zeit, Tourenplan, Routenta-
                                         gen und dem Kalender errechnet.
                                         Technische Info: Anzeige-Feld, <F9>, DB-Feld: lapool.auftrnr

                                         Route Nummer der Route.
                                         Technische Info: Anzeige-Feld, DB-Feld: lapool.routenr

                                         Auftrag Auftrags- bzw. Bestellnummer.
                                         Technische Info: Anzeige-Feld, DB-Feld: lapool.auftrnr, lapool.vorgang

                                         Pos. Positionsnummer.
                                         Technische Info: Anzeige-Feld, DB-Feld: lapool.posnr

                                         Ges. Gesamte Stückzahl aus der Position.
                                         Technische Info: Anzeige-Feld, DB-Feld: lapool.gesstk, kpos.menge

                                         Abruf Stückzahl der Position, die der Kunde für den Liefertermin anfordert.
                                         Technische Info: Anzeige-Feld, DB-Feld: lapool.abrufstk

                                         Gepl. Bereits geplante Menge der Position.
                                         Technische Info: Anzeige-Feld, DB-Feld: lapool.sollstk

                                         Verp. Verpackte Stückzahl der Position.
                                         Technische Info: Anzeige-Feld, DB-Feld: lapool.iststk

                                         Breite Breite der Scheibe aus der Position.
                                         Technische Info: Anzeige-Feld, DB-Feld: lapool.laenge

                                         Höhe Höhe der Scheibe aus der Position.
                                         Technische Info: Anzeige-Feld, DB-Feld: lapool.breite

                                         kg Gewicht der Position in Kilogramm.
                                         Technische Info: Anzeige-Feld, DB-Feld: lapool.gewicht

                                         VP Anzeige-Checkbox, wenn die Ware per via-plant geliefert.
                                         Technische Info: Anzeige-Feld
2.00 / 04-2022




                                         [FW Lager] Die Schaltfläche öffnet den Dialog Fertigwarenlager.
                                          “Fertigwarenlager Übersicht” auf Seite G-127



                 G-74                                                               A+W Enterprise Versandsteuerung
                 Softwarereferenz                                                         Funktionen im Versand




                                       [Springen] Die Schaltfläche startet den Dialog Springen zu.
                                        “Springen” auf Seite G-64
2.00 / 04-2022




                 A+W Enterprise Versandsteuerung                                                         G-75
                 Funktionen im Versand                                                              Softwarereferenz




                                         Liefereingang buchen
                                         Versandsteuerung – Datenebene > <F4> > Liefereingang buchen




                                         Abb. G-30   Liefereingang buchen


                                         In diesem Dialog wählen Sie einen Auftrag, zu dem Sie den Liefereingang bu-
                                         chen möchten. Diese Funktion steht nur bei die via-plant - Konfiguration zur
                                         Verfügung.


                                         via-plant–Konfiguration
                                         Der Funktionsumfang via-plant ist nicht der Bestandteil dieser Dokumentation.
                                         Die ausführliche Beschreibung kann bei Bedarf beim zuständigen A+W Mitar-
                                         beiter angefragt werden.
2.00 / 04-2022




                 G-76                                                             A+W Enterprise Versandsteuerung
                 Softwarereferenz                                                             Funktionen im Versand




                                       Storno des Liefereingangs
                                       Versandsteuerung – Datenebene > <F4> > Storno des Liefereingangs




                                       Abb. G-31    Informationen zum Auftrag


                                       In diesem Dialog wählen Sie einen Auftrag, zu dem Sie den Liefereingang
                                       stornieren wollen. Diese Funktion steht nur bei die via-plant-Konfiguration zur
                                       Verfügung.

                                          via-plant-Konfiguration
                                          Der Funktionsumfang via-plant ist nicht der Bestandteil dieser Dokumenta-
                                          tion. Die ausführliche Beschreibung kann bei Bedarf beim zuständigen
                                          A+W Mitarbeiter angefragt werden.
2.00 / 04-2022




                 A+W Enterprise Versandsteuerung                                                                G-77
                 Funktionen im Versand                                                              Softwarereferenz




                                         Fehlmengenkontrolle - Auswahl
                                         Versandsteuerung – Datenebene > <F4> > Fehlmengenkontrolle




                                         Abb. G-32   Fehlmengenkontrolle für…


                                         In diesem Dialog treffen Sie die Auswahl, für welchen Auftrag Sie die Positi-
                                         onsmenge kontrollieren möchten. Sie können alle Aufträge für das bestimmte
                                         Lieferdatum oder die Route prüfen oder Sie können nur einen bestimmten Auf-
                                         trag auswählen. Eine Fehlmengenkontrolle wird beispielsweise durchgeführt,
                                         wenn eine Position zu dem vorgegeben Liefertermin nicht komplett geliefert
                                         werden kann.

                                            Fehlmengenkontrolle im Versand
                                            Eine Fehlmengenkontrolle im Versand erfolgt ausschließlich auf eigene
                                            Verantwortung des Benutzers. Beim Arbeiten mit A+W Production über-
                                            nimmt die Produktionssoftware alle Mengenbuchungen. Wenn Sie jedoch
                                            die Kontrolle in der Versandsteuerung durchführen, können die Bedienun-
                                            gen für die Fehlmengenkontrolle und anschließender Buchung im System
                                            teils individuell konfiguriert werden. Sprechen Sie dazu den A+W - Mitar-
                                            beiter an.

                                         Lieferdat. Datum der Lieferung, für die Sie die Fehlmengenkontrolle durch-
                                         führen. Das Feld wird mit dem Datum vorbelegt, das Sie in dem vorherigen Di-
                                         alog gewählt haben.
                                         Technische Info: Eingabe-Feld, Datumsformat, DB-Info: lapool.ltplan

                                         Route Nummer der Route, für die Sie die Fehlmengenkontrolle durchführen.
                                         Wenn Sie das Feld leer lassen, werden alle Aufträge für das gewählte Liefer-
                                         datum in den Aktions-Dialog geladen.
                                         Technische Info: Auswahl-Feld <F9>, Numerisches Feld, DB-Info: lapool.rou-
                                         tenr

                                         Auftrag Nummer des Auftrags, für den Sie die Fehlmengenkontrolle durch-
                                         führen. Wenn Sie das Feld leer lassen, werden alle Aufträge für das gewählte
                                         Lieferdatum und die gewählte Route in den Aktions-Dialog geladen.
                                         Technische Info: Auswahl-Feld, Datumsformat, DB-Info: lapool.auftrnr

                                         Ladeliste Nummer der Ladeliste, für die Sie die Fehlmengenkontrolle durch-
                                         führen. Durch die Eingabe der Ladeliste-Nummer schränken Sie die Auswahl
2.00 / 04-2022




                                         mehr ein.
                                         Technische Info: Auswahl-Feld <F9>, Numerisches Feld, DB-Info: lapool.llnr




                 G-78                                                             A+W Enterprise Versandsteuerung
                 Softwarereferenz                                                         Funktionen im Versand




                                       [Auslösen] Über die Schaltfläche öffnen Sie den Dialog Fehlmengenkontrol-
                                       le.


                                       Ergänzende Information
                                        “Fehlmengenkontrolle - Aktion” auf Seite G-80
2.00 / 04-2022




                 A+W Enterprise Versandsteuerung                                                          G-79
                 Funktionen im Versand                                                                Softwarereferenz




                                          Fehlmengenkontrolle - Aktion
                                          Versandsteuerung – Datenebene > <F4> > Fehlmengenkontrolle > Auswahl
                                          treffen > [Auslösen]




                 Abb. G-33   Versandsteuerung – Ansicht Fehlmengenkontrolle


                                          In diesem Dialog führen Sie die Fehlmengenkontrolle durch. Beim Betreten
                                          des Dialoges ist die Spalte Verp. mit der Auftrags bzw. Positionsmenge belegt.
                                          Ist die Gesamtmenge nicht verfügbar, können Sie diese für den betroffenen
                                          Auftrag korrigieren. Die fehlende Menge wird automatisch in das Feld Rück.
                                          (Rückstand) geschrieben. Sie können die fehlende Menge auf ein anderes
                                          Datum oder eine andere Route anschließend verschieben.
                                          Die Vorauswahl führen Sie über den Suchdialog Fehlmengenkontrolle für...
                                          durch.
2.00 / 04-2022




                                           “Fehlmengenkontrolle - Auswahl” auf Seite G-78
                                          Die Felder in der Kopfzeile dienen zur Orientierung. Diese Felder geben Infor-
                                          mation darüber, wo Sie sich befinden.


                 G-80                                                               A+W Enterprise Versandsteuerung
                 Softwarereferenz                                                               Funktionen im Versand




                                       Alle Felder sind bereits in den vorherigen Kapiteln beschrieben:
                                        “Register – AuftragsInfo” auf Seite G-39
                                        “Register – PositionsInfo I” auf Seite G-57

                                       Verp. Verpackte Stückzahl. Wenn Sie die verpackte Stückzahl ändern, dann
                                       ändert sich auch der Wert im Feld Rückstand. Sie können die gesamte Posi-
                                       tion verschieben:
                                       Technische Info: Eingabe-Feld, Datumsformat, DB-Info: lapool.iststk
                                        “Verschiebung mehrerer Pos. - Aktion” auf Seite G-70

                                       Rück. Der Rückstand ist die Differenz der geplanten Stückzahl abzüglich der
                                       verpackten Stückzahl.
                                       Technische Info: Anzeige-Feld, Datumsformat, DB-Info: lapool.rueckstk
                                       Wenn die geplanten Einheiten zum geplanten Termin nicht zur Verfügung ste-
                                       hen, dann müssen Sie die ausstehenden Einheiten (Rückstand) auf einen an-
                                       deren Termin verschieben. Wenn Sie die Buchung auslösen, könne Sie die
                                       fehlende Menge als Rückstand verschieben:
                                        Verschiebung mehrerer Pos. - Aktion

                                       Datum Geplantes Versanddatum. Wenn Sie das Datum ändern, dann fragt
                                       A+W Enterprise, ob das Datum nach unten vererbt werden soll. Das bedeutet,
                                       dass alle in dem Dialog angezeigten Positionen zum geänderten Datum ver-
                                       sendet werden.
                                       Technische Info: Auswahl-Feld, Datumsformat, DB-Info: lapool.ltplan

                                       Buch. Markierungsfeld für die Buchungsdurchführung dieses Datensatzes.
                                       Technische Info: Checkbox

                                       Schaltflächen
                                       Wenn ein Rückstand vorhanden ist, dann muss die jeweilige Auftragsposition
                                       auf einen anderen Termin verschoben werden.
                                       Mit [Verschieben] öffnen Sie den Dialog Verschiebung.
                                        “Verschiebung mehrerer Pos. - Aktion” auf Seite G-70
                                       Mit [Buchen] speichern Sie die Änderungen. Die gewählte Position wird als
                                       verpackt gemeldet. Wenn die Positionsmenge komplett verpackt ist, wird der
                                       Status der Position auf kmp. (komplett) gesetzt.
                                        “Register – PositionsInfo I” auf Seite G-57
2.00 / 04-2022




                 A+W Enterprise Versandsteuerung                                                               G-81
                 Funktionen im Versand                                                               Softwarereferenz




                                         Buchen auf Transport
                                         Versandsteuerung – Datenebene > <F4> > Buchen auf Transport
                                         Komplett verpackte Positionen können Sie über diesen Menüpunkt auf Trans-
                                         port buchen. Die Buchung erfolgt im Hintergrund. Je nach Systemkonfigurati-
                                         on kann dabei auch ein Lieferschein erzeugt werden. Im Weiteren kann
                                         ebenfalls konfiguriert werden, ob die Buchungen auf Transport für die Vergan-
                                         genheit und/oder die Zukunft zulässig sind.
                                         Eine Transportbuchung führt zur entsprechenden Statusänderung:
                                          “Status zu Lieferpositionen” auf Seite G-73
                                         Die Buchungsergebnisse sehen Sie z. B. unter:
                                          “Protokoll” auf Seite G-129

                                            Transport buchen
                                            Diese Funktion ist separat konfigurierbar. Sprechen Sie dazu den A+W -
                                            Mitarbeiter an.
2.00 / 04-2022




                 G-82                                                                A+W Enterprise Versandsteuerung
                 Softwarereferenz                                                            Funktionen im Versand




                                       Transport zurückbuchen
                                       Versandsteuerung – Datenebene > <F4> >Transport rückbuchen




                                       Abb. G-34    Transportbuchung zurückholen für…


                                       In diesem Dialog wählen Sie einen Auftrag für die Transportrückbuchung. Die-
                                       se Aktion setzt voraus, dass eine Transportbuchung bereits stattgefunden
                                       war. Nachdem Sie die Transportbuchung zurückgebucht haben, können Sie
                                       einen neuen Vorablieferschein oder einen Lieferschein für die korrigierte Lie-
                                       fermenge erstellen.

                                       Lieferdat. Lieferdatum, für das die Transportbuchung zurückgebucht wird.
                                       Technische Info: Eingabe-Feld, Datumsformat, DB-Info: lapool.ltplan

                                       Haus Mandantennummer oder Hausnummer, für die die Transportbuchung
                                       zurückgebucht wird.
                                       Technische Info: Auswahl-Feld <F9>, Numerisches Feld, DB-Info: la-
                                       pool.hausnr

                                       Auftrag Auftragsnummer, für die die Transportbuchung zurückgebucht wird.
                                       Technische Info: Auswahl-Feld <F9>, Numerisches Feld, DB-Info: la-
                                       pool.auftrnr

                                       Via Haus Nummer des Hauses, über das Sie die Transportbuchung zurück-
                                       buchen.
                                       Technische Info: Auswahl-Feld <F9>, Numerisches Feld, DB-Info: la-
                                       pool.hausnr, lapool.viaflag

                                       [Auslösen] Über die Schaltfläche lösen Sie die Rückbuchung aus.
2.00 / 04-2022




                 A+W Enterprise Versandsteuerung                                                               G-83
                 Funktionen im Versand                                                                Softwarereferenz




                                         Barcode Gestellanzeige
                                         Versandsteuerung – Datenebene > <F4> > Barcode Gestellanzeige




                                         Abb. G-35    Barcode Gestellanzeige


                                         In diesem Dialog erhalten Sie Information zu den Gestell-Barcodes, wenn die-
                                         se bereits existieren. Die Information steht in der Datenbank-Tabelle bcbock.

                                         Auftrag Externe Auftragsnummer.
                                         Technische Info: Numerisches Feld, DB-Info: bcbock.auftrnr

                                         Pos Positionsnummer im Auftrag.
                                         Technische Info: Numerisches Feld, DB-Info: bcbock.posnr

                                         Gestell Gestellnummer, auf dem die Auftragsposition sich befindet. Wenn
                                         eine Auftragsposition gesplittet und auf mehrere Gestelle verteilt wird, sehen
                                         Sie in diesem Dialog alle Zuordnungen z.B.: Auftrag 4002466, Position 3.
                                         Technische Info: Numerisches Feld, DB-Info: bcbock.gnr

                                         Fach Fachnummer, falls die aktuelle Position sich in einem Fach befindet.
                                         Technische Info: Numerisches Feld, DB-Info: bcbock.subnr

                                         Stück Anzahl der Scheiben auf dem Gestell. Da pro Stück ein Datensatz in
                                         der Tabelle bcbock geschrieben wird, wird diese Menge für die jeweiligen Ge-
                                         stell summiert und hier angezeigt..
                                         Technische Info: Numerisches Feld, DB-Info: bcbock.anzahl

                                            Tabelle bcbock im Versand
                                            Die Bebuchung der Datenbanktabelle bcbock erfolgt nur dann, wenn die
                                            Funktion Freie Gestelle entsprechend konfiguriert ist. Sprechen Sie dazu
                                            den A+W - Mitarbeiter an.
2.00 / 04-2022




                 G-84                                                              A+W Enterprise Versandsteuerung
                 Softwarereferenz                                                               Funktionen im Versand




                                       Ergebnisse der Gestellplanung
                                       Versandsteuerung – Auftragsebene > <F4> > Ergebnisse der Gestellplanung




                                       Abb. G-36    Ergebnisse der Gestellplanung


                                       In diesem Dialog erhalten Sie die Information über die Gestellplanung.

                                          Datenbank-Tabellen für Gestellplanung
                                          Die Ergebnisse der Gestellplanung unterscheiden sich je nach vorhande-
                                          ner Systemkonfiguration. Wenn Sie die Funktion Freie Gestelle verwen-
                                          den, werden gestellbezogenen Daten in den Datenbank-Tabellen gest und
                                          gestzu nach der Rückmeldung aus A+W Production gebucht. Bei der Nut-
                                          zung anderer Konfigurationen werden die Tabellen kposgest oder bcbock
                                          verwendet. Aus diesem Grund ist die technische Info in den nachfolgenden
                                          Felder nicht immer aufgeführt. Für ausführliche Informationen zur Gestell-
                                          planung sprechen Sie bitte einen A+W - Mitarbeiter an.

                                       Folgende Felder werden in diesem Dialog angezeigt:

                                       Auftrag Auftragsnummer. Anzeige der Gestellplanung ist nur in der Auftrags-
                                       ebene möglich. Sie starten die Anzeige für einen bestimmten Auftrag.
                                       Technische Info: Anzeige-Feld, DB-Info: lapool.auftrnr

                                       Pos. Positionsnummer aus dem gewählten Auftrag.
                                       Technische Info: Anzeige-Feld, DB-Info: lapool.posnr

                                       Menge Positionsmenge, die auf dem aktuellen Gestell vorhanden ist.

                                       Total Gesamt-Positionsmenge.
                                       Technische Info: Anzeige-Feld, DB-Info: lapool.sollstk

                                       Gestell Gestellnummer.

                                       Typ Gestelltyp. Diese Bezeichnung wird aus den Stammdaten ermittelt.
                                       Technische Info: alphanummerisches Feld, DB-Info: gtyp.kurzbez

                                       Lieferdat Liefertermin für die aktuelle Auftragsposition.
                                       Technische Info: Anzeige-Feld, DB-Info: lapool.ltplan
2.00 / 04-2022




                                       Route Nummer der Auslieferungsroute.
                                       Technische Info: Anzeige-Feld, DB-Info: lapool.routennr



                 A+W Enterprise Versandsteuerung                                                                G-85
                 Funktionen im Versand                                                              Softwarereferenz




                                         Packmittelplanung
                                         Versandsteuerung – Auftragsebene > <F4> > Packmittelplanung




                                         Abb. G-37    Vorablieferschein für…


                                         In diesem Dialog bekommen Sie die Information über durchgeführte Packmit-
                                         telplanung.

                                            Packmittelplanung im A+W Enterprise
                                            Die Ergebnisse der Packmittelplanung sind von der Systemkonfiguration
                                            anhängig. Die Packmittelplanung aus der Auftragserfassung ist im folgen-
                                            den Part beschrieben:

                                             Verkauf, “Packmittelplanung” auf Seite D-234



                                            Kundenindividuelle Einstellungen
                                            Kundenindividuelle Einstellungen sind nicht Bestandteil dieser Dokumen-
                                            tation.
2.00 / 04-2022




                 G-86                                                               A+W Enterprise Versandsteuerung
                 Softwarereferenz                                                          Funktionen im Versand




                                       Lieferanschrift suchen
                                       Versandsteuerung – Auftragsebene > <F4> Lieferanschrift > Lieferanschrift
                                       suchen




                                       Abb. G-38    Adressen Suche


                                       In diesem Dialog können Sie eine Lieferadresse auswählen, soweit diese ge-
                                       ändert werden muss. Im Standardfall wird die Lieferadresse aus dem Auftrag
                                       in die Versandsteuerung übernommen. Die Funktion Adresse Suche ist auch
                                       in der Auftragserfassung verfügbar und auch dort beschrieben worden. Es
                                       werden alle Anschriften angezeigt, die zu dem Kunden aus dem aktuellen Auf-
                                       trag hinterlegt sind. Angezeigte Felder können je nach Systemkonfiguration
                                       teils abweichen. Über die Suchfelder filtern Sie eine gespeicherte Adresse.
                                        Verkauf, “Adressen Suche” auf Seite D-45
2.00 / 04-2022




                 A+W Enterprise Versandsteuerung                                                            G-87
                 Funktionen im Versand                                                              Softwarereferenz




                                         Neue Lieferanschrift
                                         Versandsteuerung – Auftragsebene > <F4> Lieferanschrift > Neue Lieferan-
                                         schrift




                                         Abb. G-39    Lieferanschrift


                                         In diesem Dialog erfassen Sie eine neue Lieferadresse, wenn keine Adresse
                                         gefunden werden konnte. Mit [OK] wird die Anschrift nur für diese Lieferung
                                         gespeichert. Mit <F3> schreiben Sie die neue Adresse in die Stammdaten.
                                         Die Felder zum Dialog sind im folgenden Kapitel beschrieben:
                                          Verkauf, “Neue Lieferadresse” auf Seite D-136
2.00 / 04-2022




                 G-88                                                               A+W Enterprise Versandsteuerung
                 Softwarereferenz                                                           Funktionen im Versand




                                       Gestellinformationen
                                       Versandsteuerung – Auftragsebene > <F4> Gestellinformationen




                                       Abb. G-40   Gestellinformationen


                                       In diesem Dialog kann kundenindividuell eingerichtet werden, ob und welche
                                       Gestellinformation ausgegeben werden kann.
                                       Der Zutritt zu dem Dialog wird mit der Umgebungsvariable SQL_GEST_INFO
                                       aktiviert. In dieser Variable werden die GruppeID und die SQL-Nummer hinter-
                                       legt, die die ausgegebenen Sprache, Felder und Bedienungen steuert. Die
                                       o. g. Abbildung dient nur der Veranschaulichung und wird in diesem Doku-
                                       ment nicht näher beschrieben.
2.00 / 04-2022




                 A+W Enterprise Versandsteuerung                                                             G-89
                 Funktionen im Versand                                                               Softwarereferenz




                                         Toursperre setzen/löschen
                                         Versandsteuerung – Tourenebene > <Shift> + <F4> Toursperre setzen/lö-
                                         schen




                                         Abb. G-41    Eine der Meldungen zur Tourensperre


                                         Mit dieser Funktion sperren Sie entweder die markierte Tour oder Sie entsper-
                                         ren die markierte Tour wieder. Eine Tour ist eine Route, die an einem bestimm-
                                         ten Liefertermin gefahren wird.
                                         Eine Tour wird gesperrt, wenn sie verplant ist und keine weiteren Aufträge
                                         mehr aufnehmen soll.
                                         Für die zu sperrende Tour muss eine Ausweichroute in den Stammdaten an-
                                         gelegt sein. Wenn nach der Tourensperre ein neuer Vorgang in der Auftrags-
                                         erfassung für diese gesperrte Tour gebucht wird, dann wird der neue Vorgang
                                         automatisch auf die Ausweichroute gebucht.
                                         Die Routensperre wird nur gesetzt, wenn ein Auftrag der Route von einem an-
                                         deren Haus oder Mandanten auf Transport gebucht wird.
                                         Wenn eine Toursperre gesetzt ist, dann ist das Feld TS (Tourstatus) mit dem
                                         Status Tour gesperrt (Tooltipp: rot) markiert.
                                          “Alle Touren sperren” auf Seite G-91
                                          “Routenstatus” auf Seite G-29
2.00 / 04-2022




                 G-90                                                              A+W Enterprise Versandsteuerung
                 Softwarereferenz                                                            Funktionen im Versand




                                       Alle Touren sperren
                                       Versandsteuerung – Tourenebene > <Shift> + <F4> alle Touren sperren




                                       Abb. G-42    Ergebnis der Tourensperre


                                       Mit dieser Funktion sperren Sie alle im Register angezeigten Touren.
                                       Touren werden gesperrt, wenn sie verplant sind und keine weiteren Aufträge
                                       mehr aufnehmen sollen.
                                       Für die zu sperrenden Touren müssen Ausweichrouten in den Stammdaten
                                       angelegt sein. Wenn nach der Tourensperre ein neuer Vorgang in der Auf-
                                       tragserfassung für eine der gesperrten Touren erfolgt, dann wird der neue Vor-
                                       gang automatisch auf die Ausweichroute verplant.
                                       Wenn alle Touren gesperrt sind, dann werden alle Felder TS (Tourstatus) mit
                                       dem Status Tour gesperrt (Tooltipp: rot) markiert.
                                        “Routenstatus” auf Seite G-29
2.00 / 04-2022




                 A+W Enterprise Versandsteuerung                                                               G-91
                 Funktionen im Versand                                                                Softwarereferenz




                                         Transportdaten
                                         Versandsteuerung – Tourenebene > <Shift> + <F4> > Transportdaten




                                         Abb. G-43    Transportdaten


                                         In diesem Dialog hinterlegen Sie die Transportdaten für die aktuell Tour. Sie
                                         können Transportdaten sowohl für Aufträge als auch für Einkaufsvorgänge er-
                                         fassen, sofern Sie die Einkaufsvorgänge in der Versandsteuerung konfiguriert
                                         haben.
                                          “Versandsteuerung – Menüs” auf Seite G-22

                                         Route Nummer der Route, für die die Transportdaten hinterlegt werden.
                                         Technische Info: Anzeige-Feld, DB-Feld: lapool.routennr

                                         Fahrer Name des Fahrers für die Tour. Die Mitarbeiter werden in den Stamm-
                                         daten hinterlegt.
                                         Technische Info: Auswahl-Feld, Numerisches Feld, DB-Feld: mitarb.manr

                                         Kfz Kfz für die Tour. Die Fahrzeuge werden in den Stammdaten hinterlegt.
                                         Technische Info: Auswahl-Feld, Numerisches Feld, DB-Feld: lkw.lkw.nr

                                         Anhänger Zwei Felder zur Eingabe von Anhängern für den Transport. Die
                                         Anhänger oder Auflieger werden in den Stammdaten hinterlegt.
                                         Technische Info: Auswahl-Feld, Numerisches Feld, DB-Feld: lkw.lkw.nr
                                         Die Einstellung speichern Sie mit <Ende>.
                                         Die erfasste Transportdaten werden in dem Register FahrzeugInfo angezeigt:
                                          “Register – FahrzeugInfo” auf Seite G-34
2.00 / 04-2022




                 G-92                                                                 A+W Enterprise Versandsteuerung
                 Softwarereferenz                                                         Funktionen im Versand




                                       Lagerkommissionierung
                                       Versandsteuerung – Tourenebene > <Shift> + <F4> Lagerkommissionierung




                                       Abb. G-44   Meldung zum Kommissionierdruck


                                       In diesem Dialog sehen Sie die Nummer des Kommissionierdrucks. Für La-
                                       gerware wird mit dieser Funktion die Kommissionierung oder die Lagerabbu-
                                       chung ausgelöst. Diese Funktion wird kundenindividuell konfiguriert.
2.00 / 04-2022




                 A+W Enterprise Versandsteuerung                                                          G-93
                 Storno                                                                Softwarereferenz




                          Storno
                          Versandsteuerung – Auftragsebene > <Shift> + <F4> > Storno
                          Unter dem Menü Storno sind folgende Dialoge verfügbar:
                           “Lieferscheinstorno” auf Seite G-94
                           “Auftragsstorno” auf Seite G-95
                           “Wareneingangsstorno” auf Seite G-96
                           “Storno des Versandstatus” auf Seite G-97
                          Ein Liefereingang innerhalb der via-plant Konfiguration kann in folgenden Di-
                          alog storniert werden:
                           “Storno des Liefereingangs” auf Seite G-77



                          Lieferscheinstorno
                          Versandsteuerung – Auftragsebene > <Shift> + <F4> > Storno > Lieferschein-
                          storno




                          Abb. G-45    Lieferscheinstorno


                          In diesem Dialog stornieren Sie bereits erstellte Lieferscheine. Die Kennzeich-
                          nung im Register Auftragsinfo im Feld LS (Lieferschein) wechselt in den Status
                          auf Transport gebucht (Tooltipp: gelb). Der Status S des Auftrags wechselt in
                          den Status auf Transport (Tooltipp: halb blau).
                          Bevor Sie das Storno auslösen, werden im Dialog die Auftragsdaten, den Sie
                          stornieren, angezeigt.

                          Lieferdatum Lieferdatum, an dem der Auftrag zum Kunden geliefert werden
                          soll.
                          Technische Info: Anzeige-Feld, DB-Feld: lapool.ltplan

                          Route Nummer der Route.
                          Technische Info: Anzeige-Feld, DB-Feld: lapool.routennr

                          Auftrag Auftragsnummer des zu stornierenden Lieferscheins.
                          Technische Info: Anzeige-Feld, DB-Feld: lapool.auftrnr
2.00 / 04-2022




                 G-94                                                A+W Enterprise Versandsteuerung
                 Softwarereferenz                                                                           Storno




                                       Auftragsstorno
                                       Versandsteuerung – Auftragsebene > <Shift> + <F4> > Storno
                                       > Auftragsstorno




                                       Abb. G-46    Auftragsstorno


                                       In diesem Dialog können Sie einen Auftrag stornieren. In der Regeln werden
                                       Aufträge im Bereich Verkauf storniert, da der Logistik-Mitarbeiter unter Um-
                                       ständen nicht über die nötige Verkaufs-Information verfügt. Beim Auftrags-
                                       Storno im Versand kann es zu Daten-Inkonsistenz kommen, falls der Auftrag
                                       bereits in der Produktion ist und sich im Status Lokal-Korrektur befindet.

                                       Auftrag Auftragsnummer des zu stornierenden Auftrags.
                                       Technische Info: Anzeige-Feld, DB-Feld: lapool.auftrnr

                                       Stornoinfo Informationstext für den stornierten Auftrag. Maximale Länge die-
                                       ses Textes ist 60 Zeichen.
                                       Technische Info: Alphanumerisches Feld, DB-Info: kauf.exbez2
                                       Mit <Auslösen> führen Sie die Aktion aus. Je nach Auftragsstatus kann das
                                       Programm eine Sicherheitsabfrage mit einer Statusanzeige ausgeben oder
                                       die Aktion ablehnen. Wenn Sie den Auftrag trotzdem stornieren, müssen Sie
                                       in darauffolgenden Dialog den Stornogrund eingeben. Dieser Grund wird beim
                                       Auftragsaufruf dem Benutzer im Vordergrund angezeigt.


                                       Ergänzende Informationen
                                        Verkauf, “Storno” auf Seite D-143
2.00 / 04-2022




                 A+W Enterprise Versandsteuerung                                                             G-95
                 Storno                                                             Softwarereferenz




                          Wareneingangsstorno
                          Versandsteuerung – Auftragsebene > <Shift> + <F4> > Storno
                          > Wareneingangsstorno > [Auslösen]




                          Abb. G-47   Stornoinfo


                          In diesem Dialog können Sie einen Wareneingang stornieren. Dieses Menü-
                          punkt kann nur bei Versandmodus für Einkaufsvorgängen aufgerufen werden.
                          Bevor Sie den Storno auslösen, werden im Dialog die Daten des Warenein-
                          gangs, den Sie stornieren, angezeigt.

                          Lieferdatum Lieferdatum, an dem der Wareneingang eingetroffen werden
                          soll.
                          Technische Info: Anzeige-Feld, DB-Info: lapool.ltplan

                          Route Nummer der Route.
                          Technische Info: Anzeige-Feld, DB-Info: lapool.routennr

                          Auftrag Nummer der Bestellung, zu der der Wareneingang storniert werden
                          soll.
                          Technische Info: Anzeige-Feld, DB-Info: lapool.auftrnr, lapool.vorgang=2

                          Stornoinfo Informationstext für den stornierten Wareneingang. Maximale
                          Länge dieses Textes ist 60 Zeichen.
                          Technische Info: Alphanumerisches Feld, DB-Info: kauf.exbez2
2.00 / 04-2022




                 G-96                                              A+W Enterprise Versandsteuerung
                 Softwarereferenz                                                                             Storno




                                       Storno des Versandstatus
                                       Versandsteuerung – Datenebene <Shift> + <F4> > Storno >
                                       Storno des Versandstatus




                                       Abb. G-48    Meldung zum Storno des Versandstatus


                                       Mit dieser Funktion stornieren Sie den Versandstatus. Der Versandstatus ei-
                                       nes Auftrags wird von der Versandsteuerung automatisch auf den Status
                                       Verplant gesetzt, wenn in der Versansteuerung ein Auftrag z. B. auf einen an-
                                       deren Liefertermin verschoben wird. Nach der Stornierung des Versandstatus
                                       kann der Auftrag wieder uneingeschränkt von der Auftragserfassung verän-
                                       dert werden.
                                       Der Mitarbeiter in der Versandplanung muss mit der Auftragserfassung Rück-
                                       sprache halten, wenn der Auftrag noch nicht in Produktion gegangen ist. Das
                                       hat die folgenden Gründe:
                                       •   Wenn die Auftragserfassung einen Auftrag anlegt oder ändert, dann wer-
                                           den die Daten an die Produktion übermittelt. Die Produktion fertigt danach
                                           den Auftrag zum angegebenen Liefertermin.
                                       •   Wenn die Versandsteuerung einen freigegebenen Auftrag verschiebt, dann
                                           wird diese Verschiebung nicht automatisch an die Produktion weitergege-
                                           ben.
2.00 / 04-2022




                 A+W Enterprise Versandsteuerung                                                               G-97
                 Gestelle                                                               Softwarereferenz




                            Gestelle
                            Glasscheiben werden in der Regeln bereits in der Produktion auf Gestellen
                            abgestellt und so weiter transportiert. Diese Gestelle können auch in der Ver-
                            sandsteuerung weiter verwaltet werden.
                            Die Nutzung der Gestellplanung bzw. der Gestellverwaltung ist kundenindivi-
                            duell, sodass nicht alle Funktionen und Dialoge im kompletten Umfang verfüg-
                            bar sind. Für zusätzliche Information über die Gestelle in der
                            Versandsteuerung sprechen Sie bitte den A+W - Mitarbeiter an.
                            Im Folgenden werden Dialoge, die über <Shift> + <F4> > Gestelle erreichbar
                            sind, beschrieben:
                             “Gestellzuordnung - Auswahl” auf Seite G-99
                             “Gestellzuordnung - Anzeige” auf Seite G-100
                             “Gestellauflösung - Auswahl” auf Seite G-102
                             “Gestellauflösung - Anzeige” auf Seite G-102
                             “Freie Gestelle (Übersicht)” auf Seite G-104
                             “Gebuchte Gestelle (Übersicht)” auf Seite G-106
                             “Alle Gestelle (Übersicht)” auf Seite G-107
                             “Einzelne Gestelle” auf Seite G-109
                             “Gestelle zu Auftrag” auf Seite G-110
                             “Scheibenzuordnung” auf Seite G-112
2.00 / 04-2022




                 G-98                                                  A+W Enterprise Versandsteuerung
                 Softwarereferenz                                                                            Gestelle




                                       Gestellzuordnung - Auswahl
                                       Versandsteuerung – Datenebene <Shift> + <F4> > Gestelle > Gestellzuord-
                                       nung




                                       Abb. G-49    Auswahldialog Gestellzuordnung


                                       In diesem Dialog suchen Sie nach einem Auftrag, zu dem Sie die Gestellzu-
                                       ordnung ansehen möchten. Der hier gewählte Auftrag muss bereits auf einem
                                       oder mehreren Gestellen verplant sein.

                                       Haus Hausnummer, in der Sie im Versand arbeiten.
                                       Technische Info: Anzeige-Feld, DB-Info: lapool.hausnr

                                       Lieferdat Liefertermin, dessen Daten Sie im Versand bearbeiten.
                                       Technische Info: Auswahl-Feld, Datum-Format, DB-Info: lapool.ltplan

                                       Route Routennummer, deren Daten Sie im Versand bearbeiten.
                                       Technische Info: Auswahl-Feld <F9>, DB-Info: lapool.routennr

                                       Auftrag Auftragsnummer des zu bearbeitenden Auftrags. Die Auftragsaus-
                                       wahl ist mit <F9> möglich. Im Feld dahinter wird der entsprechende Versand-
                                       Modus angezeigt.
                                       Technische Info: Numerisches Feld, DB-Info: lapool.auftrnr

                                       Ladeliste Ladelistenummer, falls zu dem Auftrag bereits eine Ladeliste ge-
                                       druckt wurde.
                                       Technische Info: Anzeige-Feld, DB-Info: lapool.llnr
                                       Mit [Auslösen] laden Sie die Gestell-Daten zu dem gewählten Auftrag. Die Er-
                                       gebnisse der Anzeigen sind im folgenden Dialog beschrieben:
                                        “Gestellzuordnung - Anzeige” auf Seite G-100
2.00 / 04-2022




                 A+W Enterprise Versandsteuerung                                                               G-99
                 Gestelle                                                                Softwarereferenz




                            Gestellzuordnung - Anzeige
                            Versandsteuerung – Datenebene <Shift> + <F4> > Gestelle > Gestellzuord-
                            nung, Auswahl getroffen




                            Abb. G-50    Gestellzuordnung


                            In diesem Dialog sehen Sie die Gestellzuordnung zu dem gewählten Auftrag.
                            Die Gestellzuordnung erfolgt in A+W Production, indem die Auftragspositio-
                            nen auf Gestelle verpackt und außer Haus gemeldet werden. Zusätzlich kann
                            auch eine Tourenzuordnung stattfinden. Die Ergebnisse der Rückmeldung se-
                            hen Sie in diesem Dialog.
                            Der Dialogtitel wird dynamisch aufgebaut, so dass Sie bereits im Titel das Lie-
                            ferdatum und die Route sehen, auf die Ihr Auftrag geplant ist.

                            Kmp Komplett-Kennzeichen für die aktuelle Auftragsposition auf dem Ge-
                            stell. Das Kennzeichen wird gesetzt, wenn die gesamte Positionsmenge be-
                            reits auf die Gestelle zugeordnet ist.
                            Technische Info: Anzeige-Feld

                            Gestell Gestellnummer, auf dem sich die aktuelle Auftragsposition befindet.
                            Technische Info: Anzeige-Feld, DB-Feld: gest.exgnr

                            GeTyp Gestelltyp der aktuellen Gestellnummer aus den Gestell-Stammda-
                            ten.
                            Technische Info: Anzeige-Feld, DB-Feld: gest.exgnr

                            Auftrag Aktuelle Auftragsnummer.
                            Technische Info: Anzeige-Feld, DB-Feld: lapool.auftrnr, gestzu.auftrnr

                            Pos Positionsnummer des gewählten Auftrags.
                            Technische Info: Anzeige-Feld, DB-Feld: lapool.posnr

                            Artikel Artikelbezeichnung aus den Stammdaten.
2.00 / 04-2022




                            Technische Info: Anzeige-Feld, DB-Feld: artikel.artbez1

                            Ges. Gesamt-Stückzahl der Position.



                 G-100                                                A+W Enterprise Versandsteuerung
                 Softwarereferenz                                                                             Gestelle




                                       Abruf Bereits abgerufene Stückzahl der Position.

                                       Breite Breite der Scheibe aus der Position.
                                       Technische Info: Numerisches Feld, DB-Feld: lapool.laenge

                                       Länge Höhe der Scheibe aus der Position.
                                       Technische Info: Numerisches Feld, DB-Feld: lapool.breite

                                       Auf Gestell Stückzahl, die sich auf dem Gestell befindet.

                                       Buch. Checkbox für die Buchung.
                                        Position wird zum Buchen markiert.
                                        Position wird nicht verbucht.
                                       Mit [Alle] markieren Sie alle Gestellsätze im Dialog, um weitere Aktion zu star-
                                       ten.
                                       Mit [Auslösen] speichern Sie die Gestellzuordnung, falls Sie diese in dem Di-
                                       alog manuell vornehmen müssen.
2.00 / 04-2022




                 A+W Enterprise Versandsteuerung                                                               G-101
                 Gestelle                                                             Softwarereferenz




                            Gestellauflösung - Auswahl
                            Versandsteuerung – Datenebene <Shift> + <F4> > Gestelle > Gestellauflö-
                            sung




                            Abb. G-51    Auswahldialog Gestellauflösung


                            In diesem Dialog wählen Sie, für welchen Liefertermin und Route Sie die Ge-
                            stellauflösung durchführen möchten.
                            Die Auswahl-Felder sind identisch mit denen in der Gestellzuordnung:
                             “Gestellzuordnung - Auswahl” auf Seite G-99



                            Gestellauflösung - Anzeige
                            Versandsteuerung – Datenebene <Shift> + <F4> > Gestelle > Gestellauflö-
                            sung, Auswahl getroffen




                            Abb. G-52    Dialog Gestellauflösung


                            In diesem Dialog lösen Sie die Gestellzuordnung aus. Wenn Sie die Gestelle
                            zur Bearbeitung markieren (Spalte Frei) und die Aktion durchführen, wird die
                            Zuordnung zur Route und zum Liefertermin aufgelöst und die verpackte Stück-
                            zahlen wieder entpackt. Anschließend kann eine neue Gestell-BDE-Buchung
2.00 / 04-2022




                            erfolgen, sofern alle Kriterien für die neue Buchung erfüllt sind.




                 G-102                                                A+W Enterprise Versandsteuerung
                 Softwarereferenz                                                                               Gestelle




                                          Gestellbuchungen per BDE in der Versandsteuerung
                                          Die Funktion Gestellbuchungen per BDE muss in Ihren System entspre-
                                          chend konfiguriert werden. Bitte sprechen Sie bei bestehendem Interesse
                                          den zuständigen A+W - Mitarbeiter an.

                                       Gestell Gestellnummer, auf dem sich die aktuelle Auftragsposition befindet.
                                       Technische Info: Anzeige-Feld, DB-Info: gest.exgnr

                                       GeTyp Gestelltyp (Bezeichnung) der aktuellen Gestellnummer aus den Ge-
                                       stell-Stammdaten.
                                       Technische Info: Anzeige-Feld, DB-Info: gest.gtypnr, gtyp.kurzbez

                                       Auftrag Aktuelle Auftragsnummer.
                                       Technische Info: Anzeige-Feld, DB-Info: lapool.auftrnr, gestzu.auftrnr

                                       Pos Positionsnummer des gewählten Auftrags.
                                       Technische Info: Anzeige-Feld, DB-Info: lapool.posnr, gestzu.posnr

                                       Artikel Artikelbezeichnung aus den Stammdaten.
                                       Technische Info: Anzeige-Feld, DB-Info: artikel.artbez1

                                       Ges. Gesamt-Stückzahl.
                                       Technische Info: Anzeige-Feld, DB-Info: lapool.geststk

                                       Breite Breite der Scheibe aus der Position.
                                       Technische Info: Anzeige-Feld, DB-Feld: lapool.laenge

                                       Länge Höhe der Scheibe aus der Position.
                                       Technische Info: Anzeige-Feld, DB-Feld: lapool.breite

                                       Auf Gest. Stückzahl, die sich auf dem Gestell befindet.
                                       Technische Info: Anzeige-Feld, DB-Info: gestzu.menge

                                       Frei Checkbox für das Markieren.
                                        Position wird zum Buchen markiert.
                                        Position wird nicht verbucht.
                                       Wenn Sie die Buchung [Auslösen] werden Sie zuerst gefragt, ob die bestehen-
                                       de Gestellzuordnung tatsächlich gelöscht und die verpackte Menge wieder
                                       entpackt werden soll.
                                       Mit [Alle] markieren Sie alle Gestellsätze im Dialog, um weitere Aktionen zu
                                       starten.
                                       Mit [Auslösen] lösen Sie die Gestellzuordnung auf.
2.00 / 04-2022




                 A+W Enterprise Versandsteuerung                                                                 G-103
                 Gestelle                                                                Softwarereferenz




                            Freie Gestelle (Übersicht)
                            Versandsteuerung – Datenebene <Shift> + <F4> > Gestelle > Freie Gestelle
                            (Übersicht)




                            Abb. G-53    Dialog Freie Gestelle (Tourenübersicht)


                            In diesem Dialog bekommen Sie Information über freie Gestelle auf der aktu-
                            ellen Tour. Beim Betreten des Dialoges wird geprüft, ob zu dem gewünschten
                            Liefertermin und Tour komplette Gestelle vorhanden sind. Ist das nicht der
                            Fall, haben Sie die Möglichkeit, sich alle Gestelle zu dieser Tour anzeigen zu
                            lassen.

                            Kmp Komplett-Kennzeichen für die aktuelle Auftragsposition auf dem Ge-
                            stell. Das Fragezeichen weist darauf hin, dass die Position noch nicht komplett
                            verfügbar ist.
                            Technische Info: Anzeige-Feld

                            Gestell Gestellnummer, auf dem sich die aktuelle Auftragsposition befindet.
                            Technische Info: Anzeige-Feld, DB-Info: gest.exgnr

                            Auftrag Auftragsnummer auf dieser Tour.
                            Technische Info: Anzeige-Feld, DB-Info: lapool.auftrnr, gestzu.auftrnr

                            Pos Positionsnummer des gewählten Auftrags.
                            Technische Info: Anzeige-Feld, DB-Info: lapool.posnr, gestzu.posnr

                            Artikel Artikelbezeichnung aus den Stammdaten.
                            Technische Info: Anzeige-Feld, DB-Info: artikel.artbez1

                            Ges. Gesamt-Stückzahl.
                            Technische Info: Anzeige-Feld, DB-Info: lapool.gesstk

                            Gepl. Geplante Stückzahl.
2.00 / 04-2022




                            Technische Info: Anzeige-Feld, DB-Info: lapool.sollstk




                 G-104                                                  A+W Enterprise Versandsteuerung
                 Softwarereferenz                                                                        Gestelle




                                       Abruf Abgerufene Stückzahl.
                                       Technische Info: Anzeige-Feld, DB-Info: lapool.abrufstk

                                       Auf Gest. Stückzahl, die sich dem Gestell befindet.
                                       Technische Info: Anzeige-Feld, DB-Info: gestzu.menge

                                       Breite Breite der Scheibe aus der Position.
                                       Technische Info: Anzeige-Feld, DB-Feld: lapool.laenge

                                       Länge Höhe der Scheibe aus der Position.
                                       Technische Info: Anzeige-Feld, DB-Feld: lapool.breite
                                       Mit [Gestell] starten Sie den Dialog Scheibenzuordnung für das ausgewählte
                                       Gestell:
                                        “Scheibenzuordnung” auf Seite G-112
2.00 / 04-2022




                 A+W Enterprise Versandsteuerung                                                          G-105
                 Gestelle                                                               Softwarereferenz




                            Gebuchte Gestelle (Übersicht)
                            Versandsteuerung – Datenebene <Shift> + <F4> > Gestelle > Gebuchte Ge-
                            stelle (Übersicht)




                            Abb. G-54    Dialog gebuchte Gestelle (Tourenübersicht)


                            In diesem Dialog werden alle gebuchte Gestelle für die aktuelle Tour ange-
                            zeigt. Sie können die gewünschten (markierten) Gestelle in diesem Dialog auf
                            eine andere Tour verschieben.

                            Buch. Checkbox für die Buchung. Markieren Sie die gewünschte Position,
                            um anschließend die Verschiebung (Schaltfläche [Verschieben]) durchzufüh-
                            ren.In dem Dialog Verschieben werden die Daten mit der aktuellen Tour vor-
                            belegt und können dann geändert werden. Wird eine abweichende Tour
                            eingetragen, werden alle Gestellmengen verschoben und auch Gestelle fest
                            umgebucht. Hier wird immer die verpackte Menge verschoben, auch wenn die
                            Verschiebung auf einen früheren Termin stattfindet.
                            In dem Dialog werden die gleiche Felder angezeigt, wie in dem Dialog zur frei-
                            en Gestellen:
                             “Freie Gestelle (Übersicht)” auf Seite G-104
                            Folgende Schaltflächen können Sie in dem Dialog verwenden:
                            •   [Verschieben]/<F3>
                                 “Verschieben” auf Seite G-66
                            •   [Gestell]/<F5>
                                 “Scheibenzuordnung” auf Seite G-112
                            •   [Summe]/<Shift> + <F9>
                                Es wird die Summe aller Glasscheiben pro Gestell gebildet und im Dialog
                                angezeigt.
                            •   [Alle/Komplette]/<Shift> + <F8>
                                Wenn in dem Dialog freie und komplette Gestelle angezeigt werden, so
2.00 / 04-2022




                                können Sie die Anzeige auf alle bzw. komplette einschränken.




                 G-106                                                  A+W Enterprise Versandsteuerung
                 Softwarereferenz                                                                               Gestelle




                                       Alle Gestelle (Übersicht)
                                       Versandsteuerung – Datenebene <Shift> + <F4> > Gestelle > Alle Gestelle
                                       (Übersicht)




                                       Abb. G-55    Dialog Alle Gestelle (Tourenübersicht)


                                       In diesem Dialog bekommen Sie die gesamte Gestellübersicht für den aktuel-
                                       len Auftrag. Über die Schaltfläche [Gestell] können Sie die Gestellmengen um-
                                       buchen:
                                        “Scheibenzuordnung” auf Seite G-112
                                       Folgende Felder werden in diesem Dialog angezeigt:

                                       Kmp Komplett-Kennzeichen für die aktuelle Auftragsposition auf dem Ge-
                                       stell.
                                          • Das Fragezeichen ? weist darauf hin, dass die Position noch nicht kom-
                                              plett verfügbar ist.
                                          • Ein Sternchen * zeigt an, dass die Position komplett ist.
                                          • Leeres Feld zeigt an, dass die Position noch nicht verpackt ist.

                                       Gestell Gestellnummer, auf dem sich die aktuelle Auftragsposition befindet.
                                       Technische Info: Anzeige-Feld, DB-Info: gest.exgnr

                                       Auftrag Auftragsnummer auf dieser Tour.
                                       Technische Info: Anzeige-Feld, DB-Info: lapool.auftrnr, gestzu.auftrnr

                                       Pos Positionsnummer des gewählten Auftrags.
                                       Technische Info: Anzeige-Feld, DB-Info: lapool.posnr, gestzu.posnr

                                       Artikel Artikelbezeichnung aus den Stammdaten.
                                       Technische Info: Anzeige-Feld, DB-Info: artikel.artbez1

                                       Ges. Gesamt-Stückzahl.
                                       Technische Info: Anzeige-Feld, DB-Info: lapool.gesstk
2.00 / 04-2022




                                       Gepl. Geplante Stückzahl.
                                       Technische Info: Anzeige-Feld, DB-Info: lapool.sollstk


                 A+W Enterprise Versandsteuerung                                                                 G-107
                 Gestelle                                                               Softwarereferenz




                            Verp. Abgerufene Stückzahl.
                            Technische Info: Anzeige-Feld, DB-Info: lapool.iststk

                            Auf Gest. Stückzahl, die sich auf dem Gestell befindet.
                            Technische Info: Anzeige-Feld, DB-Info: gestzu.menge

                            Breite Breite der Scheibe aus der Position.
                            Technische Info: Anzeige-Feld, DB-Feld: lapool.laenge.

                            Länge Höhe der Scheibe aus der Position.
                            Technische Info: Anzeige-Feld, DB-Feld: lapool.breite.

                            Lieferdat Liefertermin, zu dem das Gestell bereits fest zugeordnet ist.
                            Technische Info: Anzeige-Feld, DB-Info: gest.mdat

                            Route Routennummer, zu der das Gestell fest zugeordnet ist.
                            Technische Info: Anzeige-Feld, DB-Info: gest.routnr

                               Scheiben-Gestellzuordnung per BDE-Meldung
                               Bei der Zuordnung von Scheiben zu Gestellen per BDE-Meldung ist keine
                               feste Zuordnung möglich, wenn die gemeldeten Mengen nicht zu den Da-
                               ten im Versand passen. So bleiben diese Gestelle als freie Gestelle im Sys-
                               tem. Wenn eine feste Zuordnung zu einer Tour nicht möglich ist, weil die
                               Mengen im Versand auf unterschiedlichen Touren liegen, so können Sie
                               aus dieser Ansicht die Versandmenge aus den einzelnen Gestellen zusam-
                               menziehen, um anschließend die Zuordnung durchzuführen.
                               Voraussetzung: Die Touren, von welchen die Mengen auf die gewünschte
                               Tour verschoben werden, sind von keinem anderen Benutzer gesperrt.
2.00 / 04-2022




                 G-108                                                A+W Enterprise Versandsteuerung
                 Softwarereferenz                                                                        Gestelle




                                       Einzelne Gestelle
                                       Versandsteuerung – Datenebene <Shift> + <F4> > Gestelle > Einzelne Ge-
                                       stelle




                                       Abb. G-56   Einzelne Gestelle


                                       Über diesen Menüpunkt können Sie komplette Informationen zu einem Gestell
                                       abrufen. In dem Auswahl-Dialog wählen Sie die gewünschte Gestellnummer
                                       über <F9> oder geben Sie diese manuell ein. Mit [Auslösen] starten Sie die
                                       Scheiben-Gestellzuordnung. Die Felder zu dem Dialog Scheiben-Gestellzu-
                                       ordnung sind im folgenden Kapitel beschrieben:
                                        “Scheibenzuordnung” auf Seite G-112

                                       Gestelle Name des Gestells, zu dem die Information ermittelt werden soll.
                                       Technische Info: Auswahl-Feld, <F9> alphanumerisch, DB-Feld: gest.exgnr
2.00 / 04-2022




                 A+W Enterprise Versandsteuerung                                                           G-109
                 Gestelle                                                              Softwarereferenz




                            Gestelle zu Auftrag
                            Versandsteuerung – Datenebene <Shift> + <F4> > Gestelle > Gestelle zu Auf-
                            trag




                            Abb. G-57   Gestellsicht zum Auftrag


                            Über diesen Menüpunkt können Sie komplette Gestell-Informationen zu ei-
                            nem Auftrag abrufen. In dem Auswahl-Dialog wählen Sie die gewünschte Auf-
                            tragsnummer über <F9> oder geben diese manuell ein.
                            Mit der Schaltfläche [Auslösen] bekommen Sie die Gestellübersicht zu dem
                            gewählten Auftrag angezeigt.
                            Mit der Schaltfläche [Gestell] starten Sie die Scheiben-Gestellzuordnung.
                            Die Felder zu dem Dialog Scheiben-Gestellzuordnung sind im folgenden Ka-
                            pitel beschrieben:
                             “Scheibenzuordnung” auf Seite G-112

                            Gestelle Nummer des Gestells, zu dem die Information ermittelt werden soll.
                            Diese Nummer wird anschließend in den Dialog Gestellsicht zum Auftrag
                            übernommen und im Feld Gestell angezeigt.
                            Technische Info: Auswahl-Feld, <F9> alphanumerisch, DB-Feld: gest.exgnr

                            Auftrag Nummer des Auftrags, zu dem die Vorgänge aufgelistet werden.
                            Technische Info: Anzeige-Feld, DB-Feld: lapool.auftrnr, gestzu.auftrnr

                            Pos Positionsnummer des gewählten Auftrags.
2.00 / 04-2022




                            Technische Info: Anzeige-Feld, DB-Feld: lapool.posnr, gestzu.posnr

                            Artikel Artikelbezeichnung aus den Stammdaten.
                            Technische Info: Anzeige-Feld, DB-Feld: artikel.artbez1

                 G-110                                               A+W Enterprise Versandsteuerung
                 Softwarereferenz                                                                           Gestelle




                                       Gesamt Gesamt-Stückzahl.
                                       Technische Info: Anzeige-Feld, DB-Feld: lapool.gesstk

                                       Lieferdat Liefertermin, zu dem das Gestell bereits fest zugeordnet ist.
                                       Technische Info: Anzeige-Feld, DB-Info: gest.mdat

                                       Route Routennummer, zu der das Gestell fest zugeordnet ist.
                                       Technische Info: Anzeige-Feld, DB-Info: gest.routnr

                                       Stück Stückzahl, die sich dem Gestell befindet.
                                       Technische Info: Anzeige-Feld, DB-Info: gestzu.menge

                                       Breite Breite der Scheibe aus der Position.
                                       Technische Info: Anzeige-Feld, DB-Feld: lapool.laenge.

                                       Länge Höhe der Scheibe aus der Position.
                                       Technische Info: Anzeige-Feld, DB-Feld: lapool.breite.

                                       LS Lieferschein-Kennzeichen.
                                        “Status des Lieferscheins” auf Seite G-41
2.00 / 04-2022




                 A+W Enterprise Versandsteuerung                                                             G-111
                 Gestelle                                                               Softwarereferenz




                            Scheibenzuordnung
                            Versandsteuerung – Datenebene <Shift> + <F4> > Gestelle > Scheiben-Ge-
                            stellzuordnung




                            Abb. G-58    Dialog Scheiben-Gestellzuordnung


                            In diesem Dialog führen Sie die Scheibenzuordnung zu einem Gestell, Route
                            und Liefertermin durch, oder Sie erhalten Informationen zu bereits vorhande-
                            ne Zuordnungen. Sie können die Zuordnung löschen und das Gestell somit
                            leeren.

                               Scheiben-Gestellzuordnung
                               Das Funktionsprinzip der Gestellzuordnung ist separat beschrieben und
                               kann bei einem zuständigen A+W - Mitarbeiter angefordert werden.

                            Gestell Gestellnummer, zu dem die Gestellzuordnung durchgeführt, ange-
                            zeigt oder geändert werden soll.
                            Technische Info: Alphanumerisches Feld, DB-Feld: gest.exgnr

                            Typ Gestelltypnummer. Die Gestelltypen werden unter Logistik - Gestellver-
                            waltung - Gestellstamm - Gestelltypen hinterlegt.
                            Technische Info: Numerisches Feld, DB-Feld: gtyp.gtypnr

                            Bemerkung Informationsfeld mit 60 Zeichen für die Gestell-Scheibenzuord-
                            nung.
                            Technische Info: Alphanumerisches Feld, DB-Feld: gest.bemerk

                            Gewicht Leergewicht des ausgewählten Gestells. Das Gestellgewicht wird
                            pro Gestelltyp unter Logistik - Gestellverwaltung - Gestellstamm - Gestellty-
                            pen hinterlegt.
2.00 / 04-2022




                            Mit <Shift> + <F8> können Sie das Feld Gewicht ändern. Diese Änderung gilt
                            anschließend nur für das aktuelle Gestell und wird nicht in die Stammdaten für
                            alle Gestelle des Gestelltypes übernommen.
                            Technische Info: Numerisches Feld, DB-Feld: gtyp.eiggew


                 G-112                                                A+W Enterprise Versandsteuerung
                 Softwarereferenz                                                                          Gestelle




                                       Geändert Name des Mitarbeiters, der die letzte Änderung an den Gestellzu-
                                       ordnungsdaten vorgenommen hat. Der Name wird aus den Mitarbeiter-
                                       Stammdaten anhand der Mitarbeiternummer ermittelt.
                                       Technische Info: Anzeige-Feld, DB-Feld: gtyp.aendermanr

                                       Feste Tourzuordnung Wenn die Scheiben-Gestellzuordnung bereits erfolg-
                                       te, wird in dieser Zeile die Routen-Lieferdatum-Zuordnung als Information an-
                                       gezeigt.

                                       Gebucht Name des Mitarbeiters, der die letzte Änderung an den Gestellzu-
                                       ordnungsdaten vorgenommen hat. Der Name wird aus den Mitarbeiter-
                                       Stammdaten anhand der Mitarbeiternummer ermittelt.
                                       Technische Info: Anzeige-Feld, DB-Feld: gtyp.aendermanr

                                       Scheibenzuordnung Unter der Scheibenzuordnung wird der Name des Mit-
                                       arbeiters und das Datum der letzten Änderung bzw. Buchung ausgegeben.
                                       Der Name wird aus den Mitarbeiter-Stammdaten anhand der Mitarbeiternum-
                                       mer ermittelt.
                                       Technische Info: Anzeige-Feld, DB-Feld: gtyp.aendermanr

                                       Auftrag Nummer des Auftrags, der dem aktuellen Gestell zugeordnet ist.
                                       Technische Info: Numerisches Feld, DB-Feld: gestzu.auftrnr

                                       Pos Interne Positionsnummer aus dem Auftrag.
                                       Technische Info: Numerisches Feld, DB-Feld: gestzu.posnr

                                       Tnr Tupelnummer. Das Feld ist nur bei Einkaufsvorgängen mit verlängerter
                                       Werkbank relevant.
                                       Technische Info: Numerisches Feld, DB-Feld: aufstrukt.tnr

                                       Menge Positions-Stückzahl, die sich auf dem Gestell befindet.
                                       Technische Info: Numerisches Feld, DB-Feld: gestzu.menge

                                       Gesamt Gesamte Positions-Stückzahl aus dem Auftrag.
                                       Technische Info: Anzeige-Feld, DB-Feld: lapool.gesstk, kpos.menge

                                       Verfügbar Verfügbare Positions-Stückzahl.
                                       Technische Info: Anzeige-Feld

                                       V.Route Versand-Route. Sobald eine feste Scheiben-Gestellzuordnung vor-
                                       genommen wird, wird in diesem Feld die entsprechende Routennummer, so-
                                       wie im Feld dahinter der Liefertermin angezeigt.
                                       Technische Info: Anzeige-Feld

                                       Liefertermin Festgelegter Liefertermin. Sobald eine feste Scheiben-Gestell-
                                       zuordnung vorgenommen wird, wird in diesem Feld der entsprechende Liefer-
                                       termin, sowie im Feld davor die Versand-Route angezeigt.
                                       Technische Info: Anzeige-Feld
2.00 / 04-2022




                                       Breite Breite der Scheibe aus der Position.
                                       Technische Info: Anzeige-Feld, DB-Feld: lapool.laenge




                 A+W Enterprise Versandsteuerung                                                             G-113
                 Gestelle                                                               Softwarereferenz




                            Höhe Höhe der Scheibe aus der Position.
                            Technische Info: Anzeige-Feld, DB-Feld: lapool.breite

                            Artikel Produktbezeichnung des Positionsartikels aus den Stammdaten.

                            In diesem Dialog haben Sie noch weitere Möglichkeiten:
                            • Mit <Shift> + <F8> können Sie das Feld Gewicht ändern.
                            • Mit <F5> können Sie den Dialog Versandinfo einblenden lassen. Der Dia-
                                log wird nur dann angezeigt, wenn eine Versandinfo vorhanden ist.
                            • Mit [Leeren] oder <Strg> + <F8> leeren Sie das Gestellt. D. h., dass der In-
                                halt des Gestells ausgebucht wird.
2.00 / 04-2022




                 G-114                                                A+W Enterprise Versandsteuerung
                 Softwarereferenz                                                                          Gestelle




                                       VK/EK Information
                                       Versandsteuerung – Auftragsebene > <Shift> + <F4> > VK/EK Information




                                       Abb. G-59   Dialog VK/EK Information


                                       In diesem Dialog erhalten Sie Informationen zu dem ausgewählten Auftrag.
                                       Sofern Sie mit Bestellungen in der Versandsteuerung arbeiten, wird die Auf-
                                       tragsinformation mit der dazugehörigen Bestellinformation zusammengeführt.

                                       Auftrag Aktuelle Auftragsnummer.
                                       Technische Info: Anzeige-Feld

                                       Pos Interne Positionsnummer aus dem Auftrag.
                                       Technische Info: Anzeige-Feld

                                       Ges Gesamte Positions-Stückzahl aus dem Auftrag.
                                       Technische Info: Anzeige-Feld

                                       Abruf Bereits abgerufene Stückzahl.
                                       Technische Info: Anzeige-Feld

                                       Verp Bereits verpackte Stückzahl.
                                       Technische Info: Anzeige-Feld

                                       Breite Breite der Scheibe aus der Position.
                                       Technische Info: Anzeige-Feld

                                       Höhe Höhe der Scheibe aus der Position.
                                       Technische Info: Anzeige-Feld

                                       Bestellung Aktuelle Bestellnummer, falls zu der Auftragsposition eine Bestel-
                                       lung erstellt wurde.
                                       Technische Info: Anzeige-Feld
2.00 / 04-2022




                                       Pos Interne Positionsnummer aus der Bestellung.
                                       Technische Info: Anzeige-Feld


                 A+W Enterprise Versandsteuerung                                                             G-115
                 Gestelle                                                   Softwarereferenz




                            Datum Bestelldatum.
                            Technische Info: Anzeige-Feld

                            Modus IVersand-Modus.
                            Technische Info: Anzeige-Feld
2.00 / 04-2022




                 G-116                                      A+W Enterprise Versandsteuerung
                 Softwarereferenz                                                                        Gestelle




                                       VK/EK Info (Global)
                                       Versandsteuerung – Auftragsebene > <Shift> + <F4> > VK/EK Info (Global)




                                       Abb. G-60    Dialog - VK/EK Info (Global)


                                       Über den Menüpunkt VK/EK Info (Global) können Sie die zusammengeführten
                                       Verkaufs- und Einkaufsinformation zu einem ausgewählten Auftrag abrufen. In
                                       dem Auswahldialog (kleine Darstellung) geben Sie die Nummer ein oder wäh-
                                       len über <F9> einen gewünschten Vorgang aus. Je nach gewähltem Versand-
                                       Modus können Sie einen Auftrag oder eine Bestellung suchen.
                                       Die Suchfelder in der Kopfzeile und der Versand-Modus sind in folgendem Ka-
                                       pitel beschrieben:
                                        “Versand-Explorer” auf Seite G-15

                                       Auftrag Nummer des Auftrags.
                                       Technische Info: Anzeige-Feld, DB-Info: lapool.auftrnr
                                       Wenn Sie in dem Auswahl-Dialog eine Bestellung gewählt haben, dann steht
                                       im Feld Auftrag eine Bestellnummer und im Feld Referenz die Auftragsnum-
                                       mer.

                                       Pos Nummer der Position.
                                       Technische Info: Anzeige-Feld, DB-Info: lapool.lfdpos

                                       Artikel Artikelbezeichnung des Auftrags.
                                       Technische Info: Anzeige-Feld, DB-Info: artikel.artbez1
2.00 / 04-2022




                                       Ges Gesamte Stückzahl der Position.
                                       Technische Info: Anzeige-Feld, DB-Info: lapool.gesstk



                 A+W Enterprise Versandsteuerung                                                           G-117
                 Gestelle                                                              Softwarereferenz




                            Abruf Stückzahl der Position, die der Kunde für den Liefertermin anfordert.
                            Technische Info: Anzeige-Feld, DB-Info: lapool.abrufstk

                            Datum Lieferdatum aus dem Auftrag bzw. der Bestellung (1. Spalte im Dia-
                            log).
                            Technische Info: Anzeige-Feld, DB-Info: lapool.ltplan

                            Route Nummer der Route.
                            Technische Info: Anzeige-Feld, DB-Info: lapool.routenr

                            Haus Nummer des Hauses oder Mandanten.
                            Technische Info: Anzeige-Feld, DB-Info: lapool.hnr

                            Referenz Nummer des Referenzvorgangs. Wenn Sie in den Auswahl-Dialog
                            eine Bestellung gewählt haben, dann steht im Feld Auftrag eine Bestellnum-
                            mer und im Feld Referenz die Auftragsnummer.
                            Technische Info: Anzeige-Feld, DB-Info: lapool.auftrnr (lapool.vorgang=2 (Be-
                            stellung) oder 5 (Auftrag))

                            Pos Positionsnummer aus dem Referenzvorgang.
                            Technische Info: Anzeige-Feld, DB-Info: lapool.posnr

                            Datum Liefertermin aus dem Referenzvorgang.
                            Technische Info: Anzeige-Feld, DB-Info: lapool.ltplan

                            Route Nummer der Route aus dem Referenzvorgang.
                            Technische Info: Anzeige-Feld, DB-Info: lapool.routenr

                            Gepl. Geplante Menge.
                            Technische Info: Anzeige-Feld, DB-Info: lapool.sollstk

                            Art Versandmodus für Referenzvorgang. Folgende Werte werden angezeigt:
                            • VK-Aus. (VK-Ausgang)
                            • E1. (EK-Warenausgang)
                            • E2. (EK-Wareneingang)
                            Technische Info: Anzeige-Feld, DB-Feld: lapool.vmodus
2.00 / 04-2022




                 G-118                                                A+W Enterprise Versandsteuerung
                 Softwarereferenz                                                                           Gestelle




                                          Versandsteuerung - Übersicht
                                          Versandsteuerung – Datenebene > <Shift> + <F4> > Übersicht




                 Abb. G-61   Versandsteuerung – Übersicht


                                          Über den Menüpunkt Übersicht starten Sie den Suchdialog, über den Sie sich
                                          nach verschiedenen Kriterien eine Übersicht zusammenstellen können.
                                          Folgende Auswahlkriterien stehen Ihnen zur Verfügung:
                                             •   Haus
                                             •   Lieferdat (Geplanter Liefertermin)
                                             •   Route (Lieferroute)
                                             •   Auftrag (Auftragsnummer)
                                             •   Extern (Kunden-Bestnr.)
                                             •   Ladeliste (Nummer der Ladeliste)
                                             •   Objekt (Objektnummer)
                                             •   Kunde (Kundennummer)
                                             •   Gewicht (Positionsgewicht in kg)
                                             •   Fläche (Fläche pro Position in m²)
2.00 / 04-2022




                                             •   Breite (Scheiben-Höhe in mm)
                                             •   Höhe (Scheiben-Länge in mm)



                 A+W Enterprise Versandsteuerung                                                             G-119
                 Gestelle                                                                    Softwarereferenz




                            In allen Felder können Sie jeweils die Filterbedingungen nach Bedarf ändern:

                            Bedingung    Bedeutung

                            =            Suche nach genau diesem Wert (z. B. Feld Marktpartner = 600004
                                         listet nur Vorgänge zu diesem Marktpartner auf).

                            >            Suche nach größeren Werten (z. B. Feld Marktpartner > 600004
                                         listet nur Vorgänge mit Marktpartnernummern größer als 600004
                                         auf).

                            m            Suche nach Muster in Textfeldern (z. B. Feld Kommission Modell 12
                                         listet alle Vorgänge mit dem Kommissionstext Modell 12 auf.)

                            0            Suche nach Werten = 0 (z. B. Feld Marktpartner 0 listet den
                                         Marktpartner mit der Nummer 0 auf).

                            z            Suche alle Werte im Bereich.

                            !            Suche alles außer diesem Wert (z. B. Feld Abteilung ! 10 listet alle
                                         Abteilungen außer der Abteilung mit der Nummer 10 auf).

                            <            Suche nach kleineren Werten (z. B. Feld Marktpartner < 600004
                                         listet nur Vorgänge mit Marktpartnernummern kleiner als 600004
                                         auf).

                            Tab. G-5    Bedeutung der Filterbedingungen

                            Nach der Eingabe lösen Sie mit <F3> die Suchaktion aus. Soweit die Suche
                            erfolgreich war, wird eine Treffermenge im selben Dialogfenster ausgegeben.
                            Mit <F2> sehen Sie weitere Felder zu der Auswahl.
                            Folgende Felder werden in den Trefferdialogen angezeigt:

                            Lieferdat. Liefertermin aus dem Auftrag.
                            Technische Info: Datum-Feld, DB-Info: lapool.ltplan

                            Route Routennummer.
                            Technische Info: Anzeige-Feld, DB-Info: lapool.routennr

                            Auftrag Externe Auftragsnummer. Bei Versandmodus mit Einkaufsvorgänge
                            wird hier die Nummer der Bestellung ausgegeben.
                            Technische Info: Anzeige-Feld, DB-Info: lapool.auftrnr

                            Pos Positionsnummer aus dem Auftrag.
                            Technische Info: Anzeige-Feld, DB-Info: lapool.posnr

                            Kunde Kundennummer des Auftrags.
                            Technische Info: Anzeige-Feld, DB-Info: lapool.kunr

                            Objekt Objektnummer aus dem Auftrags, wenn diese vorhanden ist.
                            Technische Info: Anzeige-Feld, DB-Info: lapool.objnr
2.00 / 04-2022




                            Ges. Gesamte Stückzahl der Position, die für diesen Auftrag erfasst wurde.
                            Technische Info: Anzeige-Feld, DB-Info: lapool.gesstk




                 G-120                                                  A+W Enterprise Versandsteuerung
                 Softwarereferenz                                                                              Gestelle




                                       Abruf Stückzahl der Position, die der Kunde für den Liefertermin anfordert.
                                       Technische Info: Anzeige-Feld, DB-Info: lapool.abrufstk

                                       Verp. Verpackte Stückzahl der Position.
                                       Technische Info: Anzeige-Feld, DB-Info: lapool.iststk

                                       Breite Höhe der Scheibe.
                                       Technische Info: Anzeige-Feld, DB-Info: lapool.breite

                                       Höhe Breite der Scheiben.
                                       Technische Info: Anzeige-Feld, DB-Info: lapool.laenge

                                       qm Fläche der Position in Quadratmetern.
                                       Technische Info: Anzeige-Feld, DB-Info: lapool.gm

                                       LL Ladeliste-Nummer, wenn für diesen Auftrag bereits eine Ladeliste exis-
                                       tiert.
                                       Technische Info: Anzeige-Feld, DB-Info: lapool.llnr

                                       LS Anzeige, ob für diesen Auftrag bereits ein Lieferschein existiert.
                                       Technische Info: Anzeige-Feld, DB-Info: lapool.lsdrukz

                                       Artikelbezeichnung Artikelbezeichnung für die Auftragsposition.
                                       Technische Info: Anzeige-Feld, DB-Info: lapool.artbez1

                                       Modell Modellnummer aus der Auftragsposition, falls diese vorhanden ist.
                                       Technische Info: Anzeige-Feld, DB-Info: lapool.modnr

                                       kg Gewicht pro Auftragsposition.
                                       Technische Info: Anzeige-Feld, DB-Info: lapool.gewicht

                                       Fußzeile
                                       In der Fußzeile des Dialoges werden für die folgenden Felder weitere Informa-
                                       tion angezeigt:
                                       •   Externe Kunden-BestNr
                                       •   Breite (größter Wert für Scheiben-Länge aus der Treffermenge)
                                       •   Höhe (größter Wert für Scheiben-Höhe aus der Treffermenge)
                                       •   kg (Gesamt-Gewicht für alle in der Übersicht angezeigte Positionen)
                                       •   qm (Gesamt-Fläche für alle in der Übersicht angezeigte Positionen)
                                       •   Ges. (Gesamt-Anzahl der erfassten Einheiten für alle in der Übersicht an-
                                           gezeigte Positionen)
                                       •   Abruf (Gesamt-Anzahl der angeforderten Einheiten für alle in der Übersicht
                                           angezeigte Positionen)
                                       •   Verp. (Gesamt-Anzahl der verpackten Einheiten für alle in der Übersicht
                                           angezeigte Positionen)
2.00 / 04-2022




                 A+W Enterprise Versandsteuerung                                                                G-121
                 Gestelle                                                                  Softwarereferenz




                            Lieferterminänderungen
                            Versandsteuerung – Auftragsebene > <Shift> + <F4> Lieferterminänderungen




                            Abb. G-62    Lieferterminänderungen


                            In diesem Dialog werden alle Änderungen der Liefertermine angezeigt.
                            Eine ausführliche Beschreibung finden Sie im Kapitel:
                             Verkauf, “Lieferterminänderungs-Protokoll” auf Seite D-173
2.00 / 04-2022




                 G-122                                                  A+W Enterprise Versandsteuerung
                 Softwarereferenz                                                                           Gestelle




                                       Versandinformationen
                                       Versandsteuerung – Auftragsebene > <Shift> + <F4> Versandinformationen




                                       Abb. G-63     Versandinformationen


                                       In diesem Dialog können Sie einem Auftrag eine Versandart zuordnen bzw.
                                       eine bereits hinterlegte Versandart ändern und weitere Versandinformationen
                                       hinterlegen.
                                        “Register – VersandInfo I” auf Seite G-48

                                       Versandart Versandart des Auftrages. Die mögliche Versandarten hinterle-
                                       gen Sie in den Stammdaten (Schlüssel > System > Versand > Versandart).
                                       Nach dem speichernden Verlassen des Dialoges [Schaltfläche [OK]) wird die
                                       neue Versandart in das Register VersandInfo I übernommen.
                                       Technische Info: Numerisches Feld, <F9>, DB-Info: lapool.versandart

                                       Ankunftszeit Die Ankunftszeit wird aus dem Auftrag übernommen, wenn mit
                                       der via-Plant Auslieferung gearbeitet wird. Sie können die voraussichtliche
                                       Ankunftszeit alternativ in diesem Feld hinterlegen. Der Wert wird in das Feld
                                       A.Zeit in das Register Lieferanschrift übernommen.
                                        “Register– Lieferanschrift” auf Seite G-46
                                       Technische Info: Alphanumerisches Feld, DB-Info: lapool.ankunftszeit

                                       Private Long 1/2 Zwei private Felder zur Eingabe eines alphanumerischen
                                       Werts. Die Feldbezeichnungen für diese Felder kann kundenindividuell über
                                       Umgebungsvariablen konfiguriert werden.
                                       Technische Info: Alphanumerische Felder, DB-Info: lapool.private_long1, la-
                                       pool.private_long2

                                       Private Char 1/2 Zwei private Felder zur Eingabe eines numerischen Werts.
                                       Die Feldbezeichnungen für diese Felder kann kundenindividuell über Umge-
                                       bungsvariablen konfiguriert werden.
                                       Die Information aus den privaten Felder wird in das Register VersandInfo II
                                       Felder PL1/2, PC1/2 entsprechend übernommen.
                                       Technische Info: Alphanumerische Felder, DB-Info: lapool.private_char1. la-
                                       pool.private_char2
                                        “Register – VersandInfo II” auf Seite G-51
2.00 / 04-2022




                 A+W Enterprise Versandsteuerung                                                              G-123
                 Gestelle                                                               Softwarereferenz




                            Via Details
                            Versandsteuerung – Auftragsebene > <Shift> + <F4> > Via Details




                            Abb. G-64   Details der Auslieferung


                            Dieser Dialog steht Ihnen nur bei einer via-plant Konfiguration zur Verfügung
                            und wird in diesem Dokument nicht weiter beschrieben.

                               via-plant-Konfiguration
                               Der Funktionsumfang via-plant ist nicht Bestandteil dieser Dokumentation.
                               Die ausführliche Beschreibung kann bei Bedarf beim zuständigen A+W
                               Mitarbeiter angefragt werden.
2.00 / 04-2022




                 G-124                                               A+W Enterprise Versandsteuerung
                 Softwarereferenz                                                                            Gestelle




                                       Fertigwarenlager
                                       Als Fertigwarenlager wird ein Dispositionslager für Ware bezeichnet, die direkt
                                       vor der Auslieferung zum Kunden steht.Das Fertigwarenlager ermöglicht je-
                                       derzeit einen Überblick über die auszuliefernden Aufträge. Die Nutzung der
                                       Fertigwarenlager-Funktion bedarf eine gesonderte Konfiguration.
                                       Die Funktion Fertigwarenlager ist nicht nur in der Versandsteuerung sondern
                                       auch in den Einkaufs-Wareneingängen verknüpft.
                                       Folgende Dialoge zur Funktion Fertigwarenlager sind Bestandteil dieses Do-
                                       kumentes:
                                        “Fertigwarenlagerbestand” auf Seite G-126
                                        “Fertigwarenlager Übersicht” auf Seite G-127
                                        “Fertigwarenlager Inventur” auf Seite G-128
                                        “Inventur abschließen” auf Seite G-128
                                        “Protokoll” auf Seite G-129
2.00 / 04-2022




                 A+W Enterprise Versandsteuerung                                                               G-125
                 Gestelle                                                                 Softwarereferenz




                            Fertigwarenlagerbestand
                            Versandsteuerung – Touren-/Auftragsebene > <Shift> + <F4> Fertigwarenla-
                            ger > Fertigwarenlager




                            Abb. G-65   Fertigwarenlagerbestand für ...


                            In diesem Dialog tragen Sie Daten für eine Suche ein. Das Ergebnis der Su-
                            che wird im Dialog Fertigwarenlager Übersicht angezeigt. Die Übersicht listet
                            die noch nicht gelieferten Aufträge auf.

                            Haus Nummer des Hauses oder Mandanten. Über <F9> wählen Sie die
                            Hausnummer aus, soweit Sie mit einem Mehrmandanten-System arbeiten.
                            Technische Info: Numerisches Feld, <F9>, DB-Feld: lapfertwb.orghnr

                            Auftrag Auftragsnummer. Über <F9> können Sie nach einem Auftrag su-
                            chen. Wenn Sie das Feld Auftrag leer lassen, bekommen Sie die Fertigwaren-
                            lager - Übersicht für alle Aufträge. Mit der Auftragsauswahl schränken Sie
                            diese Übersicht ein.
                            Technische Info: Numerisches Feld, <F9>, DB-Feld: lapfertwb.auftrnr

                            Zielhaus Nummer des Zielhauses oder Zielmandanten.
                            Technische Info: Numerisches Feld, <F9>, DB-Feld: lapfertwb.zielhnr
2.00 / 04-2022




                 G-126                                                    A+W Enterprise Versandsteuerung
                 Softwarereferenz                                                                           Gestelle




                                       Fertigwarenlager Übersicht
                                       Versandsteuerung – Touren-/Auftragsebene> <Shift> + <F4> Fertigwarenla-
                                       ger > Fertigwarenlager, Auswahlkriterien eingeben




                                       Abb. G-66    Fertigwarenlager Übersicht


                                       In diesem Dialog erhalten Sie die Übersicht zu den Aufträgen, die sich zur
                                       Auslieferung im Fertigwarenlager befinden.

                                       Auftrag Auftragsnummer. Wenn Sie das Feld Auftrag als ein Suchkriterium
                                       eingegeben haben, werden in dieser Spalte nur Positionen dieses Auftrags
                                       gelistet.
                                       Technische Info: Numerisches Feld, <F9>, DB-Feld: lapfertwb.auftrnr

                                       Pos Positionsnummer aus dem Auftrag.
                                       Technische Info: Numerisches Feld, <F9>, DB-Feld: lapfertwb.posnr

                                       Menge Gebuchte Menge.
                                       Technische Info: Numerisches Feld, <F9>, DB-Feld: lapfertwb.istmenge

                                       Haus Nummer des Hauses oder Mandanten. Über <F9> wählen Sie die
                                       Hausnummer aus, soweit Sie mit einem Mehrmandanten-System arbeiten.
                                       Technische Info: Numerisches Feld, <F9>, DB-Feld: lapfertwb.orghnr.

                                       Zielhaus Nummer des Zielhauses oder Zielmandanten. Wenn das Feld Ziel-
                                       haus bereits belegt ist, so befindet sich diese Position auf dem Transport vom
                                       Haus (Originalhausnummer) zum Zielhaus.
                                       Technische Info: Numerisches Feld, <F9>, DB-Feld: lapfertwb.zielhnr
2.00 / 04-2022




                                       Ergänzende Information
                                        “Protokoll” auf Seite G-129



                 A+W Enterprise Versandsteuerung                                                             G-127
                 Gestelle                                                              Softwarereferenz




                            Fertigwarenlager Inventur
                            Versandsteuerung > Touren-/Auftragsebene> <Shift> + <F4> Fertigwarenla-
                            ger > Fertigwarenlager Inventur
                            Über diesen Menüpunkt starten Sie die Inventur des Fertigwarenlagers, d. h.,
                            dass das aktuelle Haus für die Zeit der Inventur gesperrt wird. Während der
                            Inventur können keine Fertigmeldungen aus der Produktion gebucht werden,
                            diese werden vom Rückmeldeserver in der Warteschlange gehalten. Nach
                            Abschluss der Inventur werden diese Buchungen nachgeholt.


                            Inventur abschließen
                            Versandsteuerung > Touren-/Auftragsebene> <Shift> + <F4> Fertigwarenla-
                            ger > Fertigwarenlager, Auswahlkriterien eingeben > Inventur abschließen
                            Über diesen Menüpunkt beenden Sie die Inventur des Fertigwarenlagers. Alle
                            Fertigmeldungen aus der Produktion werden nachgebucht.
2.00 / 04-2022




                 G-128                                               A+W Enterprise Versandsteuerung
                 Softwarereferenz                                                                           Gestelle




                                          Protokoll
                                          Versandsteuerung > Touren-/Auftragsebene> <Shift> + <F4> Fertigwarenla-
                                          ger > Fertigwarenlager > Protokoll




                 Abb. G-67   Fertigwarenlager Buchungsprotokoll


                                          In diesem Dialog sehen Sie die Informationen aus dem Buchungsprotokoll des
                                          Fertigwarenlagers.

                                          Bewegungsdaten

                                          Datum Datum der ausgeführten Buchung.
                                          Technische Info: Anzeige-Feld, DB-Feld: lapfertwbprot.datum

                                          Zeit Zeitpunkt der Buchung.
                                          Technische Info: Anzeige-Feld, DB-Feld: lapfertwbprot.zeit

                                          Lieferdat. Versanddatum, an dem der Auftrag zum Kunden geliefert wird.
                                          Wenn es sich bei dem Buchungssatz um keine auftragsbezogene Buchung
                                          handelt, wird hier das Datum 31.12.1899 angezeigt.
2.00 / 04-2022




                                          Technische Info: Anzeige-Feld, DB-Feld: lapfertwbprot.ltplan




                 A+W Enterprise Versandsteuerung                                                             G-129
                 Gestelle                                                            Softwarereferenz




                            Auftrag Nummer des Auftrags. Wenn es sich bei dem Buchungssatz um kei-
                            ne auftragsbezogene Buchung handelt, wird als Auftragsnummer -1 ange-
                            zeigt.
                            Technische Info: Anzeige-Feld, DB-Feld: lapfertwbprot.auftrnr

                            Pos. Nummer der Position. Wenn es sich bei dem Buchungssatz um keine
                            auftragsbezogene Buchung handelt, bleibt dieses Feld leer.
                            Technische Info: Anzeige-Feld, DB-Feld: lapfertwbprot.posnr

                            Gebucht Gebuchte Menge.
                            Technische Info: Anzeige-Feld, DB-Feld: lapfertwbprot.menge

                            Haus Nummer des Hauses oder Mandanten, in dem gebucht wird.
                            Technische Info: Anzeige-Feld, DB-Feld: lapfertwbprot.orghnr

                            Ziel Nummer des Zielhauses oder Zielmandanten. Wenn das Feld belegt ist,
                            dann wurde die Buchung vom Original-Haus zum Ziel-Haus durchgeführt.
                            Technische Info: Anzeige-Feld, DB-Feld: lapfertwbprot.zielhnr

                            Buchungsart Art der Buchungsdurchführung, z. B. Fehlmengenkontrolle.
                            Technische Info: Anzeige-Feld, DB-Feld: lapfertwbprot.buchtext

                            Mitarbeiter Name des Mitarbeiters, der die Buchung ausgelöst hat.
                            Technische Info: Anzeige-Feld, DB-Feld: lapfertwbprot.manr, mitarb.maname
2.00 / 04-2022




                 G-130                                             A+W Enterprise Versandsteuerung
                 Softwarereferenz                                                                             Gestelle




                                          Grafische Tourenübersicht
                                          Versandsteuerung – Datenebene > Übersicht (<Shift> + <F11>)




                 Abb. G-68   Grafische Tourenübersicht


                                          Über die Funktion Übersicht (Shift> + <F11>), die über die Prompt-Zeile wähl-
                                          bar ist, können Sie eine grafische Übersicht zu den Lieferungen erhalten.
                                          Mit folgenden Parametern legen Sie die X- und Y-Achse für diese grafische
                                          Darstellung fest:

                                          1. Parameter: Auswahl-Wert für die Y-Achse.
                                             • Stück
                                             • QM
                                             • Gewicht
                                          Mit <Enter> bestätigen Sie den ersten ausgewählten Parameter.

                                          2. Parameter: Auswahl-Wert für die X-Achse.
                                             • Alle Routen für den aktuellen Tourentag anzeigen
                                             • Nächsten Tourentage für die aktuelle Route anzeigen
                                          Mit <Enter> bestätigen Sie den zweiten ausgewählten Parameter und lösen
                                          den Grafikaufbau aus.
2.00 / 04-2022




                                          Der Titel für die grafische Tourenübersicht wird dynamisch, abhängig von den
                                          gewählten Parametern, programmintern generiert.




                 A+W Enterprise Versandsteuerung                                                                G-131
                 Drucken                                                               Softwarereferenz




                           Drucken
                           Die Druckfunktionen können von unterschiedlichen Dialogen und Ansichten
                           aus gestartet werden.
                           In diesem Abschnitt finden Sie Informationen zu folgenden Themen:
                           •   “Drucken einer Ladeliste” auf Seite G-133
                           •   “Drucken aller Ladelisten” auf Seite G-134
                           •   “Drucken Ergänzungsladelisten” auf Seite G-135
                           •   “Listendruck” auf Seite G-136
                           •   “Vorablieferschein Druck” auf Seite G-137
                           •   “Lief./Wareneing. Freigabe + Druck” auf Seite G-139
                           •   “Druckformat” auf Seite G-140
                           •   “Druckformat” auf Seite G-140

                               Konfiguration des Druckbereichs
                               Die Nutzung der Druckfunktionen in der Versandsteuerung setzt voraus,
                               dass Ihr System eine abgeschlossene Konfiguration des Druckbereichs
                               hat. Für weitere Informationen sprechen Sie bitte einen A+W - Mitarbeiter
                               an.
2.00 / 04-2022




                 G-132                                               A+W Enterprise Versandsteuerung
                 Softwarereferenz                                                                            Drucken




                                       Drucken einer Ladeliste
                                       Versandsteuerung – Datenebenen > <F4> > Drucken einer Ladeliste




                                       Abb. G-69    Dialog Drucken auf


                                       Der Druck einer Ladeliste ist nur möglich, wenn diese vorher erstellt wurde. In
                                       diesem Dialog können Sie folgende Auswahl treffen:

                                       Druckerauswahl Wählen Sie über <F9> den Druckers, auf dem die Ladeliste
                                       gedruckt wird. Drucker müssen im Vorfeld im System konfiguriert werden
                                       (System > Druckerverwaltung > Drucker einrichten).
                                       Technische Info: Numerisches Feld,<F9>, DB-Feld: drucker.drunr

                                       Anzahl der Exemplare Anzahl der zu druckenden Exemplare.
                                       Technische Info: Numerisches Feld, ohne DB-Bezug

                                       Dateiname Wenn Sie die Ladeliste in eine Datei schreiben möchten (Dru-
                                       ckerauswahl = Dateidruck), dann müssen Sie einen Dateinamen angeben.
                                       Diese, durch Druck erstellte Datei, finden Sie anschließend in dem vordefinier-
                                       ten Verzeichnis.

                                       Fußzeile
                                       Der Name der ausgewählten bzw. zugeordneten Liste wird angezeigt.
2.00 / 04-2022




                 A+W Enterprise Versandsteuerung                                                               G-133
                 Drucken                                                                 Softwarereferenz




                           Drucken aller Ladelisten
                           Versandsteuerung – Datenebenen > <F4> > Drucken aller Ladelisten




                           Abb. G-70    Auswahldialog für Ladelisten-Druck


                           Über diesen Dialog drucken Sie alle Ladelisten einer ausgewählten Zeitspan-
                           ne auf einmal.
                            “Drucken einer Ladeliste” auf Seite G-133
                           Der Ladenlisten-Druck ist nur möglich, wenn die Ladelisten vorher erstellt wur-
                           den. Bevor Sie die Listen drucken, treffen Sie folgende Auswahl:

                           Haus Nummer des Hauses, für das Sie die Ladelisten drucken.
                           Technische Info: Numerisches Feld, DB-Feld: lapool.hnr

                           von, bis Zeitraum, für den Sie die Ladelisten drucken.
                           Technische Info: Numerisches Feld, DB-Feld: lapoolll.ltplan
                           Nach dieser Auswahl startet der Dialog Druckerauswahl automatisch:
                            “Druckerauswahl” auf Seite G-140
2.00 / 04-2022




                 G-134                                                   A+W Enterprise Versandsteuerung
                 Softwarereferenz                                                                       Drucken




                                       Drucken Ergänzungsladelisten
                                       Versandsteuerung – Datenebenen > <F4> > Drucken Ergänzungsladelisten




                                       Abb. G-71   Auswahldialog für Ergänzungs-Ladelisten-Druck


                                       Über diesen Dialog drucken Sie Ergänzungsladelisten. Ergänzungsladelisten
                                       müssen immer dann gedruckt werden, wenn z. B.: Änderungen im Auftrag
                                       oder in der Versandplanung vorgenommen wurden und eine Ladeliste bereits
                                       existiert.

                                       Haus Nummer des Hauses, für das Sie die Ladelisten drucken.
                                       Technische Info: Numerisches Feld, DB-Feld: lapool.hnr

                                       von, bis Zeitraum, für den Sie die Ladelisten drucken.
                                       Technische Info: Numerisches Feld, DB-Feld: lapoolll.ltplan
                                       Nach dieser Auswahl startet der Dialog Druckerauswahl automatisch:
                                        “Druckerauswahl” auf Seite G-140
2.00 / 04-2022




                 A+W Enterprise Versandsteuerung                                                            G-135
                 Drucken                                                               Softwarereferenz




                           Listendruck
                           Versandsteuerung – Datenebenen > <F4> > Listendruck




                           Abb. G-72      Listendruck


                           In diesem Dialog sehen Sie die benutzerdefinierten Listen, die zum Drucken
                           zur Verfügung stehen. Benutzerdefinierte Listen (Reports) werden individuell
                           auf Kundenanfragen erstellt. Die Abbildung in diesem Dokument ist nur ein
                           Beispiel.
                           Nach der Auswahl der gewünschten Liste kann ein Dialog zur Eingabe der be-
                           nötigten Parameter starten. Je nach gewählter Liste, sind die entsprechenden
                           Felder aufgelistet.

                              Beispiel:

                              Listenname                        NVE Etikett

                              Parameter                         •   Liefertermin
                                                                •   Route
                                                                •   Auftrag
                                                                •   Position
                                                                •   NVE-Nummer


                           Nach der Werte-Angaben startet der Dialog Druckerauswahl automatisch:
2.00 / 04-2022




                            “Druckerauswahl” auf Seite G-140




                 G-136                                                 A+W Enterprise Versandsteuerung
                 Softwarereferenz                                                                           Drucken




                                       Vorablieferschein Druck
                                       Versandsteuerung – Auftragsebene > <F4> >Vorablieferschein Druck




                                       Abb. G-73    Vorablieferschein für…


                                       In diesem Dialog wählen Sie aus, für welchen Vorgang bzw. Vorgänge Sie Vor-
                                       ablieferschein(e) drucken wollen.
                                       Beim Dialogstart aus einer Auftragsebene wird dieser Auswahldialog mit aktu-
                                       ellen Werten je nach Versandmodus zwischen Auftrag und Bestellung bzw.
                                       Wareneingang vorbelegt.
                                       Beim Dialogstart aus der Tourenebene bleibt das Feld Auftrag leer. Lassen Sie
                                       das Feld leer, so werden nach dem [Auslösen], alle Vorablieferscheine für die-
                                       se Tour gedruckt.
                                       Mit <F3> oder [Auslösen] lösen Sie den Druck aus.
                                        “Druckerauswahl” auf Seite G-140
                                       Anschließend wird die Checkbox VL für die betroffene Vorgänge aktiviert.
                                        “Register – AuftragsInfo” auf Seite G-39
                                       Wenn für einen Auftrag nur der Vorablieferschein gedruckt ist, dann ist der
                                       Auftrag in der Versandsteuerung noch änderbar. Wenn für einen Auftrag ein
                                       Lieferschein gedruckt ist, dann ist der Auftrag in der Versandsteuerung nicht
                                       mehr änderbar.
                                       Ein Vorablieferschein ist kein eigener Vorgang in der Datenbank. Der Auf-
                                       tragsstatus ändert sich nicht durch den Vorablieferschein.

                                       Lieferdat. Datum der Lieferung, für die der Vorablieferschein gedruckt wird.
                                       Technische Info: Numerisches Feld, DB-Feld: lapool.ltplan

                                       Route Nummer der Route, für die der Vorablieferschein gedruckt wird.
                                       Technische Info: Numerisches Feld, DB-Feld: lapool.routenr
2.00 / 04-2022




                                       Auftrag Nummer des Auftrags, für den der Vorablieferschein gedruckt wird.
                                       Technische Info: Numerisches Feld, DB-Feld: lapool.auftrnr


                 A+W Enterprise Versandsteuerung                                                             G-137
                 Drucken                                                            Softwarereferenz




                           Ladeliste Ladelistennummer des Auftrags, für den der Vorablieferschein ge-
                           druckt wird.
                           Technische Info: Numerisches Feld, DB-Feld: lapool.llnr
2.00 / 04-2022




                 G-138                                            A+W Enterprise Versandsteuerung
                 Softwarereferenz                                                                          Drucken




                                       Lief./Wareneing. Freigabe + Druck
                                       Versandsteuerung – Auftragsebene > <F4> Lief./Wareneing. Freigabe +
                                       Druck




                                       Abb. G-74   Lieferscheinfreigabe für …


                                       In diesem Dialog wählen Sie aus, für welchen Auftrag ein Lieferschein ge-
                                       druckt wird.
                                       Wenn ein endgültiger Lieferschein gedruckt ist, dann sind die Versanddaten
                                       eines Auftrags nicht mehr änderbar. Der neue Status wird in den Auftrag über-
                                       nommen. Die Funktion kann so konfigurieren werden, dass beim Drucken
                                       zeitgleich die Rechnung erzeugt wird.

                                       Lieferdat. Lieferdatum, für das der Lieferschein gedruckt wird.
                                       Technische Info: Numerisches Feld, DB-Feld: lapool.ltplan

                                       Route Nummer der Route, für die der Lieferschein gedruckt wird.
                                       Technische Info: Numerisches Feld, DB-Feld: lapool.routenr

                                       Auftrag Nummer des Auftrags, für den der Lieferschein gedruckt wird.
                                       Technische Info: Numerisches Feld, DB-Feld: lapool.auftrnr

                                       Ladeliste Auswahl der Ladeliste, für die der Lieferschein gedruckt wird.
                                       Technische Info: Numerisches Feld, DB-Feld: lapool.llnr

                                          Lieferscheine in der Versandsteuerung
                                          In der Regel werden Lieferscheine erst dann erstellt, wenn die Ausliefe-
                                          rungswaren in der Produktion fertig gemeldet sind und bereits auf den
                                          Transport gebucht worden sind. Bei einer möglichen Änderung des Work-
                                          flows sprechen Sie den zuständigen A+W - Mitarbeiter an.
2.00 / 04-2022




                 A+W Enterprise Versandsteuerung                                                             G-139
                 Drucken                                                              Softwarereferenz




                           Druckformat
                           Zusatzmenü <F4> > Vorablieferschein Druck > Daten eingeben > [Auslösen]




                           Abb. G-75   Dialog - Druckenformat


                           In diesen Dialog geben Sie die druckbezogenen Daten ein.

                           Anzahl der Exemplare Anzahl der zu druckenden Exemplare.
                           Technische Info: Numerisches Feld, ohne DB-Bezug

                           sortiert nach Sortierreihenfolge beim Druck. Mögliche Werte sind:
                           • Aufträge
                           • Lieferscheinkopien
                           Technische Info: Numerisches Feld, ohne DB-Bezug


                           Druckerauswahl
                           Menü <F4> > Lief./Wareneing. Freigabe + Druck > [Auslösen]




                           Abb. G-76   Dialog - Drucken auf


                           In diesem Dialog wählen Sie den Drucker aus, auf dem gedruckt werden soll.

                           Druckerauswahl Druckernummer, auf dem das zuvor gewählte Dokument
                           gedruckt wird. Über <F9> können Sie die Liste mit den verfügbaren Druckern
                           öffnen. Drucker müssen im Vorfeld im System konfiguriert werden (System >
                           Druckerverwaltung > Drucker einrichten).
                           Technische Info: Numerisches Feld,<F9>, DB-Feld: drucker.drunr

                           Anzahl der Exemplare Die Stückzahl der zu druckenden Exemplare.
                           Technische Info: Numerisches Feld, ohne DB-Bezug

                           Fußzeile
                           In der Fußzeile wird der Name des Formulars eingeblendet, welcher ausge-
2.00 / 04-2022




                           druckt wird, z. B. Ladeliste (Versand).




                 G-140                                             A+W Enterprise Versandsteuerung
Versandsteuerung               G

                          Partindex




                   A+W Enterprise
                 Partindex                                                                                     Index




                 Index
                 A                                                 Ergänzungsladeliste
                 Adresse                                           – drucken G-135
                 – auswählen G-87                                  Explorer
                 – suchen G-87                                     – Funktion G-16
                 Auftrag                                           – Übersicht G-16
                 – Auftragsinformation G-39                        – Übersicht für Liefertermine   G-15
                 – Information, globale G-115, G-117, G-124
                 – Informationen G-73, G-76, G-77                  F
                 – Lieferanschrift G-46                            Fahrzeuginformationen
                 – Springe zu… G-64                                – Tour, zur G-34
                 – Storno durchführen G-95                         Fehlmengenkontrolle
                 – Suche Fertigwarenlager G-125                    – buchen G-80
                 – Suche, erweiterte G-13                          – durchführen G-78
                 – Versandinfo I G-48                              Fertigwarenlager
                 – Versandinfo II G-51                             – Buchungsprotokoll G-129
                 – verschieben G-66                                – Inventur, abschließen der G-128
                 – Zusatzinformation G-53                          – Inventur, starten der G-128
                 Auftragsebene                                     – Suche G-125
                 – Kurzinformation G-20                            – Übersicht G-123
                                                                   Freigabe und Druck
                 B                                                 – Lieferschein G-89, G-119, G-122, G-139
                 Benutzerdefinierte Listen                         – Lieferung für Wareneingang G-89, G-119,
                 – drucken G-136                                     G-122, G-139
                 Buchen
                 – auf Transport G-82                              G
                 – Fehlmengenkontrolle G-80                        Gestelle
                 Buchungsprotokoll                                 – Scheibenzuordnung     G-112
                 – erstellen, für Verpackte Menge   G-85
                 – Fertigwarenlager G-129
                                                                   I
                                                                   Infomenü
                 D                                                 – Übersicht G-25
                 Drucken                                           Inventur
                 – Benutzerdefinierte Listen G-136                 – abschließen, für Fertigwarenlager G-128
                 – Ergänzungsladeliste G-135                       – Fertigwarenlager, starten für G-128
                 – Ladeliste, eine G-133                           – starten, für Fertigwarenlager G-128
                 – Ladelisten, alle G-134
                 – Lieferschein G-140
                                                                   K
                 – Vorablieferschein ausdrucken G-140
                                                                   Kurzinformation
                 – Vorablieferschein, Daten eingeben für G-84,
                                                                   – Auftragsebene G-20
                   G-86, G-137
                                                                   – Lieferdatumsebene G-17
                                                                   – Positionsebene G-21
                 E                                                 – Routenebene G-19
                 Ebenen
                 – Aufbau G-9
                                                                   L
                 EK (Einkauf)
2.00 / 04-2022




                                                                   Ladeliste
                 – Info (Global), Suche starten zu G-102, G-104,
                                                                   – drucken, alle G-134
                   G-106, G-107, G-109, G-110
                                                                   – drucken, eine G-133
                 – Information, globale G-115, G-117, G-124
                                                                   – Ergänzungsladeliste G-133

                 A+W Enterprise Versandsteuerung                                                          G-143
                 Index                                                                                  Partindex




                 Lagerkommissionierung                         S
                 – Kommissionierdruck, Information zum G-93    Shift+F4
                 – Lagerabbuchung, Information zur G-93        – Scheiben-Gestellzuordnung G-112
                 Lieferanschrift                               Sperren
                 – Auftrag G-46                                – Tour, eine G-90
                 – auswählen G-87                              – Touren, alle G-91
                 – neu erfassen G-88                           Springe
                 – suchen G-87                                 – Auftrag, zu G-64
                 Lieferdatumsebene                             Starten
                 – Kurzinformation G-17                        – Fehlmengenkontrolle G-78
                 Lieferschein                                  – Inventur, Fertigwarenlager G-128
                 – drucken G-140                               Startfunktionen
                 – Freigabe und Druck G-89, G-119, G-122,      – Programmstart G-10
                   G-139                                       Storno
                 – Storno durchführen G-94                     – Auftrag G-95
                 Liefertermin                                  – Lieferschein G-94
                 – Suche G-11                                  – Versandstatus G-97
                 – verschieben G-66                            Suche
                 Liefertermine                                 – Adresse G-87
                 – Versandsteuerung, Übersicht in G-15         – Auftrag, springe zu G-64
                 Lieferterminebene                             – erweiterte Auftragssuche G-13
                 – Aufbau G-9                                  – Fertigwarenlager, Aufträge G-125
                 Lieferung Wareneingang                        – Lieferanschrift G-87
                 – Freigabe und Druck G-89, G-119, G-122,      – Liefertermin G-11
                   G-139                                       – Marktpartner G-14
                 Löschen                                       – VK/EK, Informationen zu G-102, G-104,
                 – Tourensperre G-90                             G-106, G-107, G-109, G-110

                 M                                             T
                 Marktpartner                                  Tour
                 – suchen G-14                                 – Fahrzeuginformationen einsehen       G-34
                                                               – Sperre löschen G-90
                 P                                             – Sperre setzen G-90
                 Position                                      – sperren, alle G-91
                 – Positionsinfo I G-57                        – Toureninfo G-29, G-32
                 – Positionsinfo II G-60                       – verschieben G-66
                 – verschieben nach Filterungsfunktion G-69,   Tourenebene
                   G-70, G-72                                  – Aufbau G-9
                 Positionsebene                                Toureninfo
                 – Aufbau G-9                                  – Tour G-29, G-32
                 – Kurzinformation G-21                        Transport
                 Protokoll                                     – Buchen auf G-82
                 – Fertigwarenlager, Buchungen G-129           – zurückbuchen G-83
                                                               Transportdaten
                                                               – angeben G-92
                 R
                 Route
                 – Information, gobale G-115, G-117, G-124     V
                 Routenebene                                   Verpackte Menge
                                                               – Buchungsprotokoll erstellen   G-85
2.00 / 04-2022




                 – Aufbau G-9
                 – Kurzinformation G-19                        – korrigieren G-85
                                                               Versandinfo I
                                                               – Auftrag, Details zum G-48


                 G-144                                                      A+W Enterprise Versandsteuerung
                 Partindex                                          Index




                 Versandinfo II
                 – Auftrag, Details zum G-51
                 Versandstatus
                 – stornieren G-97
                 Versandsteuerung
                 – Liefertermine, Übersicht für G-15
                 – Übersicht G-9
                 Verschieben
                 – Position, Filterung vor Verschiebung G-69,
                   G-70, G-72
                 Verschiebung (Versand)
                 – Auftrag G-66
                 – Liefertermin G-66
                 – Tour G-66
                 VK (Verkauf)
                 – Info (Global), Suche starten zu G-102, G-104,
                   G-106, G-107, G-109, G-110
                 – Information, globale G-115, G-117, G-124
                 VK/EK
                 – Info (Global), Suche starten zu G-102, G-104,
                   G-106, G-107, G-109, G-110
                 – Information, globale G-115, G-117, G-124
                 Vorablieferschein
                 – drucken durchführen G-140
                 – Drucken, Daten eingeben für G-84, G-86,
                   G-137

                 Z
                 Zurückbuchen
                 – Transport G-83
                 Zusatzinformation
                 – Auftrag G-53
2.00 / 04-2022




                 A+W Enterprise Versandsteuerung                   G-145
                 Index                          Partindex
2.00 / 04-2022




                 G-146   A+W Enterprise Versandsteuerung

