---
title: "DE AWEnterprise Lager 1.01"
category: "user_manuals"
product: "Unknown"
doc_type: "Unknown"
language: "EN"
tags: ["DE_AWEnterprise_Lager_1.01"]
version: "1.0"
last_updated: "2025-12-10"
description: "Lager              E                        deutsch             A+W Enterprise                                                                                                            Vorspann                                             Vorspann                                         In diesem Teil der Dokumentation finden Sie editorische Notizen.                                           Revisionsübersicht                                         Part"
source_file: "DE_AWEnterprise_Lager_1.01.pdf"
---


# DE AWEnterprise Lager 1.01

Lager              E




                   deutsch




        A+W Enterprise
                                                                                                           Vorspann




                                        Vorspann
                                        In diesem Teil der Dokumentation finden Sie editorische Notizen.


                                        Revisionsübersicht
                                        Part
                                        Version / Datum

                                        1.00 / 12-2015           Ersterstellung

                                        1.01 / 01-2017           Produkt- und Firmennamen angepasst.



                                        Editorial
                                        Das Editorial enthält Informationen zu folgenden Themen:
                                        •   Anmerkungen zu diesem Dokument
                                        •   Urheberrechte
                                        •   Warenzeichen
                                        •   Kontakte

                                        Anmerkungen zu diesem Dokument
                                        Diese Veröffentlichung ist ausschließlich für Endanwender von
                                        A+W Enterprise gedacht.
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
                                        © 2017, A+W Software GmbH, alle Rechte, auch des Nachdrucks, der Her-
                                        stellung von Kopien und der Übersetzung, bleiben vorbehalten.
                                        Die Dokumentation darf nur gemäß dem Lizenzvertrag ganz oder in Teilen ko-
                                        piert, in einem Archivierungssystem gespeichert oder in irgendeiner anderen
                                        Form übertragen werden. Ohne die vorherige schriftliche Genehmigung der
1.01 / 01-2017




                                        A+W Software GmbH darf die Dokumentation weder elektronisch, mecha-
                                        nisch, per Aufzeichnung oder in sonstiger Form übertragen werden.



                 A+W Enterprise Lager                                                                          E-3
                 Vorspann




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
1.01 / 01-2017




                 E-4                                                              A+W Enterprise Lager
                                                                                                                                                             Inhalt




                                        Inhalt
                                        Vorspann ................................................................................................................ E-3
                                         Revisionsübersicht .............................................................................................. E-3
                                         Editorial ............................................................................................................... E-3

                                        Softwarereferenz
                                        Übersicht ................................................................................................................. E-9
                                          Menüs im Modul Lager ........................................................................................ E-9
                                            Menü Buchung ................................................................................................. E-9
                                            Menü Stammdaten ......................................................................................... E-10
                                            Menü Inventur ................................................................................................ E-10
                                            Menü Bewertung ............................................................................................ E-11
                                            Menü Infosystem ............................................................................................ E-11
                                            Menü Druck .................................................................................................... E-12
                                            Menü System ................................................................................................. E-12
                                            Zusatzmenü ................................................................................................... E-12
                                        Suchfunktionen ..................................................................................................... E-14
                                        Lagerverwaltung ................................................................................................... E-15
                                          Lagereingang ................................................................................................... E-16
                                            Lagereingang – Stück .................................................................................... E-16
                                            Lagereingang – Menge .................................................................................. E-20
                                          Lagerausgang ................................................................................................... E-22
                                          Kistenlagereingang ............................................................................................ E-23
                                            Kistenlagereingang – Stück ........................................................................... E-23
                                            Kistenlagereingang – Menge ......................................................................... E-26
                                          Kistenlagerausgang ........................................................................................... E-28
                                          Fachlagereingang .............................................................................................. E-29
                                            Fachlagereingang – Stück ............................................................................. E-29
                                            Fachlagereingang – Menge ........................................................................... E-32
                                          Fachlagerausgang ............................................................................................. E-34
                                          Stapellagereingang ........................................................................................... E-35
                                          Stapellageränderung ......................................................................................... E-36
                                          Gestelllagereingang .......................................................................................... E-38
                                          Gestelllagerausgang ......................................................................................... E-41
                                            Gestelllagerausgang – Auftragsbezogen ....................................................... E-41
                                            Gestelllagerausgang – Umbuchung ............................................................... E-43
                                          Lagerausgang (Auftragsbezogen) .................................................................... E-45
                                          Buchungskorrektur – Übersicht ......................................................................... E-47
                                          Buchungskorrektur – Details ............................................................................. E-48
                                        Stammdatenverwaltung ........................................................................................ E-50
                                          Lagerraumverwaltung ....................................................................................... E-50
                                          Artikelstammdaten Lager ................................................................................. E-51
                                        Inventurverwaltung ............................................................................................... E-53
                                          Inventur – Standardlager ................................................................................... E-53
                                          Inventur – Kistenlager ....................................................................................... E-56
                                          Inventur – Fachlager ......................................................................................... E-58
                                          Inventur – Stapellager ....................................................................................... E-59
                                          Inventur – Gestelllager ...................................................................................... E-60
                                        Bewertung ............................................................................................................. E-63
                                          Bestandsbewertung – Standardlager ................................................................ E-63
                                          Bestandsbewertung – Kistenlager ..................................................................... E-66
1.01 / 01-2017




                                          Bestandsbewertung – Fachlager ....................................................................... E-67
                                          Bestandsbewertung – Stapellager .................................................................... E-68
                                          Bestandsbewertung – Gestelllager ................................................................... E-69




                 A+W Enterprise Lager                                                                                                                           E-5
                 Inhalt




                          Informationssystem ............................................................................................... E-70
                            Info-Lager-Artikel .............................................................................................. E-71
                               Info-Lager-Artikel – Filterdialog ...................................................................... E-71
                               Info-Lager-Artikel – Trefferliste ...................................................................... E-72
                               Info-Lager-Artikel – Trefferliste-Details .......................................................... E-73
                            Info-Lager-Varianten ........................................................................................ E-75
                               Info-Lager-Varianten – Filterdialog ................................................................ E-75
                               Info-Lager-Varianten – Trefferliste ................................................................. E-76
                               Info-Lager-Varianten – Trefferliste-Details ..................................................... E-77
                            Info-Lager-Fächer ............................................................................................. E-79
                               Info-Lager-Fächer – Filterdialog ..................................................................... E-79
                               Info-Lager-Fächer – Trefferliste ..................................................................... E-80
                               Info-Lager-Fächer – Trefferliste-Details ......................................................... E-81
                            Info-Lager-Gestelle ............................................................................................ E-82
                               Info-Lager-Gestelle – Filterdialog ................................................................... E-82
                               Info-Lager-Gestelle – Trefferliste-Allgemein .................................................. E-83
                               Info-Lager-Gestelle – Trefferliste-Details ....................................................... E-84
                            Info-Lager-Stapel .............................................................................................. E-85
                               Info-Lager-Stapel – Filterdialog ...................................................................... E-85
                               Info-Lager-Stapel – Trefferliste ...................................................................... E-86
                               Info-Lager-Stapel – Trefferliste-Details .......................................................... E-87
                            Info-Lager-Blätter .............................................................................................. E-88
                               Info-Lager-Blätter – Filterdialog ..................................................................... E-88
                               Info-Lager-Blätter – Trefferliste ...................................................................... E-89
                            Info-Lager-Historie ............................................................................................. E-91
                               Info-Lager-Historie – Filterdialog .................................................................... E-91
                               Info-Lager-Historie – Trefferliste .................................................................... E-92
                               Info-Lager-Historie – Trefferliste-Details ........................................................ E-94
                            Aufträge/Bestellungen ....................................................................................... E-96
                               Aufträge/Bestellungen – Filterdialog .............................................................. E-96
                               Aufträge/Bestellungen – Trefferliste ............................................................... E-97
                               Aufträge/Bestellungen – Trefferliste-Details .................................................. E-98
                            Buchungsstatus .............................................................................................. E-100
                               Buchungsstatus – Ungebucht ...................................................................... E-100
                               Buchungsstatus – Fehler ............................................................................. E-102
                               Buchungsstatus – Inventur .......................................................................... E-103
                               Buchungsstatus – Korrektur ......................................................................... E-104
                            Lagerinformationen – Pickliste ........................................................................ E-105
                            Lagerinformationen – Trefferliste .................................................................... E-106
                            LVR-Status ...................................................................................................... E-107
                            Reichweite – Bestandsprognose ..................................................................... E-107
                            Reichweite – Trefferliste .................................................................................. E-108
                            Dispositiver Bestand ........................................................................................ E-109
                            Bestandsprognose .......................................................................................... E-110
                          Druck .................................................................................................................. E-112
                            Kistenetiketten drucken .................................................................................. E-112
                            Listendruck ..................................................................................................... E-113
                          Systemverwaltung .............................................................................................. E-114
                            Lagerprotokoll löschen ................................................................................... E-114
                            Lager-Preiskorrektur ....................................................................................... E-114
                          Servicefunktionen ............................................................................................... E-116

                          Partindex
                          Index Lager ......................................................................................................... E-119
1.01 / 01-2017




                 E-6                                                                                              A+W Enterprise Lager
Lager                 E

         Softwarereferenz




        A+W Enterprise
                 Softwarereferenz                                                                          Übersicht




                                        Übersicht
                                        Im Modul Lager verfügen Sie über alle Funktionen, die zur erfolgreichen La-
                                        gerverwaltung erforderlich sind, z. B. Bestandsführungen, Bestandsbuchun-
                                        gen, Inventuren sowie die Planungen der Artikelzugänge und Artikelabgänge.
                                        In diesem Modul werden alle Preise als Nettopreise angegeben.
                                        Im Part Lager finden Sie folgende Themen:
                                        •   “Lagerverwaltung” auf Seite E-15
                                        •   “Stammdatenverwaltung” auf Seite E-50
                                        •   “Inventurverwaltung” auf Seite E-53
                                        •   “Bewertung” auf Seite E-63
                                        •   “Informationssystem” auf Seite E-70
                                        •   “Druck” auf Seite E-112
                                        •   “Systemverwaltung” auf Seite E-114
                                        •   “Servicefunktionen” auf Seite E-116


                                        Menüs im Modul Lager
                                        Über folgende Menüs öffnen Sie die Dialoge des Moduls Lager:
                                        •   “Menü Buchung” auf Seite E-9
                                        •   “Menü Stammdaten” auf Seite E-10
                                        •   “Menü Inventur” auf Seite E-10
                                        •   “Menü Bewertung” auf Seite E-11
                                        •   “Menü Infosystem” auf Seite E-11
                                        •   “Menü Druck” auf Seite E-12
                                        •   “Menü System” auf Seite E-12


                                        Menü Buchung
                                        Im Menü Buchung finden Sie auf der ersten Ebene folgende Einträge:
                                        •   Eingang:
                                             “Lagereingang” auf Seite E-16
                                        •   Ausgang:
                                             “Lagerausgang” auf Seite E-22
                                        •   Kisteneingang:
                                             “Kistenlagereingang” auf Seite E-23
                                        •   Kistenausgang:
                                             “Kistenlagerausgang” auf Seite E-28
                                        •   Facheingang:
                                             “Fachlagereingang” auf Seite E-29
                                        •   Fachausgang:
1.01 / 01-2017




                                             “Fachlagerausgang” auf Seite E-34
                                        •   Stapelverwaltung:
                                            Kundenspezifische Funktion, wird ausführlich in einem separaten Part er-
                                            klärt.


                 A+W Enterprise Lager                                                                           E-9
                 Übersicht                                                                Softwarereferenz




                             •   Stapeleingang:
                                  “Stapellagereingang” auf Seite E-35
                             •   Stapeländerung:
                                  “Stapellageränderung” auf Seite E-36
                             •   Gestelleingang:
                                  “Gestelllagereingang” auf Seite E-38
                             •   Gestellausgang:
                                  “Gestelllagerausgang” auf Seite E-41
                             •   Stapelbuchung (Vorgangsbez.):
                                 Kundenspezifische Funktion, wird ausführlich in einem separaten Part er-
                                 klärt.
                             •   Ausgang (Auftragsbezogen):
                                  “Lagerausgang (Auftragsbezogen)” auf Seite E-45
                             •   Korrektur:
                                  “Buchungskorrektur – Übersicht” auf Seite E-47


                             Menü Stammdaten
                             Im Menü Stammdaten finden Sie folgende Einträge:
                             •   Raum:
                                  “Lagerraumverwaltung” auf Seite E-50
                             •   Artikel:
                                  “Artikelstammdaten Lager” auf Seite E-51
                             •   Fächer:
                                 Kundenspezifische Funktion, wird ausführlich in einem separaten Part er-
                                 klärt.
                             •   Stapeltypen:
                                 Kundenspezifische Funktion, wird ausführlich in einem separaten Part er-
                                 klärt.


                             Menü Inventur
                             Im Menü Inventur finden Sie folgende Einträge:
                             •   Lager:
                                  “Inventur – Standardlager” auf Seite E-53
                             •   Kistenlager:
                                  “Inventur – Kistenlager” auf Seite E-56
                             •   Fachlager:
                                  “Inventur – Fachlager” auf Seite E-58
                             •   Stapellager:
                                  “Inventur – Stapellager” auf Seite E-59
                             •   Gestelllager:
                                  “Inventur – Gestelllager” auf Seite E-60
1.01 / 01-2017




                 E-10                                                                A+W Enterprise Lager
                 Softwarereferenz                                                                       Übersicht




                                        Menü Bewertung
                                        Im Menü Bewertung finden Sie folgende Einträge:
                                        •   Lager:
                                             “Bestandsbewertung – Standardlager” auf Seite E-63
                                        •   Kistenlager:
                                             “Bestandsbewertung – Kistenlager” auf Seite E-66
                                        •   Fachlager:
                                             “Bestandsbewertung – Fachlager” auf Seite E-67
                                        •   Stapellager:
                                             “Bestandsbewertung – Stapellager” auf Seite E-68
                                        •   Gestelllager:
                                             “Bestandsbewertung – Gestelllager” auf Seite E-69


                                        Menü Infosystem
                                        Im Menü Infosystem finden Sie auf der ersten Ebene folgende Einträge:
                                        •   Artikel:
                                             “Info-Lager-Artikel – Filterdialog” auf Seite E-71
                                        •   Variante:
                                             “Info-Lager-Varianten – Filterdialog” auf Seite E-75
                                        •   Fach:
                                             “Info-Lager-Fächer” auf Seite E-79
                                        •   Gestell:
                                             “Info-Lager-Gestelle – Filterdialog” auf Seite E-82
                                        •   Stapel:
                                             “Info-Lager-Stapel – Filterdialog” auf Seite E-85
                                        •   Blatt:
                                             “Info-Lager-Blätter – Filterdialog” auf Seite E-88
                                        •   Historie:
                                             “Info-Lager-Historie – Filterdialog” auf Seite E-91
                                        •   Aufträge/Bestellungen:
                                             “Aufträge/Bestellungen – Filterdialog” auf Seite E-96
                                        •   Buchungsstatus:
                                             “Menü 2. Ebene – Buchungsstatus” auf Seite E-12
                                        •   Auftragsliste:
                                             “Lagerinformationen – Pickliste” auf Seite E-105
                                        •   LVR-Status:
                                            Dieser Dialog wird zur Zeit nicht genutzt.
                                        •   Reichweite:
                                             “Reichweite – Bestandsprognose” auf Seite E-107
                                        •   Dispositiver Bestand:
                                             “Dispositiver Bestand” auf Seite E-109
                                        •   Prognose:
1.01 / 01-2017




                                             “Bestandsprognose” auf Seite E-110




                 A+W Enterprise Lager                                                                       E-11
                 Übersicht                                                               Softwarereferenz




                             Menü 2. Ebene – Buchungsstatus
                             •   Ungebucht:
                                  “Buchungsstatus – Ungebucht” auf Seite E-100
                             •   Fehler:
                                  “Buchungsstatus – Fehler” auf Seite E-102
                             •   Inventur:
                                  “Buchungsstatus – Inventur” auf Seite E-103


                             Menü Druck
                             Im Menü Druck finden Sie folgende Einträge:
                             •   Etiketten:
                                  “Kistenetiketten drucken” auf Seite E-112
                             •   Listendruck:
                                 Der Dialog wird im Part Verkauf beschrieben.
                                  Verkauf, “Listendruck” auf Seite D-162


                             Menü System
                             Im Menü System finden Sie folgende Einträge:
                             •   Lagerprotokoll löschen:
                                  “Lagerprotokoll löschen” auf Seite E-114
                             •   Preiskorrektur:
                                  “Lager-Preiskorrektur” auf Seite E-114


                             Zusatzmenü
                             <F4>
                             Im Zusatzmenü finden Sie folgende Einträge:

                             Menü 1. Ebene
                             •   PKZ-Preise:
                                 In den Lagereingängen können Sie Artikeln vordefinierte Preise über Preis-
                                 kennzeichen zuweisen. Die Preiskennzeichen können Sie aus einer vorde-
                                 finierten Liste auswählen.
                             •   Nullpreisbuchung:
                                 In den Lagereingängen können Sie Artikel den Preis = 0 zuweisen.
                             •   Umbuchen:
                                 Ausgewählten Datensatz in ein anderes Lager umbuchen. Die Buchung
                                 muss mit [OK] abgeschlossen werden.
                             •   Objektbuchung:
                                 Ausgewählten Datensatz einem Objekt (z. B. Baustelle) zuweisen.
                             •   Kisten:
                                  “Menü 2. Ebene – Kisten” auf Seite E-13
1.01 / 01-2017




                 E-12                                                              A+W Enterprise Lager
                 Softwarereferenz                                                                           Übersicht




                                        Menü 2. Ebene – Kisten
                                        •   Kiste abbuchen:
                                            Entfernt die Kiste des aktuellen Datensatzes aus dem Kistenlager und
                                            bucht die Artikel der Kiste automatisch in das Normallager. Die Buchung
                                            muss mit [OK] abgeschlossen werden.
                                        •   Kiste auflösen:
                                            Entfernt die Kiste des aktuellen Datensatzes aus dem Kistenlager und
                                            bucht die Artikel in ein Ziellager. Die Buchung muss mit [OK] abgeschlos-
                                            sen werden.
                                        •   Einzelblattinformation:
                                             “Menü 3. Ebene – Einzelblattinformationen” auf Seite E-13

                                        Menü 3. Ebene – Einzelblattinformationen
                                        •   Anzeige:
                                             “Fußbereich – Einzelblattinformationen” auf Seite E-25
                                        •   Editieren:
                                             “Fußbereich – Einzelblattinformationen” auf Seite E-25
1.01 / 01-2017




                 A+W Enterprise Lager                                                                           E-13
                 Suchfunktionen                                                           Softwarereferenz




                                  Suchfunktionen
                                  Informationen können Sie über die Suchfunktionen des Informationssystems
                                  suchen, z. B. zu Artikeln, Lagerarten, Aufträgen oder Bestellungen.
                                   “Informationssystem” auf Seite E-70
1.01 / 01-2017




                 E-14                                                               A+W Enterprise Lager
                 Softwarereferenz                                                                Lagerverwaltung




                                        Lagerverwaltung
                                        In der Lagerverwaltung erfassen und bearbeiten Sie die Buchungen für das
                                        Warenlager, z. B. Lagereingänge für Artikel oder Buchungskorrekturen.
                                        In diesem Abschnitt sind folgende Dialoge erklärt:
                                        •   “Lagereingang” auf Seite E-16
                                        •   “Lagerausgang” auf Seite E-22
                                        •   “Kistenlagereingang” auf Seite E-23
                                        •   “Kistenlagerausgang” auf Seite E-28
                                        •   “Fachlagereingang” auf Seite E-29
                                        •   “Fachlagerausgang” auf Seite E-34
                                        •   “Stapellagereingang” auf Seite E-35
                                        •   “Stapellageränderung” auf Seite E-36
                                        •   “Gestelllagereingang” auf Seite E-38
                                        •   “Gestelllagerausgang” auf Seite E-41
                                        •   “Lagerausgang (Auftragsbezogen)” auf Seite E-45
                                        •   “Buchungskorrektur – Übersicht” auf Seite E-47
                                        •   “Buchungskorrektur – Details” auf Seite E-48
1.01 / 01-2017




                 A+W Enterprise Lager                                                                       E-15
                 Lagerverwaltung                                                                    Softwarereferenz




                                         Lagereingang
                                         Buchung > Eingang
                                         In diesem Dialog erfassen und buchen Sie die Lagereingänge für die Lagerar-
                                         tikel des ausgewählten Lagers.
                                         In diesem Dialog finden Sie folgende Register:
                                         •   “Lagereingang – Stück” auf Seite E-16
                                         •   “Lagereingang – Menge” auf Seite E-20


                                         Lagereingang – Stück
                                         Buchung > Eingang > Stück




                 Abb. E-1   Lagereingang – Stück


                                         In diesem Register erfassen und buchen Sie die Lagereingänge in den Stück-
                                         zahlen der aktuellen Artikelvariante. Sie können in ein anderes Lager wech-
                                         seln, indem Sie eine andere Lagernummer eingeben. Das gilt auch für Lager
                                         eines anderen Lagertyps.
                                         Die Lagereingänge für Kisten, Fächer, Stapel und Gestelle buchen Sie an fol-
                                         gender Stelle:
                                          “Kistenlagereingang” auf Seite E-23
                                          “Fachlagereingang” auf Seite E-29
                                          “Stapellagereingang” auf Seite E-35
