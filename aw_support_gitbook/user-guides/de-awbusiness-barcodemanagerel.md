---
title: "DE AWBusiness BarcodeManagerEL"
category: "user_manuals"
product: "AWBusiness"
doc_type: "Unknown"
language: "EN"
tags: ["AWBusiness", "BarcodeManagerEL"]
version: "1.0"
last_updated: "2025-12-10"
description: "Barcode Manager (EL)       A                                Deutsch                       A+W Business                                                                                                           Vorspann                                            Vorspann                                        In diesem Teil der Dokumentation finden Sie editorische Notizen.                                          Revisionsübersicht                                        Version/Datum Beschreibun"
source_file: "DE-AWBusiness-BarcodeManagerEL.pdf"
---


# DE AWBusiness BarcodeManagerEL

Barcode Manager (EL)       A




                           Deutsch




                  A+W Business
                                                                                                          Vorspann




                                       Vorspann
                                       In diesem Teil der Dokumentation finden Sie editorische Notizen.


                                       Revisionsübersicht
                                       Version/Datum Beschreibung

                                       1.00/03-2023   Ersterstellung, Überführung aus docx-Dokument



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
                                       Dieses Dokument beschreibt die volle Ausbaustufe von A+W Business.

                                       Urheberrechte
                                       © 2017, A+W Software GmbH, alle Rechte, auch des Nachdrucks, der Her-
                                       stellung von Kopien und der Übersetzung, bleiben vorbehalten.
                                       Die Dokumentation darf nur gemäß dem Lizenzvertrag ganz oder in Teilen ko-
                                       piert, in einem Archivierungssystem gespeichert oder in irgendeiner anderen
                                       Form übertragen werden. Ohne die vorherige schriftliche Genehmigung von
                                       A+W Software GmbH darf die Dokumentation weder elektronisch, mecha-
                                       nisch, per Aufzeichnung oder in sonstiger Form übertragen werden.

                                       Warenzeichen
1.00 / 03-2023




                                       Alle in der Dokumentation erwähnten Hard- und Softwarebezeichnungen kön-
                                       nen gleichzeitig auch eingetragene Marken oder sonstige gewerbliche
                                       Schutzrechte Dritter sein. Die Schutzrechte Dritter sind zu beachten.


                 A+W Business Barcode Manager (EL)                                                            A-3
                 Vorspann




                            Kontakte
                            A+W Software GmbH

                            Am Pfahlgraben 4-10

                            D-35415 Pohlheim

                               +49 6404 2051-0

                               +49 6404 2051-877

                            zentrale@a-w.com

                            http://www.a-w.com
1.00 / 03-2023




                 A-4                               A+W Business Barcode Manager (EL)
                                                                                                                                                             Inhalt




                                       Inhalt
                                       Vorspann ................................................................................................................ A-3
                                        Revisionsübersicht .............................................................................................. A-3
                                        Editorial ............................................................................................................... A-3

                                       Einleitung                                                                                                            A-7
                                       Einleitung ................................................................................................................ A-9
                                       Einstellungen ........................................................................................................ A-10
                                         Scanner ............................................................................................................. A-10
                                         Erfassungsstellen in A+W Business .................................................................. A-12
                                         Mitarbeiterverwaltung in A+W Business ............................................................ A-13
                                         Interface Service ............................................................................................... A-13
                                         Kapazitätsplanung ............................................................................................ A-14
                                       Funktionen ............................................................................................................ A-15
                                         Anmeldung ........................................................................................................ A-15
                                         Hauptmenü ........................................................................................................ A-16
                                         Wareneingang ................................................................................................... A-17
                                         Produktionsmeldung .......................................................................................... A-18
                                           Fertigmeldung ................................................................................................ A-19
                                           Bruchmeldung ................................................................................................ A-20
                                         Lagerbewegungen ............................................................................................. A-21
                                           Lagerentnahme .............................................................................................. A-22
                                           Lagerzugang .................................................................................................. A-23
                                           Umbuchung .................................................................................................... A-24
                                           Kisten ............................................................................................................. A-26
                                         Gestelle ............................................................................................................. A-32
                                           Übersicht über Gestellmenü .......................................................................... A-32
                                           Gestelle beladen ............................................................................................ A-33
                                           Gestelle leeren ............................................................................................... A-35
                                           Gestelle anzeigen .......................................................................................... A-36
                                         Sonstiges ........................................................................................................... A-37
                                           Auftragsinformation ........................................................................................ A-37
                                           Anmeldeinformation ....................................................................................... A-38
                                           Mitarbeiterwechsel ......................................................................................... A-38
                                       Barcodes ............................................................................................................... A-39
                                         Ausdrucken von Barcodes ................................................................................ A-40
                                         Buchungshistorie ............................................................................................... A-41

                                       Partindex                                                                                                          A-43
                                       Index ..................................................................................................................... A-45
1.00 / 03-2023




                 A+W Business Barcode Manager (EL)                                                                                                              A-5
                 Inhalt
1.00 / 03-2023




                 A-6      A+W Business Barcode Manager (EL)