1.01 / 01-2017




                                          “Gestelllagereingang” auf Seite E-38




                 E-16                                                                         A+W Enterprise Lager
                 Softwarereferenz                                                                    Lagerverwaltung




                                        Sie können folgende Tastaturbefehle ausführen:
                                        •   Mit <Strg> + <F8> können Sie im ersten Feld zwischen dem Dialog Lage-
                                            reingang und Lagerausgang wechseln.
                                        •   Mit <F5> können Sie aus einer Spalte in die variantenbezogenen Angaben
                                            im Fußbereich wechseln.
                                        •   Mit <Pos1> verwerfen Sie Ihre Eingabe im Fußbereich.
                                        •   Mit <Ende> können Sie im Fußbereich Ihre Eingabe speichern und in den
                                            Rumpfbereich wechseln.
                                        •   Mit <Shift> + <F12> können Sie für den aktuellen Buchungssatz ein neues
                                            Datum eingeben.

                                        Kopfbereich

                                        Artikel Artikelnummer und Artikelbezeichnung.

                                        Lager Lagernummer und Lagerbezeichnung.

                                        Lieferant Lieferantennummer und Lieferantenname.

                                        Gesamtbestand Gesamtbestand des Artikels, einschließlich aller Artikelvari-
                                        anten.

                                        Gesamtwert Gesamtbetrag des Lagerartikels.

                                        Buchungsstatus Status der Buchungen im Lager.

                                        Buchungsstatus mit        Bedeutung
                                        Farbkennzeichen

                                            grau                  Im Lagereingang sind alle Buchungspositionen vom
                                                                  Prozess (Programm) gebucht worden.

                                            rot                   Im Lagereingang ist mindestens eine
                                                                  Buchungsposition vom Prozess (Programm) nicht oder
                                                                  noch nicht gebucht worden.

                                        Tab. E-1     Buchungsstatus des Lagers

                                        Letzte Änderung am, von Datum der letzten Änderung am Buchungssatz
                                        und Name des Anwenders, der die letzte Buchung ausgeführt hat.

                                        Rumpfbereich
                                        In diesem Bereich buchen Sie die Bestände und Preise der Artikelvariante in
                                        Stückzahlen.
                                        •   Variante:
                                            Maßvariante des Artikels. Mit <F9> können Sie die Variantenauswahl auf-
                                            rufen. Dabei werden nur die Varianten angezeigt, die dem aktuellen Artikel
                                            in den Stammdaten zugewiesen sind.
1.01 / 01-2017




                                        •   Lagerbez.:
                                            Lagerbezeichnung.




                 A+W Enterprise Lager                                                                            E-17
                 Lagerverwaltung                                                                   Softwarereferenz




                                   Bestände (Stück) Lagerbestand der Variante in Stückzahlen.
                                   •   Alt:
                                       Alter Artikelbestand im Lager, bevor gebucht wird.
                                   •   Buchung:
                                       Artikelbestand, der gebucht wird.
                                   •   Neu:
                                       Neu berechneter Artikelbestand. Dieser Bestand wird übernommen, wenn
                                       der neue Artikel gebucht wird. Wenn Sie den Dialog mit <Pos1> verlassen,
                                       wird der alte Lagerbestand beibehalten.

                                   Preise Die Anzeige der Währung richtet sich nach der Eigenwährung, die bei
                                   der Installation festgelegt wurde.
                                   • € / qm:
                                      Artikelpreis des Lieferanten in eigener Währung pro Mengeneinheit.
                                   • Preis:
                                      Gesamtpreis des Artikels.
                                   • (Spalte ohne Bezeichnung):
                                      Buchungsstatus der Artikelposition.

                                   Buchungsstatus mit         Bedeutung
                                   Farbkennzeichen

                                       grau                   Artikelposition ist vom Prozess (Programm) gebucht
                                                              worden.

                                       rot                    Artikelposition ist vom Prozess (Programm) nicht oder
                                                              noch nicht gebucht worden.

                                   Tab. E-2     Buchungsstatus der Artikelposition

                                   Fußbereich – Variantenbezogene Angaben

                                   Objekt Bezeichnung des Objekts bei auftragsbezogenen Lagerartikeln,
                                   z. B. Baustelle des Kunden.

                                   Kostenstelle Bezeichnung der Kostenstelle für statistische Auswertungen.

                                   Bemerkung Textfeld für zusätzliche Informationen.

                                   Mindestbestand Minimal zulässiger Lagerbestand des Artikels, um Produk-
                                   tionsengpässe zu verhindern.

                                   Alarmbestand Stückzahl des Artikelbestands, die einen Bestellvorschlag im
                                   Einkauf anlegt. Durch Alarmbestände können Sie eine Unterdeckung des La-
                                   gers verhindern.

                                   Maximalbestand Maximal zulässiger Lagerbestand des Artikels, um Lager-
                                   kosten zu minimieren.
1.01 / 01-2017




                 E-18                                                                        A+W Enterprise Lager
                 Softwarereferenz                                                                  Lagerverwaltung




                                           Automatische Bestellvorschläge durch das Lager
                                           Wenn der definierte Alarmbestand bei einer Ausgangsbuchung unterschrit-
                                           ten wird, werden durch das Lager automatisch Bestellvorschläge im Ein-
                                           kauf angelegt. Automatische Bestellvorschläge werden auch durch die
                                           nächtliche Buchungsroutine im Einkauf angelegt, wenn der Artiklebestand
                                           langfristig unter den Mindestbestand fällt. Die Menge im Bestellvorschlag
                                           richtet sich nach dem definierten Maximalbestand. Diese Bestellvorschlä-
                                           ge werden vom Einkauf freigeschaltet und in Bestellungen überführt.

                                        Gesamtpreis Gesamtpreis der Artikelvariante.

                                        Durchschnittspreis Durchschnittlicher Einkaufspreis der Artikelvariante im
                                        Lager.

                                        Höchstpreis Höchster Einkaufspreis der Artikelvariante im Lager.

                                        Niedrigstpreis Niedrigster Einkaufspreis der Artikelvariante im Lager.

                                        LIFO-Gesamtpreis Gesamtpreis der Artikelvariante im Lager, wenn die zu-
                                        letzt eingelagerten Lagerartikel als erste Artikel ausgelagert werden.

                                        FIFO-Gesamtpreis Gesamtpreis der Artikelvariante im Lager, wenn die zu-
                                        erst eingelagerten Lagerartikel als erste Artikel ausgelagert werden.

                                           Beispiel

                                           1. Lagereingang 10 Stück zu 10,- € = 100,- €
                                           2. Lagereingang 10 Stück zu 15,- € = 150,- €
                                           Gesamtwert beider Lagereingänge = 250,- €

                                           Lagerabgang 10 Stück nach LIFO = -150,- €
                                           LIFO-Gesamtpreis = 100,- €

                                           Lagerabgang 10 Stück nach FIFO = -100,- €
                                           FIFO-Gesamtpreis = 150,- €
1.01 / 01-2017




                 A+W Enterprise Lager                                                                            E-19
                 Lagerverwaltung                                                                      Softwarereferenz




                                        Lagereingang – Menge
                                        Buchung > Eingang > Menge




                 Abb. E-2   Lagereingang – Menge


                                        In diesem Register erfassen und buchen Sie die Lagereingänge in den Men-
                                        geneinheiten der aktuellen Artikelvariante.
                                        Das Register Menge ist wie das Register Stück aufgebaut.
                                         “Kopfbereich” auf Seite E-17
                                         “Fußbereich – Variantenbezogene Angaben” auf Seite E-18

                                        Rumpfbereich
                                        In diesem Bereich buchen Sie die Bestände und Preise der Artikelvariante in
                                        Mengeneinheiten.
                                        •   Variante:
                                            Maßvariante des Artikels. Mit <F9> können Sie die Variantenauswahl auf-
                                            rufen. Dabei werden nur die Varianten angezeigt, die dem aktuellen Artikel
                                            in den Stammdaten zugewiesen sind.
                                        •   Farbe:
                                            Farbe der Maßvariante des Artikels.

                                        Bestände (Mengeneinheit) Lagerbestand der Variante in den Mengen, die
                                        für diese Artikelvariante in den Stammdaten definiert ist.
                                        •   Alt:
1.01 / 01-2017




                                            Alter Artikelbestand im Lager, bevor gebucht wird.
                                        •   Buchung:
                                            Artikelbestand, der gebucht wird.


                 E-20                                                                            A+W Enterprise Lager
                 Softwarereferenz                                                                       Lagerverwaltung




                                        •   Neu:
                                            Neu berechneter Artikelbestand. Dieser Bestand wird übernommen, wenn
                                            der neue Artikel gebucht wird. Wenn Sie den Dialog mit <Pos1> verlassen,
                                            wird der alte Lagerbestand beibehalten.

                                        Preise Die Anzeige der Währung richtet sich nach der Eigenwährung, die bei
                                        der Installation festgelegt wurde.
                                        • € / qm:
                                           Artikelpreis des Lieferanten in eigener Währung pro Mengeneinheit.
                                        • Preis:
                                           Gesamtpreis des Artikels.
                                        • (Spalte ohne Bezeichnung):
                                           Buchungsstatus der Artikelposition.

                                        Buchungsstatus mit         Bedeutung
                                        Farbkennzeichen

                                            grau                   Artikelposition ist vom Prozess (Programm) gebucht
                                                                   worden.

                                            rot                    Artikelposition ist vom Prozess (Programm) nicht oder
                                                                   noch nicht gebucht worden.

                                        Tab. E-3     Buchungsstatus der Artikelposition
1.01 / 01-2017




                 A+W Enterprise Lager                                                                                E-21
                 Lagerverwaltung                                                                  Softwarereferenz




                                       Lagerausgang
                                       Buchung > Ausgang




                 Abb. E-3   Lagerausgang


                                       In diesem Dialog erfassen und buchen Sie den Lagerausgang, z. B., wenn La-
                                       gerartikel an die Produktion geliefert werden. Die Lagerausgänge für Kisten,
                                       Fächer, Stapel, Gestelle und auftragsbezogenen Warenausgänge buchen Sie
                                       an folgender Stelle:
                                        “Kistenlagerausgang” auf Seite E-28
                                        “Fachlagerausgang” auf Seite E-34
                                        “Stapellageränderung” auf Seite E-36
                                        “Gestelllagerausgang” auf Seite E-41
                                        “Lagerausgang (Auftragsbezogen)” auf Seite E-45
                                       Sie können folgende Tastaturbefehle ausführen:
                                       •   Mit <Strg> + <F8> können Sie im ersten Feld zwischen dem Dialog Lage-
                                           reingang und Lagerausgang wechseln.
                                       •   Mit <F5> können Sie aus einer Spalte in die variantenbezogenen Angaben
                                           im Fußbereich wechseln.
                                       •   Mit <Shift> + <F12> können Sie für den aktuellen Buchungssatz ein neues
                                           Datum eingeben.
                                       Die Register, Felder und Spalten sind an folgender Stelle beschrieben:
                                        “Lagereingang” auf Seite E-16
1.01 / 01-2017




                                       Die Werte in den Feldern zeigen jeweils die abzubuchenden Mengen an.




                 E-22                                                                       A+W Enterprise Lager
                 Softwarereferenz                                                                     Lagerverwaltung




                                          Kistenlagereingang
                                          Buchung > Kisteneingang
                                          In diesem Dialog buchen Sie die Lagereingänge für komplette Kisten,
                                          z. B. Gitterboxen mit 50 gleichen Scheiben.
                                          In diesem Dialog finden Sie folgende Register:
                                          •   “Kistenlagereingang – Stück” auf Seite E-23
                                          •   “Kistenlagereingang – Menge” auf Seite E-26


                                          Kistenlagereingang – Stück
                                          Buchung > Kisteneingang > Stück




                 Abb. E-4   Kistenlagereingang – Stück, Kistenlager und Einzelblattkistenlager


                                          In diesem Register buchen Sie die Lagereingänge für komplette Kisten. Sie
                                          können über die Auswahl der Lagerart im Feld Lager auswählen, ob Sie die
                                          Lagereingänge ins Kistenlager oder ins Einzelblattkistenlager buchen.
                                          Wenn Sie ein Einzelblattkistenlager auswählen, können Sie die Blätter einzeln
1.01 / 01-2017




                                          in Kisten buchen.
                                           “Fußbereich – Einzelblattinformationen” auf Seite E-25



                 A+W Enterprise Lager                                                                             E-23
                 Lagerverwaltung                                                                   Softwarereferenz




                                   Sie können folgende Tastaturbefehle ausführen:
                                   •   Mit <Strg> + <F8> können Sie im ersten Feld zwischen dem Dialog Kisten-
                                       lagereingang und Kistenlagerausgang wechseln.
                                   •   Mit <F5> können Sie aus einer Spalte in die kistenbezogenen Angaben im
                                       Fußbereich (linke Seite) wechseln.
                                   •   Mit <Shift> + <F8> können Sie aus einer Spalte in die variantenbezogenen
                                       Angaben im Fußbereich (rechte Seite) wechseln.
                                   •   Mit <Shift> + <F12> können Sie für den aktuellen Buchungssatz ein neues
                                       Datum eingeben.

                                   Kopfbereich
                                   Die Felder sind an folgender Stelle beschrieben:
                                    “Lagereingang” auf Seite E-16
                                   Zusätzlich wird folgendes Feld beschrieben:

                                   Lager Lagernummer und Lagerbezeichnung. Wenn Sie die Nummer für ein
                                   Einzelblattkistenlager eingeben, können Sie für jede Kiste die Scheiben ein-
                                   zeln erfassen.
                                    “Fußbereich – Einzelblattinformationen” auf Seite E-25

                                   Rumpfbereich
                                   In diesem Bereich buchen Sie die Bestände und Preise der Artikel in Stück-
                                   zahlen.
                                   •   Variante:
                                       Maßvariante des Artikels. Mit <F9> können Sie die Variantenauswahl auf-
                                       rufen. Dabei werden nur die Varianten angezeigt, die dem aktuellen Artikel
                                       in den Stammdaten zugewiesen sind.
                                   •   Kiste:
                                       Kistennummer.
                                   •   Kistenbezeichnung:
                                       Bezeichnung der Kiste.
                                   •   Lieferant:
                                       Lieferantennummer.
                                   •   Verpackungsart:
                                       Kennzeichen der Verpackungsart, z. B. 13 = Kleine Holzkiste.
                                   •   Neu:
                                       Neu berechneter Artikelbestand. Dieser Bestand wird übernommen, wenn
                                       der neue Artikel gebucht wird. Wenn Sie den Dialog mit <Pos1> verlassen,
                                       wird der alte Lagerbestand beibehalten.

                                   Bestände Lagerbestand der Variante in Stückzahlen. Mit <F2> können Sie
                                   durch folgende Anzeigen wechseln:
                                   •   Alt:
                                       Alter Artikelbestand im Lager, bevor gebucht wird.
1.01 / 01-2017




                                   •   Buchung:
                                       Artikelbestand, der gebucht wird.




                 E-24                                                                         A+W Enterprise Lager
                 Softwarereferenz                                                                       Lagerverwaltung




                                        •   Neu:
                                            Neu berechneter Artikelbestand. Dieser Bestand wird übernommen, wenn
                                            der neue Artikel gebucht wird. Wenn Sie den Dialog mit <Pos1> verlassen,
                                            wird der alte Lagerbestand beibehalten.

                                        Preise Die Anzeige der Währung richtet sich nach der Eigenwährung, die bei
                                        der Installation festgelegt wurde.
                                        • € / qm:
                                           Artikelpreis des Lieferanten in eigener Währung pro Mengeneinheit.
                                        • Preis:
                                           Gesamtpreis des Artikels.
                                        • (Spalte ohne Bezeichnung):
                                           Buchungsstatus der Artikelposition.

                                        Buchungsstatus mit         Bedeutung
                                        Farbkennzeichen

                                            grau                   Artikelposition ist vom Prozess (Programm) gebucht
                                                                   worden.

                                            rot                    Artikelposition ist vom Prozess (Programm) nicht oder
                                                                   noch nicht gebucht worden.

                                        Tab. E-4     Buchungsstatus der Artikelposition

                                        Fußbereich – Kistenbezogene Angaben
                                        Die Felder sind an folgender Stelle beschrieben:
                                         “Lagereingang” auf Seite E-16
                                        Zusätzlich werden folgende Felder beschrieben:

                                        Lieferant Lieferantennummer und Lieferantenname.

                                        Verpackungsart Kennzeichen der Verpackungsart.

                                        Reserviert Auftragsnummer, für die die Kiste reserviert wurde.

                                        Etikett Anzeige für den Etikettendruck.
                                        • J = Etiketten drucken.
                                        • N = Keine Etiketten drucken.

                                        Fußbereich – Einzelblattinformationen
                                        Die Einzelblattinformationen können Sie nur aufrufen, wenn Sie im Kopfbe-
                                        reich im Feld Lager ein Einzelblattkistenlager ausgewählt haben.
                                        •   Mit <Shift> + <F12> können Sie sich die Einzelblattinformationen anzeigen
                                            lassen.
                                        •   Mit <Strg> + <E> können Sie die Einzelblattinformationen bearbeiten.
1.01 / 01-2017




                                        Im Dialog rechts unten wird die Tabelle für die Einzelblattinformationen mit den
                                        folgenden Spalten angezeigt:




                 A+W Enterprise Lager                                                                                E-25
                 Lagerverwaltung                                                                      Softwarereferenz




                                        •   Blatt:
                                            Nummer des Blattes.
                                        •   Bezeichnung:
                                            Bezeichnung des Blattes.
                                        •   EU/Stück:
                                            Stückpreis des Blattes.
                                        •   Ausbeute:
                                            Ausbeute in Prozent.
                                        •   Reserviert:
                                            Reservierungskennzeichen.
                                            – J = Variante ist für einen Vorgang reserviert.
                                            – N = Variante ist nicht für einen Vorgang reserviert.


                                        Kistenlagereingang – Menge
                                        Buchung > Kisteneingang > Menge




                 Abb. E-5   Kistenlagereingang – Menge


                                        In diesem Register buchen Sie die Bestände und Preise der Artikel in Mengen-
                                        einheit.
                                        Das Register Menge ist wie das Register Stück aufgebaut.
                                         “Kopfbereich” auf Seite E-24
                                         “Fußbereich – Kistenbezogene Angaben” auf Seite E-25
1.01 / 01-2017




                 E-26                                                                            A+W Enterprise Lager
                 Softwarereferenz                                                                       Lagerverwaltung




                                        Rumpfbereich
                                        In diesem Bereich buchen Sie die Bestände und Preise der Artikel in Mengen-
                                        einheit.
                                        •   Variante:
                                            Maßvariante des Artikels. Mit <F9> können Sie die Variantenauswahl auf-
                                            rufen. Dabei werden nur die Varianten angezeigt, die dem aktuellen Artikel
                                            in den Stammdaten zugewiesen sind.
                                        •   Kiste:
                                            Kistennummer.
                                        •   Kistenbezeichnung:
                                            Bezeichnung der Kiste.
                                        •   Lieferant:
                                            Lieferantennummer.
                                        •   Verpackungsart:
                                            Kennzeichen der Verpackungsart, z. B. 13 = Kleine Holzkiste.
                                        •   Neu:
                                            Neu berechneter Artikelbestand. Dieser Bestand wird übernommen, wenn
                                            der neue Artikel gebucht wird. Wenn Sie den Dialog mit <Pos1> verlassen,
                                            wird der alte Lagerbestand beibehalten.

                                        Bestände Lagerbestand der Variante in der Mengeneinheit, die in den
                                        Stammdaten definiert ist.
                                        •   ME:
                                            Neu berechneter Artikelbestand in Mengeneinheiten. Dieser Bestand wird
                                            übernommen, wenn der neue Artikel gebucht wird. Wenn Sie den Dialog
                                            mit <Pos1> verlassen, wird der alte Lagerbestand beibehalten.

                                        Preise Die Anzeige der Währung richtet sich nach der Eigenwährung, die bei
                                        der Installation festgelegt wurde.
                                        • € / qm:
                                           Artikelpreis des Lieferanten in eigener Währung pro Mengeneinheit.
                                        • Preis:
                                           Gesamtpreis des Artikels.
                                        • (Spalte ohne Bezeichnung):
                                           Buchungsstatus der Artikelposition.

                                        Buchungsstatus mit         Bedeutung
                                        Farbkennzeichen

                                            grau                   Artikelposition ist vom Prozess (Programm) gebucht
                                                                   worden.

                                            rot                    Artikelposition ist vom Prozess (Programm) nicht oder
                                                                   noch nicht gebucht worden.

                                        Tab. E-5     Buchungsstatus der Artikelposition
1.01 / 01-2017




                 A+W Enterprise Lager                                                                                E-27
                 Lagerverwaltung                                                                     Softwarereferenz




                                        Kistenlagerausgang
                                        Buchung > Kistenausgang




                 Abb. E-6   Kistenlagerausgang


                                        In diesem Dialog buchen Sie Lagerausgänge für komplette Kisten. Wenn Sie
                                        nur einen Teil der Artikel aus einer Kiste ausbuchen möchten, müssen Sie zu-
                                        erst die Kiste auflösen und die Artikel der Kiste auf ein anderes Lager buchen.
                                        Sie können folgende Tastaturbefehle ausführen:
                                        •   Mit <Strg> + <F8> können Sie im ersten Feld zwischen dem Dialog Kiste-
                                            neingang und Kistenausgang wechseln.
                                        •   Mit <F5> können Sie aus einer Spalte in die kistenbezogenen Angaben im
                                            Fußbereich (linke Seite) wechseln.
                                        •   Mit <Shift> + <F8> können Sie aus einer Spalte in die variantenbezogenen
                                            Angaben im Fußbereich (rechte Seite) wechseln.
                                        •   Mit <Shift> + <F12> können Sie für den aktuellen Buchungssatz ein neues
                                            Datum eingeben.
                                        •   Mit <Strg> + <F12> können Sie komplette Kisten buchen. Damit wird die
                                            gesamte Kiste ausgebucht.
                                        •   Mit <Strg> + <F8> können Sie Kisten auflösen und die Artikel aus der Kiste
                                            auf ein Ziellager buchen. Damit werden die einzelnen Scheiben der Kiste
                                            in das Ziellager gebucht.
                                        Die Register, Felder und Spalten sind an folgender Stelle beschrieben:
                                         “Kistenlagereingang” auf Seite E-23
1.01 / 01-2017




                 E-28                                                                          A+W Enterprise Lager
                 Softwarereferenz                                                                   Lagerverwaltung




                                         Fachlagereingang
                                         Buchung > Facheingang
                                         In diesem Dialog können Sie Artikel auf Fächer eines Fachlagers buchen.
                                         In diesem Dialog finden Sie folgende Register:
                                         •   “Fachlagereingang – Stück” auf Seite E-29
                                         •   “Fachlagereingang – Menge” auf Seite E-32


                                         Fachlagereingang – Stück
                                         Buchung > Facheingang > Stück




                 Abb. E-7   Fachlagereingang – Stück


                                         In diesem Register erfassen und buchen Sie die Bestände und Preise der ak-
                                         tuellen Artikelvariante in Stückzahlen.
                                         Sie können folgende Tastaturbefehle ausführen:
                                         •   Mit <Strg> + <F8> können Sie im ersten Feld zwischen dem Dialog Fach-
                                             lagereingang und Fachlagerausgang wechseln.
                                         •   Mit <F5> können Sie aus einer Spalte in die variantenbezogenen Angaben
                                             im Fußbereich wechseln.
                                         •   Mit <Shift> + <F12> können Sie für den aktuellen Buchungssatz ein neues
                                             Datum eingeben.
1.01 / 01-2017




                 A+W Enterprise Lager                                                                          E-29
                 Lagerverwaltung                                                                   Softwarereferenz




                                   Kopfbereich
                                   Die Felder sind an folgender Stelle beschrieben:
                                    “Lagereingang” auf Seite E-16

                                   Rumpfbereich
                                   In diesem Register buchen Sie die Bestände und Preise der Artikel in Stück-
                                   zahlen.
                                   •   Variante:
                                       Maßvariante des Artikels. Mit <F9> können Sie die Variantenauswahl auf-
                                       rufen. Dabei werden nur die Varianten angezeigt, die dem aktuellen Artikel
                                       in den Stammdaten zugewiesen sind.
                                   •   Fach:
                                       Bezeichnung des Fachs.

                                   Bestände (Stück) Lagerbestand der Variante in Stückzahlen.
                                   •   Alt:
                                       Alter Artikelbestand im Lager, bevor gebucht wird.
                                   •   Buchung:
                                       Artikelbestand, der gebucht wird.
                                   •   Neu:
                                       Neu berechneter Artikelbestand. Dieser Bestand wird übernommen, wenn
                                       der neue Artikel gebucht wird. Wenn Sie den Dialog mit <Pos1> verlassen,
                                       wird der alte Lagerbestand beibehalten.

                                   Preise Die Anzeige der Währung richtet sich nach der Eigenwährung, die bei
                                   der Installation festgelegt wurde.
                                   • € / qm:
                                      Artikelpreis des Lieferanten in eigener Währung pro Mengeneinheit.
                                   • Preis:
                                      Gesamtpreis des Artikels.
                                   • (Spalte ohne Bezeichnung):
                                      Buchungsstatus der Artikelposition.

                                   Buchungsstatus mit         Bedeutung
                                   Farbkennzeichen

                                       grau                   Artikelposition ist vom Prozess (Programm) gebucht
                                                              worden.

                                       rot                    Artikelposition ist vom Prozess (Programm) nicht oder
                                                              noch nicht gebucht worden.

                                   Tab. E-6     Buchungsstatus der Artikelposition

                                   Fußbereich – Variantenbezogene Angaben

                                   Objekt Bezeichnung des Objekts bei auftragsbezogenen Lagerartikeln,
1.01 / 01-2017




                                   z. B. Baustelle des Kunden.

                                   Kostenstelle Bezeichnung der Kostenstelle für statistische Auswertungen.


                 E-30                                                                        A+W Enterprise Lager
                 Softwarereferenz                                                                  Lagerverwaltung




                                        Bemerkung Textfeld für zusätzliche Informationen.

                                        Mindestbestand Minimal zulässiger Lagerbestand des Artikels, um Produk-
                                        tionsengpässe zu verhindern.

                                        Alarmbestand Stückzahl des Artikelbestands, die einen Bestellvorschlag im
                                        Einkauf anlegt. Durch Alarmbestände können Sie eine Unterdeckung des La-
                                        gers verhindern.

                                        Maximalbestand Maximal zulässiger Lagerbestand des Artikels, um Lager-
                                        kosten zu minimieren.

                                        Gesamtpreis Gesamtpreis der Artikelvariante.

                                        Durchschnittspreis Durchschnittlicher Einkaufspreis der Artikelvariante im
                                        Lager.

                                        Höchstpreis Höchster Einkaufspreis der Artikelvariante im Lager.

                                        Niedrigstpreis Niedrigster Einkaufspreis der Artikelvariante im Lager.

                                        LIFO-Gesamtpreis Gesamtpreis der Artikelvariante im Lager, wenn die zu-
                                        letzt eingelagerten Lagerartikel als erste Artikel ausgelagert werden.

                                        FIFO-Gesamtpreis Gesamtpreis der Artikelvariante im Lager, wenn die zu-
                                        erst eingelagerten Lagerartikel als erste Artikel ausgelagert werden.
1.01 / 01-2017




                 A+W Enterprise Lager                                                                            E-31
                 Lagerverwaltung                                                                      Softwarereferenz




                                        Fachlagereingang – Menge
                                        Buchung > Facheingang > Menge




                 Abb. E-8   Fachlagereingang – Menge


                                        In diesem Register erfassen und buchen Sie die Bestände und Preise der ak-
                                        tuellen Artikelvariante in Mengeneinheit.
                                        Das Register Menge ist wie das Register Stück aufgebaut.
                                         “Kopfbereich” auf Seite E-30
                                         “Fußbereich – Variantenbezogene Angaben” auf Seite E-30

                                        Rumpfbereich
                                        In diesem Bereich buchen Sie die Bestände und Preise der Artikel in Mengen-
                                        einheit.
                                        •   Variante:
                                            Maßvariante des Artikels. Mit <F9> können Sie die Variantenauswahl auf-
                                            rufen. Dabei werden nur die Varianten angezeigt, die dem aktuellen Artikel
                                            in den Stammdaten zugewiesen sind.
                                        •   Fach:
                                            Bezeichnung des Fachs.

                                        Bestände (Mengeneinheit) Lagerbestand der Variante in Mengeneinheit.
                                        •   Alt:
                                            Alter Artikelbestand im Lager, bevor gebucht wird.
1.01 / 01-2017




                                        •   Buchung:
                                            Artikelbestand, der gebucht wird.



                 E-32                                                                            A+W Enterprise Lager
                 Softwarereferenz                                                                       Lagerverwaltung




                                        •   Neu:
                                            Neu berechneter Artikelbestand. Dieser Bestand wird übernommen, wenn
                                            der neue Artikel gebucht wird. Wenn Sie den Dialog mit <Pos1> verlassen,
                                            wird der alte Lagerbestand beibehalten.

                                        Preise Die Anzeige der Währung richtet sich nach der Eigenwährung, die bei
                                        der Installation festgelegt wurde.
                                        • € / qm:
                                           Artikelpreis des Lieferanten in eigener Währung pro Mengeneinheit.
                                        • Preis:
                                           Gesamtpreis des Artikels.
                                        • (Spalte ohne Bezeichnung):
                                           Buchungsstatus der Artikelposition.

                                        Buchungsstatus mit         Bedeutung
                                        Farbkennzeichen

                                            grau                   Artikelposition ist vom Prozess (Programm) gebucht
                                                                   worden.

                                            rot                    Artikelposition ist vom Prozess (Programm) nicht oder
                                                                   noch nicht gebucht worden.

                                        Tab. E-7     Buchungsstatus der Artikelposition
1.01 / 01-2017




                 A+W Enterprise Lager                                                                                E-33
                 Lagerverwaltung                                                                   Softwarereferenz




                                        Fachlagerausgang
                                        Buchung > Fachlagerausgang




                 Abb. E-9   Fachlagerausgang


                                        In diesem Dialog können Sie Artikel vom Fachlager abbuchen.
                                        Sie können folgende Tastaturbefehle ausführen:
                                        •   Mit <Strg> + <F8> können Sie im ersten Feld zwischen dem Dialog Fach-
                                            lagereingang und Fachlagerausgang wechseln.
                                        •   Mit <F5> können Sie aus einer Spalte in die variantenbezogenen Angaben
                                            im Fußbereich wechseln.
                                        •   Mit <Shift> + <F12> können Sie für den aktuellen Buchungssatz ein neues
                                            Datum eingeben.
                                        Die Register, Felder und Spalten sind an folgender Stelle beschrieben:
                                         “Fachlagereingang” auf Seite E-29
1.01 / 01-2017




                 E-34                                                                        A+W Enterprise Lager
                 Softwarereferenz                                                                   Lagerverwaltung




                                        Stapellagereingang
                                        Buchung > Stapeleingang




                                        Abb. E-10    Stapellagereingang


                                        In diesem Dialog können Sie Artikel auf einen Stapel buchen. Sie können ver-
                                        schiedene Artikel mit unterschiedlichen Abmessungen auf einen Stapel bu-
                                        chen.
                                        Sie können folgende Tastaturbefehle ausführen:
                                        •   Mit <Strg> + <F8> können Sie im ersten Feld zwischen dem Dialog Stapel-
                                            lagereingang und Stapellageränderung wechseln.
                                        •   Mit <F2> können Sie die Anzeige zwischen Artikel in Stückzahl und Artikel
                                            in Mengeneinheit umschalten.
                                        •   Mit <Shift> + <F8> können Sie vom System eine neue Stapelnummer ver-
                                            geben lassen.
                                        •   Mit <Shift> + <F9> können Sie alle Stapelzeilen kopieren und einer neuen
                                            Stapelnummer zuordnen.
                                        •   Mit <Shift> + <F12> können Sie für den aktuellen Buchungssatz ein neues
                                            Datum eingeben.
                                        •   Mit <Strg> + <F12> können Sie einen Stapel einbuchen.
                                        •   Mit <Ende> können Sie die Stapelbuchung buchen.

                                        Kopfbereich

                                        Lager Lagernummer und Lagerbezeichnung.
1.01 / 01-2017




                                        Lieferant Lieferantennummer und Lieferantenname.




                 A+W Enterprise Lager                                                                          E-35
                 Lagerverwaltung                                                               Softwarereferenz




                                   Letzte Änderung am, von Datum der letzten Änderung am Buchungssatz
                                   und Name des Anwenders, der die letzte Buchung ausgeführt hat.

                                   Rumpfbereich
                                   •   Stapel:
                                       Nummer des Stapelplatzes.
                                   •   Bezeichnung:
                                       Bezeichnung des Stapelplatzes.
                                   •   Artikel:
                                       Artikelnummer des Artikels, der auf dem Stapelplatz eingelagert wird.
                                   •   Variante:
                                       Bezeichnung der Artikelvariante.
                                   •   Anzahl:
                                       Stückzahl des Artikels.
                                       Mit <F2> können Sie auf Artikel in Mengeneinheit umschalten.
                                   •   Menge / qm:
                                       Menge in Quadratmetern.
                                   •   Preis / qm:
                                       Preis pro Mengeneinheit.


                                   Stapellageränderung
                                   Buchung > Stapeländerung




                                   Abb. E-11    Stapellageränderung


                                   In diesem Dialog können Sie nach Artikeln suchen die in Stapeln vorkommen,
1.01 / 01-2017




                                   um sie in ein anderes Lager zu buchen.




                 E-36                                                                    A+W Enterprise Lager
                 Softwarereferenz                                                                   Lagerverwaltung




                                        Sie können folgende Tastaturbefehle ausführen:
                                        •   Mit <Strg> + <F8> können Sie im Kopfbereich zwischen dem Dialog Sta-
                                            pellagereingang und Stapellageränderung wechseln.
                                        •   Mit <Strg> + <F8> können Sie im Rumpfbereich den ausgewählten Stapel
                                            auflösen. Wenn ein Stapel aufgelöst wird, müssen die Artikel aus dem auf-
                                            gelösten Stapel auf ein anderes Lager gebucht werden. Das Lager für die
                                            Artikel geben Sie in der Spalte Ziellager ein.
                                        •   Mit <Shift> + <F9> können Sie im Rumpfbereich den ausgewählten Daten-
                                            satz kopieren.
                                        •   Mit <F2> können Sie die Anzeige zwischen Artikel in Stückzahl und Artikel
                                            in Mengeneinheit umschalten.
                                        •   Mit <Shift> + <F12> können Sie für den aktuellen Buchungssatz ein neues
                                            Datum eingeben.
                                        •   Mit <Strg> + <F12> können Sie einen Stapel ausbuchen.
                                        •   Mit <Ende> können Sie die Stapeländerung buchen.
                                        Die Felder und Spalten sind an folgender Stelle beschrieben:
                                         “Stapellagereingang” auf Seite E-35
                                        Zusätzlich werden folgende Felder angezeigt:

                                        Kopfbereich

                                        Artikel 1, Artikel 2 Suche über eine Folge von Artikelnummern.

                                        Rumpfbereich
                                        •   Ziellager:
                                            Nummer des Ziellagers.
1.01 / 01-2017




                 A+W Enterprise Lager                                                                          E-37
                 Lagerverwaltung                                                                      Softwarereferenz




                                          Gestelllagereingang
                                          Buchung > Gestelleingang




                 Abb. E-12   Gestelllagereingang


                                          In diesem Dialog können Sie Artikel auf Gestellen in ein Gestelllager einbu-
                                          chen.
                                          Sie können folgende Tastaturbefehle ausführen:
                                          •   Mit <Strg> + <F8> können Sie im ersten Feld zwischen dem Dialog Ge-
                                              stelllagereingang und Gestelllagerausgang wechseln.
                                          •   Mit <Shift> + <F12> können Sie für den aktuellen Buchungssatz ein neues
                                              Datum eingeben.

                                          Kopfbereich
                                          Im Kopfbereich müssen Sie entweder den Artikel und das Lager angeben oder
                                          das Gestell.

                                          Artikel Artikelnummer und Artikelbezeichnung.

                                          Lager Lagernummer und Lagerbezeichnung.

                                          Gestell Externe Bezeichnung des Lagergestells.

                                          Gesamtbestand Gesamtbestand des Artikels, einschließlich aller Artikelvari-
1.01 / 01-2017




                                          anten.




                 E-38                                                                           A+W Enterprise Lager
                 Softwarereferenz                                                                   Lagerverwaltung




                                        Gesamtwert Gesamtbetrag des Lagerartikels.

                                        Buchungsstatus Status der Buchungen im Lager.

                                        Buchungsstatus mit       Bedeutung
                                        Farbkennzeichen

                                            grau                 Im Lagereingang sind alle Buchungspositionen vom
                                                                 Prozess (Programm) gebucht worden.

                                            rot                  Im Lagereingang ist mindestens eine
                                                                 Buchungsposition vom Prozess (Programm) nicht oder
                                                                 noch nicht gebucht worden.

                                        Tab. E-8     Buchungsstatus des Lagers

                                        Letzte Änderung am, von Datum der letzten Änderung am Buchungssatz
                                        und Name des Anwenders, der die letzte Buchung ausgeführt hat.

                                        Rumpfbereich
                                        •   Variante:
                                            Maßvariante des Artikels. Mit <F9> können Sie die Variantenauswahl auf-
                                            rufen. Varianten eines Artikels werden nur angezeigt, wenn die Varianten
                                            im Stammdatenmodul angelegt sind.
                                        •   Gestell:
                                            Externe Gestellbezeichnung des Lagergestells.
                                        •   G:
                                            Artikelvarianten, die sich auf dem Gestell befinden.
                                             Verschiedene Artikelvarianten stehen auf einem Gestell.
                                             Nur gleiche Artikelvarianten stehen auf einem Gestell.
                                        •   Fach:
                                            Bezeichnung des Fachs.
                                        •   Fifo-Datum:
                                            Datum für die Gestellbuchung nach dem Fifo-Prinzip.
                                        •   Menge:
                                            Aktuelle Stückzahl der Artikel auf dem Lagergestell.
                                        •   Buchung:
                                            Artikelbestand, der gebucht wird.
                                        •   € / qm:
                                            Artikelpreis des Lieferanten in eigener Währung pro Mengeneinheit.
1.01 / 01-2017




                 A+W Enterprise Lager                                                                           E-39
                 Lagerverwaltung                                                                Softwarereferenz




                                   •   Preis:
                                       Gesamtpreis des Artikels.
                                   •   Buchungsstatus:
                                       Status der Buchungen im Gestelllagereingang.

                                   Buchungsstatus mit        Bedeutung
                                   Farbkennzeichen

                                       grau                  Buchungsposition ist vom Prozess (Programm)
                                                             gebucht worden.

                                       rot                   Buchungsposition ist vom Prozess (Programm) nicht
                                                             oder noch nicht gebucht worden.

                                   Tab. E-9     Buchungsstatus des Gestelllagereingangs
1.01 / 01-2017




                 E-40                                                                     A+W Enterprise Lager
                 Softwarereferenz                                                                      Lagerverwaltung




                                          Gestelllagerausgang
                                          Buchung > Gestellausgang
                                          In diesem Dialog können Sie gestellbezogene Lagerabgänge buchen oder Ar-
                                          tikel zwischen Gestellen umbuchen.
                                          In diesem Dialog finden Sie folgende Register:
                                          •   “Gestelllagerausgang – Auftragsbezogen” auf Seite E-41
                                          •   “Gestelllagerausgang – Umbuchung” auf Seite E-43


                                          Gestelllagerausgang – Auftragsbezogen
                                          Buchung > Gestellausgang > Auftragsbezogen




                 Abb. E-13   Gestelllagerausgang – Auftragsbezogen


                                          In diesem Register buchen Sie die auftragsbezogenen Lagerabgänge.
                                          Sie können folgende Tastaturbefehle ausführen:
                                          •   Mit <Strg> + <F8> können Sie im ersten Feld zwischen dem Dialog Ge-
                                              stelllagereingang und Gestelllagerausgang wechseln.
                                          •   Mit <F2> können Sie zwischen den Registern Auftragsbezogen und Umbu-
                                              chung umschalten.
                                          •   Mit <F5> können Sie in die variantenbezogenen Angaben im Fußbereich
                                              wechseln.