Barcode Manager (EL)         A

                       Einleitung




                  A+W Business
                 Einleitung                                                                             Einleitung




                                       Einleitung
                                       Die Online - Betriebsdatenerfassung mittels Barcode-Scanner erfolgt mittels
                                       eines Windows-CE basierten Scanner der Firma Datalogic (Scorpio). Das ei-
                                       gentliche Programm läuft dabei auf einem Terminal-Server, an den sich der
                                       Scanner via Remote-Desktop verbindet. Alle Lesungen die am Scanner vor-
                                       genommen werden, sendet der Scanner als Tastatureingabe in das jeweils ak-
                                       tive Datenfeld.
                                       Damit das Programm für die BDE nach der Anmeldung des Scanners am Ter-
                                       minal-Server automatisch startet, ist es erforderlich eine Verknüpfung zum
                                       BDE-Programm für den Benutzer in die Autostart-Gruppe zu kopieren. Das zu
                                       verknüpfende Programm hat den Namen abcscanner.exe und befindet sich im
                                       A+W Business Programme Ordner (z.B. C:\Program Files\A+W\ALFAK
                                       2011\Program\German). Bevor das Programm gestartet wird muss auf dem
                                       Rechner das A+W Business Startprogramm einmalig ausgeführt werden und
                                       es muss die richtige Datenbankverbindung im Login-Dialog eingegeben wer-
                                       den. Das BDE-Programm verbindet sich ab diesem Moment immer mit den
                                       gerade eingegebenen Informationen an die Datenbank.
                                       Das automatische Starten des Programmes kann ab A+W Business 5.5 Up-
                                       date 3 durch ein Konfigurationsprogramm (A+W Business 5 Scanner Auto-
                                       Start Config) im Startmenu ConfigTools eingestellt werden. In diesem
                                       Programm kann für den aktuelle angemeldeten Benutzer das Scannerpro-
                                       gramm (sprachabhängig) ausgewählt werden, das beim Anmelden dieses Be-
                                       nutzers gestartet werden soll.
1.00 / 03-2023




                 A+W Business Barcode Manager (EL)                                                           A-9
                 Einstellungen                                                                      Einleitung




                                 Einstellungen
                                 Scanner
                                 Die Konfiguration des Scanners kann auf einem beliebigen Arbeitsplatz durch-
                                 geführt werden. Zuerst wird die dem Scanner beiliegende Konfigurations-Soft-
                                 ware auf einem PC installiert und anschließend wird der Scanner per USB
                                 verbunden. Dann wird die Konfigurations-Software gestartet (Datalocic Confi-
                                 guration Utility). In dem Programm wird zunächst die Einstellung Postamble im
                                 Menü Hw Configuration > Laser > Parameters > Reader Parameters > Text
                                 Formatting vorgenommen. Hier wird einfach ein Tabulator eingegeben. Die
                                 Eingabe des Tabulators kann auf zwei Arten erfolgen. Entweder man gibt ein
                                 Tabulator in einem Editor (z.B. Notepad oder Word) ein und kopiert diesen
                                 über die Zwischenablage in das Datenfeld. Oder man drückt die Taste ALT,
                                 hält sie gedrückt währen man auf dem Nummernblock die Ziffern 0 0 9 nach-
                                 einander eingibt und die ALT Taste wieder los lässt.
                                 Dadurch wird am Ende einer jeden Lesung ein [TAB] an das BDE-Programm
                                 gesendet um eine vollständige Lesung des Barcodes zu signalisieren.




                                 Abb. A-1    Vollständigkeit der Barcode- Lesung


                                 Die zweite und letzte Einstellung lautet CheckEvaluation im Menü Hw Confi-
1.00 / 03-2023




                                 guration > Laser > Parameters > Reader Parameters > Code39 > Standard.
                                 Diese Einstellung muss auf Enabled gesetzt werden, damit die Prüfziffern des
                                 Code39 Barcodes überprüft und nicht als gültige Daten an das Programm ge-
                                 sendet werden.


                 A-10                                                   A+W Business Barcode Manager (EL)
                 Einleitung                                                                          Einstellungen




                                       Abb. A-2      Code 39 Einstellung


                                       Die zweite und letzte Einstellung lautet CheckEvaluation im Menü Hw Confi-
                                       guration > Laser > Parameters > Reader Parameters > Code39 > Standard.
                                       Diese Einstellung muss auf Enabled gesetzt werden, damit die Prüfziffern des
                                       Code39 Barcodes überprüft und nicht als gültige Daten an das Programm ge-
                                       sendet werden).
1.00 / 03-2023




                 A+W Business Barcode Manager (EL)                                                           A-11
                 Einstellungen                                                                            Einleitung




                                          Erfassungsstellen in A+W Business
                                          Fertigung > Erfassungsstellen Produktion




                 Abb. A-3    Erfassungsstellen Produktion


                                          In diesem Dialog hinterlegen Sie BDE-Typ der jeweilige Typ der Erfassungs-
                                          stelle. Diese werden für den Wareneingang und die Fertigmeldung benötigt.
                                          Ist beispielsweise eine eindeutige Zuordnung von Erfassungsstelle zu BDE-
                                          Typ gemacht (in der obigen Abbildung z.B. für den Wareneingang) so ist es
                                          nicht mehr nötig die Erfassungsstelle am Scanner einzulesen, wenn man den
                                          entsprechenden Programmpunkt wählt.
1.00 / 03-2023




                 A-12                                                         A+W Business Barcode Manager (EL)
                 Einleitung                                                                                     Einstellungen




                                       Mitarbeiterverwaltung in A+W Business




                                       Abb. A-4      Mitarbeiterverwaltung - Einstellung


                                       In der Mitarbeiterverwaltung ist es erforderlich für diejenigen Mitarbeiter die
                                       Personalnummer einzugeben, die sich per Mitarbeiter-Barcode an dem Scan-
                                       ner anmelden sollen.


                                       Interface Service
                                       Um Fertigmeldungen per Scanner zu buchen, werden die gelesenen Fertigmeldungen
                                       in der Datenbank gepuffert und anschließend vom AIS verarbeitet. Damit der AIS die
                                       gelesenen Buchungen zuordnen kann, ist es wichtig den Instanz-Namen des AIS als
                                       „sysadm“ zu definieren.
                                       Das ist auch der Default nach der Installation. Wenn bei einer Installation mehr als eine
                                       Instanz des AIS zum Einsatz kommt ist es wichtig diese Einstellung zu prüfen.