1.01 / 01-2017




                 A+W Enterprise Lager                                                                            E-41
                 Lagerverwaltung                                                              Softwarereferenz




                                   •   Mit <Shift> + <F12> können Sie für den aktuellen Buchungssatz ein neues
                                       Datum eingeben.
                                   •   Mit <Shift> + <F8> können Sie eine Position auflösen.

                                   [Zurücksetzen] Verwirft die eingegebenen Änderungen.

                                   Kopfbereich
                                   Im Kopfbereich müssen Sie entweder den Artikel und das Lager angeben oder
                                   das Gestell.
                                   Die Felder sind an folgender Stelle beschrieben:
                                    “Gestelllagereingang” auf Seite E-38

                                   Rumpfbereich
                                   •   Variante:
                                       Maßvariante des Artikels. Mit <F9> können Sie die Variantenauswahl auf-
                                       rufen. Varianten eines Artikels werden nur angezeigt, wenn die Varianten
                                       im Stammdatenmodul angelegt sind.
                                   •   Gestell:
                                       Externe Gestellbezeichnung des Lagergestells.
                                   •   G:
                                       Artikelvarianten, die sich auf dem Gestell befinden.
                                        Verschiedene Artikelvarianten stehen auf einem Gestell.
                                        Nur gleiche Artikelvarianten stehen auf einem Gestell.
                                   •   Fach:
                                       Bezeichnung des Fachs.
                                   •   Fifo-Datum:
                                       Datum für die Gestellbuchung nach dem Fifo-Prinzip.
                                   •   Menge:
                                       Aktuelle Stückzahl der Artikel auf dem Lagergestell.
                                   •   Buchung:
                                       Artikelbestand, der gebucht wird.
                                   •   Auftrag:
                                       Auftragsnummer für die auftragsbezogene Gestellbuchung.
                                   •   Position:
                                       Nummer der Gestellposition im Gestelllager.
1.01 / 01-2017




                 E-42                                                                   A+W Enterprise Lager
                 Softwarereferenz                                                                         Lagerverwaltung




                                         •   Buchungsstatus:
                                             Status der Buchungen im Lager.

                                         Buchungsstatus mit          Bedeutung
                                         Farbkennzeichen

                                             grau                    Buchungsposition ist vom Prozess (Programm)
                                                                     gebucht worden.

                                             rot                     Buchungsposition ist vom Prozess (Programm) nicht
                                                                     oder noch nicht gebucht worden.

                                             gelb                    Gestelldaten wurden verändert: Bei der
                                                                     auftragsbezogenen Buchung wurde von diesem
                                                                     Gestell eine Menge oder Teilmenge für die Buchung
                                                                     verplant.

                                             halb gelb / halb grau   Nachbearbeitung ist notwendig: Ein neuer Satz wurde
                                                                     angelegt, mit der verbleibenden Gestellmenge für das
                                                                     Unterteil der Auftragsposition.

                                         Tab. E-10      Buchungsstatus des Gestelllagerausgangs


                                         Gestelllagerausgang – Umbuchung
                                         Buchung > Gestellausgang > Umbuchung




                 Abb. E-14   Gestelllagerausgang – Umbuchung
1.01 / 01-2017




                                         In diesem Register können Sie die Artikel auf ein neues Gestell bzw. neues
                                         Fach umbuchen.




                 A+W Enterprise Lager                                                                                 E-43
                 Lagerverwaltung                                                              Softwarereferenz




                                   Sie können folgende Tastaturbefehle ausführen:
                                   •   Mit <Strg> + <F8> können Sie im ersten Feld zwischen dem Dialog Ge-
                                       stelllagereingang und Gestelllagerausgang wechseln.
                                   •   Mit <F2> können Sie zwischen den Registern Auftragsbezogen und Umbu-
                                       chung umschalten.
                                   •   Mit <F5> können Sie in die variantenbezogenen Angaben im Fußbereich
                                       wechseln.
                                   •   Mit <Shift> + <F12> können Sie für den aktuellen Buchungssatz ein neues
                                       Datum eingeben.
                                   •   Mit <Shift> + <F8> können Sie eine Position auflösen.

                                   [Zurücksetzen] Verwirft die eingegebenen Änderungen.

                                   Kopfbereich
                                   Im Kopfbereich müssen Sie entweder den Artikel und das Lager angeben oder
                                   das Gestell.
                                   Die Felder sind an folgender Stelle beschrieben:
                                    “Gestelllagereingang” auf Seite E-38

                                   Rumpfbereich
                                   •   Variante:
                                       Maßvariante des Artikels. Mit <F9> können Sie die Variantenauswahl auf-
                                       rufen. Varianten eines Artikels werden nur angezeigt, wenn die Varianten
                                       im Stammdatenmodul angelegt sind.
                                   •   Gestell:
                                       Externe Gestellbezeichnung des Lagergestells.
                                   •   G:
                                       Artikelvarianten, die sich auf dem Gestell befinden.
                                        Verschiedene Artikelvarianten stehen auf einem Gestell.
                                        Nur gleiche Artikelvarianten stehen auf einem Gestell.
                                   •   Fach:
                                       Bezeichnung des Fachs.
                                   •   Fifo-Datum:
                                       Datum für die Gestellbuchung nach dem Fifo-Prinzip.
                                   •   Menge:
                                       Aktuelle Stückzahl der Artikel auf dem Lagergestell.
                                   •   Buchung:
                                       Artikelbestand, der gebucht wird.
                                   •   Gestell neu:
                                       Nummer des Gestells, auf das der Artikel umgebucht wird.
                                   •   Fach neu:
                                       Bezeichnung des Fachs, auf das das Gestell umgebucht wird.
1.01 / 01-2017




                 E-44                                                                   A+W Enterprise Lager
                 Softwarereferenz                                                                        Lagerverwaltung




                                        •   Buchungsstatus:
                                            Status der Buchungen im Lager.

                                        Buchungsstatus mit          Bedeutung
                                        Farbkennzeichen

                                            grau                    Buchungsposition ist vom Prozess (Programm)
                                                                    gebucht worden.

                                            rot                     Buchungsposition ist vom Prozess (Programm) nicht
                                                                    oder noch nicht gebucht worden.

                                            gelb                    Gestelldaten wurden verändert: Bei der
                                                                    auftragsbezogenen Buchung wurde von diesem
                                                                    Gestell eine Menge oder Teilmenge für die Buchung
                                                                    verplant.

                                            halb gelb / halb grau   Nachbearbeitung ist notwendig: Ein neuer Satz wurde
                                                                    angelegt, mit der verbleibenden Gestellmenge für das
                                                                    Unterteil der Auftragsposition.

                                        Tab. E-11      Buchungsstatus des Gestelllagerausgangs



                                        Lagerausgang (Auftragsbezogen)
                                        Buchung > Ausgang (Auftragsbezogen)




                                        Abb. E-15      Lagerausgang (Auftragsbezogen)


                                        In diesem Dialog können Sie auftragsbezogene Lagerabgänge manuell bu-
                                        chen. In den Artikelstammdaten ist definiert, ob ein Artikel nur manuell ge-
                                        bucht werden kann.
1.01 / 01-2017




                 A+W Enterprise Lager                                                                                E-45
                 Lagerverwaltung                                                               Softwarereferenz




                                   Sie können folgende Tastaturbefehle ausführen:
                                   •   Mit <F2> können Sie sich die Spalte Termin für den Liefertermin der Posi-
                                       tion anzeigen lassen.
                                   •   Mit <F3> können Sie die Buchung auslösen.
                                   •   Mit <Shift> + <F12> können Sie für den aktuellen Buchungssatz ein neues
                                       Datum eingeben.

                                   Kopfbereich

                                   Auftrag Auftragsnummer.

                                   Anfahrt Liefertermin, an dem der Auftrag beim Kunden angeliefert wird.

                                   Kunde Kundennummer und Kundenname.

                                   Erfasst am, von Datum der Auftragserfassung und Name des Erfassers.

                                   Gebucht am, von Datum der Lagerausgansbuchung und Name des Mitar-
                                   beiters, der die Lagerausgangsbuchung gebucht hat.

                                   Rumpfbereich
                                   •   Pos:
                                       Nummer der Auftragsposition.
                                   •   Artikel:
                                       Artikelnummer.
                                   •   Bezeichnung:
                                       Artikelbezeichnung.
                                   •   Variante:
                                       Maßvariante der Position.
                                   •   Gesamt:
                                       Gesamtmenge pro Position.
                                   •   Verbucht:
                                       Menge der Position, die bereits abgebucht wurde.
                                   •   Buchen:
                                       Menge der Position, die vom Lager abgebucht werden soll.
                                   Mit <F2> können Sie sich die Spalte Termin für den Liefertermin der Position
                                   anzeigen lassen.
                                   •   Termin:
                                       Liefertermin der Position.
1.01 / 01-2017




                 E-46                                                                    A+W Enterprise Lager
                 Softwarereferenz                                                                   Lagerverwaltung




                                        Buchungskorrektur – Übersicht
                                        Buchung > Korrektur




                                        Abb. E-16    Buchungskorrektur – Übersicht


                                        In diesem Dialog können Sie die Suchkriterien festlegen, um sich die Buchun-
                                        gen anzeigen zu lassen und zu korrigieren.
                                        Um Buchungen korrigieren zu können, müssen zuerst Lagerdaten durch das
                                        Lagerbuchungssystem angelegt worden sein. Sicherungs-Lagerdaten werden
                                        nur angelegt, wenn Zeitpunkte zur automatischen Speicherung der Lagerda-
                                        ten definiert werden, z. B. der 15. eines jeden Monats. Fehlerhafte Buchungs-
                                        sätze dürfen nicht im Buchungssystem vorhanden sein.
                                        Die Details der Übersicht können Sie sich in der Detailansicht anzeigen las-
                                        sen.
                                         “Buchungskorrektur – Details” auf Seite E-48
                                        Sie können folgende Tastaturbefehle ausführen:
                                        •   Mit <F5> wechseln Sie zwischen der Übersicht und der Detailansicht der
                                            ausgewählten Position.
                                        •   Mit <Shift> + <F12> können Sie für den aktuellen Buchungssatz ein neues
                                            Datum eingeben.

                                        Kopfbereich

                                        Artikel Artikelnummer und Artikelbezeichnung.

                                        Lager Lagernummer und Lagerbezeichnung.

                                        von Datum, bis Datum Zeitraum, für den Buchungen aufgelistet werden.
1.01 / 01-2017




                 A+W Enterprise Lager                                                                           E-47
                 Lagerverwaltung                                                              Softwarereferenz




                                   Rumpfbereich
                                   •   Variante:
                                       Artikelvariante.
                                   •   Farbe:
                                       Farbvariante des Artikels.
                                   •   Lieferant:
                                       Lieferantennummer.
                                   •   Menge:
                                       Mengeneinheit des Artikels in der zu korrigierenden Buchung.
                                   •   Anzahl:
                                       Stückzahl der zu korrigierenden Buchung.
                                   •   Preis:
                                       Stückpreis der Variante.
                                   •   Stat.:
                                       Bezeichnung des Buchungsstatus, z. B. Lagereingang.
                                   •   Datum:
                                       Datum, an dem die Buchung korrigiert wurde.


                                   Buchungskorrektur – Details
                                   Buchung > Korrektur > Filtern > <F5>




                                   Abb. E-17    Buchungskorrektur – Details


                                   In diesem Dialog werden die Details einer Buchungskorrektur aus der Über-
                                   sicht angezeigt und korrigiert.
                                   Sie können folgende Tastaturbefehle ausführen:
                                   •   Mit <F5> wechseln Sie zwischen der Übersicht und der Detailansicht der
                                       ausgewählten Position.
1.01 / 01-2017




                                   •   Mit <Shift> + <F12> können Sie für den aktuellen Buchungssatz ein neues
                                       Datum eingeben.




                 E-48                                                                   A+W Enterprise Lager
                 Softwarereferenz                                                               Lagerverwaltung




                                        Kopfbereich
                                        Die Felder sind an folgender Stelle beschrieben:
                                         “Kopfbereich” auf Seite E-47

                                        Rumpfbereich

                                        Kiste Kistennummer.

                                        Fach Bezeichnung des Fachs.

                                        Variante Artikelvariante.

                                        Farbe Farbvariante des Artikels.

                                        Lieferant Lieferantennummer.

                                        Auftrag Auftragsnummer, bei auftragsbezogenen Lagerbuchungen.

                                        Position Nummer der Auftragsposition.

                                        Menge Mengeneinheit des Artikels in der zu korrigierenden Buchung.

                                        Anzahl Stückzahl der zu korrigierenden Buchung.

                                        Preis Stückpreis der Variante.

                                        Status Bezeichnung des Buchungsstatus, z. B. Lagereingang.

                                        Datum Datum, an dem die Buchung korrigiert wurde.
1.01 / 01-2017




                 A+W Enterprise Lager                                                                        E-49
                 Stammdatenverwaltung                                                                Softwarereferenz




                                        Stammdatenverwaltung
                                        In den Stammdaten verwalten Sie den Lagerraum und die Bestandsgrenzen
                                        für Lagerartikel, z. B. legen Sie neue Lagerplätze im Lager an. Außerdem de-
                                        finieren Sie die Lagerartikel und deren Bestandsgrenzen.
                                        In diesem Abschnitt sind folgende Dialoge erklärt:
                                        •   “Lagerraumverwaltung” auf Seite E-50
                                        •   “Artikelstammdaten Lager” auf Seite E-51


                                        Lagerraumverwaltung
                                        Stammdaten > Raum




                                        Abb. E-18    Lagerraumverwaltung


                                        In diesem Dialog können Sie neue Lagerräume anlegen. Die festgelegte Zu-
                                        ordnung von Lagernummer, Lagerbezeichnung, Lagerart und Inventurart kann
                                        nach dem Speichern nicht mehr geändert werden. Für einen Lagerraum müs-
                                        sen Sie immer die Art des Lagers und der Inventur festlegen.
                                        Mit <Ende> speichern Sie die Daten des Lagerraums.

                                        Kopfbereich

                                        Lager Nummer und Bezeichnung des Lagers.

                                        Kurzbez. Kurzbezeichnung des Lagers.

                                        im Haus Nummer und Bezeichnung des Hauses oder Mandanten.

                                        Rumpfbereich

                                        Inventurart Art der Bestandskontrolle.
                                        •   Permanent = Permanente Inventur.
                                        •   Zyklisch = Zyklische Inventur zum Bilanzstichtag.
1.01 / 01-2017




                                         “Inventur – Standardlager” auf Seite E-53




                 E-50                                                                           A+W Enterprise Lager
                 Softwarereferenz                                                              Stammdatenverwaltung




                                        Lagerart Art des Lagers:
                                        •   Normallager = Lager für alle Artikel ohne Restriktionen.
                                        •   Kistenlager = Lager für komplette Kisten. Angebrochene Kisten müssen
                                            aufgelöst und auf ein anderes Lager gebucht werden.
                                        •   Fachlager = Lager für alle Artikel mit zugewiesener Bezeichnung des
                                            Fachs.
                                        •   Hochregallager = Lager mit Lagerplätzen in Hochregalen.
                                        •   Stapellager = Lager für Scheiben mit einheitlichen Abmessungen.
                                        •   Einzelblattkistenlager = Lager zur Buchung einzelner Glasblätter in Kisten.
                                        •   Gestelllager = Lager mit Lagerplätzen auf Gestellen.

                                        Schnittstelle Angabe der Softwareschnittstelle. Auswahl für ein kundensei-
                                        tig angeschlossenes Lagerverwaltungssystem.

                                        Größe Lagerfläche in Mengeneinheit.

                                        Fixe Kosten Fixe Kosten der Lagerfläche in Eigenwährung pro Quadratme-
                                        ter.

                                        Variable Kosten Variable Kosten der Lagerfläche in Eigenwährung pro Qua-
                                        dratmeter.

                                        WE-Lager Nummer des Wareneingangslagers.


                                        Artikelstammdaten Lager
                                        Stammdaten > Artikel




                                        Abb. E-19    Artikelstammdaten Lager


                                        In diesem Dialog können Sie die Bestandsgrenzen der Lagerartikel festlegen.
1.01 / 01-2017




                                        Die Bestandsgrenzen der Lagerartikel werden durch den Minimalbestand,
                                        Alarmbestand und Maximalbestand festgelegt.



                 A+W Enterprise Lager                                                                            E-51
                 Stammdatenverwaltung                                                              Softwarereferenz




                                        Sie können folgende Tastaturbefehle ausführen:
                                        •   Wenn Sie sich in einer Spalte im Rumpfbereich befinden, können Sie
                                            mit <Ende> die Festlegung der Bestandsgrenzen speichern.
                                        •   Mit <F5> können Sie in den Fußbereich wechseln.

                                        Kopfbereich

                                        Artikel Artikelnummer und Artikelbezeichnung.

                                        Lager Lagernummer und Lagerbezeichnung.

                                        Bestellvariante Artikelvariante für Nachbestellungen.

                                        Bestellfarbe Farbvariante des Artikels für Nachbestellungen.

                                        Bestandsgrenzen

                                        Mindestbestand Minimal zulässiger Lagerbestand des Artikels, um Produk-
                                        tionsengpässe zu verhindern.

                                        Alarmbestand Stückzahl des Artikelbestands, die einen Bestellvorschlag im
                                        Einkauf anlegt. Durch Alarmbestände können Sie eine Unterdeckung des La-
                                        gers verhindern.

                                        Maximalbestand Maximal zulässiger Lagerbestand des Artikels, um Lager-
                                        kosten zu minimieren.

                                        Rumpfbereich
                                        Mit <F2> können Sie die Anzeige zwischen Artikel in Stückzahl und Artikel in
                                        Mengeneinheit umschalten.

                                        Variante Maßvariante des Artikels.

                                        Farbe Farbvariante des Artikels.

                                        Fußbereich

                                        Bemerkung Mit <F5> können Sie in das Textfeld für Bemerkungen zur Arti-
                                        kelvariante wechseln.
1.01 / 01-2017




                 E-52                                                                        A+W Enterprise Lager
                 Softwarereferenz                                                                 Inventurverwaltung




                                          Inventurverwaltung
                                          Mit der Inventurverwaltung gleichen Sie die gezahlten Bestände mit den vom
                                          System gebuchten Beständen ab und korrigieren die Zahlen entsprechend im
                                          System.
                                          In diesem Abschnitt sind folgende Dialoge erklärt:
                                          •   “Inventur – Standardlager” auf Seite E-53
                                          •   “Inventur – Kistenlager” auf Seite E-56
                                          •   “Inventur – Fachlager” auf Seite E-58
                                          •   “Inventur – Stapellager” auf Seite E-59
                                          •   “Inventur – Gestelllager” auf Seite E-60


                                          Inventur – Standardlager
                                          Inventur > Lager




                 Abb. E-20   Inventur-Standardlager


                                          In diesem Dialog können Sie die Inventur für das Standardlager durchführen
                                          und abschließen.
1.01 / 01-2017




                 A+W Enterprise Lager                                                                          E-53
                 Inventurverwaltung                                                                 Softwarereferenz




                                          Lager in Inventur
                                          Wenn ein Lager für die Inventur freigeschaltet wird, wird eine Kopie des La-
                                          gers mit negativen Lagernummern erzeugt, das sogenannte Inventurlager.
                                          In dieses Inventurlager werden die gezählten Bestände eingetragen.
                                          Während der Inventur werden die Eingänge und Ausgänge weiterhin auf
                                          die positive Lagernummer gebucht. Damit ist gewährleistet, dass während
                                          der Inventur Eingangs- und Ausgangsbuchungen für dieses Lager erfasst
                                          werden können.
                                          Nach einem Inventurabschluss werden die geänderten Bestände aus dem
                                          Inventurlager mit den Eingangs- und Ausgangsbuchungen aktualisiert, die
                                          während der Inventur erfasst wurden.

                                      Die Dialoge für die Inventur in den verschiedenen Lagerarten sind identisch
                                      aufgebaut und werden daher für das Standardlager beschrieben. Die Be-
                                      schreibung gilt daher gleichermaßen für:
                                      •   Kistenlager
                                      •   Fachlager
                                      •   Stapellager
                                      •   Gestelllager
                                      Sie können folgende Tastaturbefehle ausführen:
                                      •   Mit <F2> können Sie die Anzeige zwischen Artikel in Stückzahl und Artikel
                                          in Mengeneinheit umschalten.
                                      •   Mit <Shift> + <F8> können Sie die Inventur abschließen.
                                      •   Mit <Shift> + <F12> können Sie die Inventur verwerfen.

                                      Kopfbereich

                                      von Artikel, bis Artikel Wertebereich der Artikelnummern um die Inventur-
                                      liste zu filtern.

                                      von Lager, bis Lager Eingabe der Lagernummern:
                                      •   Wenn Sie in den Feldern von Lager, bis Lager dieselbe Lagernummer ein-
                                          geben, wird das Lager für die Inventur freigeschaltet.
                                      •   Wenn Sie in den Feldern von Lager, bis Lager einen Bereich von Lager-
                                          nummern eingeben, werden die Datensätze zur Ansicht in den Dialog ge-
                                          laden.

                                      Inventur/Bewertung vom Datum der Inventur.

                                      Rumpfbereich
                                      Folgende Spalten werden angezeigt:
                                      •   Artikel:
                                          Artikelnummer.
                                      •   Lager:
                                          Lagernummer.
1.01 / 01-2017




                                      •   Variante:
                                          Maßvariante der Position.



                 E-54                                                                         A+W Enterprise Lager
                 Softwarereferenz                                                                 Inventurverwaltung




                                        •   S:
                                            Storno des Artikels.
                                            – N = Kein Storno des Artikels.
                                            – J = Artikel wurde storniert.
                                        •   Soll-Anzahl:
                                            Anzeige für Soll-Stückzahl des Artikels im Lager.
                                        •   Ist-Anzahl:
                                            Eingabe für Ist-Stückzahl des gezählten Artikels im Lager.
                                        •   Preis:
                                            Gesamtpreis des Ist-Bestands des Artikels.
                                        •   ME:
                                            Durchschnittspreises pro Mengeneinheit für den Ist-Bestand, z. B. 75,00 €
                                            pro qm.
                                        •   Bemerkung:
                                            Inventurvermerk für statistische Auswertungen.
                                        Mit <F2> können Sie die folgenden Spalten anzeigen lassen:
                                        •   Soll-Bestand:
                                            Anzeige für Soll-Wert der Mengeneinheit des Artikelbestands im Lager.
                                        •   Ist-Bestand:
                                            Eingabe für Ist-Wert der gezählten Mengeneinheit des Artikelbestands im
                                            Lager.

                                        Fußbereich

                                        Artikel Artikelbezeichnung des ausgewählten Artikels.

                                        D-Preis Durchschnittspreis des ausgewählten Artikels für den Ist-Bestand.

                                        G-Preis Gesamtpreis des ausgewählten Artikels für den Ist-Bestand.

                                        Lager Lagerbezeichnung des ausgewählten Lagers.

                                        LIFO-Preis Artikelpreis im Lager, wenn nach der LIFO-Buchungsmethode
                                        abgebucht und berechnet wird.

                                        FIFO-Preis Artikelpreis im Lager, wenn nach der FIFO-Buchungsmethode
                                        abgebucht und berechnet wird.
1.01 / 01-2017




                 A+W Enterprise Lager                                                                           E-55
                 Inventurverwaltung                                                                    Softwarereferenz




                                           Inventur – Kistenlager
                                           Inventur > Kistenlager




                 Abb. E-21   Inventur-Kistenlager


                                           In diesem Dialog können Sie die Inventur für das Kistenlager durchführen und
                                           abschließen.
                                           Die Beschreibung für die Felder finden Sie an folgender Stelle:
                                            “Kopfbereich” auf Seite E-54

                                           Rumpfbereich
                                           •   Kiste:
                                               Kistennummer.
                                           •   Lager:
                                               Lagernummer.
                                           •   Artikel:
                                               Artikelnummer.
                                           •   Variante:
                                               Maßvariante der Position.
                                           •   S:
                                               Storno des Artikels.
                                               – N = Kein Storno des Artikels.
                                               – J = Artikel wurde storniert.
1.01 / 01-2017




                                           •   Menge:
                                               Gesamte Scheibenfläche in einer Kiste.



                 E-56                                                                            A+W Enterprise Lager
                 Softwarereferenz                                                                 Inventurverwaltung




                                        •   Anzahl:
                                            Anzahl der Scheiben in der Kiste.
                                        •   VA:
                                            Kennzeichen der Verpackungsart.
                                        •   Liefnr.:
                                            Lieferantennummer.
                                        •   ME:
                                            Durchschnittspreises pro Mengeneinheit für den Ist-Bestand, z. B. 75,00 €
                                            pro qm.
                                        •   Bemerkung:
                                            Inventurvermerk für statistische Auswertungen.

                                        Fußbereich

                                        Artikel Artikelbezeichnung.

                                        Lager Lagerbezeichnung.

                                        Kiste Kistenbezeichnung.

                                        Verpackart Kennzeichen der Verpackungsart.

                                        Lieferant Lieferantenname.
1.01 / 01-2017




                 A+W Enterprise Lager                                                                           E-57
                 Inventurverwaltung                                                                  Softwarereferenz




                                         Inventur – Fachlager
                                         Inventur > Fachlager




                 Abb. E-22   Inventur-Fachlager


                                         In diesem Dialog können Sie die Inventur für das Fachlager durchführen und
                                         abschließen.
                                         Die Beschreibung für die Felder finden Sie an folgender Stelle:
                                          “Kopfbereich” auf Seite E-54
                                          “Fußbereich” auf Seite E-55

                                         Rumpfbereich
                                         •   Lager:
                                             Lagernummer.
                                         •   Artikel:
                                             Artikelnummer.
                                         •   Variante:
                                             Maßvariante der Position.
                                         •   S:
                                             Storno des Artikels.
                                             – N = Kein Storno des Artikels.
                                             – J = Artikel wurde storniert.
                                         •   Fach:
1.01 / 01-2017




                                             Bezeichnung des Fachs.
                                         •   Menge:
                                             Menge des Artikels in Mengeneinheit.


                 E-58                                                                          A+W Enterprise Lager
                 Softwarereferenz                                                                    Inventurverwaltung




                                           •   Anzahl:
                                               Eingabe für Ist-Bestand des gezählten Artikelbestands im Stapel.
                                           •   Preis:
                                               Gesamtpreis des Ist-Bestands des Artikels.
                                           •   Bemerkung:
                                               Inventurvermerk für statistische Auswertungen.


                                           Inventur – Stapellager
                                           Inventur > Stapellager




                 Abb. E-23   Inventur-Stapellager


                                           In diesem Dialog können Sie die Inventur für das Stapellager durchführen und
                                           abschließen.
                                           Die Beschreibung für die Felder finden Sie an folgender Stelle:
                                            “Kopfbereich” auf Seite E-54
                                            “Fußbereich” auf Seite E-55

                                           Rumpfbereich
                                           •   Lager:
                                               Lagernummer.
                                           •   Artikel:
                                               Artikelnummer.
1.01 / 01-2017




                                           •   Variante:
                                               Maßvariante der Position.



                 A+W Enterprise Lager                                                                             E-59
                 Inventurverwaltung                                                                    Softwarereferenz




                                           •   S:
                                               Storno des Artikels.
                                               – N = Kein Storno des Artikels.
                                               – J = Artikel wurde storniert.
                                           •   Stapel:
                                               Stapelnummer.
                                           •   Bezeichnung:
                                               Bezeichnung des Stapels.
                                           •   Anzahl:
                                               Eingabe für Ist-Bestand des gezählten Artikelbestands im Stapel.
                                           •   Preis:
                                               Gesamtpreis des Ist-Bestands des Artikels.
                                           •   Bemerkung:
                                               Inventurvermerk für statistische Auswertungen.


                                           Inventur – Gestelllager
                                           Inventur > Gestelllager




                 Abb. E-24   Inventur-Gestelllager


                                           In diesem Dialog können Sie die Inventur für das Gestelllager durchführen und
                                           abschließen.
                                           Die Beschreibung für die Felder finden Sie an folgender Stelle:
1.01 / 01-2017




                                            “Kopfbereich” auf Seite E-54
                                            “Fußbereich” auf Seite E-55




                 E-60                                                                            A+W Enterprise Lager
                 Softwarereferenz                                                                  Inventurverwaltung




                                        Rumpfbereich
                                        •   Lager:
                                            Lagernummer.
                                        •   Artikel:
                                            Artikelnummer.
                                        •   Variante:
                                            Maßvariante der Position.
                                        •   S:
                                            Storno des Artikels.
                                            – N = Kein Storno des Artikels.
                                            – J = Artikel wurde storniert.
                                        •   Soll-Anzahl:
                                            Soll-Bestand des Artikels.
                                        •   Ist-Anzahl:
                                            Eingabe für Ist-Bestand des gezählten Artikelbestands im Stapel.
                                        •   Preis:
                                            Gesamtpreis des Ist-Bestands des Artikels.
                                        •   ME:
                                            Menge.
                                        •   Bemerkung:
                                            Inventurvermerk für statistische Auswertungen.
                                        Mit <F2> können Sie die folgenden Spalten anzeigen lassen:
                                        •   G:
                                            Artikelvarianten, die sich auf dem Gestell befinden.
                                             Verschiedene Artikelvarianten stehen auf einem Gestell.
                                             Nur gleiche Artikelvarianten stehen auf einem Gestell.
                                        •   Gestell:
                                            Bezeichnung des Gestells.
                                        •   Fach:
                                            Bezeichnung des Fachs.
                                        •   Soll:
                                            Soll-Bestand des Artikels.
                                        •   Ist:
                                            Ist-Bestand des Artikels.
                                        •   FIFO-Datum:
                                            Datum für die Gestellbuchung nach dem Fifo-Prinzip.
                                        •   Status:
                                            Status der Buchungen im Gestelllager.

                                        Buchungsstatus mit        Bedeutung
                                        Farbkennzeichen

                                            grau                  Buchungsposition ist vom Prozess (Programm)
                                                                  gebucht worden.
1.01 / 01-2017




                                            rot                   Buchungsposition ist vom Prozess (Programm) nicht
                                                                  oder noch nicht gebucht worden.

                                        Tab. E-12    Buchungsstatus im Gestelllager



                 A+W Enterprise Lager                                                                            E-61
                 Inventurverwaltung                                                                 Softwarereferenz




                                      Buchungsstatus mit        Bedeutung
                                      Farbkennzeichen

                                        gelb                    Buchungsposition ist geändert worden.

                                        halb gelb / halb grau   Buchungsposition ist ein Unterteil eines Auftrags.
                                                                Buchungsposition muss auf ein anderes Lager gebucht
                                                                werden, z. B. Fachlager.

                                      Tab. E-12    Buchungsstatus im Gestelllager
1.01 / 01-2017




                 E-62                                                                        A+W Enterprise Lager
                 Softwarereferenz                                                                           Bewertung




                                         Bewertung
                                         In der Bewertung können Sie die wertmäßigen Verluste des Umlaufvermö-
                                         gens innerhalb einer Inventur bearbeiten. Für die Inventur können die Gegen-
                                         stände des Umlaufvermögens mit dem Niederstwertprinzip (Anschaffungs-,
                                         Herstellungs- oder Tageswert) in der Schlussbilanz eingesetzt werden.
                                         In diesem Abschnitt sind folgende Dialoge erklärt:
                                         •   “Bestandsbewertung – Standardlager” auf Seite E-63
                                         •   “Bestandsbewertung – Kistenlager” auf Seite E-66
                                         •   “Bestandsbewertung – Fachlager” auf Seite E-67
                                         •   “Bestandsbewertung – Stapellager” auf Seite E-68
                                         •   “Bestandsbewertung – Gestelllager” auf Seite E-69


                                         Bestandsbewertung – Standardlager
                                         Bewertung > Lager




                 Abb. E-25   Bestandsbewertung – Standardlager


                                         In diesem Dialog können Sie eine wertmäßige Korrektur des Artikelbestands
                                         innerhalb einer Inventur durchführen, z. B. wenn die Werte eines Lagerartikels
                                         von den aktuellen Werten abweichen.
1.01 / 01-2017




                 A+W Enterprise Lager                                                                            E-63
                 Bewertung                                                               Softwarereferenz




                             Die Dialoge für die Bestandsbewertung in den verschiedenen Lagerarten sind
                             identisch aufgebaut und werden daher für das Standardlager beschrieben. Die
                             Beschreibung gilt daher gleichermaßen für:
                             •   Kistenlager
                             •   Fachlager
                             •   Stapellager
                             •   Gestelllager
                             Sie können folgende Tastaturbefehle ausführen:
                             •   Mit <F2> können Sie die Anzeige zwischen Artikel in Stückzahl und Artikel
                                 in Mengeneinheit umschalten. Die Funktion gilt nur für das Standardlager.
                             •   Mit <Ende> können Sie die wertmäßige Korrektur abschließen.

                             Kopfbereich

                             von Artikel, bis Artikel Wertebereich der Artikelnummern um die Liste zu
                             filtern.

                             von Lager, bis Lager Eingabe der Lagernummern:
                             •   Wenn Sie in den Feldern von Lager, bis Lager dieselbe Lagernummer ein-
                                 geben, wird das Lager für die Bestandsbewertung freigeschaltet.
                             •   Wenn Sie in den Feldern von Lager, bis Lager einen Bereich von Lager-
                                 nummern eingeben, werden die Datensätze zur Ansicht in den Dialog ge-
                                 laden.

                             Inventur/Bewertung vom Datum der Bestandsbewertung.

                             Rumpfbereich
                             Folgende Spalten werden angezeigt:
                             •   Lager:
                                 Lagernummer.
                             •   Artikel:
                                 Artikelnummer.
                             •   Variante:
                                 Maßvariante der Position.
                             •   S:
                                 Storno des Artikels.
                                 – N = Kein Storno des Artikels.
                                 – J = Artikel wurde storniert.
                             •   Soll-Anzahl:
                                 Anzeige für Soll-Stückzahl des Artikels im Lager.
                             •   Ist-Anzahl:
                                 Anzeige für Ist-Stückzahl des gezählten Artikels im Lager.
                             •   Preis:
                                 Eingabe für den Gesamtpreis des Ist-Bestands des Artikels.
1.01 / 01-2017




                 E-64                                                              A+W Enterprise Lager
                 Softwarereferenz                                                                        Bewertung




                                        •   ME:
                                            Eingabe des Durchschnittspreises pro Mengeneinheit für den Ist-Bestand,
                                            z. B. 75,00 € pro qm.
                                        •   Bemerkung:
                                            Inventurvermerk für statistische Auswertungen.
                                        Mit <F2> können Sie die folgenden Spalten anzeigen lassen:
                                        •   Soll-Bestand:
                                            Anzeige für Soll-Wert der Mengeneinheit des Artikelbestands im Lager.
                                        •   Ist-Bestand:
                                            Anzeige für Ist-Wert der gezählten Mengeneinheit des Artikelbestands im
                                            Lager.

                                        Fußbereich

                                        Artikel Artikelbezeichnung des ausgewählten Artikels.

                                        D-Preis Durchschnittspreis des ausgewählten Artikels für den Ist-Bestand.

                                        G-Preis Gesamtpreis des ausgewählten Artikels für den Ist-Bestand.

                                        Lager Lagerbezeichnung des ausgewählten Lagers.

                                        LIFO-Preis Artikelpreis im Lager, wenn nach der LIFO-Buchungsmethode
                                        abgebucht und berechnet wird.

                                        FIFO-Preis Artikelpreis im Lager, wenn nach der FIFO-Buchungsmethode
                                        abgebucht und berechnet wird.
1.01 / 01-2017




                 A+W Enterprise Lager                                                                         E-65
                 Bewertung                                                                           Softwarereferenz




                                         Bestandsbewertung – Kistenlager
                                         Bewertung > Kistenlager




                 Abb. E-26   Bestandsbewertung-Kistenlager


                                         In diesem Dialog können Sie eine wertmäßige Korrektur des Artikelbestands
                                         innerhalb einer Inventur durchführen, z. B. wenn die Werte von Kisten von den
                                         aktuellen Werten abweichen.
                                         Die Bestandsbewertung darf nur innerhalb eines einzelnen Lagers ausgeführt
                                         werden.
                                         Die Felder und Spalten sind an folgender Stelle beschrieben:
                                          “Bestandsbewertung – Standardlager” auf Seite E-63
1.01 / 01-2017




                 E-66                                                                           A+W Enterprise Lager
                 Softwarereferenz                                                                         Bewertung




                                         Bestandsbewertung – Fachlager
                                         Bewertung > Fachlager




                 Abb. E-27   Bestandsbewertung-Fachlager


                                         In diesem Dialog können Sie eine wertmäßige Korrektur des Artikelbestands
                                         innerhalb einer Inventur durchführen, z. B. wenn die Werte von Lagerartikeln
                                         eines Faches von den aktuellen Werten abweichen.
                                         Die Bestandsbewertung darf nur innerhalb eines einzelnen Lagers ausgeführt
                                         werden.
                                         Die Felder und Spalten sind an folgender Stelle beschrieben:
                                          “Bestandsbewertung – Standardlager” auf Seite E-63
1.01 / 01-2017




                 A+W Enterprise Lager                                                                           E-67
                 Bewertung                                                                           Softwarereferenz




                                         Bestandsbewertung – Stapellager
                                         Bewertung > Stapellager




                 Abb. E-28   Bestandsbewertung-Stapellager


                                         In diesem Dialog können Sie eine wertmäßige Korrektur des Artikelbestands
                                         innerhalb einer Inventur durchführen, z. B. wenn die Werte von Artikeln eines
                                         Stapels von den aktuellen Werten abweichen.
                                         Die Bestandsbewertung darf nur innerhalb eines einzelnen Lagers ausgeführt
                                         werden.
                                         Die Felder und Spalten sind an folgender Stelle beschrieben:
                                          “Bestandsbewertung – Standardlager” auf Seite E-63
1.01 / 01-2017




                 E-68                                                                           A+W Enterprise Lager
                 Softwarereferenz                                                                           Bewertung




                                          Bestandsbewertung – Gestelllager
                                          Bewertung > Gestelllager




                 Abb. E-29   Bestandsbewertung-Gestelllager


                                          In diesem Dialog können Sie eine wertmäßige Korrektur des Artikelbestands
                                          innerhalb einer Inventur durchführen, z. B. wenn die Werte von Artikeln eines
                                          Gestells von den aktuellen Werten abweichen.
                                          Die Bestandsbewertung darf nur innerhalb eines einzelnen Lagers ausgeführt
                                          werden.
                                          Die Felder und Spalten sind an folgender Stelle beschrieben:
                                           “Bestandsbewertung – Standardlager” auf Seite E-63
                                          Sie können folgenden Tastaturbefehl ausführen:
                                          Mit <F2> können Sie die Anzeige für Artikel von Stückzahl zu Mengeneinheit
                                          umschalten. Die Funktion gilt nur für das Gestelllager.
1.01 / 01-2017




                 A+W Enterprise Lager                                                                             E-69
                 Informationssystem                                                                  Softwarereferenz




                                      Informationssystem
                                      Im Informationssystem können Sie die Lagerdaten überwachen. Über das In-
                                      formationssystem können Sie die Suchfunktionen ausführen.
                                      In diesem Abschnitt sind folgende Dialoge erklärt:
                                      •   “Info-Lager-Artikel” auf Seite E-71
                                      •   “Info-Lager-Varianten” auf Seite E-75
                                      •   “Info-Lager-Fächer” auf Seite E-79
                                      •   “Info-Lager-Gestelle” auf Seite E-82
                                      •   “Info-Lager-Stapel” auf Seite E-85
                                      •   “Info-Lager-Blätter” auf Seite E-88
                                      •   “Info-Lager-Historie” auf Seite E-91
                                      •   “Aufträge/Bestellungen” auf Seite E-96
                                      •   “Buchungsstatus” auf Seite E-100
                                      •   “Lagerinformationen – Pickliste” auf Seite E-105
                                      •   “Lagerinformationen – Trefferliste” auf Seite E-106
                                      •   “LVR-Status” auf Seite E-107
                                      •   “Reichweite – Bestandsprognose” auf Seite E-107
                                      •   “Reichweite – Trefferliste” auf Seite E-108
                                      •   “Dispositiver Bestand” auf Seite E-109
                                      •   “Bestandsprognose” auf Seite E-110
                                      Zusätzlich können Sie sich individuelle Informationsübersichten mittels
                                      SQL-Abfragen zusammenstellen.
                                       Verkauf, “SQL-Abfragen – Ausführen” auf Seite D-217
1.01 / 01-2017




                 E-70                                                                           A+W Enterprise Lager
                 Softwarereferenz                                                                      Informationssystem




                                        Info-Lager-Artikel
                                        Infosystem > Artikel
                                        In diesem Dialog können Sie sich die Lagerbestände oder Artikelbestände an-
                                        zeigen lassen.
                                        Zu diesem Dialog werden folgende Unterdialoge angezeigt:
                                        •   “Info-Lager-Artikel – Filterdialog” auf Seite E-71
                                        •   “Info-Lager-Artikel – Trefferliste” auf Seite E-72
                                        •   “Info-Lager-Artikel – Trefferliste-Details” auf Seite E-73


                                        Info-Lager-Artikel – Filterdialog
                                        Infosystem > Artikel




                                        Abb. E-30     Info-Lager-Artikel – Filterdialog


                                        In diesem Dialog können Sie die Suchkriterien festlegen, um sich die Lager-
                                        bestände oder Artikelbestände anzeigen zu lassen. Die Ergebnisse der Suche
                                        können Sie sich in der Trefferliste und in der Detailansicht anzeigen lassen.
                                         “Info-Lager-Artikel – Trefferliste” auf Seite E-72
                                         “Info-Lager-Artikel – Trefferliste-Details” auf Seite E-73

                                        Artikel Artikelnummer.

                                        Lager Lagernummer.

                                        Menge Artikel in Mengeneinheit.

                                        Gesamtpreis Gesamtpreis des Artikelbestands im ausgewählten Lager.

                                        Durchschnittspreis Durchschnittlicher Preis pro Mengeneinheit des Arti-
                                        kels.

                                        Letzte Änderung Datum, an dem der Buchungssatz zuletzt gebucht wurde.