1.00 / 03-2023




                 A+W Business Barcode Manager (EL)                                                                        A-13
                 Einstellungen                                                                                 Einleitung




                                          Kapazitätsplanung
                                          Kapazitätsplanung > Stammdaten > Organisation > Aggregate




                 Abb. A-5    Aggregat-Zuordnung für Erfassungsstelle


                                          Soll die Verbuchung der Fertigmeldungen mit der A+W Business Kapazitäts-
                                          planung erfolgen, so ist es nötig für das jeweilige Aggregat eine eindeutige Er-
                                          fassungsstelle einzutragen. Das geschieht in der Aggregat-Verwaltung unter
                                          Kapazitätsplanung > Stammdaten > Organisation > Aggregate. Die jeweils zu
                                          verwendende Arbeitsart wird dabei immer über den Barcode eingelesen.
1.00 / 03-2023




                 A-14                                                            A+W Business Barcode Manager (EL)
                 Einleitung                                                                               Funktionen




                                       Funktionen
                                       Im Folgenden sind die einzelnen Dialoge der BDE aufgeführt und deren Funk-
                                       tionsweise erläutert:
                                        “Anmeldung” auf Seite A-15
                                        “Hauptmenü” auf Seite A-16
                                        “Wareneingang” auf Seite A-17
                                        “Produktionsmeldung” auf Seite A-18
                                        “Lagerbewegungen” auf Seite A-21
                                        “Gestelle” auf Seite A-32
                                        “Sonstiges” auf Seite A-37



                                       Anmeldung
                                       Scanner-Start




                                       Abb. A-6      BDE - Anmeldung über Personalbarcode39 Einstellung


                                       Nach erfolgreicher Anmeldung eines Anwenders gelangt man direkt in das
                                       Hauptmenü. Von hier aus gelangt man in den jeweiligen Dialog um Warenein-
                                       gänge, Lagerbuchungen, Gestell-Belegungen oder Fertigmeldungen durch-
                                       zuführen.
                                        “Hauptmenü” auf Seite A-16
1.00 / 03-2023




                 A+W Business Barcode Manager (EL)                                                             A-15
                 Funktionen                                                                    Einleitung




                              Hauptmenü
                              Scanner > Hauptmenü




                              Abb. A-7     BDE - Hauptmenü


                              Über die Hauptmenü des Scanners erreichen Sie folgende Funktionen:
                               “Wareneingang” auf Seite A-17
                               “Produktionsmeldung” auf Seite A-18
                               “Lagerbewegungen” auf Seite A-21
                               “Gestelle” auf Seite A-32
                               “Sonstiges” auf Seite A-37
                              Mit der Option [Back/ Zurück] kehren Sie zu vorherigem Dialog.
1.00 / 03-2023




                 A-16                                                 A+W Business Barcode Manager (EL)
                 Einleitung                                                                               Funktionen




                                       Wareneingang
                                       Scanner > Hauptmenü > Wareneingang




                                       Abb. A-8      BDE - Wareneingang


                                       Hier werden die Barcodes der Bestellpositionen eingelesen, für die ein Wa-
                                       reneingang verbucht werden soll:
                                       Nachdem der Barcode mit der Bestellposition gelesen wurde wird die Ein-
                                       gangsmenge per Tastatur eingegeben. Standardmäßig zeigt das Programm
                                       hier die komplette Menge der Bestellposition an und muss nur bei einer ab-
                                       weichenden Menge geändert werden. Sollte keine Änderung nötig sein, wird
                                       mit dem Barcode der nächsten Bestellposition fortgefahren. Das Programm
                                       sammelt diese Lesungen zunächst ohne eine tatsächliche Buchung durchzu-
                                       führen. Das passiert erst, wenn man auf dem Scanner die ENTER-Taste ge-
                                       tätigt, oder den Barcode einer anderen Bestellung einliest. Wird der ZURÜCK-
                                       Button oder die ESC-Taste betätigt und es sind noch nicht verbuchte Bestell-
                                       positionen im Speicher, so fragt das Programm nach, ob diese jetzt verbucht
                                       werden sollen.
                                       Wenn es sich bei der gerade eingelesenen Bestellposition um eine Kiste han-
                                       delt, so kann direkt danach ein Kisten-Identnummern-Barcode eingelesen
                                       werden und ggf. der Inhalt der Kiste geändert werden. Es wird dann automa-
                                       tisch nur eine Menge von 1 Stück eingetragen und diese ist auch nicht mehr
                                       änderbar. Für Kisten mit Identnummern kann ein abweichender Inhalt einge-
                                       geben werden.
                                       Nach jeder Lesung einer Bestellposition wird in dem unteren Mengen-Feld an-
                                       gezeigt wie viel Artikel bestellt wurden und wie viele bereits geliefert wurden
1.00 / 03-2023




                 A+W Business Barcode Manager (EL)                                                              A-17
                 Funktionen                                                                   Einleitung




                              Produktionsmeldung
                              Scanner > Hauptmenü > Produktionsmeldung




                              Abb. A-9     BDE - Produktionsmeldung


                              Die Fertig- und Bruchmeldungen befinden sich im Untermenü Produktions-
                              meldung, welches im Hauptmenü des Scanners die bisherige Fertigmeldung
                              ersetzt.
                               “Fertigmeldung” auf Seite A-19
                               “Bruchmeldung” auf Seite A-20