1.01 / 01-2017




                 A+W Enterprise Lager                                                                               E-71
                 Informationssystem                                                                       Softwarereferenz




                                      Info-Lager-Artikel – Trefferliste
                                      Infosystem > Artikel > Filtern




                                      Abb. E-31      Info-Lager-Artikel – Trefferliste


                                      In diesem Dialog werden die Ergebnisse der Suche nach Lagerartikeln ange-
                                      zeigt.
                                      Details zu den Lagerartikeln werden in der Detailansicht angezeigt.
                                       “Info-Lager-Artikel – Trefferliste-Details” auf Seite E-73
                                      Mit <F5> wechseln Sie zwischen der Trefferliste und der Detailansicht der aus-
                                      gewählten Position.

                                      Trefferliste
                                      Folgende Spalten werden angezeigt:
                                      •   Artikel:
                                          Artikelnummer.
                                      •   Lager:
                                          Lagernummer.
                                      •   Bestand:
                                          Lagerbestand des Artikels in Mengeneinheit.
                                      •   G-Preis:
                                          Gesamtpreis des Artikels.
                                      •   D-Preis:
                                          Durchschnittspreis pro Mengeneinheit.
                                      •   H-Preis:
                                          Höchster Einkaufspreis pro Mengeneinheit.
                                      •   N-Preis:
                                          Niedrigster Einkaufspreis pro Mengeneinheit.
1.01 / 01-2017




                 E-72                                                                                A+W Enterprise Lager
                 Softwarereferenz                                                                  Informationssystem




                                        Info-Lager-Artikel – Trefferliste-Details
                                        Infosystem > Artikel > Filtern > <F5>




                                        Abb. E-32    Info-Lager-Artikel – Trefferliste-Details


                                        In diesem Dialog werden die Details zur Trefferliste der Lagerartikel angezeigt.
                                        Mit <F5> wechseln Sie zwischen der Trefferliste und der Detailansicht der aus-
                                        gewählten Position.

                                        Details

                                        Artikel Artikelnummer und Artikelbezeichnung.

                                        Lager Lagernummer.

                                        Bestand Lagerbestand des Artikels in Mengeneinheit.

                                        Mindestbestand Minimalbestand des Artikels auf Lager.

                                        Alarmbestand Alarmbestand des Artikels auf Lager.

                                        Bestandobergrenze Maximalbestand des Artikels auf Lager.

                                        Höchstbestand Maximalstückzahl des Artikels auf Lager, seit der letzten In-
                                        ventur.

                                        Niedrigstbestand Minimalstückzahl des Artikels auf Lager, seit der letzten
                                        Inventur.

                                        D-Bestand Durchschnittlicher Lagerbestand des Artikels, seit der letzten In-
1.01 / 01-2017




                                        ventur.

                                        D-Verbrauch Durchschnittliche Lagerabbuchung des Artikels, seit der letzten
                                        Inventur.


                 A+W Enterprise Lager                                                                             E-73
                 Informationssystem                                                             Softwarereferenz




                                      Gesamtpreis Gesamtpreis des Artikels.

                                      D-Preis Durchschnittspreis pro Mengeneinheit.

                                      Höchstpreis Höchster Einkaufspreis des Artikels.

                                      Niedrigstpreis Niedrigster Einkaufspreis des Artikels.

                                      LIFO-Gesamtpreis Gesamtpreis der Artikelvariante im Lager, wenn nach
                                      der LIFO-Buchungsmethode abgebucht und berechnet wird.

                                      FIFO-Gesamtpreis Gesamtpreis der Artikelvariante im Lager, wenn nach
                                      der FIFO-Buchungsmethode abgebucht und berechnet wird.

                                      Letzte Änderung am, von Datum, an dem der Buchungssatz gebucht wur-
                                      de und Name des Anwenders, der die Buchung ausgeführt hat.
1.01 / 01-2017




                 E-74                                                                      A+W Enterprise Lager
                 Softwarereferenz                                                                        Informationssystem




                                        Info-Lager-Varianten
                                        Infosystem > Variante
                                        In diesem Dialog können Sie sich die Informationen zu den Artikelvarianten
                                        nach ausgewählten Kriterien anzeigen lassen.
                                        Zu diesem Dialog werden folgende Unterdialoge angezeigt:
                                        •   “Info-Lager-Varianten – Filterdialog” auf Seite E-75
                                        •   “Info-Lager-Varianten – Trefferliste” auf Seite E-76
                                        •   “Info-Lager-Varianten – Trefferliste-Details” auf Seite E-77


                                        Info-Lager-Varianten – Filterdialog
                                        Infosystem > Variante




                                        Abb. E-33     Info-Lager-Varianten – Filterdialog


                                        In diesem Dialog können Sie die Informationen zu den Artikelvarianten nach
                                        ausgewählten Kriterien filtern. Die Ergebnisse werden in einer Trefferliste an-
                                        gezeigt. Die Details können Sie in der Detailansicht einsehen.
                                         “Info-Lager-Varianten – Trefferliste” auf Seite E-76
                                         “Info-Lager-Varianten – Trefferliste-Details” auf Seite E-77

                                        Artikel Artikelnummer.

                                        Lager Lagernummer.

                                        Variante Maßvariante des Artikels in der Kiste.

                                        Farbe Farbvariante des Artikels.

                                        Kiste Kistennummer.

                                        Kistenbezeichnung Bezeichnung der Kiste.
1.01 / 01-2017




                                        Letzte Änderung Datum, an dem der Buchungssatz gebucht wurde.

                                        Menge Artikel in Mengeneinheit.


                 A+W Enterprise Lager                                                                                 E-75
                 Informationssystem                                                                         Softwarereferenz




                                           Anzahl Stückzahl des Artikels.

                                           Gesamtpreis Gesamtpreis des Artikelbestands.

                                           Durchschnittspreis Durchschnittlicher Preis pro Mengeneinheit des Arti-
                                           kels.


                                           Info-Lager-Varianten – Trefferliste
                                           Infosystem > Variante > Filtern




                 Abb. E-34   Info-Lager-Varianten – Trefferliste


                                           In diesem Dialog können Sie die Informationen zu den Artikelvarianten nach
                                           ausgewählten Kriterien filtern. Die Ergebnisse werden in einer Trefferliste an-
                                           gezeigt. Die Details können Sie in der Detailansicht einsehen.
                                            “Info-Lager-Varianten – Trefferliste-Details” auf Seite E-77
                                           Mit <F5> wechseln Sie zwischen der Trefferliste und der Detailansicht der aus-
                                           gewählten Position.

                                           Trefferliste
                                           •   Artikel:
                                               Artikelnummer.
                                           •   Bezeichnung:
                                               Artikelbezeichnung.
1.01 / 01-2017




                                           •   Lager:
                                               Lagernummer.




                 E-76                                                                                  A+W Enterprise Lager
                 Softwarereferenz                                                                     Informationssystem




                                           •   Kiste:
                                               Kistennummer.
                                           •   Variante:
                                               Maßvariante des Artikels in der Kiste.
                                           •   Farbe:
                                               Farbvariante des Artikels.
                                           •   Anzahl:
                                               Stückzahl des Artikels.
                                           •   Bestand:
                                               Artikelbestand in Mengeneinheit.
                                           •   Netto-ME:
                                               Netto-Menge pro Kiste in Mengeneinheit des Artikels.
                                           •   Preis:
                                               Gesamtpreis des Artikels.


                                           Info-Lager-Varianten – Trefferliste-Details
                                           Infosystem > Variante > Filtern > <F5>




                 Abb. E-35   Info-Lager-Varianten – Trefferliste-Details


                                           In diesem Dialog werden die Details zur Trefferliste der Artikelvarianten ange-
                                           zeigt.
                                           Mit <F5> wechseln Sie zwischen der Trefferliste und der Detailansicht der aus-
                                           gewählten Position.

                                           Details

                                           Artikel Artikelnummer und Artikelbezeichnung.

                                           Lager Lagernummer.

                                           Kiste Kistennummer und Kistenbezeichnung.
1.01 / 01-2017




                                           Variante Abmessungen der Variante.




                 A+W Enterprise Lager                                                                               E-77
                 Informationssystem                                                              Softwarereferenz




                                      Farbe Farbvariante des Artikels.

                                      Anzahl Stückzahl des Artikels.

                                      Bestand Artikelbestand in Mengeneinheit.

                                      Netto Menge Netto-Menge pro Kiste in Mengeneinheit des Artikels.

                                      Mindestbestand Minimalbestand des Artikels auf Lager.

                                      Alarmbestand Alarmbestand des Artikels auf Lager.

                                      Bestandobergrenze Maximalbestand des Artikels auf Lager.

                                      Höchstbestand Maximalstückzahl des Artikels auf Lager, seit der letzten In-
                                      ventur.

                                      Niedrigstbestand Minimalstückzahl des Artikels auf Lager, seit der letzten
                                      Inventur.

                                      D-Bestand Durchschnittlicher Lagerbestand des Artikels, seit der letzten In-
                                      ventur.

                                      D-Verbrauch Durchschnittliche Lagerabbuchung des Artikels, seit der letzten
                                      Inventur.

                                      Gesamtpreis Gesamtpreis des Artikels.

                                      D-Preis Durchschnittspreis pro Mengeneinheit.

                                      Höchstpreis Höchster Einkaufspreis des Artikels.

                                      Niedrigstpreis Niedrigster Einkaufspreis des Artikels.

                                      LIFO-Gesamtpreis Gesamtpreis der Artikelvariante im Lager, wenn nach
                                      der LIFO-Buchungsmethode abgebucht und berechnet wird.

                                      FIFO-Gesamtpreis Gesamtpreis der Artikelvariante im Lager, wenn nach
                                      der FIFO-Buchungsmethode abgebucht und berechnet wird.

                                      Letzte Änderung am, von Datum, an dem der Buchungssatz gebucht wur-
                                      de und Name des Anwenders, der die Buchung ausgeführt hat.
1.01 / 01-2017




                 E-78                                                                      A+W Enterprise Lager
                 Softwarereferenz                                                                     Informationssystem




                                        Info-Lager-Fächer
                                        Infosystem > Fach
                                        In diesem Dialog können Sie sich die Informationen zu den Lagerfächern an-
                                        zeigen lassen.
                                        Zu diesem Dialog werden folgende Unterdialoge angezeigt:
                                        •   “Info-Lager-Fächer – Filterdialog” auf Seite E-79
                                        •   “Info-Lager-Fächer – Trefferliste” auf Seite E-80
                                        •   “Info-Lager-Fächer – Trefferliste-Details” auf Seite E-81


                                        Info-Lager-Fächer – Filterdialog
                                        Infosystem > Fach




                                        Abb. E-36     Info-Lager-Fächer – Filterdialog


                                        In diesem Dialog können Sie die Informationen zu den Lagerfächern nach
                                        ausgewählten Kriterien filtern. Die Ergebnisse werden in einer Trefferliste an-
                                        gezeigt. Die Details können Sie in der Detailansicht einsehen.
                                         “Info-Lager-Fächer – Trefferliste” auf Seite E-80
                                         “Info-Lager-Fächer – Trefferliste-Details” auf Seite E-81

                                        Artikel Artikelnummer.

                                        Lager Lagernummer.

                                        Fach Bezeichnung des Fachs.

                                        Variante Abmessungen der Variante.

                                        Farbe Farbvariante des Artikels.

                                        Datum Datum, an dem der Buchungssatz gebucht wurde.

                                        Anzahl Stückzahl des Artikels.
1.01 / 01-2017




                                        Menge Artikel in Mengeneinheit.




                 A+W Enterprise Lager                                                                              E-79
                 Informationssystem                                                                       Softwarereferenz




                                      Info-Lager-Fächer – Trefferliste
                                      Infosystem > Fach > Filtern




                                      Abb. E-37      Info-Lager-Fächer – Trefferliste


                                      In diesem Dialog werden die Ergebnisse der Suche nach Lagerfächern ange-
                                      zeigt. Die Details können Sie in der Detailansicht einsehen.
                                       “Info-Lager-Artikel – Trefferliste-Details” auf Seite E-73
                                      Mit <F5> wechseln Sie zwischen der Trefferliste und der Detailansicht der aus-
                                      gewählten Position.

                                      Trefferliste
                                      •   Artikel:
                                          Artikelnummer.
                                      •   Lager:
                                          Lagernummer.
                                      •   Fach:
                                          Bezeichnung des Fachs.
                                      •   Variante:
                                          Abmessungen der Variante.
                                      •   Menge:
                                          Artikel in Mengeneinheit.
                                      •   Stück:
                                          Stückzahl des Artikels.
                                      •   Preis:
                                          Gesamtpreis des Artikels.
                                      •   Datum:
                                          Datum, an dem der Buchungssatz gebucht wurde.
1.01 / 01-2017




                 E-80                                                                                A+W Enterprise Lager
                 Softwarereferenz                                                                 Informationssystem




                                        Info-Lager-Fächer – Trefferliste-Details
                                        Infosystem > Fach > Filtern > <F5>




                                        Abb. E-38    Info-Lager-Fächer – Trefferliste-Details


                                        In diesem Dialog werden die Details zur Trefferliste der Lagerfächer ange-
                                        zeigt.
                                        Mit <F5> wechseln Sie zwischen der Trefferliste und der Detailansicht der aus-
                                        gewählten Position.

                                        Details

                                        Artikel Artikelnummer.

                                        Lager Lagernummer.

                                        Fach Bezeichnung des Fachs.

                                        Variante Abmessungen der Variante.

                                        Farbe Farbvariante des Artikels.

                                        Menge Artikel in Mengeneinheit.

                                        Stück Stückzahl des Artikels.

                                        Preis Gesamtpreis des Artikels.
1.01 / 01-2017




                 A+W Enterprise Lager                                                                           E-81
                 Informationssystem                                                                     Softwarereferenz




                                      Info-Lager-Gestelle
                                      Infosystem > Gestell
                                      In diesem Dialog können Sie sich die Informationen zu den Lagergestellen an-
                                      zeigen lassen.
                                      Zu diesem Dialog werden folgende Unterdialoge angezeigt:
                                      •   “Info-Lager-Gestelle – Filterdialog” auf Seite E-82
                                      •   “Info-Lager-Gestelle – Trefferliste-Allgemein” auf Seite E-83
                                      •   “Info-Lager-Gestelle – Trefferliste-Details” auf Seite E-84


                                      Info-Lager-Gestelle – Filterdialog
                                      Infosystem > Gestell




                                      Abb. E-39     Info-Lager-Gestelle – Filterdialog


                                      In diesem Dialog können Sie die Informationen zu den Lagergestellen nach
                                      ausgewählten Kriterien filtern. Die Ergebnisse werden in einer Trefferliste an-
                                      gezeigt. Die Details können Sie in der Detailansicht einsehen.
                                       “Info-Lager-Gestelle – Trefferliste-Allgemein” auf Seite E-83
                                       “Info-Lager-Gestelle – Trefferliste-Details” auf Seite E-84

                                      Lager Lagernummer.

                                      Gestellnr. Nummer des Lagergestells.

                                      Gestell Bezeichnung des Gestells.

                                      Fach Bezeichnung des Fachs.

                                      Artikel Artikelnummer.

                                      Variante Abmessungen der Variante.

                                      Farbe Farbvariante des Artikels.
1.01 / 01-2017




                                      Anzahl Stückzahl des Artikels.

                                      Fifo-Datum Datum für die Gestellbuchung nach dem Fifo-Prinzip.


                 E-82                                                                            A+W Enterprise Lager
                 Softwarereferenz                                                                          Informationssystem




                                           Info-Lager-Gestelle – Trefferliste-Allgemein
                                           Infosystem > Gestell > Filtern > Allgemein




                 Abb. E-40   Info-Lager-Gestelle – Trefferliste-Allgemein


                                           In diesem Dialog werden die Ergebnisse der Suche nach Lagergestellen an-
                                           gezeigt. Die Details können Sie in der Detailansicht einsehen.
                                            “Info-Lager-Gestelle – Trefferliste-Details” auf Seite E-84
                                           Mit <F5> wechseln Sie zwischen der Trefferliste und der Detailansicht der aus-
                                           gewählten Position.

                                           Trefferliste
                                           •   Lager:
                                               Lagernummer.
                                           •   Artikel:
                                               Artikelnummer.
                                           •   Variante:
                                               Abmessungen der Variante.
                                           •   Gestellnr.:
                                               Nummer des Lagergestells.
                                           •   Gestell:
                                               Bezeichnung des Gestells.
                                           •   Fach:
                                               Bezeichnung des Fachs.
                                           •   Bezeichnung:
1.01 / 01-2017




                                               Bezeichnung des Fachs.
                                           •   Stück:
                                               Stückzahl des Artikels.


                 A+W Enterprise Lager                                                                                   E-83
                 Informationssystem                                                                    Softwarereferenz




                                           •   Preis:
                                               Gesamtpreis des Artikels.
                                           •   Fifo-Datum:
                                               Datum für die Gestellbuchung nach dem Fifo-Prinzip.


                                           Info-Lager-Gestelle – Trefferliste-Details
                                           Infosystem > Gestell > Filtern > Details




                 Abb. E-41   Info-Lager-Gestelle – Trefferliste-Details


                                           In diesem Dialog werden die Details zur Trefferliste der Lagergestelle ange-
                                           zeigt.
                                           Mit <F5> wechseln Sie zwischen der Trefferliste und der Detailansicht der aus-
                                           gewählten Position.

                                           Details

                                           Artikel Artikelnummer.

                                           Variante Abmessungen der Variante.

                                           Farbe Farbvariante des Artikels.

                                           Stück Stückzahl des Artikels.

                                           Preis Gesamtpreis des Artikels.
1.01 / 01-2017




                                           Lager Lagernummer.




                 E-84                                                                            A+W Enterprise Lager
                 Softwarereferenz                                                                     Informationssystem




                                        Gestell Bezeichnung des Gestells.

                                        Fach Bezeichnung des Fachs.

                                        Fifo-Datum Datum für die Gestellbuchung nach dem Fifo-Prinzip.

                                        Letzte Änderung am, von Datum der letzten Änderung am Buchungssatz
                                        und Name des Anwenders, der die letzte Buchung ausgeführt hat.


                                        Info-Lager-Stapel
                                        Infosystem > Stapel
                                        In diesem Dialog können Sie sich die Informationen zu den Lagerstapeln an-
                                        zeigen lassen.
                                        Zu diesem Dialog werden folgende Unterdialoge angezeigt:
                                        •   “Info-Lager-Stapel – Filterdialog” auf Seite E-85
                                        •   “Info-Lager-Stapel – Trefferliste” auf Seite E-86
                                        •   “Info-Lager-Stapel – Trefferliste-Details” auf Seite E-87


                                        Info-Lager-Stapel – Filterdialog
                                        Infosystem > Stapel




                                        Abb. E-42     Info-Lager-Stapel – Filterdialog


                                        In diesem Dialog können Sie die Informationen zu den Lagerstapeln nach aus-
                                        gewählten Kriterien filtern. Die Ergebnisse werden in einer Trefferliste ange-
                                        zeigt. Die Details können Sie in der Detailansicht einsehen.
                                         “Info-Lager-Stapel – Trefferliste” auf Seite E-86
                                         “Info-Lager-Stapel – Trefferliste-Details” auf Seite E-87

                                        Artikel Artikelnummer.

                                        Lager Lagernummer.
1.01 / 01-2017




                                        Stapel Stapelnummer.

                                        Stapelbez. Bezeichnung des Stapels.


                 A+W Enterprise Lager                                                                              E-85
                 Informationssystem                                                                            Softwarereferenz




                                            Variante Abmessungen der Variante.

                                            Farbe Farbvariante des Artikels.

                                            Datum Datum, an dem der Buchungssatz gebucht wurde.

                                            Anzahl Stückzahl des Artikels.

                                            Menge Artikel in Mengeneinheit.


                                            Info-Lager-Stapel – Trefferliste
                                            Infosystem > Stapel > Filtern




                 Abb. E-43   Info-Lager-Stapel – Trefferliste


                                            In diesem Dialog werden die Ergebnisse der Suche nach Lagerstapel ange-
                                            zeigt. Die Details können Sie in der Detailansicht einsehen.
                                             “Info-Lager-Stapel – Trefferliste-Details” auf Seite E-87
                                            Mit <F5> wechseln Sie zwischen der Trefferliste und der Detailansicht der aus-
                                            gewählten Position.

                                            Trefferliste
                                            •   Stapel:
                                                Stapelnummer.