1.00 / 03-2023




                 A-18                                                 A+W Business Barcode Manager (EL)
                 Einleitung                                                                               Funktionen




                                       Fertigmeldung
                                       Scanner > Hauptmenü > Produktionsmeldung > Fertigmeldung Report




                                       Abb. A-10     BDE - Produktions-Rückmeldung


                                       Über den Dialog der Fertigmeldung lassen sich Statusänderungen an Auf-
                                       tragspositionen durchführen. Alle Lesungen die hier durchgeführt werden,
                                       werden zunächst in der Datenbank gespeichert und durch den AIS als STSD-
                                       Rückmeldung verarbeitet. Statusänderungen an den Aufträgen werden daher
                                       Zeit versetzt ausgeführt. Näheres zur Konfiguration des AIS für STSD-Rück-
                                       meldungen sind dem vorherigen Kapitel zu entnehmen.
                                       Nachdem eine Auftragsposition gelesen wurde, wird die Menge eingetragen,
                                       die fertig gemeldet werden soll. Das Programm blendet hier immer die kom-
                                       plette Positionsmenge vor. Zum Speichern der Fertigmeldung ist die ENTER-
                                       Taste zu drücken. Der Datensatz wird danach vom AIS verarbeitet und der
                                       Status des Auftrages ggf. angepasst. Soll pro Scannung nur ein Stück verar-
                                       beitet werden, kann die Option „Menge=1“ gewählt werden. Ist diese Option
                                       aktiviert, wird beim Scannen eines Barcodes sofort 1 Stück als fertig eingetra-
                                       gen. Eine zusätzliche Eingabeder Menge oder ein Bestätigen mit Enter ist da-
                                       mit nicht mehr nötig.
                                       Über den Dialog Bruchmeldung lassen sich ebenfalls Statusänderungen an
                                       Aufträgen durchführen, im Gegensatz zur Fertigmeldung allerdings nur nega-
                                       tive.
1.00 / 03-2023




                 A+W Business Barcode Manager (EL)                                                              A-19
                 Funktionen                                                                   Einleitung




                              Bruchmeldung
                              Scanner > Hauptmenü > Produktionsmeldung > Bruchmeldung - Report




                              Abb. A-11   BDE - Bruchmeldung


                              Bedienung und Verbuchung funktionieren analog zur Fertigmeldung, aller-
                              dings ist es möglich, Bruchgrund und –erfasser mit anzugeben. Diese können
                              entweder per Druck auf die Schaltfläche auf dem Scanner oder per Barcode
                              ausgewählt werden. Die Barcodes können in den Programmen Reklamations-
                              grund und –verursacher über das Formular Etiketten ausgedruckt werden.
                              Nach der Buchung eines Satzes werden die Informatonen zur letzten Bu-
                              chung zusammengefasst auf dem Scanner angezeigt.
1.00 / 03-2023




                 A-20                                             A+W Business Barcode Manager (EL)
                 Einleitung                                                                            Funktionen




                                       Lagerbewegungen
                                       Scanner > Hauptmenü > Lagerbewegung




                                       Abb. A-12     BDE - Menü Lagerbewegung


                                       Beim Start der Lagerbuchung wird zuerst gewählt, ob ein Zugang oder ein Ab-
                                       gang von Ware erfolgen soll. Zusätzlich ist das Menü für Kisten von hier er-
                                       reichbar.
                                        “Lagerentnahme” auf Seite A-22
                                        “Lagerzugang” auf Seite A-23
                                        “Umbuchung” auf Seite A-24
                                        “Kisten” auf Seite A-26
1.00 / 03-2023




                 A+W Business Barcode Manager (EL)                                                           A-21
                 Funktionen                                                                   Einleitung




                              Lagerentnahme
                              Scanner > Hauptmenü > Lagerbewegung > Entnahme




                              Abb. A-13   BDE - Lagerentnahme


                              Der darauf folgende Dialog funktioniert für den Zugang und Abgang größten
                              Teils identisch. Nachdem der Lagerortbarcode gelesen worden ist, kann der
                              Lagerartikelbarcode gelesen werden und die jeweilige Menge für die Zu-
                              gangs- bzw. Abgangsbuchung eingegeben werden. Durch Betätigung der
                              ENTER-Taste wird die Buchung direkt ausgeführt.
1.00 / 03-2023




                 A-22                                             A+W Business Barcode Manager (EL)
                 Einleitung                                                           Funktionen




                                       Lagerzugang
                                       Scanner > Hauptmenü > Lagerbewegung > Zugang




                                       Abb. A-14     BDE - Lagerzugang
1.00 / 03-2023




                 A+W Business Barcode Manager (EL)                                         A-23
                 Funktionen                                                                     Einleitung




                              Umbuchung
                              Scanner > Hauptmenü > Lagerbewegung > Umbuchung




                              Abb. A-15   BDE - Lagerort wählen


                              Es gibt nun unter dem Menüpunkt Lagerbewegung die Funktion Umbuchung.
                              Wählt man diesen muss man zunächst einmal einen Lagerort – Barcode scan-
                              nen.
                              Danach gelangt man in den Dialog zur Umbuchung von Lagerartikeln. Hier
                              muss der Anwender ein Lagerartikel scannen, also eine LagerID eines Lage-
                              rartikels, woraufhin der aktuelle Bestand angezeigt wird. Nun sollte man zu-
                              nächst die Menge, die umgebucht werden soll, definieren.
1.00 / 03-2023




                              Abb. A-16   BDE - Umbuchung Lagerartikel




                 A-24                                              A+W Business Barcode Manager (EL)
                 Einleitung                                                                       Funktionen




                                       Dann kann der Anwender einen neuen Lagerort vorgeben und die Buchung
                                       ausführen. Auf dem Schirm erscheint eine Erfolgsmeldung:




                                       Abb. A-17     BDE - erfolgreiche Umbuchung
1.00 / 03-2023




                 A+W Business Barcode Manager (EL)                                                     A-25
                 Funktionen                                                                   Einleitung




                              Kisten
                              Scanner > Hauptmenü > Lagerbewegung > Kisten




                              Abb. A-18    BDE - Kistenlager Menü


                              Ab der A+W Business Version 12.5 steht zusätzlich noch das Untermenü Ki-
                              sten zur Verfügung. Mit diesem Menü können die folgenden Funktionen auf-
                              gerufen werden:
                               “Kisteninhalt ändern” auf Seite A-27
                               “Auflösen von Kisten” auf Seite A-28
                               “Lagerort von Kisten ändern” auf Seite A-29
                               “Kiste auf Inventur setzen” auf Seite A-30
                               “Warenausgang Kiste” auf Seite A-31