1.01 / 01-2017




                                            •   Bezeichnung:
                                                Bezeichnung des Stapels.
                                            •   Artikel:
                                                Artikelnummer.


                 E-86                                                                                     A+W Enterprise Lager
                 Softwarereferenz                                                                 Informationssystem




                                        •   Lager:
                                            Lagernummer.
                                        •   Variante:
                                            Abmessungen der Variante.
                                        •   Menge:
                                            Artikel in Mengeneinheit.
                                        •   Stück:
                                            Stückzahl des Artikels.
                                        •   Preis:
                                            Gesamtpreis des Artikels.
                                        •   Datum:
                                            Datum, an dem der Buchungssatz gebucht wurde.


                                        Info-Lager-Stapel – Trefferliste-Details
                                        Infosystem > Stapel > Filtern > <F5>




                                        Abb. E-44    Info-Lager-Stapel – Trefferliste-Details


                                        In diesem Dialog werden die Details zur Trefferliste der Lagerstapel angezeigt.
                                        Mit <F5> wechseln Sie zwischen der Trefferliste und der Detailansicht der aus-
                                        gewählten Position.

                                        Details

                                        Artikel Artikelnummer.
1.01 / 01-2017




                                        Lager Lagernummer.



                 A+W Enterprise Lager                                                                            E-87
                 Informationssystem                                                                 Softwarereferenz




                                      Stapel Stapelnummer.

                                      Variante Abmessungen der Variante.

                                      Farbe Farbvariante des Artikels.

                                      Menge Artikel in Mengeneinheit.

                                      Stück Stückzahl des Artikels.

                                      Preis Gesamtpreis des Artikels.

                                      Letzte Änderung am, von Datum der letzten Änderung am Buchungssatz
                                      und Name des Anwenders, der die letzte Buchung ausgeführt hat.


                                      Info-Lager-Blätter
                                      Infosystem > Blatt
                                      In diesem Dialog können Sie sich die Informationen zu den Glasblättern im
                                      Einzelblattkistenlager anzeigen lassen.
                                      Zu diesem Dialog werden folgende Unterdialoge angezeigt:
                                      •   “Info-Lager-Blätter – Filterdialog” auf Seite E-88
                                      •   “Info-Lager-Blätter – Trefferliste” auf Seite E-89


                                      Info-Lager-Blätter – Filterdialog
                                      Infosystem > Blatt




                                      Abb. E-45     Info-Lager-Blätter – Filterdialog


                                      In diesem Dialog können Sie die Informationen zu den Glasblättern im Einzel-
                                      blattkistenlager nach ausgewählten Kriterien filtern. Die Ergebnisse werden in
                                      einer Trefferliste angezeigt.
                                       “Info-Lager-Blätter – Trefferliste” auf Seite E-89
1.01 / 01-2017




                 E-88                                                                          A+W Enterprise Lager
                 Softwarereferenz                                                              Informationssystem




                                        Blatt Nummer des Glasblattes.

                                        Blattbezeichnung Bezeichnung des Glasblattes.

                                        Artikel Artikelnummer.

                                        Lager Lagernummer.

                                        Kiste Kistennummer.

                                        Kistenbezeichnung Bezeichnung der Kiste.

                                        Variante Abmessungen der Variante.

                                        Farbe Farbvariante des Artikels.

                                        Preis Stückpreis des Glasblattes.

                                        Ausbeute Ausbeute des Glasblattes in Prozent.


                                        Info-Lager-Blätter – Trefferliste
                                        Infosystem > Blatt > Filtern




                                        Abb. E-46    Info-Lager-Blätter – Trefferliste


                                        In diesem Dialog werden die Ergebnisse der Suche nach Glasblättern im Ein-
                                        zelblattkistenlager angezeigt.
1.01 / 01-2017




                 A+W Enterprise Lager                                                                       E-89
                 Informationssystem                                                                Softwarereferenz




                                      Trefferliste
                                      •   Artikel:
                                          Artikelnummer.
                                      •   Lager:
                                          Lagernummer.
                                      •   Kiste:
                                          Kistennummer.
                                      •   Variante:
                                          Abmessungen der Variante.
                                      •   Blatt:
                                          Nummer des Glasblattes.
                                      •   Bezeichnung:
                                          Bezeichnung des Glasblattes.
                                      •   Preis:
                                          Stückpreis des Glasblattes.
                                      •   Ausb.:
                                          Ausbeute des Glasblattes in Prozent.
                                      •   R.:
                                          Reservierungskennzeichen.
                                          – J = Variante ist für einen Vorgang reserviert.
                                          – N = Variante ist nicht für einen Vorgang reserviert.
1.01 / 01-2017




                 E-90                                                                        A+W Enterprise Lager
                 Softwarereferenz                                                                       Informationssystem




                                        Info-Lager-Historie
                                        Infosystem > Historie
                                        In diesem Dialog können Sie die Informationen über die Lagerbuchungen an-
                                        zeigen lassen.
                                        Zu diesem Dialog werden folgende Unterdialoge angezeigt:
                                        •   “Info-Lager-Historie – Filterdialog” auf Seite E-91
                                        •   “Info-Lager-Historie – Trefferliste” auf Seite E-92
                                        •   “Info-Lager-Historie – Trefferliste-Details” auf Seite E-94


                                        Info-Lager-Historie – Filterdialog
                                        Infosystem > Historie




                                        Abb. E-47     Info-Lager-Historie – Filterdialog


                                        In diesem Dialog können Sie die Informationen über die Lagerbuchungen
                                        nach ausgewählten Kriterien filtern. Die Ergebnisse werden in einer Trefferlis-
                                        te angezeigt. Die Details können Sie in der Detailansicht einsehen.
                                         “Info-Lager-Historie – Trefferliste” auf Seite E-92
                                         “Info-Lager-Historie – Trefferliste-Details” auf Seite E-94

                                        Artikel Artikelnummer.

                                        Lager Lagernummer.

                                        Lieferant Lieferantennummer.

                                        Auftrag Auftragsnummer.

                                        Opti-Nr Die Job-Nummer für die Schnittstelle XTV wird nur angezeigt, wenn
                                        die Funktion entsprechend konfiguriert wurde.

                                        Variante Maßvariante des Artikels.

                                        Farbe Farbvariante des Artikels.
1.01 / 01-2017




                                        Stapel Stapelnummer.




                 A+W Enterprise Lager                                                                                E-91
                 Informationssystem                                                                              Softwarereferenz




                                            Blattbez. Bezeichnung des Glasblattes.

                                            Kiste Kistennummer.

                                            Datum Datum, an dem der Buchungssatz gebucht wurde.

                                            Anzahl Stückzahl des Artikels.

                                            Menge Artikel in Mengeneinheit.

                                            Preis Gesamtpreis des Artikels.

                                            Kostenstelle Bezeichnung der Kostenstelle.

                                            Status Status des aktuellen Satzes, z. B. Lagerausgang.


                                            Info-Lager-Historie – Trefferliste
                                            Infosystem > Historie > Filtern




                 Abb. E-48   Info-Lager-Historie – Trefferliste


                                            In diesem Dialog werden die Ergebnisse der Suche nach Lagerbuchungen an-
                                            gezeigt. Die Details können Sie in der Detailansicht einsehen.
                                             “Info-Lager-Historie – Trefferliste-Details” auf Seite E-94
                                            Mit <F5> wechseln Sie zwischen der Trefferliste und der Detailansicht der aus-
1.01 / 01-2017




                                            gewählten Position.




                 E-92                                                                                       A+W Enterprise Lager
                 Softwarereferenz                                                              Informationssystem




                                        Trefferliste
                                        •   Artikel:
                                            Artikelnummer.
                                        •   Lager:
                                            Lagernummer.
                                        •   Variante:
                                            Maßvariante des Artikels.
                                        •   Fach:
                                            Bezeichnung des Fachs.
                                        •   Stück:
                                            Stückzahl des Artikels.
                                        Mit <F2> können Sie sich die folgenden Spalten anzeigen lassen:
                                        •   Kiste:
                                            Kistennummer.
                                        •   VA:
                                            Kennzeichen der Verpackungsart.
                                        •   Lieferant:
                                            Lieferantennummer.
                                        •   Stapel:
                                            Stapelnummer.
                                        •   L-Preis:
                                            Artikelpreis im Lager, wenn nach der LIFO-Buchungsmethode abgebucht
                                            und berechnet wird.
                                        •   F-Preis:
                                            Artikelpreis im Lager, wenn nach der FIFO-Buchungsmethode abgebucht
                                            und berechnet wird.
                                        •   Auftr.:
                                            Auftragsnummer.
1.01 / 01-2017




                 A+W Enterprise Lager                                                                       E-93
                 Informationssystem                                                                     Softwarereferenz




                                            Info-Lager-Historie – Trefferliste-Details
                                            Infosystem > Historie > Filtern > <F5>




                 Abb. E-49   Info-Lager-Historie – Trefferliste-Details


                                            In diesem Dialog werden die Details zur Trefferliste der Lagerbuchungen an-
                                            gezeigt.
                                            Mit <F5> wechseln Sie zwischen der Trefferliste und der Detailansicht der aus-
                                            gewählten Position.

                                            Details

                                            Artikel Artikelnummer.

                                            Lager Lagernummer.

                                            Kiste Kistennummer.

                                            Verpackart Kennzeichen der Verpackungsart.

                                            Lieferant Lieferantennummer.

                                            Fach Bezeichnung des Fachs.

                                            Blatt Nummer und Bezeichnung des Blattes.
1.01 / 01-2017




                                            Auftrag Auftragsnummer.




                 E-94                                                                             A+W Enterprise Lager
                 Softwarereferenz                                                             Informationssystem




                                        Opti-Nr Die Job-Nummer für die Schnittstelle XTV wird nur angezeigt, wenn
                                        die Funktion entsprechend konfiguriert wurde.

                                        Kunde Kundennummer und Kundenname.

                                        Variante Maßvariante des Artikels.

                                        Farbe Farbvariante des Artikels.

                                        Buchungsanzahl Stückzahl, die für diesen Buchungssatz gebucht wurde.

                                        Buchungsmenge Gesamtmenge in Mengeneinheit, die gebucht wurde.

                                        Buchungspreis Gesamtpreis der gebuchten Mengen.

                                        LIFO-Preis Artikelpreis im Lager, wenn nach der LIFO-Buchungsmethode
                                        abgebucht und berechnet wird.

                                        FIFO-Preis Artikelpreis im Lager, wenn nach der FIFO-Buchungsmethode
                                        abgebucht und berechnet wird.

                                        Kostenstelle Bezeichnung der Kostenstelle.

                                        Letzte Buchung am, von Datum der letzten Änderung am Buchungssatz
                                        und Name des Anwenders, der die letzte Buchung ausgeführt hat.

                                        Bemerkung Zusätzliche Informationen aus der Lagereingangsbuchung.
1.01 / 01-2017




                 A+W Enterprise Lager                                                                       E-95
                 Informationssystem                                                                     Softwarereferenz




                                      Aufträge/Bestellungen
                                      Infosystem > Aufträge/Bestellungen
                                      In diesem Dialog können Sie die Informationen zu auftrags- oder bestellbezo-
                                      genen Buchungen anzeigen lassen.
                                      Zu diesem Dialog werden folgende Unterdialoge angezeigt:
                                      •   “Aufträge/Bestellungen – Filterdialog” auf Seite E-96
                                      •   “Aufträge/Bestellungen – Trefferliste” auf Seite E-97
                                      •   “Aufträge/Bestellungen – Trefferliste-Details” auf Seite E-98


                                      Aufträge/Bestellungen – Filterdialog
                                      Infosystem > Aufträge/Bestellungen




                                      Abb. E-50     Aufträge/Bestellungen – Filterdialog


                                      In diesem Dialog können Sie die Informationen zu auftrags- oder bestellbezo-
                                      genen Buchungen im Lager nach ausgewählten Kriterien filtern. Die Ergebnis-
                                      se werden in einer Trefferliste angezeigt. Die Details können Sie in der
                                      Detailansicht einsehen.
                                       “Aufträge/Bestellungen – Trefferliste” auf Seite E-97
                                       “Aufträge/Bestellungen – Trefferliste-Details” auf Seite E-98

                                      Auftrag Auftragsnummer oder Bestellnummer.

                                      Artikel Artikelnummer.

                                      Lager Lagernummer.

                                      Variante Nummer der Artikelvariante.

                                      Farbe Nummer der Farbvariante.
1.01 / 01-2017




                 E-96                                                                             A+W Enterprise Lager
                 Softwarereferenz                                                                            Informationssystem




                                           Buchung Buchungsstatus des Auftrags oder der Bestellung.
                                           Folgende Optionen stehen zur Auswahl:
                                           • 0 = noch keine Buchung ausgeführt.
                                           • 1 = Teilbuchung einer Position ausgeführt.
                                           • 2 = Position komplett gebucht.
                                           • 3 = Auftrag oder Bestellung wurde komplett gebucht.

                                           Datum Datum, an dem die Lagerbuchung zum Auftrag oder zur Bestellung
                                           ausgeführt wurde.


                                           Aufträge/Bestellungen – Trefferliste
                                           Infosystem > Aufträge/Bestellungen > Filtern




                 Abb. E-51   Aufträge/Bestellungen – Trefferliste


                                           In diesem Dialog werden die Ergebnisse der Suche nach auftrags- oder be-
                                           stellbezogenen Buchungen im Lager angezeigt. Die Details können Sie in der
                                           Detailansicht einsehen.
                                            “Aufträge/Bestellungen – Trefferliste-Details” auf Seite E-98
                                           Mit <F5> wechseln Sie zwischen der Trefferliste und der Detailansicht der aus-
                                           gewählten Position.

                                           Trefferliste
                                           •   Auftrag:
1.01 / 01-2017




                                               Auftragsnummer oder Bestellnummer.
                                           •   Position:
                                               Nummer der Position im Auftrag oder in der Bestellung.


                 A+W Enterprise Lager                                                                                     E-97
                 Informationssystem                                                                      Softwarereferenz




                                           •   Artikel:
                                               Artikelnummer.
                                           •   Lager:
                                               Lagernummer.
                                           •   Variante:
                                               Nummer der Artikelvariante.
                                           •   Anzahl:
                                               Zu verbuchende Stückzahl pro Position.
                                           •   Menge:
                                               Buchungsmenge in der Mengeneinheit des Artikels.
                                           •   Verbucht:
                                               Buchungsanzahl in Stück, die gebucht wurde.
                                           •   Datum:
                                               Datum, an dem die Lagerbuchung zum Auftrag oder zur Bestellung ausge-
                                               führt wurde.


                                           Aufträge/Bestellungen – Trefferliste-Details
                                           Infosystem > Aufträge/Bestellungen > Filtern > <F5>




                 Abb. E-52   Aufträge/Bestellungen – Trefferliste-Details


                                           In diesem Dialog werden die Details zur Trefferliste der auftrags- oder bestell-
                                           bezogenen Buchungen im Lager angezeigt.
                                           Mit <F5> wechseln Sie zwischen der Trefferliste und der Detailansicht der aus-
                                           gewählten Position.
1.01 / 01-2017




                 E-98                                                                              A+W Enterprise Lager
                 Softwarereferenz                                                              Informationssystem




                                        Details

                                        Artikelnummer Artikelnummer und Artikelbezeichnung.

                                        Lager Lagernummer.

                                        Variante Nummer der Artikelvariante.

                                        Farbe Nummer der Farbvariante.

                                        Auftrag Auftragsnummer oder Bestellnummer.

                                        Position Nummer der Position im Auftrag oder in der Bestellung.

                                        Anzahl Zu verbuchende Stückzahl pro Position.

                                        Menge Buchungsmenge in der Mengeneinheit des Artikels.

                                        Buchung Buchungsstatus des Auftrags oder der Bestellung.
                                        Folgende Optionen stehen zur Auswahl:
                                        • 0 = noch keine Buchung ausgeführt.
                                        • 1 = Teilbuchung einer Position ausgeführt.
                                        • 2 = Position komplett gebucht.
                                        • 3 = Auftrag oder Bestellung wurde komplett gebucht.

                                        Datum Datum, an dem die Lagerbuchung zum Auftrag oder zur Bestellung
                                        ausgeführt wurde.

                                        Verbucht (Anzahl) Verbuchte Stückzahl des Artikels.

                                        Verbucht (Menge) Verbuchte Menge in der Mengeneinheit des Artikels.

                                        Erfasser (Mitarbeiter) Erfassungsdatum und Mitarbeiter, der diese Buchung
                                        erfasst hat.

                                        Verbucht (Mitarbeiter) Buchungsdatum und Mitarbeiter, der diese Buchung
                                        durchgeführt hat.
1.01 / 01-2017




                 A+W Enterprise Lager                                                                       E-99
                 Informationssystem                                                              Softwarereferenz




                                      Buchungsstatus
                                      Infosystem > Buchungsstatus
                                      Im Buchungsstatus können Sie sich die Buchungsinformationen zu den La-
                                      gern anzeigen lassen, die nicht gebuchten oder fehlerhaften Buchungssätze
                                      enthalten oder Lager die sich gerade in der Inventur befinden. Im Dialog Bu-
                                      chungsstatus – Korrektur können Sie die Daten für den Buchungsstatus korri-
                                      gieren.
                                      Zu diesem Dialog werden folgende Unterdialoge angezeigt:
                                      •   “Buchungsstatus – Ungebucht” auf Seite E-100
                                      •   “Buchungsstatus – Fehler” auf Seite E-102
                                      •   “Buchungsstatus – Inventur” auf Seite E-103
                                      •   “Buchungsstatus – Korrektur” auf Seite E-104


                                      Buchungsstatus – Ungebucht
                                      Infosystem > Buchungsstatus > Ungebucht




                                      Abb. E-53    Buchungsstatus – Ungebucht


                                      In diesem Dialog können Sie sich Buchungsinformationen zu den Lagern an-
                                      zeigen lassen, die nicht gebuchte Buchungssätze enthalten.
                                      Sie können folgende Tastaturbefehle ausführen:
                                      •   Mit <F5> können Sie den Dialog Buchungsstatus – Korrektur aufrufen.
                                      •   Mit <F2> können Sie sich weitere Spalten anzeigen lassen.

                                      Rumpfbereich
                                      •   Artikel:
                                          Artikelnummer.
1.01 / 01-2017




                                      •   Lager:
                                          Lagernummer.



                 E-100                                                                     A+W Enterprise Lager
                 Softwarereferenz                                                               Informationssystem




                                        •   Kiste:
                                            Kistennummer.
                                        •   Variante:
                                            Maßvariante des Artikels.
                                        •   Farbe:
                                            Nummer der Artikelfarbe.
                                        •   Anzahl:
                                            Anzahl der nicht gebuchten Artikel.
                                        •   Status:
                                            Nummer des Status der aktuellen Buchung, z. B. Lagerausgang.
                                        •   Fehler:
                                            Nummer für den Fehlerstatus. Der Fehlerstatus steht im Fußbereich im
                                            Klartext.
                                        Mit <F2> können Sie sich weitere Spalten anzeigen lassen.
                                        •   Menge:
                                            Mengeneinheit des Artikels.
                                        •   Preis:
                                            Preis pro Mengeneinheit, z. B. Artikel pro Stück.
                                        •   Datum:
                                            Datum der Lagerbuchung.
                                        •   Auftrag:
                                            Auftragsnummer.
                                        •   Position:
                                            Positionsnummer im Auftrag.

                                        Fußbereich
                                        Die Feldbeschreibungen entsprechen den Spaltenbeschreibungen des Dia-
                                        logs.
1.01 / 01-2017




                 A+W Enterprise Lager                                                                       E-101
                 Informationssystem                                                             Softwarereferenz




                                      Buchungsstatus – Fehler
                                      Infosystem > Buchungsstatus > Fehler




                                      Abb. E-54    Buchungsstatus – Fehler


                                      In diesem Dialog können Sie sich Buchungsinformationen zu den Lagern an-
                                      zeigen lassen, die fehlerhafte Buchungssätze enthalten. Im Dialog Buchungs-
                                      status – Korrektur können Sie die Daten für den Buchungsstatus korrigieren.
                                      Sie können folgende Tastaturbefehle ausführen:
                                      •   Mit <F5> können Sie den Dialog Buchungsstatus – Korrektur aufrufen.
                                      •   Mit <F2> können Sie sich weitere Spalten anzeigen lassen.

                                      Rumpfbereich
                                      •   Artikel:
                                          Artikelnummer.
                                      •   Lager:
                                          Lagernummer.
                                      •   Kiste:
                                          Kistennummer.
                                      •   Variante:
                                          Maßvariante des Artikels.
                                      •   Farbe:
                                          Nummer der Artikelfarbe.
                                      •   Anzahl:
                                          Anzahl der nicht gebuchten Artikel.
                                      •   Status:
                                          Nummer des Status der aktuellen Buchung, z. B. Lagerausgang.
                                      •   Fehler:
                                          Nummer für den Fehlerstatus. Der Fehlerstatus steht im Fußbereich im