1.00 / 03-2023




                 A-26                                                 A+W Business Barcode Manager (EL)
                 Einleitung                                                                               Funktionen




                                       Kisteninhalt ändern
                                       Scanner > Hauptmenü > Lagerbewegung > Kisten > Inhalt ändern




                                       Abb. A-19     BDE - Kisteninhalt ändern


                                       Mit dieser Funktion kann die Blattanzahl in einer Kiste reduziert werden. Dazu
                                       wird erst ein Kistenbarcode gescannt und danach die angezeigte Menge auf
                                       den neuen Wert gesetzt. Durch Bestätigen der Enter Taste wird die Buchung
                                       ausgelöst.
1.00 / 03-2023




                 A+W Business Barcode Manager (EL)                                                              A-27
                 Funktionen                                                                      Einleitung




                              Auflösen von Kisten
                              Scanner > Hauptmenü > Lagerbewegung > Kisten > Auflösen




                              Abb. A-20   BDE - Kistenlager Menü


                              Mit dieser Funktion kann eine Kiste aufgelöst werden (d.h. die Kiste wird ge-
                              löscht und die verbleibenden Scheiben werden auf das Lager gebucht). Hier-
                              zu wird erst eine Kiste gescannt und danach kann der Inhalt noch editiert
                              werden. Durch Bestätigen der Enter Taste wird die Buchung ausgelöst.
1.00 / 03-2023




                 A-28                                               A+W Business Barcode Manager (EL)
                 Einleitung                                                                              Funktionen




                                       Lagerort von Kisten ändern
                                       Scanner > Hauptmenü > Lagerbewegung > Kisten > Lagerort ändern




                                       Abb. A-21     BDE - Kistenlager Menü


                                       Mit dieser Funktion kann der Lagerort einer Kiste verändert werden. Dazu wird
                                       erst eine Kiste gescannt und danach der Barcode des neuen Lagerortes. Die
                                       Buchung wird dann sofort ausgelöst
1.00 / 03-2023




                 A+W Business Barcode Manager (EL)                                                             A-29
                 Funktionen                                                                        Einleitung




                              Kiste auf Inventur setzen
                              Scanner > Hauptmenü > Lagerbewegung > Kisten > Zu Inventur Liste




                              Abb. A-22    BDE - Kisten auf Inventur setzen


                              Mit dieser Funktion wird eine Kiste auf die aktuelle Inventurliste gesetzt. Nach
                              dem die Kiste gescannt wurde kann der neue Lagerort gescannt werden.
                              Nach dem beide Scannungen durchgeführt wurden, kann die aktuelle Menge
                              der Scheiben in der Kiste noch editiert werden. Durch Bestätigen der Enter Ta-
                              ste wird die Buchung ausgelöst.
1.00 / 03-2023




                 A-30                                                 A+W Business Barcode Manager (EL)
                 Einleitung                                                                            Funktionen




                                       Warenausgang Kiste
                                       Scanner > Hauptmenü > Lagerbewegung > Kisten > Warenausgang Kiste




                                       Abb. A-23     BDE - Kisten Warenausgang


                                       Mit dieser Funktion können Kisten mit Identnummer einer Auftragsposition zu-
                                       geordnet werden. Zunächst muss ein Auftragspositions-Barcode gescannt
                                       werden. Danach wird per Scannen des Kisten-Barcodes die Blattanzahl der
                                       Kiste ermittelt. Dieser kann dementsprechend editiert werden. Durch Bestäti-
                                       gen der Enter Taste wird die Buchung ausgelöst.
1.00 / 03-2023




                 A+W Business Barcode Manager (EL)                                                           A-31
                 Funktionen                                                                      Einleitung




                              Gestelle
                              Damit Gestelle verarbeitet werden können, müssen die folgenden Bedingun-
                              gen vorher geprüft werden:
                              •   Gestellnummern müssen eindeutig sein. Es darf also nicht ein Gestell mit
                                  der gleichen Nummer aber unterschiedlicher Gestellart angelegt werden.
                                  Wenn die gleiche Nummer verwendet wird, sollte der Gestellnummer ein
                                  Buchstabe (Für die Gestellart) vorangestellt werden.
                              •   Beim Verbuchen von Gestellen wird die Breite und Höhe des Gestells und
                                  das Beladungsgewicht geprüft. Diese Werte können pro Gestellart einge-
                                  stellt werden.
                              •   Die Verbuchung von Gestellen ist für den Versand entwickelt worden, d.h.
                                  es können nur Hauptpositionen einem Gestell hinzugefügt werden.
                              •   Es können nur Gestelle beladen werden, die nicht außer Haus gebucht
                                  sind, nicht als verloren gemeldet und nicht gesperrt sind.
                              •   Mit Punkt 5 ist sichergestellt, das beim Gestellausgang die Zuordnung des
                                  Gestells vollständig gebucht sein sollte


                              Übersicht über Gestellmenü
                              Scanner > Hauptmenü > Gestelle




                              Abb. A-24    BDE - Menü Gestelle


                              Im Untermenü Gestelle sind folgende Funktionen verfügbar:
                               “Gestelle beladen” auf Seite A-33
                               “Gestelle leeren” auf Seite A-35
                               “Gestelle anzeigen” auf Seite A-36
1.00 / 03-2023




                 A-32                                                 A+W Business Barcode Manager (EL)
                 Einleitung                                                                           Funktionen




                                       Gestelle beladen
                                       Scanner > Hauptmenü > Gestelle > Beladen




                                       Abb. A-25     BDE - Gestelle Beladen


                                       Zum Beladen von Gestellen muss zuerst das Gestell ausgewählt werden, das
                                       beladen werden soll. Ab dem Scannen des Gestellbarcode, können dann im
                                       darauf folgenden Dialog Auftragspositionen dem Gestell hinzugefügt werden.




                                       Abb. A-26     BDE - Gestelle Beladen - Auftragspositionen


                                       Nach der erfolgreichen Auswahl eines Gestells kann man Auftragspositionen
                                       dem Gestell hinzufügen. Hierbei werden zwei unterschiedliche Modi unter-
1.00 / 03-2023




                                       stützt, die mit den Knöpfen „Menge = 1“ und „Eingabe Menge“ ausgewählt
                                       werden können. Der aktuell eingestellte Modus ist grün markiert.



                 A+W Business Barcode Manager (EL)                                                         A-33
                 Funktionen                                                                     Einleitung




                              Für das Hinzufügen von Auftragspositionen muss der T2 Barcode verwendet
                              werden.
                              Im Modus „Eingabe Menge“ wird nach dem der Positionsbarcode gescannt
                              wurde, die noch nicht auf Gestellen abgestellte Menge im Mengenfeld des
                              Dialoges angezeigt. Diese kann dann editiert werden, wenn eine kleinere An-
                              zahl abgestellt werden soll. Durch ein Drücken der Enter Taste auf dem Scan-
                              ner wird die Buchung gestätigt.
                              Im Modus „Menge = 1“ wird die Verbuchung sofort nach dem Scannen des
                              Auftragspositionsbarcodes ausgeführt. Hierbei wird immer nur 1 Stück ver-
                              bucht.
                              Das Ergebnis der letzten Buchung wird immer im Fenster „Letzte Buchung“
                              angezeigt.
                              Um das Gestell zu wechseln, kann der Zurück Knopf getätigt werden und dann
                              ein anderes Gestell ausgewählt werden.
1.00 / 03-2023




                 A-34                                              A+W Business Barcode Manager (EL)
                 Einleitung                                                                            Funktionen




                                       Gestelle leeren
                                       Scanner > Hauptmenü > Gestelle > Leeren




                                       Abb. A-27     BDE - Gestelle Leeren


                                       Mit diesem Dialog kann ein Gestell als leer gemeldet werden. Dabei werden
                                       alle Zuordnungen der vorher auf dem Gestell abgestellten Auftragspositionen
                                       gelöscht.

                                          Keine Sicherungsabfrage
                                          Beim Leeren eines Gestells erfolgt keine Bestätigungsabfrage!
1.00 / 03-2023




                 A+W Business Barcode Manager (EL)                                                           A-35
                 Funktionen                                                                     Einleitung




                              Gestelle anzeigen
                              Scanner > Hauptmenü > Gestelle > Anzeigen




                              Abb. A-28   BDE - Gestelle anzeigen


                              Mit diesem Dialog kann die aktuelle Zuordnung von Auftragspositionen auf ei-
                              nem Gestell angezeigt werden. Wird ein Gestellbarcode gescannt, werden im
                              Belegungsfenster die Auftragspositionen mit der jeweils abgestellten Menge
                              angezeigt. Zusätzlich wird noch die Kundennummer mit ausgegeben. Die Li-
                              ste enthält jeweils sechs Einträge. Mit dem Vor und Zurück Knopf kann diese
                              geblättert werden.
1.00 / 03-2023




                 A-36                                               A+W Business Barcode Manager (EL)
                 Einleitung                                                                            Funktionen




                                       Sonstiges
                                       Scanner > Hauptmenü > Sonstiges
                                       Über den Menüpunkt Sonstiges erreicht man die Dialoge für die Auftragsposi-
                                       tionsinfo, die Anmeldeinfo und den Dialog zum Wechseln des Mitarbeiters:
                                        “Auftragsinformation” auf Seite A-37
                                        “Anmeldeinformation” auf Seite A-38
                                        “Mitarbeiterwechsel” auf Seite A-38


                                       Auftragsinformation
                                       Scanner > Hauptmenü > Sonstiges > Auftragsinformation




                                       Abb. A-29     BDE - Auftragsinformation


                                       Die Auftragspositionsinfo zeigt nach der Lesung eines Auftragspositions-Bar-
                                       codes die Bezeichnung der Position, deren Abmessung, die Stückzahl, die ge-
                                       lieferte Menge den Preis pro Preiseinheit und das Lieferdatum an.
1.00 / 03-2023




                 A+W Business Barcode Manager (EL)                                                           A-37
                 Funktionen                                                                     Einleitung




                              Anmeldeinformation
                              Scanner > Hauptmenü > Sonstiges > Anmeldeinformation




                              Abb. A-30   BDE - Sonstiges


                              Der Dialog für die Anmeldeinformationen zeigt den aktuell angemeldeten Be-
                              nutzer, die Datenbank, das Datenbanksystem (Microsoft SQL Server oder
                              Unify SQL Base), die Erfassungsstelle, das Aggregat und die Arbeitsart an.


                              Mitarbeiterwechsel
                              Scanner > Hauptmenü > Sonstiges > Mitarbeiterwechsel




                              Abb. A-31   BDE - Anmelden


                              Der Dialog zum Mitarbeiterwechsel ist in folgenden Abschnitt beschrieben:
                               “Anmeldung” auf Seite A-15