1.01 / 01-2017




                                          Klartext.




                 E-102                                                                    A+W Enterprise Lager
                 Softwarereferenz                                                               Informationssystem




                                        Mit <F2> können Sie sich weitere Spalten anzeigen lassen.
                                        •   Menge:
                                            Mengeneinheit des Artikels.
                                        •   Preis:
                                            Preis pro Mengeneinheit, z. B. Artikel pro Stück.
                                        •   Datum:
                                            Datum der Lagerbuchung.
                                        •   Auftrag:
                                            Auftragsnummer.
                                        •   Position:
                                            Positionsnummer im Auftrag.

                                        Fußbereich
                                        Die Feldbeschreibungen entsprechen den Spaltenbeschreibungen des Dia-
                                        logs.


                                        Buchungsstatus – Inventur
                                        Infosystem > Buchungsstatus > Inventur




                                        Abb. E-55    Buchungsstatus – Inventur


                                        In diesem Dialog können Sie sich Buchungsinformationen zu den Lager an-
                                        zeigen lassen, die nicht gebuchten oder fehlerhaften Buchungssätze enthal-
                                        ten oder Lager die sich gerade in der Inventur befinden. Im Dialog
                                        Buchungsstatus – Korrektur können Sie die Daten für den Buchungsstatus
                                        korrigieren.
                                        Sie können folgenden Tastaturbefehl ausführen:
                                        •   Mit <F5> können Sie den Dialog Buchungsstatus – Korrektur aufrufen.
1.01 / 01-2017




                 A+W Enterprise Lager                                                                       E-103
                 Informationssystem                                                                Softwarereferenz




                                      Rumpfbereich
                                      •   Lager:
                                          Lagernummer des Lagers, das zur Inventur freigeschaltet ist.
                                      •   Bezeichnung:
                                          Bezeichnung des Lagers in Inventur.
                                      •   Datum:
                                          Datum, an dem das Lager zur Inventur vorbereitet wurde.
                                      •   Mitarbeiter:
                                          Mitarbeiternummer des Mitarbeiters, der das Lager zur Inventur vorbereitet
                                          hat.


                                      Buchungsstatus – Korrektur
                                      Infosystem > Buchungsstatus > Ungebucht, Fehler, Inventur > <F5>




                                      Abb. E-56    Buchungsstatus – Korrektur


                                      In diesem Dialog können Sie die Daten des Buchungsstatus der folgenden Di-
                                      aloge korrigieren:
                                      •   Buchungsstatus – Ungebucht
                                      •   Buchungsstatus – Fehler
                                      •   Buchungsstatus – Inventur

                                      Rumpfbereich

                                      Artikel Artikelnummer und Artikelbezeichnung.

                                      Lager Lagernummer und Lagerbezeichnung.

                                      Lieferant Lieferantennummer und Lieferantenname.
1.01 / 01-2017




                                      Kiste Kistennummer und Kistenbezeichnung.

                                      Fach Bezeichnung des Fachs im Fachlager.


                 E-104                                                                       A+W Enterprise Lager
                 Softwarereferenz                                                                 Informationssystem




                                        Auftrag Auftragsnummer, bei auftragsbezogenen Lagerbuchungen.

                                        Variante Maßvariante des Artikels.

                                        Farbe Nummer der Artikelfarbe.

                                        Buchungsanzahl Gebuchte Menge in Stück.

                                        Buchungsmenge Gebuchte Menge in der entsprechenden Mengeneinheit.

                                        Buchungspreis Gesamtpreis der Artikel.

                                        verbucht am Datum der letzten Buchung des aktuellen Buchungssatzes.

                                        von Name des Mitarbeiters, der den aktuellen Buchungssatz zuletzt gebucht
                                        hat.

                                        Fußbereich

                                        Artikel Artikelbezeichnung.

                                        Lager Lagerbezeichnung.

                                        Fehler Fehlerstatus im Klartext.

                                        Status Status der aktuellen Buchung im Klartext, z. B. Lagerausgang.


                                        Lagerinformationen – Pickliste
                                        Infosystem > Auftragsliste




                                        Abb. E-57    Lagerinformationen – Pickliste


                                        In diesem Dialog können Sie sich die auftragsbezogenen Lagerartikel anzei-
                                        gen lassen. Für die Ausgabe der Lagerinformationen der Pickliste wird die Ad-
                                        hoc-SQL Gruppe 1 und die SQL-Abfrage 26 verwendet. Bei Bedarf muss
                                        diese Abfrage separat angepasst werden. Die Abfrage können Sie über
                                        <Strg> + <F4> > SQL-Abfragen > Ändern anpassen.

                                        Auftrag Auftragsnummer, für die die Pickliste erstellt wird.
1.01 / 01-2017




                 A+W Enterprise Lager                                                                          E-105
                 Informationssystem                                                                Softwarereferenz




                                      Lagerinformationen – Trefferliste
                                      Infosystem > Auftragsliste > Filtern




                                      Abb. E-58      Lagerinformationen – Trefferliste


                                      In diesem Dialog wird Ihnen die Trefferliste für auftragsbezogene Lagerartikel
                                      angezeigt.

                                      Trefferliste
                                      •   Artikel:
                                          Artikelnummer.
                                      •   Bezeichnung:
                                          Artikelbezeichnung.
                                      •   Farbe:
                                          Bezeichnung der Farbvariante des Artikels.
                                      •   Variante:
                                          Abmessungen der Artikelvariante.
                                      •   Menge:
                                          Stückzahl des Artikels.
                                      •   Auftrag:
                                          Auftragsnummer.
                                      •   Spalten ohne Namen:
                                          Positionsnummer im Auftrag.
1.01 / 01-2017




                 E-106                                                                       A+W Enterprise Lager
                 Softwarereferenz                                                                   Informationssystem




                                        LVR-Status
                                        Infosystem > LVR-Status




                                        Abb. E-59    SQL-Abfragen – Lagerverwaltungsrechner (LVR)


                                        Dieser Dialog wird zur Zeit nicht genutzt.


                                        Reichweite – Bestandsprognose
                                        Infosystem > Reichweite




                                        Abb. E-60    Reichweite – SQL-Abfragen


                                        In diesem Dialog können Sie sich die Bestandsprognose für Lagerartikel an-
                                        zeigen lassen. Für die Ausgabe der Bestandsprognose der Reichweite wird
                                        die Adhoc-SQL Gruppe 1 und die SQL-Abfrage 21 verwendet. Bei Bedarf
                                        muss diese Abfrage separat angepasst werden. Die Abfrage können Sie über
                                        <Strg> + <F4> > SQL-Abfragen > Ändern anpassen.

                                        Von Artikel Startwert für den Wertebereich der Artikelnummer, um die Tref-
                                        ferliste zu filtern.

                                        Bis Artikel Maximalwert für den Wertebereich der Artikelnummer, um die
                                        Trefferliste zu filtern.

                                        Von Lager Startwert für den Wertebereich der Lagernummer, um die Treffer-
                                        liste zu filtern.

                                        Bis Lager Maximalwert für den Wertebereich der Lagernummer, um die Tref-
                                        ferliste zu filtern.
1.01 / 01-2017




                 A+W Enterprise Lager                                                                          E-107
                 Informationssystem                                                              Softwarereferenz




                                      Reichweite – Trefferliste
                                      Infosystem > Reichweite > Filtern




                                      Abb. E-61      Reichweite – Trefferliste


                                      In diesem Dialog wird Ihnen anhand von Lagerbuchungen eine Prognose an-
                                      gezeigt, für wie viele Monate der aktuelle Bestand des Lagerartikels für die
                                      Produktion ausreicht.

                                      Trefferliste
                                      •   Artikel:
                                          Artikelnummer.
                                      •   Bestand:
                                          Aktueller Lagerbestand des Artikels.
                                      •   Verbrauch:
                                          Verbrauch des Artikels in der Vergangenheit.
                                      •   Reichweite (Mon):
                                          Geschätzte Zeit in Monaten, die der Artikel noch auf Lager zur Verfügung
                                          steht.
1.01 / 01-2017




                 E-108                                                                      A+W Enterprise Lager
                 Softwarereferenz                                                                  Informationssystem




                                        Dispositiver Bestand
                                        Infosystem > Dispositiver Bestand




                                        Abb. E-62    Dispositiver Bestand


                                        In diesem Dialog können Sie sich den aktuellen Lagerbestand des Artikels, die
                                        bestellten, verplanten und verfügbaren Mengen des Lagerartikels anzeigen
                                        lassen.

                                        Kopfbereich

                                        Datum Filterkriterium nach Datum.

                                        Artikel Filterkriterium für die Artikelnummer.

                                        Variante Filterkriterium für die Maßvariante.

                                        Rumpfbereich
                                        •   Variante:
                                            Maßvariante des Artikels.
                                        •   Lager:
                                            Lagernummer des Lagers, in dem der Artikel eingelagert ist.
                                        •   Bezeichnung:
                                            Bezeichnung des Lagerartikels.
                                        •   Bestand:
                                            Aktueller Bestand des Lagerartikels.
                                        •   Bestellt:
                                            Aktuell bestellte Menge des Lagerartikels.
                                        •   Verplant:
                                            Aktuell verplante Menge des Lagerartikels, z. B. für die Produktion.
1.01 / 01-2017




                                        •   Verfügbar:
                                            Aktuell verfügbare Menge des Lagerartikels.




                 A+W Enterprise Lager                                                                              E-109
                 Informationssystem                                                              Softwarereferenz




                                      Fußbereich

                                      Gesamtsumme Summierter Wert jeweils für eine Spalte. Folgende Spalten
                                      werden aufsummiert angezeigt:
                                      •   Bestand
                                      •   Bestellt
                                      •   Verplant
                                      •   Verfügbar


                                      Bestandsprognose
                                      Infosystem > Prognose




                                      Abb. E-63    Bestandsprognose


                                      In diesem Dialog können Sie sich für einen ausgewählten Zeitraum die Prog-
                                      nose für den Lagerbestand des Artikels anzeigen lassen. Verplante Bestände
                                      entstehen durch erfasste Aufträge. Die Prognose zeigt den Lagerbestand auf-
                                      grund von im System vorhandenen Aufträgen und bereits bestehenden Be-
                                      stellungen.
                                      Die Unter- oder Überdeckung der Lagerbestände kann durch definierte Alarm-
                                      bestände verhindert werden.
                                       “Artikelstammdaten Lager” auf Seite E-51
                                      Mit <Shift> + <F5> lassen Sie sich für den ausgewählten Artikel die Bestands-
                                      prognose in der grafischen Übersicht anzeigen.
1.01 / 01-2017




                 E-110                                                                      A+W Enterprise Lager
                 Softwarereferenz                                                                Informationssystem




                                        Kopfbereich

                                        Artikel Artikelnummer für die gefilterte Auflistung.

                                        Lager Lagernummer. Wenn in diesem Feld kein Eintrag erfolgt, wird eine la-
                                        gerübergreifende Bestandsprognose erstellt.

                                        Variante Maßvariante des Artikels.

                                        Datum Zeitraum der Bestandsprognose.

                                        Periode Zeitabstände in der Bestandsprognose.

                                        Rumpfbereich
                                        Die Spalten sind im Kopfbereich beschrieben. Zusätzlich werden folgende
                                        Spalten angezeigt:
                                        •   Datum:
                                            Datumsangabe für die Bestandsprognose zu verplanten, bestellten und zu
                                            dem Zeitpunkt auf Lager vorhandenen Artikeln.
                                        •   Verplant:
                                            Verplante Artikel aus dem Lager, zu dem entsprechend in der ersten Spalte
                                            angezeigten Datum.
                                        •   Bestellt:
                                            Bestellte Artikel für das Lager, zu dem entsprechend in der ersten Spalte
                                            angezeigten Datum.
                                        •   Bestand:
                                            Bestand des Artikels auf Lager, zu dem entsprechend in der ersten Spalte
                                            angezeigten Datum.
1.01 / 01-2017




                 A+W Enterprise Lager                                                                          E-111
                 Druck                                                               Softwarereferenz




                         Druck
                         Im Druck können Sie Informationen über die Lagerdaten oder Etiketten dru-
                         cken. Sie können das Seitenlayout für den Listendruck oder die Etiketten frei
                         definieren.
                         In diesem Abschnitt sind folgende Dialoge erklärt:
                         •   “Kistenetiketten drucken” auf Seite E-112
                         •   “Listendruck” auf Seite E-113


                         Kistenetiketten drucken
                         Druck > Etiketten




                         Abb. E-64     Kistenetiketten drucken


                         In diesem Dialog können Sie sich die offenen Druckaufträge für Kistenetiket-
                         ten anzeigen lassen und drucken.
                         Mit <Shift> + <F3> starten Sie den Etikettendruck.
                         •   Kiste:
                             Kistennummer.
                         •   Anzahl:
                             Stückzahl der Artikel in der Kiste.
                         •   Artikel:
                             Artikelnummer.
                         •   Variante:
                             Maßvariante des Artikels.
1.01 / 01-2017




                         •   Lager:
                             Lagernummer.



                 E-112                                                         A+W Enterprise Lager
                 Softwarereferenz                                                                            Druck




                                        •   Kost.St.:
                                            Bezeichnung der Kostenstelle.
                                        •   Spalte ohne Bezeichnung:
                                            Anzeige für den Etikettendruck:
                                            – J = Etiketten drucken.
                                            – N = Keine Etiketten drucken.
                                        •   Anz.:
                                            Anzahl der zu druckenden Etiketten.
                                        •   Erfasst:
                                            Datum, an dem der Kisteneingang erfasst wurde.
                                        •   Gedruckt:
                                            Datum, an dem das Etikett der Kiste zuletzt ausgedruckt wurde.


                                        Listendruck
                                        Druck > Listendruck




                                        Abb. E-65    Listendruck


                                        Der Dialog ist ausführlich an folgender Stelle beschrieben:
                                         Verkauf, “Listendruck” auf Seite D-162
1.01 / 01-2017




                 A+W Enterprise Lager                                                                        E-113
                 Systemverwaltung                                                               Softwarereferenz




                                    Systemverwaltung
                                    In der Systemverwaltung können Sie die Lagerprotokolle und die Preiskorrek-
                                    turen der Lagerartikel verwalten.
                                    In diesem Abschnitt sind folgende Dialoge erklärt:
                                    •   “Lagerprotokoll löschen” auf Seite E-114
                                    •   “Lager-Preiskorrektur” auf Seite E-114


                                    Lagerprotokoll löschen
                                    System > Lagerprotokoll löschen




                                    Abb. E-66    Lagerprotokoll löschen


                                    In diesem Dialog können Sie ein Lagerprotokoll im System löschen.

                                    Artikel Artikelnummer.

                                    Lager Lagernummer.

                                    Variante Maßvariante des Artikels.

                                    Farbe Farbvariante des Artikels.


                                    Lager-Preiskorrektur
                                    System > Preiskorrektur




                                    Abb. E-67    Lager-Preiskorrektur
1.01 / 01-2017




                                    In diesem Dialog können Sie den Durchschnittspreis für eingekaufte Lagerar-
                                    tikel korrigieren. Fehlerhafte Preisbuchungen für Lagerartikel verfälschen den
                                    Durchschnittspreis in der Statistik und können nur über den Höchstpreis und
                                    den Niedrigstpreis korrigiert werden.


                 E-114                                                                    A+W Enterprise Lager
                 Softwarereferenz                                                                Systemverwaltung




                                        Artikel Artikelnummer.

                                        Lager Lagernummer.

                                        Variante Maßvariante des Artikels.

                                        Farbe Farbvariante des Artikels.

                                        Höchstpreis Höchster Einkaufspreis der Variante im Lager.

                                        Niedrigstpreis Niedrigster Einkaufspreis der Variante im Lager.
1.01 / 01-2017




                 A+W Enterprise Lager                                                                      E-115
                 Servicefunktionen                                                                 Softwarereferenz




                                     Servicefunktionen
                                     Servicefunktionen werden nur auf Anforderung durch den Servicemitarbeiter
                                     der A+W Software GmbH ausgeführt.
                                     Die Servicefunktionen finden Sie an folgender Stelle:
                                      Versandsteuerung, “Servicefunktionen” auf Seite E-90
1.01 / 01-2017




                 E-116                                                                        A+W Enterprise Lager
Lager                E

               Partindex




        A+W Enterprise
                 Partindex                                                                              Index




                 Index
                 A                                           D
                 Artikelbestand                              Dispositiver Bestand
                 – Fachlager korrigieren E-67                – Infosystem E-109
                 – Gestelllager korrigieren E-69             Druck
                 – Kistenlager korrigieren E-66              – Kistenetiketten E-112
                 – Standardlager korrigieren E-63            – Listen E-113
                 – Stapellager korrigieren E-68
                 Artikelstammdaten                           F
                 – Bestandsgrenzen für Lagerartikel   E-51   Fachlager
                 Aufträge/Bestellungen                       – Artikelbestand korrigieren   E-67
                 – Infosystem E-96, E-97, E-98               – Ausgänge buchen E-34
                                                             – Eingänge buchen E-29
                 B                                           – Inventur E-58
                 Bestände anzeigen
                 – Artikelvarianten E-75, E-76, E-77         G
                 – Blätter E-88, E-89                        Gestelllager
                 – Lagerartikel E-71, E-72, E-73             – Artikelbestand korrigieren   E-69
                 – Lagerfächer E-79, E-80, E-81              – Ausgänge buchen E-41
                 – Lagergestelle E-82, E-83, E-84            – Eingänge buchen E-38
                 – Lagerhistorie E-91, E-92, E-94            – Inventur E-60
                 – Lagerstapel E-85, E-86, E-87
                 Bestandsbewertung
                 – Fachlager E-67                            I
                 – Gestelllager E-69                         Info-Lager-Artikel
                 – Kistenlager E-66                          – Bestände anzeigen E-71, E-72, E-73
                 – Standardlager E-63                        Info-Lager-Blätter
                 – Stapellager E-68                          – Bestände anzeigen E-88, E-89
                 Bestandsgrenzen für Lagerartikel            Info-Lager-Fächer
                 – Artikelstammdaten E-51                    – Bestände anzeigen E-79, E-80, E-81
                 Bestandsprognose                            Info-Lager-Gestelle
                 – Infosystem E-110                          – Bestände anzeigen E-82, E-83, E-84
                 Buchung                                     Info-Lager-Historie
                 – Auftragsbezug, mit E-45                   – Bestände anzeigen E-91, E-92, E-94
                 – Fachlager E-29, E-34                      Info-Lager-Stapel
                 – Gestelllager E-38, E-41                   – Bestände anzeigen E-85, E-86, E-87
                 – Kistenlager E-23, E-28                    Info-Lager-Varianten
                 – Standardlager E-16, E-22                  – Bestände anzeigen E-75, E-76, E-77
                 – Stapellageränderung E-36                  Infosystem
                 – Stapellagereingang E-35                   – Aufträge/Bestellungen E-96, E-97, E-98
                 Buchungskorrektur                           – Bestandsprognose E-110
                 – offene Buchungen bearbeiten E-47, E-48    – Buchungsstatus, Fehler E-102
                 Buchungsstatus                              – Buchungsstatus, Inventur E-103
                 – Fehler E-102                              – Buchungsstatus, Korrektur E-104
                 – Inventur E-103                            – Buchungsstatus, nicht gebuchte
                 – Korrektur E-104                             Buchungssätze E-100
                                                             – Dispositiver Bestand E-109
1.01 / 01-2017




                 – nicht gebuchte Buchungssätze E-100
                                                             – Reichweite Bestand E-108




                 A+W Enterprise Lager                                                               E-119
                 Index                                                                      Partindex




                 Inventur                              S
                 – Fachlager E-58                      SQL-Abfragen
                 – Gestelllager E-60                   – Lagerinformationen E-105
                 – Kistenlager E-56                    – Reichweite Bestand E-107
                 – Standardlager E-53                  Standardlager
                 – Stapellager E-59                    – Artikelbestand korrigieren E-63
                                                       – Ausgänge buchen E-22
                 K                                     – Eingänge buchen E-16
                 Kistenetiketten                       – Inventur E-53
                 – Druck E-112                         Stapellager
                 Kistenlager                           – Änderungen buchen E-36
                 – Artikelbestand korrigieren   E-66   – Artikelbestand korrigieren E-68
                 – Ausgänge buchen E-28                – Ausgänge buchen E-36
                 – Eingänge buchen E-23                – Eingang buchen E-35
                 – Inventur E-56                       – Inventur E-59

                 L
                 Lagerartikel
                 – Preiskorrektur E-114
                 Lagerausgang
                 – auftragsbezogen buchen E-45
                 – buchen E-22
                 Lagereingang
                 – buchen E-16
                 Lagerinformationen
                 – Pickliste E-106
                 – SQL-Abfragen E-105
                 Lagerprotokoll
                 – löschen E-114
                 Lagerraumverwaltung
                 – Lagerräume, neu anlegen E-50
                 Listendruck
                 – drucken E-113
                 Löschen
                 – Lagerprotokoll E-114

                 M
                 Menüs    E-9

                 P
                 Pickliste
                 – Lagerinformationen E-106
                 Preiskorrektur
                 – Lagerartikel E-114

                 R
                 Reichweite
                 – Infosystem E-108
1.01 / 01-2017




                 – SQL-Abfragen E-107




                 E-120                                                          A+W Enterprise Lager