1.00 / 03-2023




                              Nach der Lesung eines gültigen Mitarbeiterbarcodes wird der aktuelle Mitar-
                              beiter abgemeldet und der neue Mitarbeiter angemeldet.



                 A-38                                              A+W Business Barcode Manager (EL)
                 Einleitung                                                                                          Barcodes




                                             Barcodes
                                             Für die einzelnen Dialoge und Funktionen sind bestimmte Barcodes erforder-
                                             lich. Bei den Barcodes handelt es sich um Code39 Barcodes mit Prüfziffer und
                                             einem Stern als Anfangs- und Ende-Zeichen.


                 Bezeichnung                                    Präfix   Nutzdaten                       Beispiel

                 Personalbarcode                                PE       Die Personalnummer aus der      *PE000000199F*
                                                                         Mitarbeiterverwaltung

                 Erfassungsstellenbarcode ohne Arbeitsart für   ES       Die ID der Erfassungsstelle     *ES00000000166*
                 Wareneingang

                 Erfassungsstellenbarcode mit Arbeitsart für    EA       :Die ID der Erfassungsstelle und *EA0000000015-101P*
                 Fertigmeldung                                           die ID der Arbeitsart getrennt mit
                                                                         Bindestrich

                 Auftragsbarcode für Fertigmeldung und          T2       Auftragsnummer +                *T200000243001001%*
                 Scheiben-Gestell-Zuordnung                              Positionsnummer (3stellig) +
                                                                         Teilenummer (3stellig)

                 Auftragsbarcode für Auftragsinfo               D2 oder Auftragsnummer +                *D200000243002Q*
                                                                T2      Positionsnummer (3stellig) +    oder
                                                                        Teilenummer (3stellig) (Nur T2) *T200000243002001Q*

                 Bestellbarcode für Wareneingang                D5       Bestellnummer +                 *D50000070650001.*
                                                                         Positionsnummer (3stellig)

                 Kistenbarcode für Lagerabgang und              BO       Identnummer einer Kiste.       *BOBC00002H*
                 Wareneingang                                            Achtung Identnummer darf keine
                                                                         führende Null enthalten!

                 Lagerortbarcode für Lagerbuchung               LA       Die ID des Lagerortes           *LA0000000001W*
                                                                                                         oder *L0000000001W*

                 Lagerartikel Barcode für Lagerbuchung          LP       Die LagerID des Lagerartikels   *LP0000000164E*

                 Gestellnummer                                  GE       Die Gestellnummer               *GE9099E*

                 Reklamationsgrund                              BR       Die Nummer des                  *BR1$*
                                                                         Reklamationsgrundes

                 Reklamationsverursacher                        BC       Die Nummer des                  *BC2P*
                                                                         Reklamationsverursachers
1.00 / 03-2023




                 A+W Business Barcode Manager (EL)                                                                        A-39
                 Barcodes                                                                       Einleitung




                            Ausdrucken von Barcodes
                            In den folgenden Programmen im A+W Business wurde eine Barcode-Druck-
                            funktionalität für die Online - Betriebsdatenerfassung (mittels Barcode-Scan-
                            ner) implementiert:
                            •   Mitarbeiterverwaltung (Stammdaten > Firma > Mitarbeiter)
                            •   Erfassungsstellen Produktion (z.B. Stammdaten > Fertigung > Sonstige >
                                Erfassungsstellen Produktion)
                            •   Vorgabezeiten (Kapazitätsplanung > Stammdaten > Vorgabezeiten > Vor-
                                gabezeiten)
                            •   Druckprogramm (z.B. Dokumente > Auftrag > Druck Auftrag)
                            •   Lagerdefinition (Stammdaten > Lager > Lagerdefinition)
                            •   Lagerverwaltung (Lagerwirtschaft > Lagerverwaltung)
                            •   Gestelle (Fertigung > Gestellverwaltung > Gestelle)
                            •   Reklamatuiongrund (Stammdaten > Produkte > Allgemein > Reklamati-
                                onsgrund)
                            •   Reklamationsverursacher (Stammdaten > Produkte > Allgemein > Rekla-
                                mationsverursacher)
                            Die Barcodes werden, wenn die Nutzdaten nicht die mögliche Datenlänge
                            überschreiten, mit Nullen (0) aufgefüllt (Ausnahme Gestellbarcodes). Des
                            Weiteren erhalten alle Barcodes eine abschließende Prüfziffer. In der Mitarbei-
                            terverwaltung (1) wurde zudem eine allgemeine Druckfunktionalität eingebaut.
                            Die Barcodes enthalten die Personalnummer (hier 199) des Mitarbeiters (Bei-
                            spiel: PE000000199F). Der Erfassungsstellenbarcode (2) wird aus der ID der
                            Erfassungsstelle gebildet (Beispiel: ES00000000166). In dem Programm Vor-
                            gabezeiten (3) hat der Anwender jetzt die Möglichkeit einen Erfassungsstel-
                            lenbarcode mit Arbeitsart für die Fertigmeldung in der Online - BDE zu
                            drucken. Dieser setzt sich aus der ID der Erfassungsstelle und der ID der Ar-
                            beitsart getrennt mit Bindestrich zusammen (Beispiel: EA0000000015-101P).
                            Das Druckprogramm für den Formulardruck (4) kann ab sofort auch einen Auf-
                            tragsbarcode (Auftragsinfo in Online - BDE) oder einen Bestellbarcode (Wa-
                            reneingang in Online - BDE) drucken. Dieser Barcode beinhaltet die
                            Dokumentennummer, die 3-stellige Positionsnummer und eine 3 stellige Tei-
                            lenummer (immer 000, da hier nur Hauptpositionen ausgegeben werden)
                            (Beispiel Auftrag: T200000243002000Q - Beispiel Bestellung:
                            D50000070650001.). Für die Lagerbuchung in der BDE muss entsprechend
                            der Lagerort gescannt werden. Hierfür wurde zum einen der Barcode-Druck in
                            dem Lagerdefinition-Dialog (5) überarbeitet und zum anderen die Online -
                            BDE erweitert. Die Online - BDE kann ab sofort solche Lagerortbarcodes mit
                            einem L-Präfix verarbeiten. Der Barcode beinhaltet die ID des Lagerortes
                            (Beispiel: *L0000000001W*). Abschließend sind für die Lagerbuchung Barco-
                            des der Lagerartikel (5) notwendig. In der Lagerverwaltung können nun die
                            entsprechenden Barcodes, die die ID des Lagerartikels enthalten, gedruckt
                            werden (Beispiel: LP0000000164E). Für Gestelle kann in der Gestellverwal-
                            tung (7) eine Liste von Gestellen selektiert werden und dann für diese der Bar-
                            code ausgedruckt werden (Funktionen > Gestellbarcodes drucken). Da
                            Gestelle alphanummerisch sind, werden diese nicht mit führenden Nullen auf-
1.00 / 03-2023




                            gefüllt.
                            Hinweis: Alle Barcodes werden in die Report-Variable F_IDENT_C39 des je-
                            weiligen Formulars/Reports geschrieben.


                 A-40                                              A+W Business Barcode Manager (EL)
                 Einleitung                                                                                   Barcodes




                                       Buchungshistorie
                                       Es ist jetzt möglich, sich die getätigten Fertig- und Bruchmeldungen protokol-
                                       lieren zu lassen. Um die Funktionalität zu aktivieren, muss in den Firmen-
                                       stammdaten auf Register 15.Kapazitätsplanung der Schalter ‚Historientabelle
                                       für Fertigmeldungen füllen' aktiviert werden.
                                       Wurde der Schalter aktiviert, werden die verarbeiteten Meldungen in der Ta-
                                       belle FS_BOOK_HISTORY protokolliert. Ist die Verbuchung in die A+W Busi-
                                       ness Kapazitätsplanung aktiv, so werden die Meldungen auch bei Verbuchung
                                       in selbige protokolliert. Das gilt auch für Meldungen, die per Dialog im A+W
                                       Business getätigt werden. Ansonsten werden die Buchungen in die PD_AW-
                                       BAR protokolliert.
                                       Dabei werden folgende Daten gespeichert
                                       •   Auftragsnummer
                                       •   Positionsnummer
                                       •   Stücklistenelement
                                       •   Zeitpunkt der Scannung
                                       •   Mitarbeiter
                                       •   Erfassungsstelle
                                       •   Arbeitsart (Nur bei Buchung in Kapazitätsplanung, ansonsten 0)
                                       •   Bruchgrund (Nur bei Bruchmeldungen)
                                       •   Bruchverursacher (Nur bei Bruchmeldungen)
                                       •   Verbuchte Menge
                                       •   Ursprung (BDE, manuell, implizit)


                                       Außerdem gibt es einen Dialog zur Auswertung der Buchungshistorie (Stati-
                                       stik > Buchugshistorie). Man kann dort per QBE Modus die anzuzeigenden
                                       Sätze filtern, so dass man hier genaue Statistiken z.B. pro Mitarbeiter erstellen
                                       kann.
1.00 / 03-2023




                 A+W Business Barcode Manager (EL)                                                                A-41
                 Barcodes                                                                     Einleitung




                            Abb. A-32   BDE - Anmelden


                            Beim Druck kann man sich die angezeigten Sätze dann noch zusätzlich nach
                            zwei dynamischen Kriterien gruppieren lassen, die ebenfalls im Dialog einge-
                            stellt werden.
1.00 / 03-2023




                 A-42                                            A+W Business Barcode Manager (EL)
Barcode Manager (EL)         A

                       Partindex




                  A+W Business
                 Partindex                                                                        Index




                 Index
                 A                                      – Inventurliste A-30
                 Aggregate                              – Kiste auflösen A-28
                 – Kapazitätsplanung   A-14             – Kisteninhalt ändern A-27
                 Anmeldung A-15                         – Kistenlagerort ändern A-29
                                                        – Kistenwarenausgang A-31
                                                        Kistenverwaltung A-26
                 B
                 BDE
                 – Anmeldeinformation A-38              L
                 – Anmeldung A-15                       Lagerbewegungen A-21
                 – Auftragsinformation A-37             – Kiste auf Inventurliste setzen   A-30
                 – Ausdrucken von Barcodes A-39, A-40   – Kiste auflösen A-28
                 – Barcodes A-39                        – Kistenbuchungen A-26
                 – Funktionen A-15                      – Kisteninhalt ändern A-27
                 – Gestelle A-32                        – Kistenort ändern A-29
                 – Gestellfunktionen A-33, A-35, A-36   – Kistenwarenausgang A-31
                 – Gestellmenü A-32                     – Lagerentnahme A-22
                 – Hauptmenü A-16                       – Lagerumbuchungen A-24
                 – Lagerbewegungen A-21                 – Lagerzugang A-23
                 – Mitarbeiterwechsel A-38              Lagerentnahme A-22
                 – Produktionsmeldung A-18              Lagerumbuchung A-24
                 – Sonstige Funktionen A-37             Lagerzugang A-23
                 Bruchmeldung A-20
                 Buchungshistorie A-41                  M
                                                        Menü A-16
                 E                                      Mitarbeiter
                 Einstellungen                          – A+W Business A-12, A-13
                 – Scanner A-10                         Mitarbeiterwechsel A-15
                 Erfassungsstellen
                 – A+W Business Stammdaten    A-12      P
                                                        Produktionsmeldung A-18
                 F                                      – Bruchmeldung A-20
                 Fertigmeldung A-19                     – Fertigmeldung A-19
                 Funktionen
                 – Überblick A-15                       S
                                                        Scanner
                 G                                      – Einstellungen A-10
                 Gestelle A-32                          – Hauptmenü A-16
                 – Anzeigen A-36                        – Wareneingang A-17
                 – Beladen A-33                         Sonstiges A-37
                 – Leeren A-35
                 – Menüübersicht A-32                   U
                                                        Ummelden     A-38
                 I
                 Interface Service   A-13               W
1.00 / 03-2023




                                                        Wareneingang     A-17
                 K
                 Kistenbuchungen


                 A+W Business Barcode Manager (EL)                                                A-45
                 Index                            Partindex
1.00 / 03-2023




                 A-46    A+W Business Barcode Manager (EL)

