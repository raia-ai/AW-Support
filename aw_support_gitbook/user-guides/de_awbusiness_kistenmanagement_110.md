---
title: "DE AWBusiness Kistenmanagement 1.10"
category: "user_manuals"
product: "Unknown"
doc_type: "Unknown"
language: "EN"
tags: ["DE_AWBusiness_Kistenmanagement_1.10"]
version: "1.0"
last_updated: "2025-12-10"
description: "Kistenmanagement            K                                 Deutsch                        A+W Business                                                                                                           Vorspann                                           Vorspann                                       In diesem Teil der Dokumentation finden Sie editorische Notizen.                                         Revisionsübersicht                                       Part            Beschreibu"
source_file: "DE_AWBusiness_Kistenmanagement_1.10.pdf"
---


# DE AWBusiness Kistenmanagement 1.10

Kistenmanagement            K




                            Deutsch




                   A+W Business
                                                                                                          Vorspann




                                      Vorspann
                                      In diesem Teil der Dokumentation finden Sie editorische Notizen.


                                      Revisionsübersicht
                                      Part            Beschreibung
                                      Version/Datum

                                      1.10/012-2019   Aktualisierung der Einstellungen in den Stammdaten. Übernahme
                                                      der Kistenbestellungen aus dem Part Einkauf und der
                                                      Lagerabbuchungen aus dem Part Fertigung.

                                      1.00/012-2018   Ersterstellung Kistenmanagement: Ausgliederung aus den Parts
                                                      Lager, Einkauf und Fertigung.



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
                                      © 2020, A+W Software GmbH, alle Rechte, auch des Nachdrucks, der Her-
                                      stellung von Kopien und der Übersetzung, bleiben vorbehalten.
                                      Die Dokumentation darf nur gemäß des Lizenzvertrages ganz oder in Teilen
                                      kopiert, in einem Archivierungssystem gespeichert oder in irgendeiner ande-
1.10 / 12-2019




                                      ren Form übertragen werden. Ohne die vorherige schriftliche Genehmigung
                                      von A+W Software GmbH darf die Dokumentation weder elektronisch, mecha-
                                      nisch, per Aufzeichnung oder in sonstiger Form übertragen werden.



                 A+W Business Kistenmanagement                                                                  K-3
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

                            aw.zentrale@a-w.com

                            http://www.a-w.com
1.10 / 12-2019




                 K-4                                                  A+W Business Kistenmanagement
                                                                                                                                                           Inhalt




                                      Inhalt
                                      Vorspann ................................................................................................................ K-3
                                       Revisionsübersicht .............................................................................................. K-3
                                       Editorial ............................................................................................................... K-3

                                      Tutorial                                                                                                             K-7
                                      Übersicht ................................................................................................................. K-9
                                        Dokumentation .................................................................................................. K-10
                                        Menü-Übersicht ................................................................................................. K-11
                                      Grundgedanken zum Lager .................................................................................. K-12
                                        Lagermaße ........................................................................................................ K-13
                                        Lagerverwaltung ................................................................................................ K-14
                                      Grundeinstellungen ............................................................................................... K-16
                                        Preise ................................................................................................................ K-16
                                        Firmendaten ...................................................................................................... K-18
                                        Statusänderungen durch Zu- und Abgänge ...................................................... K-21
                                        Lagerkategorien ................................................................................................ K-22
                                      Stammdaten für Kisten ......................................................................................... K-23
                                        Kistendaten ....................................................................................................... K-24
                                          Lagermaß für Kiste anlegen ........................................................................... K-25
                                          Lagerartikel für Kiste anlegen ........................................................................ K-26
                                        Kiste mit Stückliste ............................................................................................ K-29
                                          Stammdaten für Kisten mit Stückliste ............................................................ K-30
                                          Stücklisten-Kiste in der Lagerverwaltung ....................................................... K-35
                                          Stücklisten-Kiste in der Positionserfassung ................................................... K-36
                                      Aufträge ................................................................................................................ K-37
                                        Verkaufsauftrag mit Kiste .................................................................................. K-38
                                        Produktionsaufträge .......................................................................................... K-42
                                          Einstellungen in der Lieferantenkartei ............................................................ K-43
                                          Produktionsauftrag erfassen .......................................................................... K-45
                                      Lagerverwaltung für Kisten ................................................................................... K-49
                                        Lagerverwaltung von Kisten .............................................................................. K-49
                                        Lagerbestellung von Kisten ............................................................................... K-50
                                        Wareneingang per Barcode .............................................................................. K-55
                                        Warenausgang Kisten ....................................................................................... K-56
                                          Ausbuchung von Kisten ................................................................................. K-56
                                          Warenausgang buchen .................................................................................. K-59
                                        Manuelle Lagerbuchungen ................................................................................ K-61
                                          Zugang manuell erfassen .............................................................................. K-61
                                          Lagerort einer Kiste ändern ........................................................................... K-65
                                          Kisteninhalt korrigieren (Blattanzahl) ............................................................. K-66
                                          Kisten aufbrechen (auflösen) ......................................................................... K-67

                                      Softwarereferenz                                                                                                  K-69
                                      Übersicht ............................................................................................................... K-71
                                      Lagerverwaltung ................................................................................................... K-72
                                        Menüs in der Lagerverwaltung .......................................................................... K-72
                                          Menü Funktionen ........................................................................................... K-72
                                          Menü Optionen .............................................................................................. K-73
                                        Lagerverwaltung ................................................................................................ K-73
1.10 / 12-2019




                                          Lagerverwaltung – Lagerartikel ...................................................................... K-74
                                          Lagerverwaltung – Preise .............................................................................. K-78
                                          Lagerverwaltung – Zusatz .............................................................................. K-81




                 A+W Business Kistenmanagement                                                                                                                K-5
                 Inhalt




                          Lagerbewegung .................................................................................................... K-83
                            Menü Optionen .................................................................................................. K-83
                            Lagerbewegung ................................................................................................. K-83
                              Lagerbewegung – Abgang, Zugang ............................................................... K-84
                              Lagerbewegung – Umbuchung ...................................................................... K-86
                              Lagerbewegung – Blattanzahl ....................................................................... K-87
                              Lagerbewegung – Aufbruch ........................................................................... K-88
                            Bemerkung (Lagerbewegung) ........................................................................... K-89
                          Suche .................................................................................................................... K-90
                            Lagersuche – Lagersuche ................................................................................. K-91
                            Lagersuche – Zukünftiger Lagerbestand ........................................................... K-94
                          Lagerbestellung .................................................................................................... K-96
                            Menüs im Bestellpool ........................................................................................ K-96
                              Menü Funktionen ........................................................................................... K-96
                              Menü Optionen .............................................................................................. K-97
                            Bestellpool ......................................................................................................... K-99
                          Kisten – Ein- und Ausgang ................................................................................. K-102
                            Wareneingang (Kisten) .................................................................................... K-102
                              Wareneingang – Auswahl ............................................................................ K-103
                              Wareneingang – Komplett ........................................................................... K-105
                              Wareneingang – Positionsweise .................................................................. K-107
                              Wareneingang – Identnummer .................................................................... K-110
                              Wareneingang – Protokoll (Identnummern) ................................................. K-112
                            Einstellungen (ID) ............................................................................................ K-113
                            Warenausgang Kisten ..................................................................................... K-114

                          Partindex                                                                                                      K-115
                          Index ................................................................................................................... K-117
1.10 / 12-2019




                 K-6                                                                          A+W Business Kistenmanagement
Kistenmanagement              K

                          Tutorial




                   A+W Business
                 Tutorial                                                                                  Übersicht




                                      Übersicht
                                      Das Tutorial zum Kistenmanagement beschäftigt sich mit den Einstellungen
                                      zur Erfassung und Buchung von Kisten mit zugeschnittenen Gläsern.

                                          Funktionen sind von den freigeschalteten Modulen abhängig
                                          Bitte beachten Sie, dass die unterschiedlichen Funktionen nur dann zur
                                          Verfügung stehen, wenn die zugehörigen Module und Schnittstellen instal-
                                          liert und freigeschaltet sind.

                                          Wenn Sie in dieser Beschreibung Funktionen finden, die in Ihrer Installati-
                                          on nicht zugänglich sind, wenden Sie sich bitte an die A+W Software
                                          GmbH.

                                      Themenblöcke
                                      In diesem Tutorial finden Sie folgende Themenblöcke:
                                      •   Grundgedanken zum Lager
                                      •   Grundeinstellungen
                                      •   Stammdaten für Kisten
                                      •   Aufträge
                                      •   Lagerverwaltung für Kisten

                                      Vorausgesetzte Kenntnisse
                                      Das Tutorial richtet sich an Teilnehmer, die in A+W Business mit Kisten arbei-
                                      ten. Die Teilnehmer müssen das Konzept der Stammdaten und der Lagerver-
                                      waltung, den Verkauf und den Einkauf in A+W Business kennen.
1.10 / 12-2019




                 A+W Business Kistenmanagement                                                                  K-9
                 Übersicht                                                                               Tutorial




                             Dokumentation
                             Für das Kistenmanagement stehen folgende Dokumente zur Verfügung:

                             Format                   Umfang

                             PDF                      Vollständige Unterlagen
                                                      • Tutorial
                                                      • Softwarereferenz

                             Online-Hilfe <F1>        Kontextsensitive Dialog-Hilfe der A+W Business-
                                                      Softwarereferenz und Tutorials.


                             Ergänzende Beschreibungen finden Sie in den Parts Lager, Einkauf und Fer-
                             tigung, die jeweils auch über die Online-Hilfe zur Verfügung stehen.

                             Aufbau des Tutorials
                             Das Tutorial besteht aus Themenblöcken mit jeweils mehreren Lerneinheiten.
                             Jede Lerneinheit besteht aus folgenden Komponenten:

                             Überblick                Jede Lerneinheit beginnt mit einem Überblick über die
                                                      wichtigsten Inhalte:

                             Konzepte                 Konzepte und Begriffe der jeweiligen Lerneinheit
                                                      werden zunächst erläutert.

                             Handlungsanleitung       Die Handlungsanleitungen sind als Beispiele gedacht,
                                                      um den Ablauf zu zeigen. Die darin dargestellten
                                                      Bezeichnungen sind frei erfunden.


                             Darstellungskonventionen
                             Einzelne Satzteile werden in besonderer Form dargestellt. Diese haben fol-
                             gende Bedeutung:

                             Kursiv                   sind Zeichenfolgen ausgezeichnet, die Elemente der
                                                      Software bezeichnen, z. B. der Dialog Lagerinfo.

                             Fett                     sind Zeichenfolgen ausgezeichnet, die Sie über die
                                                      Tastatur eingeben, z. B.: Geben Sie den Wert 0 ein.

                             >                        Mit dem sogenannten Brotkrumenpfad ist der Weg
                                                      kennzeichnet, auf dem Sie einen Dialog öffnen, z. B.
                                                      Stammdaten > Produkt > Artikel > Lagermaße.

                             []                       Eckige Klammern bezeichnen Schaltflächen im Dialog,
                                                      z. B.: Mit [OK] speichern Sie die Daten.

                             <>                       Spitze Klammern bezeichnen Tasten oder
                                                      Tastenkombinationen auf der Tastatur, z. B.: Mit <F1>
                                                      öffnen Sie die Online-Hilfe.
1.10 / 12-2019




                 K-10                                                  A+W Business Kistenmanagement
                 Tutorial                                                                                   Übersicht




                                        Menü-Übersicht
                                        In diesem Abschnitt finden Sie eine kurze Übersicht über die Programm-
                                        bereiche, in denen Sie die Dialoge finden, die in dieser Dokumentation gezeigt
                                        werden.




                 Abb. K-1   Menü für Kistenmanagement


                                        Stammdaten
                                        •   Lagermaße:
                                            In diesem Dialog erfassen Sie die Kisten mit unterschiedlichen Preis-
                                            schlüsseln.

                                        Lagerwirtschaft
                                        •   Lagerverwaltung:
                                            In diesem Dialog erfassen und pflegen Sie die Daten für Lagerartikel.
                                        •   Lagerbewegung:
                                            In diesem Dialog buchen Sie Warenzugänge und Warenabgänge, Ände-
                                            rungen von Lagerorten und den Aufbruch von Kisten.
                                        •   Suche:
                                            In diesem Dialog prüfen Sie die Verfügbarkeit von Produkten in einem be-
                                            stimmten Zeitraum.

                                        Fertigung
                                        •   Warenausgang Kisten:
                                            In diesem Dialog erfassen Sie den Warenausgang von Kisten, die einem
                                            Auftrag zugeordnet sind.

                                        Dokumente
                                        •   Wareneingang:
                                            In diesem Dialog erfassen Sie die Kisten, die in den Bestand aufgenom-
                                            men werden sollen.
1.10 / 12-2019




                 A+W Business Kistenmanagement                                                                   K-11
                 Grundgedanken zum Lager                                                                           Tutorial




                                      Grundgedanken zum Lager
                                      Im Modul Lagerwirtschaft von A+W Business können Sie Bandmaße, Lager-
                                      maße, Restblätter, Kisten, Ganzglastüren, Beschläge, Rahmenteile und Zube-
                                      hör wie Spiegelaufhängungen, Dichtungsbänder usw. verwalten.
                                      Eine ausführliche Beschreibung zum Lager finden Sie im Part Lagerwirtschaft.
                                      Daraus werden die wichtigsten Stichpunkte für das Kistenmanagement hier
                                      nur kurz zusammengefasst.

                                      Lagerführung
                                      Bevor Sie Ihr Lager in A+W Business einrichten, müssen Sie entscheiden, auf
                                      welcher Basis die Bestände geführt werden sollen: als Fläche (qm) oder in
                                      Stückzahlen. Als dritte Möglichkeit steht die kombinierte Lagerführung zur Ver-
                                      fügung, wobei der maßabhängige Lagermodus mit den Rückmeldungen aus
                                      der Optimierung kombiniert wird, so dass neben den Lagermaßen auch die
                                      zugeschnittenen Bandmaße automatisch ausgebucht werden können.
                                      Nach der Entscheidung zum Modus ordnen Sie das entsprechende Lager-
                                      kennzeichen pro Glasprodukt zu und legen in den Firmendaten den Lagerfüh-
                                      rungsmodus fest.

                                      Lagerführungsmodus und Reservierung
                                      Wenn im (Produktions-)Auftrag ein Produkt mit der Beschaffungsart Lagerent-
                                      nahme erfasst wird, wird die entsprechende Menge (plus Verschnitt bei Fest-
                                      maßen) des Lagerartikels als reserviert gekennzeichnet. Die Reservierung
                                      kann wahlweise manuell aus dem aktuellen Bestand ausgebucht werden oder
                                      automatisch, wenn der Lieferschein oder die Rechnung gedruckt wird.
                                      Die Einstellungen werden in der Anzeige von Bestandsmengen im Dialog La-
                                      gerinfo (Lagervorschau) und bei den automatischen Bestellvorschlägen sicht-
                                      bar, die beim Erreichen von Mindestmengen angestoßen werden können.

                                      Verbrauch von Stücklisten in Produktionsaufträgen
                                      Bei Produktionsaufträgen kann der Verbrauch von Stücklistenelementen im
                                      Lager verbucht werden. Kisten haben dann eine Stückliste, wenn z. B. Bilder-
                                      rahmen-Gläser in Papier verpackt sind und diese Papierverpackungen auf ei-
                                      ner Palette stellen.

                                           Beispiel

                                           In einem Produktionsauftrag wird ein VSG mit 2 x Float 3 erfasst. Nach der
                                           Fertigmeldung des Produktionsauftrages wird das VSG auf das Lager
                                           gebucht, das Float 3 wird vom Lager abgebucht.

                                           Wenn für das gleiche VSG ein normaler Kundenauftrag erfasst wird, wird nur
                                           das VSG vom Lager abgebucht. Das Float 3 hat keine Lagerführung, da es
                                           bereits durch den Produktionsauftrag vom Lager gebucht worden ist.
1.10 / 12-2019




                 K-12                                                                A+W Business Kistenmanagement
                 Tutorial                                                                     Grundgedanken zum Lager




                                             Lieferantenkartei
                                             Wenn eine Kiste mit den identischen Maßen auch eingekauft wird, müssen Sie
                                             den Lieferanten in der Lieferantenkartei eintragen. Über die Warengruppe, die
                                             der Kiste in den Lagermaßen zugeordnet ist, wird der Lieferant gefunden.


                                             Lagermaße
                                             Das Lagermaß Kiste ist für Lagerbuchungen zwingend erforderlich. Für die Er-
                                             fassung einer Kiste als Auftrags- oder Bestellposition muss daher ein Lager-
                                             artikel/-maß Kiste angelegt sein.
                                             Wenn Sie ein Lagermaß in den Stammdaten angelegt haben, bietet A+W
                                             Business die Möglichkeit, sofort in die Lagerverwaltung zu wechseln.


                                                                                                 A


                                                                                                B

                                                                                                C
                                                                                                         D




                            F            E




                 A Produktverwaltung Lagermaße        C Lagermaße mit verschiedenen    E Zuordnung der Preistabellen
                   (Stammdaten)                         Abmessungen                    F Ermittlung des EK im Lager
                 B Produktnummer, zu der die          D Lagerartikel zu den Lagermaßen
                   Lagermaße gehören                    (Lagerverwaltung)
                 Abb. K-2       Lagermaße (Produktverwaltung) und zugehörige Lagerartikel
1.10 / 12-2019




                                             Jedem Lagermaß kann eine eigene Preistabelle zugeordnet werden.
                                             Wenn Sie mit dem Lagerkennzeichen maßabhängig arbeiten, müssen Sie für
                                             alle Lagermaße auch Lagerartikel angelegen.


                 A+W Business Kistenmanagement                                                                       K-13
                 Grundgedanken zum Lager                                                                           Tutorial




                                            Lagerverwaltung
                                            Zu jedem (Glas-)Produkt gehören auch ein Lagermaß und ein Lagerartikel.
                                            Jeder Lagerartikel kann in verschiedenen Ausprägungen angelegt werden,
                                            z. B. Float 5 mm in mehreren Abmessungen.


                                              J                    I




                 A

                                                                                                                       H
                 B

                 C


                 D

                 E
                                                                                                                       G




                                                      F

                 A   Produktnummer                                     F   Bestandsprüfung für Lagervorschau
                 B   Maße des Lagerartikels                            G   Definierte Lagerartikel
                 C   Standard-Lagerort                                 H   Hauptartikel
                 D   Lagerkategorie                                    I   Blattzahl bei Kisten
                 E   Kennzeichen Lager-Hauptartikel                    J   Lagerort (4 Ebenen)
                 Abb. K-3     Definition des Lagerartikels


                                            In den Lagermaßen (Stammdaten) kann für jedes Produkt eine Kiste mit der
                                            Beschaffungsart Lagerentnahme angelegt werden, z. B. pro Abmessung eine
                                            Kiste.
                                            Wenn es Kisten mit gleichen Maßen aber unterschiedlicher Blattanzahl (I) gibt,
                                            so muss auch dafür jeweils ein eigener Lagerartikel angelegt werden. Um den
                                            Kisten-Artikel exakt zu bestimmen, werden u. a. Breite und Höhe und die Blat-
                                            tanzahl ausgewertet, um den Mindestbestand zu bestimmen.
1.10 / 12-2019




                                            Für jede Ausprägung einer Kiste wird also ein Lagerartikel benötigt, in dem die
                                            Produktnummer, die Abmessung und die Blattanzahl hinterlegt sind.



                 K-14                                                                  A+W Business Kistenmanagement
                 Tutorial                                                             Grundgedanken zum Lager




                                      Sie können in der Lagerverwaltung mehrere Lagermaße miteinander verknüp-
                                      fen, indem Sie einen Lager-Hauptartikel (H) angeben. Die Bestandsprüfung im
                                      Dialog Lagerinfo wird dann nur für den Lager-Hauptartikel durchgeführt und
                                      nur für diesen müssen Sie einen Mindestbestand hinterlegen.
                                      Wenn die Bestände nicht pro Lagerort (F) geprüft werden, muss ein Hauptar-
                                      tikel (E, H) zugeordnet werden, um die verfügbaren Quadratmeter des Glases
                                      zu ermitteln.
1.10 / 12-2019




                 A+W Business Kistenmanagement                                                             K-15
                 Grundeinstellungen                                                                                   Tutorial




                                               Grundeinstellungen
                                               Neben den Produkten und den Lagerartikeln müssen weitere Einstellungen
                                               festgelegt werden, damit die Kisten korrekt verwaltet werden können.
                                               In diesem Kapitel finden Sie Informationen folgenden Grundeinstellungen:
                                               •   “Preise” auf Seite K-16
                                               •   “Firmendaten” auf Seite K-18
                                               •   “Statusänderungen durch Zu- und Abgänge” auf Seite K-21
                                               •   “Lagerkategorien” auf Seite K-22


                                               Preise
                                               Über die Preislisten für Kisten werden die Preise im Einkauf und im Verkauf
                                               berechnet, z. B. auch, wenn einzelne Blätter einer Kiste verkauft werden.
                                               Wenn Sie das Glas in Kisten mit anderen Preisen berechnen wollen, müssen
                                               Sie eine entsprechende Preisliste für den Verkauf und den Einkauf anlegen.
                                               Wenn Sie außerdem unterschiedliche Glaspreise je nach Stückzahl verwen-
                                               den wollen, sind dafür ebenfalls zusätzliche Preislisten erforderlich.
                                               Die Preise sind ausführlich im Part Stammdaten beschrieben.


                                  A                         B




                 A Preisschlüssel für Kisten                             B Preis pro Preisschlüssel
                 Abb. K-4     Beispiel Kistenpreise


                                               In diesem Beispiel sehen Sie, dass der Preis für die Gläser einer Kiste unter-
                                               schiedlich berechnet werden, z. B. für die komplette Kiste oder für ein einzel-
                                               nes Blatt aus der Kiste.
                                               Damit der Durchschnitts-EK ermittelt werden kann, müssen folgende Bedin-
                                               gungen erfüllt sein:
1.10 / 12-2019




                                               •   Das Produkt muss auch als Lagerartikel angelegt sein.
                                               •   Das Kennzeichen für den EK muss in den Firmendaten gesetzt sein.




                 K-16                                                                    A+W Business Kistenmanagement
                 Tutorial                                                                          Grundeinstellungen




                                         Preislisten prüfen

                                          So prüfen Sie die Stammdaten Ihrer Preislisten
                                         1 Wählen Sie im Menü Stammdaten > Preise und prüfen Sie die Einstellun-
                                           gen in den Dialogen Jahrgang, Schlüssel und Tarif.
                                             Sie brauchen nur die Einträge zu prüfen, die für Preise (und sonstige Ei-
                                             genkalkulationen) für Lagermaße und Kisten verwendet werden.
                                         2 Wählen Sie im Menü Stammdaten > Preise > Preise.




                    Abb. K-5   EK-Preistabellen


                                              Stammdaten, “Preise” auf Seite B-714
                                         3 Prüfen Sie, ob alle EK- und VK-Preise definiert und auf dem aktuellen
                                           Stand sind, und ergänzen oder korrigieren Sie diese ggf.
                                         4 Wechseln Sie zu dem Register, in dem der Preis definiert ist, und prüfen
                                           Sie, ob der EK-Preis korrekt eingetragen ist, oder korrigieren Sie diesen
                                           ggf.




                    Abb. K-6   Definierte Einkaufspreise


                                         5 Wählen Sie im Menü Start > Speichern, um die Änderungen zu speichern.
                                             Die Daten werden gespeichert.
1.10 / 12-2019




                 A+W Business Kistenmanagement                                                                    K-17
                 Grundeinstellungen                                                                           Tutorial




                                           Firmendaten
                                           In den Firmendaten werden die Einstellungen zum Wareneingang von Kisten
                                           und zum Lagerzugang durch Produktionsaufträge festgelegt. Diese Einstel-
                                           lungen sind im Part Lagerwirtschaft ausführlich beschrieben.

                                           Einstellungen für Kisten prüfen

                                            So prüfen Sie die Einstellungen für das Lager
                                           1 Wählen Sie im Menü Stammdaten > Firma > Firmendaten.
                                               Stammdaten, “Firmendaten” auf Seite B-918
                                           2 Wechseln Sie zum Register Parameter und prüfen Sie die Einstellungen
                                             für die virtuellen Positionsnummern.




                                                                                                             A




                 A Virtuelle Positionsnummern für den Wareneingang von Kisten
                 Abb. K-7     Firmendaten – Parameter


                                              Die virtuelle Positionsnummer wird benötigt, damit der Wareneingang von
                                              Kistenpositionen mit einer Stückzahl > 1 korrekt verbucht werden kann.
1.10 / 12-2019




                                           3 Wechseln Sie zum Register Lager / EK / EDI.




                 K-18                                                               A+W Business Kistenmanagement
                 Tutorial                                                                             Grundeinstellungen




                                               Den Lagerzugang aus einem Produktionsauftrag können Sie auf zwei Ar-
                                               ten erfassen:
                                               •   Sobald durch eine Produktionsrückmeldung der Status des Produkti-
                                                   onsauftrages über diesen Status hinaus steigt, wird der Lagerzugang
                                                   automatisch verbucht.
                                               •   Wenn Sie nicht mit Produktionsrückmeldungen arbeiten, können Sie
                                                   den Zugang über die manuelle Statusmeldung im Modul Fertigung er-
                                                   fassen. Wenn Sie den Produktionsauftrag dort auf einen Status setzen,
                                                   der über dem o. g. Grenzstatus liegt, werden der Lagerabgang der ver-
                                                   brauchten Materialien und der Lagerzugang der gefertigten Lagerartikel
                                                   automatisch gebucht.
                                               Wenn kein abweichender Lagerort definiert ist, werden die Auftragsmen-
                                               gen dem Standard-Lagerort zugeordnet.




                 A




                 B


                 C
                 D

                                                                                                                       F

                 E




                 A Einstellungen zur Ermittlung des Einkaufspreises    D Lagerbuchungen für Produktionsaufträge
                 B Einstellung zur Aktualisierung des Lagerbestands    E Anzahl der Vorschautage für den Dialog Lagerinfo
                 C Identnummern löschen                                F Grenzstatus für die Erfassungsstellen (für
                                                                         Produktionsaufträge)
                 Abb. K-8     Firmendaten – Lager / EK / EDI
1.10 / 12-2019




                                           4 Wählen Sie die Einstellungen für Lagerbestellungen (A) aus.




                 A+W Business Kistenmanagement                                                                       K-19
                 Grundeinstellungen                                                                          Tutorial




                                         Für die Kisten ist nur wichtig, wie der Einkaufspreis ermittelt werden soll.
                                         Die Einstellungen zur Ermittlung des Einkaufspreises sind im Part Stamm-
                                         daten beschrieben.
                                         Alle anderen Einstellungen in diesem Bereich sind ausführlich im Part La-
                                         gerwirtschaft beschrieben.
                                      5 Wählen Sie im Bereich Lagerführungsmodus (B) die Funktionen aus, die
                                        bei der Aktualisierung des Lagerbestands berücksichtigt werden sollen.
                                         •   Reservierung ohne Bestandsaktualisierung:
                                             Aktivieren Sie diese Option, wenn reservierte Mengen nicht aus dem
                                             aktuellen Bestand ausgebucht werden sollen. Die Abbuchungen müs-
                                             sen Sie dann zum gegebenen Zeitpunkt manuell durchführen. Bei der
                                             Auftragserfassung wird der aktuelle Bestand daher nicht angezeigt.
                                         •   Reservierung mit Bestandsaktualisierung:
                                             Diese Option ist standardmäßig aktiviert, damit reservierte Mengen mit
                                             dem Druck des Lieferscheins bzw. der Rechnung aus dem aktuellen
                                             Bestand ausgebucht werden.
                                         •   Lagerführung auf Stücklistenebene:
                                             Aktivieren Sie diese Checkbox, wenn Produkte im Lager auch dann ge-
                                             führt werden sollen, wenn sie Bestandteile einer Stückliste sind.
                                         •   Lagerabbuchung vor Formulardruck durchführen:
                                             Aktivieren Sie diese Checkbox, wenn Lagerartikel abgebucht werden
                                             sollen, bevor der Formulardruck ausgeführt wird. Falls bei der Lager-
                                             abbuchung ein Problem auftritt, wird der Auftrag aus den zu druckenden
                                             Dokumenten entfernt, also nicht gedruckt.
                                         •   Artikel mit Identnummer löschen wenn kein Bestand (C):
                                             Kisten mit dem Bestand = 0 sind nicht mehr im Lager vorhanden. Akti-
                                             vieren Sie diese Checkbox, wenn in der Lagerverwaltung die Kisten mit
                                             Identnummer aus der Übersicht gelöscht werden sollen, für die kein Be-
                                             stand angezeigt wird.
                                         •   Verbrauch von Stücklisten in Produktionsaufträgen (D):
                                             Wenn Sie mit Produktionsaufträgen arbeiten, können Sie festlegen, ob
                                             der Verbrauch von Stücklistenelementen automatisch im Lager abge-
                                             bucht wird.
                                      6 Tragen Sie die Anzahl der Werktage (E) ein.
                                         Die Anzahl der Werktage wird für die Vorschau im Dialog Lagerinfo ausge-
                                         wertet. Sie gibt an, über welchen Zeitraum in die Zukunft die zukünftigen
                                         Lagerbestände angezeigt werden.
                                      7 Wählen Sie im Menü Start > Speichern, um Änderungen zu speichern.
                                         Die Daten werden gespeichert. Nach Änderungen der Firmendaten sollten
                                         Sie A+W Business neu starten.

                                         Statuszuordnung für Lagerabbuchung
                                         Wenn Sie die Option Lagerabbuchung vor Formulardruck durchführen ak-
                                         tiviert haben, sollten Sie die Statuszuordnung für die Lagerabbuchung prü-
                                         fen. Die Mindest-, Vergabe- und Sperrstatus müssen so organisiert sein,
1.10 / 12-2019




                                         dass die Lagerabbuchung vor dem Druck ausgeführt werden kann. Wenn
                                         die Statuszuordnung die Umkehrung der Reihenfolge nicht zulässt, wird
                                         unter Umständen die Lagerabbuchung nicht durchgeführt.


                 K-20                                                           A+W Business Kistenmanagement
                 Tutorial                                                                     Grundeinstellungen




                                      Statusänderungen durch Zu- und Ab-
                                      gänge
                                      Warenab- und Warenzugänge können den Status von Dokumenten verändern
                                      und mit der Statusveränderung zu Bestandsänderungen im Lager führen.
                                      Wenn die Statuspunkte und Statuszuordnungen entsprechend definiert sind,
                                      gilt dies auch für Teillieferungen.
                                      Wenn Sie in den Firmendaten die Option Lagerabbuchung vor Formulardruck
                                      durchführen aktiviert haben, müssen der Mindest-, Vergabe- und Sperrstatus
                                      so organisiert sein, dass die Lagerabbuchung vor dem Druck ausgeführt wer-
                                      den kann. Wenn die Statuszuordnung die Umkehrung der Reihenfolge nicht
                                      zulässt, wird unter Umständen die Lagerabbuchung nicht durchgeführt.

                                      Statuszuordnungen prüfen
                                      Eine ausführliche Beschreibung finden Sie im Part Lagerwirtschaft.


                                       So prüfen Sie die Statusverwaltung
                                      1 Wählen Sie im Menü Stammdaten > Auftrag > Statusverwaltung.
                                          Stammdaten, “Statusverwaltung” auf Seite B-885
                                      2 Prüfen Sie, ob der Anwenderstatus für den Lagereingang und für den La-
                                        gerabgang vorhanden ist.
                                         Legen Sie diese ggf. an.
                                         Prüfen Sie als Nächstes die Statuszuordnungen.
                                      3 Wählen Sie im Menü Stammdaten > Auftrag > Statuszuordnung.
                                          Stammdaten, “Statuszuordnung” auf Seite B-887
                                      4 Prüfen Sie, ob die Statuszuordnungen von Lagereingang und Lagerab-
                                        gang für die Dokumententypen Auftrag und Bestellung festgelegt sind:
                                         •   Warenabgang Lager: Status Lieferschein gedruckt oder Rechnung ge-
                                             druckt
                                         •   Wareneingang Lager: Status Wareneingang gebucht
                                      5 Legen Sie die fehlenden Zuordnungen an und korrigieren Sie die vorhan-
                                        denen ggf.
1.10 / 12-2019




                 A+W Business Kistenmanagement                                                             K-21
                 Grundeinstellungen                                                                        Tutorial




                                      Lagerkategorien
                                      Lagerkategorien werden im Dialog Lagerverwaltung den Lagerartikeln zuge-
                                      ordnet. Dabei werden die Lagerartikel zu Gruppen (Lagerkategorien) zusam-
                                      mengefasst, die als Suchkriterium eingesetzt werden können.

                                      Lagerkategorie prüfen

                                       So legen Sie eine Lagerkategorie fest
                                      1 Wählen Sie im Menü Stammdaten > Lager > Kategorie.




                                         Abb. K-9     Lagerkategorien


                                          Stammdaten, “Lagerkategorien” auf Seite B-739
                                      2 Wählen Sie im Menü Start > Neu, um in den Erfassungs-Modus zu wech-
                                        seln.
                                      3 Geben Sie für die Lagerkategorie eine ID ein, z. B. Ziffern oder Bezeich-
                                        nungen wie Rohmaterial, Kisten, Produktion.
                                      4 Wählen Sie im Menü Start > Speichern, um die Daten zu speichern.
                                         Die Daten werden gespeichert.
1.10 / 12-2019




                 K-22                                                          A+W Business Kistenmanagement
                 Tutorial                                                                  Stammdaten für Kisten




                                      Stammdaten für Kisten
                                      In diesem Kapitel finden Sie Informationen dazu, wie Sie die Daten anlegen,
                                      um die Preisberechnung für Kisten differenzieren und Kisten im Lager verwal-
                                      ten zu können. Dazu gehören die Definition der Lagermaße und die Definition
                                      der Lagerartikel.
                                      In diesem Kapitel finden Sie Informationen zu folgenden Themen:
                                      •   “Kistendaten” auf Seite K-24
                                      •   “Kiste mit Stückliste” auf Seite K-29
1.10 / 12-2019




                 A+W Business Kistenmanagement                                                              K-23
                 Stammdaten für Kisten                                                                                  Tutorial




                                         Kistendaten
                                         Lernziele

                                         • Lagermaße und Lagerartikel für Kisten anlegen.
                                         • Produkt (Artikel) für Kiste anlegen.


                                         Nutzen

                                         • Wenn Sie die Produkte korrekt anlegen, können die Berechnungen und die
                                           Reservierung von Stück und Flächen durchgeführt werden.
                                         • Die jeweils aktuelle Anzeige des Bestands inklusive der Reservierungen erleichtert
                                           den Einkauf.


                                         Merke

                                         Produkte                    Die Produkte aus den Stammdaten dienen zur
                                                                     Erfassung und Preisfindung in Dokumenten. Sie werden
                                                                     nicht automatisch als Lagerbestand geführt, sondern nur
                                                                     aufgrund zusätzlicher Einstellungen und Definitionen.

                                         Lagerartikel                Alle Produkte, die im Lager mit Bestandsmengen geführt
                                                                     werden, müssen auch als Lagerartikel angelegt sein.

                                         Bandmaß                     Platte, wie sie vom Hersteller geliefert wird. Aus ihr
                                                                     werden die Gläser für den Verkauf zugeschnitten.

                                         Lagerplatte                 Tatsächlich im Lager befindliches Glas mit bestimmtem
                                                                     Maß, z. B. Float 4 mm in 1200 x 1800 mm oder
                                                                     3500 x 5100 mm. Lagerplatten mit definierten Maßen
                                                                     werden als auch Lagermaß bezeichnet.
                                                                     Lagerplatten können als Ganzes (1200 x 1800)
                                                                     verarbeitet werden. Aus ihnen können aber auch Gläser
                                                                     zugeschnitten werden, z. B. 600 x 900 aus der Platte
                                                                     1200 x 1800 oder aus der Platte 3210 x 5100.

                                         Lagermaß (Festmaß)          Die als Lagermaß festgelegten Gläser werden ohne
                                                                     Zuschnitt verkauft. Ihnen sind eigene Preistabellen
                                                                     (Lagermaßtabelle) zugeordnet. Ein maßabhängiger
                                                                     Lagerartikel ist immer auch ein Lagermaß.

                                         Lagerkennzeichen            Das Lagerkennzeichen legt fest, ob die Bestände eines
                                         (Lagerbuchungsart)          Lagerartikels als Fläche (qm) oder in Stückzahlen
                                                                     gewertet werden.

                                         Beschaffungsart             Das Kennzeichen legt fest, wie ein Produkt
                                                                     standardmäßig beschafft wird, z. B. durch Zuschnitt,
                                                                     Lagerentnahme, Produktion, Bestellung.

                                         Voreinstellungen            Keine
1.10 / 12-2019




                 K-24                                                                  A+W Business Kistenmanagement
                 Tutorial                                                                         Stammdaten für Kisten




                                           Lagermaß für Kiste anlegen
                                           Das Lagermaß Kiste ist für Lagerbuchungen zwingend erforderlich. Für die Er-
                                           fassung einer Kiste als Auftrags- oder Bestellposition muss daher ein Lager-
                                           artikel/-maß Kiste angelegt sein.


                                            So legen Sie Lagermaße in den Stammdaten an
                                           1 Wählen Sie im Menü Stammdaten > Produkt > Artikel > Lagermaße.
                                              Der Dialog Lagermaße wird geöffnet.
                                               Stammdaten, “Lagermaße” auf Seite B-637
                                           2 Wählen Sie im Menü Start > Neu und legen Sie das Lagermaß an.




                 A




                 B

                 C




                 D




                 A Maße der Scheiben und Inhalt der Kiste          C Preisermittlung im Lager
                 B Preistabellen für Verkauf und Einkauf           D Beschaffungsart
                 Abb. K-10    Lagermaß für Preisfindung anlegen


                                              Falls Sie in der Lagerverwaltung bereits einen entsprechenden Lagerarti-
                                              kel definiert haben sollten, tragen Sie die gleichen Werte für Breite und
                                              Höhe (A) ein.
                                           3 Geben Sie im Feld Inhalt an, wie viele Blätter in der Kiste enthalten sind.
1.10 / 12-2019




                                           4 Geben Sie die Preisschlüssel für den Verkauf und den Einkauf (B) an.
                                              Sie müssen je ein eigenes Lagermaß anlegen, wenn Sie unterschiedliche
                                              Preise berechnen, z. B. für den Verkauf der gesamten Kiste, für einzelne


                 A+W Business Kistenmanagement                                                                     K-25
                 Stammdaten für Kisten                                                                              Tutorial




                                             Blätter aus der Kiste und/oder für den Zuschnitt einzelner Blätter, die der
                                             Kiste entnommen werden.
                                         5 Markieren Sie die Checkbox EK Suche Lager (C), wenn das Lagermaß in
                                           die Preisermittlung einbezogen werden soll.
                                         6 Sie können zusätzlich eine Bezeichnung und Kurzbezeichnung (Match-
                                           code) eingeben, um z. B. den Lagerartikel besser identifizieren zu können.
                                         7 Geben Sie Beschaffungsart (D) an, z. B. bei Lagerartikeln Lagerentnahme.
                                         8 Wählen Sie im Menü Start > Speichern, um die Daten zu speichern.
                                             Die Daten werden gespeichert. Anschließend wird die Abfrage angezeigt,
                                             ob Sie dieses Lagermaß auch als Lagerartikel anlegen möchten.
                                         9 Wählen Sie [Ja], wenn das Lagermaß auch als Lagerartikel verwaltet wer-
                                           den soll.
                                             Der Dialog Lagerverwaltung wird geöffnet.


                                         Lagerartikel für Kiste anlegen
                                         Für einen Lagerartikel Kiste müssen Sie mindestens folgende Einstellungen
                                         festlegen, um ihn im Lager verwalten zu können:
                                         •   Artikelnummer und Bezeichnung
                                         •   Maße bei Lagermaßen, Maße und Inhalt
                                         •   Lagerort und Standard-Lagerort (Default-Lagerort)
                                         •   Bestände

                                             Inbetriebnahme des Lagers
                                             Wenn noch gar keine Lagerartikel angelegt sind, können Sie sich diese
                                             Aufgabe durch die sogenannte Erstinventur erleichtern. Dieser Ablauf ist
                                             im Part Lagerwirtschaft beschrieben.


                                          So legen Sie einen Lagerartikel an
                                         1 Wählen Sie im Menü Lagerwirtschaft > Lagerverwaltung.
                                             Der Dialog Lagerverwaltung wird geöffnet.
                                              Softwarereferenz, “Lagerverwaltung – Lagerartikel” auf Seite G-186
1.10 / 12-2019




                 K-26                                                                A+W Business Kistenmanagement
                 Tutorial                                                                           Stammdaten für Kisten




                                           2 Wählen Sie im Menü Start > Neu, um in den Erfassungs-Modus zu wech-
                                             seln.
                                               Wenn Sie den Dialog Lagerverwaltung aus den Stammdaten heraus geöff-
                                               net haben, entfällt dieser Schritt. Die Felder für Artikel und Maße sind dann
                                               bereits gefüllt.




                 A


                 B

                 C




                 D




                 E




                                                   F
                 A Nummer des Lagerartikels                           D Hauptartikel
                 B Maße und Inhalt der Kiste                          E Bestände
                 C Lagerort                                           F Bestandsprüfung
                 Abb. K-11   Felder für neuen Lagerartikel freigeschaltet


                                           3 Geben Sie die Nummer (A), die Maße und den Inhalt der Kiste (B) ein.
                                           4 Wählen Sie einen Lagerort aus (C).
                                               Wenn Sie keinen Lagerort auswählen, wird der Lagerort <k.A.> eingetra-
                                               gen. In der Lagerwirtschaft wird dieser wie die definierten Lagerorte behan-
                                               delt, z. B. bei der Inventur und bei Abfragen.
                                               Wenn Sie einen Lagerartikel an mehreren Lagerorten verwalten, müssen
                                               Sie einen dieser Lagerorte als Standard festlegen.
                                           5 Markieren Sie dazu die Checkbox Default-Lagerort.
                                           6 Wählen Sie im Feld Hauptartikel (D) den Artikel aus, für den Sie einen Min-
1.10 / 12-2019




                                             destbestand für die Bestandsprüfung hinterlegen wollen.
                                               Für Kisten ist das die Lagerplatte, aus der die Blätter geschnitten werden.



                 A+W Business Kistenmanagement                                                                        K-27
                 Stammdaten für Kisten                                                                              Tutorial




                                           7 Aktivieren Sie die Checkbox Bestandsprüfung pro Lagerort (F), wenn für
                                             den Lagerartikel alle Lagerorte bei der Bestandsprüfung getrennt bewertet
                                             werden sollen.
                                           8 Wechseln Sie zum Register Preise und geben Sie die Mengeneinheit an,
                                             mit der der Durchschnittspreis berechnet wird.




                 A



                                                            B
                 A Durchschnittspreis                                 B Mengeneinheit
                 Abb. K-12   Durchschnittspreis für Lagerartikel


                                           9 Wechseln Sie zum Register Zusatz und prüfen Sie, ob für die Kisten aus
                                             der Produktion der Lieferant 0 eingetragen ist.
                                               Mit dieser Einstellung geben Sie an, dass Sie selbst der Lieferant sind. Die-
                                               se Einstellung hat keine Auswirkungen auf die Kisten, die Sie alternativ
                                               auch bei einem Lieferanten bestellen können, denn solche Kisten werden
                                               nicht im Lager vorgehalten.
                                           10 Wählen Sie im Menü Start > Speichern, um die Daten zu speichern.
                                               Die Daten werden gespeichert.
                                           11 Wiederholen Sie die Schritte für alle Festmaße, die als Kisten erfasst wer-
                                              den können.
                                               Für Kisten legen Sie pro Glas, Abmessung, Inhalt und Preisschlüssel einen
1.10 / 12-2019




                                               Lagerartikel an.
                                               Damit sind alle Informationen hinterlegt, die A+W Business braucht, um
                                               Reservierungen und Buchungen durchzuführen.


                 K-28                                                                 A+W Business Kistenmanagement
                 Tutorial                                                                          Stammdaten für Kisten




                                      Kiste mit Stückliste
                                      Lernziele

                                      • Produktaufbau bei Kisten mit Stücklisten (Paletten) kennenlernen.


                                      Nutzen

                                      • Kisten mit einer tief gestaffelten Stückliste können als Produkt angelegt und erfasst
                                        werden.


                                      Merke

                                      Produktaufbau                Kisten mit Stückliste sind Artikel, die einen komplexeren
                                                                   Aufbau haben als einfache Glas-Kisten.

                                      Voreinstellungen             Lagerverwaltung
                                                                   Stammdaten:
                                                                   • Produktverwaltung
                                                                   • Lieferantenkartei
                                                                   Firmendaten:
                                                                   • Register Parameter
                                                                   • Register Lager / EK / EDI
1.10 / 12-2019




                 A+W Business Kistenmanagement                                                                         K-29
                 Stammdaten für Kisten                                                                           Tutorial




                                         Stammdaten für Kisten mit Stückliste
                                         Unter Kisten mit Stückliste sind Artikel zu verstehen, die einen komplexeren
                                         Aufbau haben als die bisher bekannten Glas-Kisten. Man kann beispielsweise
                                         Bilderrahmen-Gläser in Papier einpacken und diese Papierverpackungen auf
                                         eine Palette stellen.
                                         Dazu wird die Palette als Hauptprodukt und die Papierbox mit den Gläsern als
                                         dessen Stückliste angelegt. Sowohl die Palette als auch die Papierbox gehö-
                                         ren dabei zur Produktart Kiste.

                                            Vorkenntnisse für diese Einheit
                                            In dieser Einheit werden keine neuen Dialoge oder Funktionen erarbeitet.
                                            Die Sonderform von Kisten mit Stücklisten stellt einen speziellen Produkt-
                                            aufbau dar, der mit den bereits bekannten Mitteln eingerichtet wird.
                                            Informationen zu den Produktstücklisten finden Sie im Part Stammdaten.

                                         Stücklistenaufbau


                                                                                              A
                                                                                              B




                                         A Hauptprodukt: Palette                 B Stückliste: Box mit Gläsern
                                         Abb. K-13    Produktverwaltung – Stückliste mit komplexer Kiste


                                         In der Abbildung ist der Stücklistenaufbau für eine solche Palette dargestellt.
                                         Sie benötigen also ein Produkt für die Palette, ein Produkt für die Box und das
                                         Glas selbst.
1.10 / 12-2019




                 K-30                                                                A+W Business Kistenmanagement
                 Tutorial                                                                       Stammdaten für Kisten




                                      Produktart
                                      Damit die Palette und die Box von A+W Business als Kisten interpretiert wer-
                                      den, muss für beide die Produktart 200 - Kiste eingestellt sein.




                                      Abb. K-14    Produktverwaltung – Register Produkt


                                      Beschaffungsart und Lagerbuchungsart
                                      Damit beide Produkte im Lager geführt werden können, muss die Beschaf-
                                      fungsart auf Lagerentnahme und die Lagerbuchungsart maßabhängig einge-
                                      stellt sein.




                                      Abb. K-15    Produktverwaltung – Register Lager/Einkauf


                                         Palette mit Stückliste anlegen
                                         Wenn Sie die Palette mit der Stückliste anlegen, müssen Sie darauf ach-
                                         ten, dass die Beschaffungsart richtig übernommen wird.

                                      Standardmaße
                                      Die Erfassung des Produktes in der Positionserfassung wird etwas einfacher,
                                      wenn eine Standard-Breite und eine Standard-Höhe für das Produkt eingetra-
                                      gen sind. In der Positionserfassung wird dann nach der Eingabe der Produkt-
                                      nummer automatisch der passende Kistenartikel ausgewählt.




                                      Abb. K-16    Produktverwaltung – Register Produkt (optional)
1.10 / 12-2019




                 A+W Business Kistenmanagement                                                                  K-31
                 Stammdaten für Kisten                                                                            Tutorial




                                         Preiskennzeichen
                                         Im Gegensatz zu den bisher bekannten Kisten werden die Kennzeichen Preis-
                                         relevant VK / EK auf Ebene des Hauptproduktes und der Stückliste zur Preis-
                                         berechnung ausgewertet.
                                         Zuvor wurde der Preis der Kisten immer nur in dessen Stückliste berechnet
                                         und dargestellt. Über die Kennzeichen Preisrelevant ist das für Kisten mit
                                         Stücklisten konfigurierbar. Abhängig von diesen Kennzeichen wird der Preis
                                         im Verkauf also durch den Preis der Stücklisten-Komponente, der Hauptposi-
                                         tion oder durch beide bestimmt.
                                         Wenn in unserem Beispiel der Preis der Palette nur aus der Summe der Preise
                                         der Boxen, also aus der Stückliste, zusammensetzt werden soll, dann muss
                                         das Kennzeichen des Hauptartikels deaktiviert und das der ersten Stücklisten-
                                         Komponente, also der Box, aktiviert werden.

                                         Produkt                   Preisrelevant              Preisberechnung

                                         Palette                   Ja                         Preis pro Palette und
                                                                                              Anzahl der Boxen
                                         Box                       Ja

                                         Palette                   Ja                         Preis pro Palette
                                         Box                       nein

                                         Palette                   Nein                       Preis aus Anzahl der
                                                                                              Boxen
                                         Box                       Ja

                                         Tab. K-1    Preisberechnung bei Einstellung des Kennzeichens Preisrelevant
1.10 / 12-2019




                 K-32                                                              A+W Business Kistenmanagement
                 Tutorial                                                                              Stammdaten für Kisten




                                          Preisverwaltung
                                          In der Preisverwaltung können die Preise der Kisten wie gewohnt eingegeben
                                          werden.




                 Abb. K-17   Preisverwaltung – Register Matrix


                                          Sinnvoll ist z. B. eine Matrix mit den beiden Grenztypen Breite exakt und Höhe
                                          exakt. Damit können Stückpreise für verschiedene Abmessungen hinterlegt
                                          werden.

                                          Lagermaße (Produktverwaltung)
                                          Für jede Ausprägung der Palette und der Box muss im Dialog Lagermaße ein
                                          Lagermaß angelegt werden. Als Ausprägung gelten dabei die Maße der Glä-
                                          ser. Die Beschaffungsart muss auf Lagerentnahme gesetzt werden, damit das
                                          Lagermaß im Bestand geführt werden kann.

                                              Beispiel

                                              Das Lagermaß Palette mit Boxen soll aus jeweils 80 Boxen bestehen, die
                                              jeweils 25 Gläsern enthalten.
                                              Wichtig ist, dass für jede Abmessung nur jeweils ein Lagermaß mit einem
                                              eindeutigen Inhalt hinterlegt wird. D. h., dass für das Maß 600 x 700 nicht
                                              Paletten mit 50 und mit 80 Boxen angelegt werden dürfen.
1.10 / 12-2019




                 A+W Business Kistenmanagement                                                                              K-33
                 Stammdaten für Kisten                                                                       Tutorial




                 Abb. K-18   Produktverwaltung Lagermaße – Palette mit 80 Boxen und Box mit 25 Gläsern


                                          Für die Lagermaße kann (wie gewohnt) eine Umleitung auf andere Preis-
                                          schlüssel angegeben werden.
                                          Wenn das neue Lagermaß gespeichert wird, können Sie über die Abfrage di-
                                          rekt in die Lagerverwaltung wechseln, um die zugehörigen Lagerartikel anzu-
                                          legen.
1.10 / 12-2019




                 K-34                                                                A+W Business Kistenmanagement
                 Tutorial                                                                       Stammdaten für Kisten




                                          Stücklisten-Kiste in der Lagerverwaltung
                                          Die Lagerartikel werden analog zu den Produkt-Lagermaßen angelegt. Der
                                          Artikel wird mit der gleichen Abmessung und dem gleichen Inhalt angelegt. Er-
                                          gänzend werden der aktuelle Bestand und der Lagerort angegeben.
                                          Für die automatische Erzeugung von Lagerbestellungen müssen außerdem
                                          Werte in den Feldern Mindestbestand und Bestellmenge eingegeben sein.




                 Abb. K-19   Lagerverwaltung – Paletten mit 80 Boxen, Box mit 25 Gläsern
1.10 / 12-2019




                 A+W Business Kistenmanagement                                                                   K-35
                 Stammdaten für Kisten                                                                         Tutorial




                                           Stücklisten-Kiste in der Positionserfassung
                                           Wenn Sie die Palette in einer Position erfassen, geben Sie zunächst wie ge-
                                           wohnt die Produktnummer ein:
                                           •   Wenn in den Produktstammdaten eine Standard-Breite und Standard-
                                               Höhe eingegeben sind, wird die Kiste automatisch mit den Inhalten aus
                                               den Produkt-Lagermaßen erstellt.
                                           •   Wenn Sie das Produkt mit einer anderen Abmessung erfassen wollen oder
                                               wenn keine Standard-Abmessung angegeben ist, können Sie über die La-
                                               gersuche die gewünschte Palette auswählen.
                                           Im Register Stückliste sind die Komponenten mit den entsprechenden Inhal-
                                           ten vorbelegt.




                                                                                                               A




                                                                                                                    B




                 A Anzahl der Boxen auf der Palette                    B Anzahl der Gläser pro Box
                 Abb. K-20    Dokumentenverwaltung – Register Stückliste: Palette


                                           Die Kiste mit Stückliste kann wie jedes andere Produkt erfasst werden. Wenn
                                           sie als Lagerartikel geführt wird, kann sie auch dazu dienen, den Lagerbe-
                                           stand durch Produktionsaufträge aufzufüllen.
1.10 / 12-2019




                                           Ergänzende Informationen
                                            Verkauf, “Auftragskopf” auf Seite C-39
                                            Verkauf, “Bestellkennzeichen ändern” auf Seite C-310


                 K-36                                                                 A+W Business Kistenmanagement
                 Tutorial                                                                                  Aufträge




                                      Aufträge
                                      Aufträge für Kisten fallen in zweierlei Formen an:
                                      •   Verkaufsauftrag für einen Kunden.
                                          Wenn Sie außer den produzierten Kisten auch bestellte Kisten verkaufen,
                                          müssen die Einstellungen für den Lieferanten auch in der Lieferantenkartei
                                          festgelegt sein.
                                      •   Produktionsauftrag, um den Lagerbestand zu füllen.
                                      In diesem Kapitel finden Sie Informationen zu folgenden Themen:
                                      •   “Verkaufsauftrag mit Kiste” auf Seite K-38
                                      •   “Produktionsaufträge” auf Seite K-42
1.10 / 12-2019




                 A+W Business Kistenmanagement                                                                 K-37
                 Aufträge                                                                                       Tutorial




                                           Verkaufsauftrag mit Kiste
                                           In einen Verkaufsauftrag erfassen Sie eine Kiste für einen Kunden. Diese Kis-
                                           te kann aus Ihrem Lagerbestand entnommen werden oder bei einem Lieferan-
                                           ten bestellt werden.


                                            So erfassen Sie eine Kiste als Auftragsposition
                                           1 Wählen Sie Dokumente > Auftrag und erfassen Sie die Kopfdaten.




                                                                                                                     A




                                                                                                                     B




                 A Auftragsbereich                                  B Auftragstyp
                 Abb. K-21   Auftragskopf für Verkaufsauftrag


                                              Achten Sie auf die Einstellungen zum Auftragsbereich und zum Auf-
                                              tragstyp.
                                           2 Speichern Sie die Daten und wechseln Sie zum Register Positionen.
                                              Die Positionserfassung wird geöffnet.
                                           3 Wählen Sie im Menü Start > Neu, um eine neue Position zu erfassen.
1.10 / 12-2019




                 K-38                                                                 A+W Business Kistenmanagement
                 Tutorial                                                                                  Aufträge




                 Abb. K-22   Produktnummer für das Glas in der Kiste eingeben


                                          4 Geben Sie die Produktnummer des Glases ein, das Sie als komplette Kiste
                                            erfassen wollen.
                                          5 Wählen Sie im Menü Start > Lagersuche, um den Dialog Lagerinfo zu öff-
                                            nen.
1.10 / 12-2019




                 A+W Business Kistenmanagement                                                                K-39
                 Aufträge                                                                                     Tutorial




                 A




                 B




                 A Produktnummer des Glases                           B Kiste (ohne Bestand)
                 Abb. K-23   Lagerinformation zu Kisten


                                              Der Dialog Lagerinfo wird mit einer Liste aller Kisten und Lagermaße an-
                                              gezeigt, die für die Produktnummer vorhanden sind. Kisten mit dem Lager-
                                              ort <k.A>-<k.A>-<k.A> sind Kisten, die als Lagerartikel angelegt sind.
                                              Kisten mit Bestand haben in aller Regel eine ID.
                                          6 Übernehmen Sie die markierte Kiste mit einem Doppelklick.
                                              Achten Sie dabei auf die angegebenen Maße, wenn Sie mit unterschiedli-
                                              chen Kisten für ein Produkt arbeiten.
1.10 / 12-2019




                 K-40                                                              A+W Business Kistenmanagement
                 Tutorial                                                                                          Aufträge




                                               Der Dialog wird geschlossen und die Positionserfassung wird wieder ange-
                                               zeigt.




                 A




                 A Beschaffungsart

                 Abb. K-24   Position mit Kiste erfasst


                                           7 Wählen Sie die Beschaffungsart (A).
                                               •   Lagerentnahme:
                                                   Die Kiste wird aus dem Lagerbestand entnommen.
                                               •   Bestellung (komplett):
                                                   Die Kiste wird bei dem Lieferanten bestellt, der in der Lieferantenkartei
                                                   eingetragen ist.
                                                   Bei dieser Einstellung muss der Auftrag anschließend an den Einkauf
                                                   übergeben werden.
                                           8 Korrigieren Sie ggf. die Stückzahl, wenn Sie mehr als eine Kiste erfassen
                                             wollen.
                                           9 Wählen Sie im Menü Start > Speichern, um die Daten zu speichern.
                                               Die Daten werden gespeichert. Sie können jetzt weitere Positionen erfas-
                                               sen und den Auftrag auf die gewohnte Weise abschließen.
1.10 / 12-2019




                                               Wenn Sie den Wareneingang der Kistenlieferung durch einen Lieferanten
                                               buchen, wird die gelieferte Kiste dem Auftrag zugeordnet. Eine ausführli-
                                               che Beschreibung finden Sie im Part Einkauf.


                 A+W Business Kistenmanagement                                                                        K-41
                 Aufträge                                                                               Tutorial




                            Produktionsaufträge
                            Produktionsaufträge werden verwendet, um den eigenen Lagerbestand auf-
                            zufüllen. Alle Artikel, die in einem solchen Auftrag erfasst werden, werden au-
                            tomatisch auf die Beschaffungsart Produktion umgesetzt. Im Gegensatz zu
                            Kunden-Aufträgen werden die Positionen nicht im Lager reserviert, sondern
                            als bestellt markiert.

                            Manuelle und automatische Lagerbestellung


                                                                 Lagerbestellung
                                                                    Lagerort




                                                                  Mindestbestand
                                                                  unterschritten?



                                                                         ja




                                                                    Standard-
                                                                  Bestellmenge?



                                                                         ja




                                                                    Suche in der
                                                                 Lieferanten-Kartei




                                                 Standard-                             Interner
                                                 Lieferant?                             Kunde



                                                     ja                                   ja




                                              Bestellvorschlag                     Produktionsauftrag
                                              Lagerbestellung                    Dokumentenverwaltung



                            Abb. K-25    Lagerbestellung vs. Produktionsauftrag
1.10 / 12-2019




                            In diesem Ablaufplan ist dargestellt, wie A+W Business auf die unterschiedli-
                            chen Voreinstellungen in der Lieferantenkartei reagiert.




                 K-42                                                          A+W Business Kistenmanagement
                 Tutorial                                                                                      Aufträge




                                          Das Programm prüft, ob die aktuellen Lagerbestände zuzüglich der bereits be-
                                          stellten Mengen und abzüglich der reservierten Mengen den Mindestbestand
                                          unterschreiten. Wenn dies der Fall ist, wird als Vorschlag ein Vielfaches der
                                          (Standard-) Bestellmenge angezeigt.


                                          Einstellungen in der Lieferantenkartei
                                          Wenn im Dialog Lagerverwaltung ein Mindestbestand und eine (Standard-)
                                          Bestellmenge für den Lagerartikel hinterlegt sind, kann das System automati-
                                          sche Bestellvorschläge generieren. Diese werden im Dialog Lagerbestellung
                                          aufgelistet.
                                          Normalerweise werden auf diesem Weg Bestellungen vom Typ Lagerbestel-
                                          lung generiert. Wenn jedoch in der Lieferantenkartei statt eines Standard-Lie-
                                          feranten ein interner Kunde hinterlegt ist, können Produktionsaufträge
                                          automatisch erzeugt werden.




                 Abb. K-26   Interner Kunde für Produktionsaufträge


                                          In der Lieferantenkartei wird ein interner Kunde eingetragen, für den der Pro-
                                          duktionsauftrag automatisch erfasst wird. Die Option Interner Kunde kann auf
                                          der Ebene der Warengruppen oder der Produkte aktiviert werden. Dabei ha-
                                          ben die Einstellungen für Produkte Vorrang vor denen für Warengruppen.
1.10 / 12-2019




                 A+W Business Kistenmanagement                                                                    K-43
                 Aufträge                                                                             Tutorial




                            Bestellmenge
                            Der Multiplikator wird so berechnet, dass durch den Vorschlag der Mindestbe-
                            stand überschritten wird.




                            Abb. K-27     Mengenangaben für Lagerartikel (Dialog Lagerverwaltung)


                               Beispiel

                               Das VSG mit der Produktnummer 107 wird als Lagerartikel geführt.
                               Aktueller Lagerbestand: 10 Stk.
                               Mindestbestand: 30 Stk.
                               Bestellmenge: 5 Stk.
                               Die Bestellmenge für das VSG 107 wird folgendermaßen berechnet:
                               Differenz zwischen aktuellem Bestand und Mindestbestand: 20 Stk. In dieser
                               Differenz ist die Bestellmenge 5 Stk. viermal enthalten.
                               Bestellmenge: 4 x 5 = 20 Stk.
                               Aktueller Bestand plus bestellte Menge: 10 + 20 = 30 Stk.


                            Die errechnete Menge wird in den Bestellvorschlag übernommen. Sie kann im
                            Dialog Lagerbestellung angepasst werden. Wie Sie die Bestellungen bearbei-
                            ten und übergeben, ist im Part Einkauf beschrieben.
                            Der Produktionsauftrag wird erst durch die Übergabe erzeugt und in dem Auf-
                            tragsnummernverwalter angelegt, der zuletzt aktiviert war. Der Produktions-
                            auftrag kann bearbeitet und an die Produktion weitergeleitet werden.
1.10 / 12-2019




                 K-44                                                    A+W Business Kistenmanagement
                 Tutorial                                                                                 Aufträge




                                      Produktionsauftrag erfassen
                                      Wenn Sie Produktionsaufträge manuell erfassen, können Sie einen früher er-
                                      fassten Auftrag immer wieder durch Kopieren erneut erfassen und an die Pro-
                                      duktion übergeben.

                                          Etiketten für den Wareneingang
                                          Um eine selbst produzierte Kiste im Wareneingang per BDE zu erfassen,
                                          wird ein Etikett/Barcode benötigt. Dafür muss der Druckpunkt 973 zuge-
                                          ordnet werden.

                                      In diesem Kapitel finden Sie folgende Handlungssequenzen:
                                      •   “So erfassen Sie die Kopfdaten für einen Produktionsauftrag” auf
                                          Seite K-45
                                      •   “So erfassen Sie das Glas für die Kiste” auf Seite K-47
                                      •   “So erfassen Sie einen Produktionsauftrag durch Kopieren” auf Seite K-48


                                       So erfassen Sie die Kopfdaten für einen Produktionsauftrag
                                      1 Wählen Sie Dokumente > Auftrag > Auftrag.
                                          Der Dialog Dokumentenverwaltung wird geöffnet. In dieser Beschreibung
                                          ist dies der Modus Bearbeiten.
                                      2 Prüfen Sie im Menü Funktionen > Dokument > NV Auswahl, ob der richtige
                                        Nummernverwalter eingestellt ist, und korrigieren Sie ggf. die Einstellung.
                                          Sie können die Zuordnung des Auftrags zu einem Nummernverwalter auch
                                          im Auftragskopf sehen.
                                      3 Wählen Sie ggf. im Menü Start > Neu, um in den Erfassungs-Modus zu
                                        wechseln.
1.10 / 12-2019




                 A+W Business Kistenmanagement                                                               K-45
                 Aufträge                                                                                     Tutorial




                                                                                                                     A




                                                                                                                     B




                 A Auftragsbereich                                 B Produktionsauftrag
                 Abb. K-28   Kopfdaten für Produktionsauftrag


                                          4 Geben Sie die erforderlichen Kopfdaten ein.
                                          5 Tragen Sie ggf. in den Feldern unter dem Namen eine Erläuterung zum
                                            Auftrag ein, z. B. dass die Scheiben in Kisten verpackt werden sollen.
                                          6 Wählen Sie den Auftragstyp Produktionsauftrag (B).
                                          7 Prüfen Sie die weiteren Angaben.
                                          8 Wählen Sie im Menü Start > Speichern, um die Daten zu speichern.
                                              Die Kopfdaten werden gespeichert. Sie können jetzt zum Register Positio-
                                              nen wechseln und die Auftragspositionen erfassen.
                                              Wenn Sie Daten im Auftragskopf ändern, wird das Register Positionen wie-
                                              der gesperrt. Sie müssen die Änderungen speichern, um das Register Po-
                                              sitionen wieder freizuschalten.
1.10 / 12-2019




                 K-46                                                              A+W Business Kistenmanagement
                 Tutorial                                                                                    Aufträge




                                           So erfassen Sie das Glas für die Kiste
                                          1 Wählen Sie Dokumente > Auftrag > Auftrag auswählen > Register Positio-
                                            nen oder <F9>.
                                             Die Positionserfassung wird geöffnet.
                                          2 Wählen Sie im Menü Start > Neu, um eine neue Position zu erfassen.
                                          3 Geben Sie die Produktnummer des Glases ein, das als Kiste produziert
                                            werden soll.




                 Abb. K-29   Produktnummer für das Glas in der Kiste eingeben


                                          4 Setzen Sie die Stückzahl auf den Inhalt der Kiste oder ein Vielfaches des
                                            Inhalts.
                                          5 Wählen Sie im Menü Start > Speichern, um die Daten zu speichern.
                                             Die Daten werden gespeichert. Übergeben Sie den Produktionsauftrag an
                                             die Produktion.
                                             Wenn Sie regelmäßig Produktionsaufträge erfassen, können Sie den zuvor
                                             erfassten Auftrag kopieren und sich so die Arbeit erleichtern.
                                             Eine ausführliche Beschreibung finden Sie im Part Verkauf.
1.10 / 12-2019




                                             •   Vor dem Kopieren müssen Sie den Dokumententyp des Ziel-Doku-
                                                 ments auf Produktionsauftrag einstellen.



                 A+W Business Kistenmanagement                                                                  K-47
                 Aufträge                                                                                       Tutorial




                                               •   Wenn nur bestimmte Positionen aus dem Auftrag übernommen werden
                                                   sollen, können Sie diese auswählen.
                                               •   Im neuen Dokument können Sie die Daten anpassen.


                                            So erfassen Sie einen Produktionsauftrag durch Kopieren
                                           1 Wählen Sie Dokumente > Auftrag > Auftrag auswählen.
                                               Die Auftragserfassung wird geöffnet.
                                           2 Wählen Sie im Menü Funktionen > Dokumente kopieren.




                 A


                                                                                                                      B




                 A Kopieren von Auftrag nach Auftrag                        B Dokumententyp des Ziel-Auftrags
                 Abb. K-30    Produktionsauftrag durch Kopieren erstellen


                                           3 Wechseln Sie zum Register Kopieren positionsweise und markieren Sie
                                             die Position(en), die kopiert werden sollen.
                                           4 Korrigieren Sie ggf. die Zielmenge.
                                           5 Wählen Sie im Menü Start > Ausführen, um die Kopie zu erzeugen.
1.10 / 12-2019




                 K-48                                                                 A+W Business Kistenmanagement
                 Tutorial                                                                Lagerverwaltung für Kisten




                                      Lagerverwaltung für Kisten
                                      Für Lagerartikel werden sowohl der Wareneingang als auch der Warenab-
                                      gang erfasst, damit Sie die Bestände verwalten können.
                                      Der Warenein- und Warenabgang von Kisten kann über Barcodes (BDE) oder
                                      manuell erfasst werden.
                                      In diesem Kapitel finden Sie Informationen zu folgenden Themen:
                                      •   “Lagerverwaltung von Kisten” auf Seite K-49
                                      •   “Lagerbestellung von Kisten” auf Seite K-50
                                      •   “Wareneingang per Barcode” auf Seite K-55
                                      •   “Manuelle Lagerbuchungen” auf Seite K-61
                                      •   “Warenausgang Kisten” auf Seite K-56

                                      Scannen
                                      In Verbindung mit AWPort können Lagerbuchungen auch über Barcodes er-
                                      fasst werden. Dazu gehören nicht nur die Wareneingänge und Warenausgän-
                                      ge, sondern auch die Auflösung einer Kiste und andere Umbuchungen.
                                      Durch Scannen können ganze Kisten einem bestimmten Auftrag oder einer
                                      Auftragsposition zugeordnet werden oder mit der entsprechenden Blattanzahl
                                      für die Inventur erfasst werden.
                                       “Wareneingang per Barcode” auf Seite K-55
                                      Weitere Informationen zum Barcode und den Formaten entnehmen Sie bitte
                                      der Dokumentation zu AWPort.


                                      Lagerverwaltung von Kisten
                                      Gelieferte Kisten haben in aller Regel eine ID vom Lieferanten, mit der sie im
                                      Wareneingang erfasst werden.
                                      Jede Kiste wird mit einer eigenen Kisten-ID im verbucht und im Lager geführt.
                                      Dazu muss in den Firmendaten die Checkbox für die virtuellen Identnummern
                                      aktiviert sein.
                                       “Firmendaten” auf Seite K-18
                                       “Wareneingang per Barcode” auf Seite K-55

                                      Kisten aufbrechen
                                      Um einzelne Blätter aus einer Kiste zu erfassen, muss die Kiste aufgelöst wer-
                                      den. Dabei wird eine Kiste (mit ID) zunächst aus dem Lagerbestand entfernt.
                                      Die Anzahl der Blätter wird dann dem Lagerbestand des entsprechenden La-
                                      gerartikels (Lagermaß) zugebucht.
1.10 / 12-2019




                 A+W Business Kistenmanagement                                                                 K-49
                 Lagerverwaltung für Kisten                                                                   Tutorial




                                         Lagerbestellung von Kisten
                                         Der Bestand von Kisten kann entweder durch einen automatisch oder einen
                                         manuell erzeugten Produktionsauftrag aufgefüllt werden.
                                         Lagerbestellungen können auch manuell über die Dokumentenverwaltung er-
                                         zeugt werden.
                                          “So erfassen Sie eine Lagerbestellung mit Kisten” auf Seite K-52

                                         Bestellvorschläge
                                         In der Regel werden Bestellungen aus der Lagerwirtschaft heraus erzeugt, um
                                         die Bestände auf dem gewünschten Niveau zu halten.




                 A
                 B




                 A Mindestbestand                                   B Menge für Bestellvorschlag
                 Abb. K-31   Lagerverwaltung – Bestandszahlen


                                         Wenn Sie im Dialog Lagerverwaltung Mindestmengen (A) für einen Lagerarti-
                                         kel hinterlegt haben, werden Bestellvorschläge automatisch mit der hinterleg-
                                         ten Bestellmenge (B) erzeugt. Sie können diese vor der Übergabe an den
                                         Einkauf prüfen und ggf. den Lieferanten und den Termin ändern. Mit der Über-
                                         gabe an den Einkauf wird aus dem Vorschlag eine Lagerbestellung erzeugt.
1.10 / 12-2019




                 K-50                                                                A+W Business Kistenmanagement
                 Tutorial                                                                 Lagerverwaltung für Kisten




                                      Lagerzugang durch Produktionsauftrag
                                      In den Firmendaten müssen Sie ist im Register Lager / EK / EDI den Grenz-
                                      status für die Erfassungsstellen einstellen, ab dem ein Auftrag als produziert
                                      gilt. Als Grenzstatus gilt der für die gewählte Erfassungsstelle hinterlegte Sta-
                                      tus.




                                      Abb. K-32    Firmendaten – Lager / EK / EDI: Erfassungsstelle für Statusumsetzung


                                      Den Lagerzugang aus einem Produktionsauftrag können Sie auf zwei Arten
                                      erfassen:
                                      •  Sobald durch eine Produktionsrückmeldung der Status des Produktions-
                                         auftrages über diesen Status hinaus steigt, wird der Lagerzugang automa-
                                         tisch verbucht.
                                      • Wenn Sie nicht mit Produktionsrückmeldungen arbeiten, können Sie den
                                         Zugang über die manuelle Statusmeldung im Modul Fertigung erfassen.
                                         Wenn Sie den Produktionsauftrag dort auf einen Status setzen, der über
                                         dem o. g. Grenzstatus liegt, werden der Lagerabgang der verbrauchten
                                         Materialien und der Lagerzugang der gefertigten Lagerartikel automatisch
                                         gebucht.
                                      Wenn kein abweichender Lagerort definiert wurde, werden die Auftragsmen-
                                      gen dem Standard-Lagerort zugeordnet.
                                      Die Verbuchung von Produktionsaufträgen wird im Part Fertigung ausführlich
                                      behandelt.


                                      Ergänzende Informationen
                                       Stammdaten, “Firmendaten – Lager/EK/EDI” auf Seite B-957
                                       Verkauf, “Auftragskopf” auf Seite C-39
                                       Verkauf, “Bestellkennzeichen ändern” auf Seite C-310
                                       Fertigung, “Produktionsaufträge” auf Seite E-130
1.10 / 12-2019




                 A+W Business Kistenmanagement                                                                   K-51
                 Lagerverwaltung für Kisten                                                                    Tutorial




                                         Manuelle Lagerbestellung von Kisten erfassen
                                         In der nachfolgenden Handlungsanleitung wird eine Lagerbestellung für Kis-
                                         ten erfasst.
                                         Manuelle Bestellungen sind ausführlich im Part Einkauf beschrieben.
                                          Einkauf, “Manuelle Bestellung” auf Seite D-79


                                          So erfassen Sie eine Lagerbestellung mit Kisten
                                         1 Wählen Sie Dokumente > Bestellung > Bestellung.
                                              Der Dialog Dokumentenverwaltung wird geöffnet.
                                         2 Wählen Sie im Feld Typ den Eintrag Lagerbestellung.




                                              Wenn Sie den Typ auf <k.A.> einstellen, können Sie den Wareneingang
                                              nicht automatisch auf das Lager buchen.
                                         3 Wechseln Sie zum Register Positionen.
                                         4 Geben Sie die Produktnummer ein.
                                              Die Anzahl können Sie nach der Auswahl des Lagerartikels angeben.
                                              Maße brauchen Sie nicht einzutragen, diese werden aus dem Lagerartikel
                                              übernommen.
                                         5 Wählen Sie im Menü Start > Lagersuche, um den Dialog Lagerinfo zu öff-
                                           nen.
                                              Sie können den Dialog auch über die Taste <F3> öffnen.
1.10 / 12-2019




                 K-52                                                               A+W Business Kistenmanagement
                 Tutorial                                                                   Lagerverwaltung für Kisten




                    A




                    B




                    A Produktnummer der Glasart                         B Kiste (ohne ID)
                    Abb. K-33   Lagerinfo – Lagersuche

                                              Verkauf, “Lagerinfo” auf Seite C-741
                                             Der Dialog Lagerinfo wird mit einer Liste aller Lagermaße und Kisten an-
                                             gezeigt. Für Kisten ist in der Spalte Inh. der Wert größer als 1.
                                         6 Suchen Sie die gewünschte Kiste ohne Kisten-ID aus und übernehmen Sie
                                           sie mit einem Doppelklick.
                                             Der Dialog wird geschlossen und die Positionserfassung wird wieder ange-
                                             zeigt. In der Erfassungszeile werden für Kisten alle Felder ab Menge ge-
                                             sperrt. Die Preisfelder werden aktualisiert.
1.10 / 12-2019




                 A+W Business Kistenmanagement                                                                  K-53
                 Lagerverwaltung für Kisten                                                                       Tutorial




                                        A                 B
                    A Stückzahl                                              B Menge
                    Abb. K-34     Kiste in der Positionserfassung


                                            7 Geben Sie die gewünschte Stückzahl ein.
                                                Die Anzeige der Details wird aktualisiert.
                                            8 Wiederholen Sie die Schritte 4 bis 7, um alle Bestellpositionen zu erfassen.
                                            9 Wählen Sie im Menü Start > Speichern, um die Daten zu speichern.
                                                Die Daten werden gespeichert.
                                            10 Drucken und versenden Sie die Bestellung.
1.10 / 12-2019




                 K-54                                                                  A+W Business Kistenmanagement
                 Tutorial                                                                 Lagerverwaltung für Kisten




                                          Wareneingang per Barcode
                                          In der Regel werden alle Lagerbuchungen per BDE (Betriebsdatenerfassung)
                                          erfasst. Dazu müssen die Kisten mit jeweils einem eigenen Barcode-Etikett
                                          versehen sein.

                                             Etiketten für den Wareneingang
                                             Um eine selbst produzierte Kiste im Wareneingang per BDE zu erfassen,
                                             wird ein Etikett/Barcode benötigt. Dafür muss der Druckpunkt 973 zuge-
                                             ordnet werden.


                                           So erfassen Sie eine Kiste per Barcode
                                          1 Wählen Sie im Modul Dokumente > Bestellung > Wareneingang > Waren-
                                            eingang.
                                          2 Wählen Sie die Option Scanner und scannen Sie das Etikett der Kiste.
                                          3 Wählen Sie im Menü Start > Ausführen.
                                             Wenn Sie einen Barcode für die Eingangsbuchung haben, können Sie die-
                                             sen scannen. Damit ist die Kiste in den Warenbestand am Default-Lagerort
                                             aufgenommen.
                                             Sie können nacheinander alle produzierten Kisten scannen und anschlie-
                                             ßend buchen.
                                          4 Wechseln Sie zum Register Positionsweise und markieren Sie die Check-
                                            box Komplett buchen der Kiste.
1.10 / 12-2019




                 Abb. K-35   Positionsweise buchen




                 A+W Business Kistenmanagement                                                                 K-55
                 Lagerverwaltung für Kisten                                                                           Tutorial




                                          5 Wählen Sie im Menü Start > Ausführen.
                                              Damit ist die Kiste gebucht und im Lagerbestand vorhanden.




                 Abb. K-36   Lagersuche – Kiste mit ID im Bestand



                                          Warenausgang Kisten
                                          In der Regel werden Kisten mit dem Druck des Lieferscheins aus dem Lager-
                                          bestand ausgebucht. Statt des Lieferscheindrucks kann aber auch der Rech-
                                          nungsdruck die Buchung auslösen.


                                          Ausbuchung von Kisten
                                          In der Regel werden Kisten mit dem Druck des Lieferscheins aus dem Lager-
                                          bestand ausgebucht. Statt des Lieferscheindrucks kann aber auch der Rech-
                                          nungsdruck die Buchung auslösen.
                                          Da der Erfasser eines Auftrags nicht weiß, welche Kiste tatsächlich ausgelie-
                                          fert wird, erfasst er zunächst die Dummy-Kiste mit den gewünschten Maßen.
                                          Der Lagerbestand kann jedoch erst aktualisiert werden, wenn die tatsächlich
                                          im Lager stehende Kiste mit einer eigenen ID erfasst und ausgebucht wird.

                                          Beispiel
                                          Im Auftrag wird eine Dummy-Kiste (ohne ID) mit den gewünschten Maßen er-
                                          fasst. Als Menge wird 3 angegeben. Damit werden drei Stück der Dummy-Kis-
                                          te reserviert.

                                                                            Ausbuchung

                                           vor Lieferscheindruck                    nach Lieferscheindruck

                                           • Im Warenausgang werden die echten      • Der Lieferschein wird gedruckt.
                                             Kisten mit ID gescannt.                • Damit werden die reservierten
                                           • Die Reservierung auf die Dummy-Kiste     Dummy-Kisten ausgebucht.
                                             wird storniert.                        • Mit dem Warenausgang Kiste
                                           • Die drei Kisten mit ID werden als        werden drei echte Kisten mit ID
                                             reserviert gekennzeichnet.               gescannt.
                                           • Der Lieferschein wird gedruckt. Mit    • Die Reservierung der Dummy-Kisten
                                             dem Warenausgang werden die drei         wird storniert.
                                             Kisten ausgebucht.                     • Die drei Kisten werden ausgebucht.
1.10 / 12-2019




                                          Tab. K-2      Ausbuchung von Kisten vor oder nach Druck des Lieferscheins




                 K-56                                                                A+W Business Kistenmanagement
                 Tutorial                                                                   Lagerverwaltung für Kisten




                                          Folgende Schritte sind i. d. R. der Ausbuchung vorausgegangen:
                                          •   Im Kundenauftrag wurde das Produkt erfasst:




                    Abb. K-37   Produkt 1005 erfasst


                                          •   Über [F1] im Dialog Lagerinfo wurde die Dummy-Kiste ausgewählt:




                                                                                                                A




                                                                                            B

                    A Dummy-Kiste ohne ID              B Reservierungen auf Dummy-Kiste
                    Abb. K-38   Auswahl der Dummy-Kiste


                                          •   Die Kiste wurde in den Auftrag übernommen und z. B. mit der Positions-
                                              menge 3 gespeichert:
1.10 / 12-2019




                 A+W Business Kistenmanagement                                                                  K-57
                 Lagerverwaltung für Kisten                                                                      Tutorial




                    Abb. K-39   Positionsmenge 3 gespeichert


                                         •     Im Lager wurden 3 zusätzliche Reservierungen auf die Dummy-Kiste ge-
                                               bucht:




                                                                                                A
                    A Reservierungen auf Dummy-Kiste um 3 erhöht
                    Abb. K-40   Reservierung


                                         •     Im Buchungsjournal (Lagerwirtschaft) ist die Positionsmenge als reserviert
                                               gekennzeichnet:




                                         Abb. K-41      Position des Auftrags ist reserviert
1.10 / 12-2019




                                         Als nächstes werden Kisten mit ID zugewiesen und nach dem Druck des Lie-
                                         ferscheins ausgebucht.


                 K-58                                                                    A+W Business Kistenmanagement
                 Tutorial                                                               Lagerverwaltung für Kisten




                                         Warenausgang buchen

                                          So buchen Sie den Warenausgang von Kisten
                                         1 Wählen Sie im Menü Fertigung > Lieferwesen > Warenausgang Kisten.




                    Abb. K-42   Warenausgang-Kiste – Kundenauftrag aufrufen


                                         2 Wählen Sie die Option nach Scanner.
                                         3 Erfassen Sie den Barcode der Auftragsnummer und der Positionsnummer.
                                            Die Nummern werden in den Feldern Dokument angezeigt.
                                            Wenn Sie nicht mit einem Scanner arbeiten, wählen Sie die Option nach
                                            Auftragsnummer und geben die Nummer ein.
                                         4 Wählen Sie im Menü Start > Ausführen, um die Auftragsdaten einzulesen.
                                            Die Anzeige wechselt zum Register Identnummern.
1.10 / 12-2019




                 A+W Business Kistenmanagement                                                               K-59
                 Lagerverwaltung für Kisten                                                                       Tutorial




                    Abb. K-43   Auftragsposition mit Unterpositionen


                                              Jede Kiste wird in einer eigenen Zeile als virtuelle Position angezeigt. Die
                                              Felder in der Spalte Identnummer sind leer, da noch keine Kiste mit ID zu-
                                              gewiesen wurde.
                                          5 Scannen Sie die Kisten-ID der ersten Kiste, die reserviert werden soll.
                                              Wenn Sie nicht mit einem Scanner arbeiten, wählen Sie im Feld Identnum-
                                              mer eine der angezeigten IDs aus. Nur Kisten-IDs von Kisten des erfassten
                                              Typs werden angezeigt.
                                          6 Wählen Sie im Menü Start > Ausführen, um die Kiste zuzuordnen.
                                          7 Wiederholen Sie die Schritte 5 und 6 ggf., um weitere Kisten mit ID zuzu-
                                            ordnen.


                                          Ergänzende Informationen
                                           Stammdaten, “Firmendaten – Parameter” auf Seite B-936
                                           Stammdaten, “Virtuelle Positionsnummern verwenden” auf Seite B-943
                                           Verkauf, “Lagerinfo” auf Seite C-741
                                           Softwarereferenz, “Warenausgang” auf Seite E-239
1.10 / 12-2019




                 K-60                                                                A+W Business Kistenmanagement
                 Tutorial                                                                 Lagerverwaltung für Kisten




                                      Manuelle Lagerbuchungen
                                      Wenn Sie nicht mit der BDE arbeiten, können Sie alle Lagerbuchungen auch
                                      manuell starten.
                                      In diesem Kapitel finden Sie Informationen zu folgenden Themen:
                                      •   “Zugang manuell erfassen” auf Seite K-61
                                      •   “Lagerort einer Kiste ändern” auf Seite K-65
                                      •   “Kisteninhalt korrigieren (Blattanzahl)” auf Seite K-66
                                      •   “Kisten aufbrechen (auflösen)” auf Seite K-67


                                      Zugang manuell erfassen
                                      Sie können die Kisten manuell in den Lagerbestand aufnehmen oder aus dem
                                      Lagerbestand ausbuchen.

                                          Voraussetzung
                                          In den Firmendaten muss die Checkbox für die virtuelle Vergabe von Posi-
                                          tionsnummern markiert sein.

                                           “Firmendaten” auf Seite K-18
                                      Zu dieser Lerneinheit gibt es folgende Handlungsanleitungen:
                                      •   “So stellen Sie die ID für Kisten ein” auf Seite K-61
                                      •   “So legen Sie eine neue Kiste im Lagerbestand an” auf Seite K-62
                                      •   “So buchen Sie einen Warenabgang manuell” auf Seite K-63


                                       So stellen Sie die ID für Kisten ein
                                      1 Wählen Sie im Modul Dokumente > Bestellung > Wareneingang > Waren-
                                        eingang.
                                      2 Wählen Sie im Menü Optionen > Gruppe Identnummernvergaben > Ein-
                                        stellungen.




                                      3 Ersetzen Sie die Buchstabenfolge durch das gewünschte Kennzeichen.
1.10 / 12-2019




                                          Achten Sie darauf, dass Sie die Platzhalter für die Ziffern nicht überschrei-
                                          ben.
                                      4 Klicken Sie auf [OK], um die Änderung zu speichern.


                 A+W Business Kistenmanagement                                                                   K-61
                 Lagerverwaltung für Kisten                                                                    Tutorial




                                            So legen Sie eine neue Kiste im Lagerbestand an
                                           1 Wählen Sie im Menü Lagerwirtschaft > Lagerverwaltung.
                                              Der Dialog Lagerverwaltung wird angezeigt.
                                           2 Wählen Sie im Menü Optionen > Identnummer automatisch vergeben.
                                              Damit die automatische ID für Kisten mit dem neuen Kennzeichen verge-
                                              ben. Die Zählung beginnt mit jedem neuen Kennzeichen bei 1 und wird je-
                                              weils um 1 Nummer erhöht.
                                              Im Register Lagerartikel ist das Feld Ident gesperrt.
                                           3 Geben Sie im Feld Artikel die Produktnummer des Glases ein, zu dem eine
                                             Kiste verbucht werden soll.
                                           4 Wählen Sie im Menü Start > Suchen.




                                                                                                                   C



                 A




                                                                                                                   D



                 B




                 A Lagerort                                          C Kiste
                 B Lagerbestand                                      D Lagerartikel ohne ID
                 Abb. K-44   Kistendaten


                                           5 Markieren Sie die Kiste (C, D), zu der Sie den Bestand eintragen wollen.
                                              Damit werden alle erforderlichen Daten übernommen und Sie können eine
                                              neue Kiste im Bestand anlegen.
                                           6 Wählen Sie im Menü Start > Neu.
1.10 / 12-2019




                                              Die Felder werden freigeschaltet.
                                           7 Wählen Sie den Lagerort (A) aus, an dem die neue Kiste steht.


                 K-62                                                                A+W Business Kistenmanagement
                 Tutorial                                                                Lagerverwaltung für Kisten




                                      8 Geben Sie im Feld Lagerbestand die Zahl 1 ein.
                                         Da jede Kiste eine eigene Identnummer erhalten soll, dürfen Sie nur die 1
                                         eintragen.
                                      9 Wählen Sie im Menü Start > Speichern, um die Daten zu speichern.




                                         Im Feld für den Lagerbestand wird eine neue Kiste mit einer ID angezeigt.
                                      10 Wiederholen Sie Schritt 6 und Schritt 9, bis Sie alle Kisten in den Bestand
                                         aufgenommen haben.
                                         Beachten Sie dabei, ob alle Kisten an denselben Lagerort gebucht werden
                                         sollen. Alle anderen Werte brauchen sie nicht zu ändern, bis Sie alle Kisten
                                         gebucht haben.


                                       So buchen Sie einen Warenabgang manuell
                                      1 Wählen Sie im Menü Lagerwirtschaft > Lagerbewegung > Register Ab-
                                        gang.
                                      2 Geben Sie entweder die Produktnummer oder die Ident-Nr. der Kiste ein
                                        und wählen Sie im Menü Start > Suchen.
                                         Die Suche beschränkt sich damit auf diese eine Kiste.
                                         Alternativ können Sie die Suche auch auf die Produktnummer und den La-
                                         gerort einschränken.
                                         Im Bereich Lagerorte werden alle Lagerartikel aufgeführt, die dem Suchkri-
                                         terium entsprechen.
1.10 / 12-2019




                 A+W Business Kistenmanagement                                                                 K-63
                 Lagerverwaltung für Kisten                                                                  Tutorial




                                              Abb. K-45   Manueller Lagerabgang von Kisten


                                         3 Markieren Sie die Kiste, die Sie ausbuchen wollen.
                                         4 Tragen Sie im Feld Menge eine 1 ein, um den Bestand um die markierte
                                           Kiste zu reduzieren.
                                         5 Ändern Sie ggf. das Buchungsdatum und tragen Sie ggf. eine Bemerkung
                                           ein.
                                         6 Wählen Sie im Menü Start > Speichern, um die Änderungen zu speichern.
                                              Die Daten werden gespeichert und der Bestand wird auf 0 gesetzt.
1.10 / 12-2019




                 K-64                                                              A+W Business Kistenmanagement
                 Tutorial                                                               Lagerverwaltung für Kisten




                                      Lagerort einer Kiste ändern
                                      In dieser Einheit lernen Sie, wie Sie eine Kiste von einem Lagerort zu einem
                                      anderen verschieben. Diese Bewegung wird durch eine Umbuchung erfasst.
                                      Dadurch werden die Lagerartikel beim alten Lagerort als Abgang und beim
                                      neuen als Zugang verbucht.


                                       So buchen Sie einen Lagerort um
                                      1 Wählen Sie im Menü Lagerwirtschaft > Lagerbewegung.
                                         Der Dialog Lagerbewegung wird angezeigt.
                                          Softwarereferenz, “Lagerbewegung” auf Seite G-195
                                      2 Wechseln Sie zum Register Umbuchung.
                                      3 Geben Sie im Feld Produkt die Produktnummer oder die (Kisten-)ID ein.
                                      4 Wählen Sie im Menü Start > Suchen, um in die Suche zu starten.

                                                                            A                    B




                                         A Aktueller Lagerort                   B Neuen Lagerort wählen
                                         Abb. K-46    Lagerbewegung – Umbuchung


                                      5 Markieren Sie die Kiste, die Sie an einen anderen Lagerort buchen wollen.
                                      6 Wählen Sie im Bereich Lagerort (B) den neuen Lagerort aus.
                                      7 Wählen Sie im Menü Start > Speichern, um die Änderungen zu speichern.
1.10 / 12-2019




                                         Die Kiste wird am alten Lagerort aus- und am neuen zugebucht.
                                         Wenn Sie die Option Protokoll beim Beenden aktiviert haben, wird der Di-
                                         alog Lagerhistorie geöffnet. Sie können dann alle Lagerbewegungen als
                                         Protokoll drucken.

                 A+W Business Kistenmanagement                                                               K-65
                 Lagerverwaltung für Kisten                                                                     Tutorial




                                         Kisteninhalt korrigieren (Blattanzahl)
                                         Wenn sich im Lager herausstellt, dass der Inhalt einer Kiste nicht mit den An-
                                         gaben auf dem Lieferschein übereinstimmt, muss die Anzahl der Blätter korri-
                                         giert werden. In dieser Einheit lernen Sie, wie Sie den Inhalt einer Kiste
                                         korrigieren.

                                              Nur Kisten mit einer ID
                                              Der Inhalt einer Kiste kann nur geändert werden, wenn die Kiste mit einer
                                              eigenen Kisten-ID erfasst ist.


                                          So korrigieren Sie die Blattanzahl einer Kiste
                                         1 Wählen Sie im Menü Lagerwirtschaft > Lagerbewegung.
                                              Der Dialog Lagerbewegung wird angezeigt.
                                         2 Wechseln Sie zum Register Blattanzahl.
                                         3 Geben Sie im Feld Produkt die Produktnummer oder die Kisten-ID ein.
                                         4 Wählen Sie im Menü Start > Suchen, um in die Suche zu starten.

                                                                                     A                            B




                                              A Kiste                                B Blattanzahl
                                              Abb. K-47    Blattanzahl korrigieren


                                         5 Markieren Sie die gewünschte Kiste (A).
                                              Das Feld Inhalt wird freigeschaltet.
1.10 / 12-2019




                                         6 Geben Sie die neue Blattanzahl (B) ein.




                 K-66                                                                A+W Business Kistenmanagement
                 Tutorial                                                                Lagerverwaltung für Kisten




                                      7 Wählen Sie im Menü Start > Speichern, um die Änderungen zu speichern.
                                         Die Daten werden gespeichert.


                                      Kisten aufbrechen (auflösen)
                                      Sie können Kisten aufbrechen, um die Gläser für die Produktion zur Verfügung
                                      zu stellen oder einzeln im Auftrag zu erfassen. Sie können nur Kisten mit einer
                                      ID auflösen.

                                         Lagerartikel mit Scheibenmaßen müssen angelegt sein
                                         Wenn Sie eine Kiste auflösen, werden die Blätter in den Lagerbestand ge-
                                         bucht. Die Lagermaße für die Blätter werden ggf. automatisch angelegt. In
                                         diesem Fall werden die Blätter auf den Lagerort der aufgelösten Kiste ge-
                                         bucht.


                                       So lösen Sie eine Kiste auf
                                      1 Wählen Sie im Menü Lagerwirtschaft > Lagerbewegung.
                                         Der Dialog Lagerbewegung wird angezeigt.
                                      2 Wechseln Sie zum Register Aufbruch.
                                      3 Geben Sie im Feld Produkt die Produktnummer oder die Kisten-ID ein.
                                      4 Wählen Sie im Menü Start > Suchen, um in die Suche zu starten.

                                                                                  A                    B       C




                                         A Kiste soll aufgelöst werden           B Inhalt
1.10 / 12-2019




                                                                                 C Anzahl der Kisten
                                         Abb. K-48    Lagerbewegung – Kiste auflösen




                 A+W Business Kistenmanagement                                                                 K-67
                 Lagerverwaltung für Kisten                                                                   Tutorial




                                         5 Markieren Sie die gewünschte Kiste.
                                              Die Felder Anzahl Kiste (C) und Abweichender Inhalt (B) werden freige-
                                              schaltet.
                                         6 Geben Sie im Feld Anzahl Kiste eine 1 ein und prüfen Sie, ob der Inhalt der
                                           Kiste korrekt ist.
                                              Korrigieren Sie ggf. den Wert in Feld Abweichender Inhalt.
                                         7 Wählen Sie im Menü Start > Speichern, um die Änderungen zu speichern.
                                              Die Kiste wird aus- und die Scheiben werden als Lagerartikel zugebucht.
                                         8 Aktualisieren Sie ggf. die Anzeige der Lagerorte, indem Sie sie neu einle-
                                           sen.
                                         9 Löschen Sie ggf. die leere Kiste manuell aus dem Bestand.
1.10 / 12-2019




                 K-68                                                               A+W Business Kistenmanagement
Kistenmanagement                K

                   Softwarereferenz




                   A+W Business
                 Softwarereferenz                                                                     Übersicht




                                      Übersicht
                                      Im Modul Lagerwirtschaft werden alle Daten zum Lager gepflegt und ausge-
                                      wertet. Außerdem führen Sie in diesem Modul die Inventur durch und buchen
                                      Lagerbewegungen.
                                      In der Softwarereferenz finden Sie Informationen zu folgenden Themen:
                                      •   “Lagerverwaltung” auf Seite K-72
                                      •   “Lagerbewegung” auf Seite K-83
                                      •   “Suche” auf Seite K-90
                                      •   “Lagerbestellung” auf Seite K-96
                                      •   “Kisten – Ein- und Ausgang” auf Seite K-102
1.10 / 12-2019




                 A+W Business Kistenmanagement                                                            K-71
                 Lagerverwaltung                                                                Softwarereferenz




                                   Lagerverwaltung
                                   Lagerwirtschaft > Lagerverwaltung
                                   Im Dialog Lagerverwaltung können Sie sich alle Artikel anzeigen lassen, die
                                   im Lager verwaltet werden.
                                   In diesem Kapitel finden Sie Informationen zu folgenden Themen:
                                   •   “Menüs in der Lagerverwaltung” auf Seite K-72
                                   •   “Lagerverwaltung” auf Seite K-73


                                   Menüs in der Lagerverwaltung
                                   Lagerwirtschaft > Lagerverwaltung
                                   Über die Menüs können Sie die Standardeinstellung des Dialoges bestimmen
                                   und andere Dialoge öffnen, ohne den Dialog zu schließen.
                                   In diesem Kapitel finden Sie Informationen zu folgenden Themen:
                                   •   “Menü Funktionen” auf Seite K-72
                                   •   “Menü Optionen” auf Seite K-73


                                   Menü Funktionen
                                   Lagerwirtschaft > Lagerverwaltung > Menü Funktionen
                                   Über dieses Menü können Sie andere Dialoge öffnen, ohne die Lagerverwal-
                                   tung zu schließen.
                                   Folgende Einträge werden angezeigt:
                                   •   Lagerhistorie:
                                       Öffnet den Dialog Lagerhistorie mit dem Protokoll der Vorgänge, die in der
                                       Lagerverwaltung gebucht wurden.
                                   •   Buchungsjournal:
                                       Öffnet den Dialog Buchungsjournal mit dem Protokoll der Lagerbuchungen
                                       aus Aufträgen und Bestellungen.
1.10 / 12-2019




                 K-72                                                        A+W Business Kistenmanagement
                 Softwarereferenz                                                                   Lagerverwaltung




                                      Menü Optionen
                                      Lagerwirtschaft > Lagerverwaltung > Menü Optionen
                                      Über dieses Menü können Sie die Standardeinstellung des Dialoges bestim-
                                      men. Sie können die Optionen aktivieren oder deaktivieren. Die Einstellung
                                      wird nicht zurückgesetzt, wenn Sie den Dialog schließen.
                                      Folgende Einträge werden angezeigt:
                                      •   Artikel mit Bestand = 0 nicht drucken:
                                          Nur Artikel, deren Bestand größer als 0 ist, werden gedruckt. Diese Einstel-
                                          lung ist sinnvoll, wenn es sehr viele Kisten mit einer ID aber ohne Bestand
                                          gibt. Diese sind dann in der Regel als Kiste ausgeliefert worden und aus
                                          dem Bestand gelöscht. Die Einstellung gilt nur für den Druck, im Dialog
                                          werden alle Artikel angezeigt.
                                      •   Identnummer automatisch vergeben:
                                          Die ID der Kiste kann auch automatisch vergeben werden, wenn sie ma-
                                          nuell als Bestand gebucht wird.


                                      Lagerverwaltung
                                      Lagerwirtschaft > Lagerverwaltung
                                      Im Dialog Lagerverwaltung werden die Lagerartikel erfasst, die im Lager mit
                                      Beständen gehalten werden.
                                      Lagermaße werden in A+W Business auch in der Produktverwaltung gepflegt.
                                      Sie dienen dort dazu, Preisschlüssel, Warengruppen, usw. zuzuordnen.
                                      Im Dialog Lagerverwaltung finden Sie folgende Register:
                                      •   Lagerverwaltung – Lagerartikel
                                      •   Lagerverwaltung – Preise
                                      •   Lagerverwaltung – Zusatz

                                          Lagerverwaltung auf der Ebene der Stücklisten
                                          Sie können im Lager auch Produkte verwalten, die als Stücklisten-Kompo-
                                          nenten in anderen Produkten enthalten sind. Dazu muss in den Firmenda-
                                          ten die Checkbox Lagerführung auf Stücklistenebene aktiviert sein.

                                           Stammdaten, “Lagerführung auf Stücklistenebene” auf Seite B-960
1.10 / 12-2019




                 A+W Business Kistenmanagement                                                                  K-73
                 Lagerverwaltung                                                                            Softwarereferenz




                                          Lagerverwaltung – Lagerartikel
                                          Lagerwirtschaft > Lagerverwaltung > Register Lager-Artikel




                 Abb. K-49   Lagerverwaltung – Lagerartikel


                                          In diesem Register können Sie die Artikel prüfen, die im Lager verwaltet wer-
                                          den. Der angezeigte Bestand wird mit jeder Lagerbuchung aktualisiert. Sie
                                          können neue Artikel hinzufügen und die verschiedenen Mengen korrigieren.
                                          Für das Bestellwesen legen Sie außerdem Mindest- und Bestellmengen fest.
                                           Tutorial, “So legen Sie einen Lagerartikel an” auf Seite K-26

                                          Artikel

                                          Artikel Produktnummer aus den Stammdaten. Wenn Sie einen neuen La-
                                          gerartikel erfassen möchten, müssen Sie ihn zuerst in den Stammdaten anle-
                                          gen.

                                          Lager-ID Identnummer, die beim Wareneingang vergeben wurde.

                                          Bezeichnung Produktbezeichnungen aus den Stammdaten.

                                          Breite x Höhe / Inhalt Maße des Lagerartikels in mm (nur Lagermaße) und
1.10 / 12-2019




                                          Inhalt der Kiste. Bei Kisten tragen Sie ein, wie viele Blätter die Kiste enthält.
                                          Für alle anderen Lagerartikel steht automatisch eine 1.




                 K-74                                                                  A+W Business Kistenmanagement
                 Softwarereferenz                                                                  Lagerverwaltung




                                      Variante Wenn zu einem Artikel Varianten angelegt sind, so wird die Farbe
                                      angezeigt.

                                      Default-Lagerort Wenn Sie Lagerorte definiert haben, werden diese zur
                                      Auswahl angeboten.
                                      Wenn Sie einen Lagerartikel an mehreren Lagerorten halten, kann ein Stan-
                                      dard-Lagerort festgelegt werden.
                                      ☐ Der angezeigte Lagerort ist für den Lagerartikel nicht als Standard festge-
                                      legt.
                                      ☑ Der angezeigte Lagerort ist für den Lagerartikel als Standard-Lagerort fest-
                                      gelegt.
                                       Stammdaten, “Lagerdefinition” auf Seite B-737

                                         Lagerort <k.A.>
                                         Auch wenn Sie eigene Lagerorte hinterlegt haben, bleiben die Lagerorte
                                         <k.A.> erhalten und können bebucht werden.

                                      Ident. Die Kisten-ID, die beim Wareneingang oder manuell vergeben wurde.
                                      Die ID wird nur angezeigt, wenn Sie in der Übersicht der Lagerartikel eine Kis-
                                      te markiert haben.

                                      Details

                                      Kategorie Wenn Sie in den Stammdaten Lagerkategorien definiert haben,
                                      können Sie dieses Feld als Suchkriterium verwenden. Beim Anlegen neuer
                                      Lagerartikel können Sie eine Kategorie zuordnen.

                                      Lief.-Ident Die Kisten-ID des Lieferanten wird nur angezeigt, wenn Sie im
                                      Bereich Lagerartikel eine Kiste markiert haben.

                                      Hauptartikel Lagerartikel mit mehreren Maßen können Sie miteinander ver-
                                      knüpfen, indem Sie einen Hauptartikel angeben. Die Bestandsprüfung (für die
                                      Lagervorschau im Dialog Lagerinfo) wird dann nur für den Hauptartikel durch-
                                      geführt und nur für diesen müssen Sie einen Mindestbestand hinterlegen.
                                      Wenn bei den zugeordneten Lagerartikeln ebenfalls Mindestbestände festge-
                                      legt sind, werden diese bei der Prüfung ignoriert.
                                       Tutorial, “Lagerverwaltung” auf Seite K-14

                                      Produktionslauf / Datum Zur Zeit nicht genutzt.

                                      Datum Datum, an dem der Lagerartikel zuletzt geändert wurde.

                                      In Produktion In Verbindung mit A+W Production können Sie festlegen, ob
                                      der Lagerartikel der Produktion zugeordnet ist.
                                      ☐ Der Lagerartikel ist frei verfügbar.
                                      ☑ Der Lagerartikel ist der Produktion zugeordnet (nur Info).
1.10 / 12-2019




                 A+W Business Kistenmanagement                                                                 K-75
                 Lagerverwaltung                                                               Softwarereferenz




                                   Bestände

                                   Lagerbestand Anzeige des aktuellen Bestands. Der Bestand wird bei jeder
                                   Ab- oder Zubuchung aktualisiert. Für Kisten mit einer ID wird jeweils der Be-
                                   stand 1 angezeigt.
                                   Wenn Sie den Lagerartikel neu angelegt haben, ist das Feld freigeschaltet und
                                   Sie können den Anfangsbestand eintragen.

                                   Bestand > 0 Diese Checkbox ist nur im Auswahlmodus freigeschaltet. Sie
                                   können damit als Suchkriterium festlegen, ob Artikel ohne Bestandsmenge
                                   angezeigt werden.
                                   ☐ Im Suchergebnis werden auch Artikel angezeigt, deren aktueller Bestand 0
                                   ist.
                                   ☑ Im Suchergebnis werden nur Artikel angezeigt, deren aktueller Bestand
                                   mindestens 1 ist.

                                   Mindestbestand Der Mindestbestand bildet die Grundlage für automatische
                                   Bestellvorschläge. Sie werden erzeugt, wenn der Lagerbestand den Mindest-
                                   bestand unterschreitet. Dabei werden die Reservierungen und die Bestellun-
                                   gen mitberücksichtigt. Diese automatischen Bestellvorschläge können Sie im
                                   Dialog Bestellpool prüfen und an den Einkauf übergeben.
                                    “Lagerbestellung” auf Seite K-96

                                   Mindestbestand > 0 Diese Checkbox ist nur im Auswahlmodus freigeschal-
                                   tet. Sie können damit als Suchkriterium festlegen, ob der Mindestbestand grö-
                                   ßer als 0 sein muss.
                                   ☐ Im Suchergebnis werden alle Artikel angezeigt.
                                   ☑ Im Suchergebnis werden nur Artikel angezeigt, deren Mindestbestand grö-
                                   ßer als Null ist.

                                   Bestellmenge Dieser Wert gibt an, welche Menge standardmäßig bestellt
                                   wird. Bei der automatischen Lagerbestellung wird der Wert übernommen.

                                   Bestand < Mindestbestand Diese Checkbox ist nur im Auswahlmodus frei-
                                   geschaltet. Sie können damit als Suchkriterium festlegen, ob der Bestand un-
                                   ter dem Mindestbestand liegen soll.
                                   ☐ Im Suchergebnis werden alle Artikel angezeigt.
                                   ☑ Im Suchergebnis werden nur Artikel angezeigt, deren aktueller Bestand
                                   kleiner als der Mindestbestand ist.

                                   Maximalbestand Mit der Eingabe von Maximalmengen pro Lagerartikel
                                   kann verhindert werden, dass das Lager überfüllt ist. Der eingetragene Wert
                                   dient nur der manuellen Kontrolle.

                                   Sollbestand Zur Zeit nicht genutzt.

                                   Bestandsprüfung pro Lagerort Wenn Sie den Bestand pro Lagerort pfle-
                                   gen, können Sie die den Bestand pro Lager prüfen.
1.10 / 12-2019




                                   ☐ Der Bestand wird für alle Lagerorte gemeinsam geprüft.
                                   ☑ Der Bestand wird pro Lagerort geprüft.



                 K-76                                                       A+W Business Kistenmanagement
                 Softwarereferenz                                                                 Lagerverwaltung




                                      Lagerartikel
                                      In den Übersichten werden die Lagerartikel angezeigt, die den Suchkriterien
                                      entsprechen. Die obere Liste zeigt die Lagerartikel insgesamt an. Wenn Sie
                                      einen Eintrag markieren, werden in der unteren Liste die Artikel pro Lagerort
                                      angezeigt. Wenn Checkbox Bestand > 0 aktiviert ist, werden nur Lagerorte
                                      aufgelistet, deren Bestand größer als 0 ist.
                                      Folgende Spalten werden angezeigt:
                                      •   Artikel, Mengeneinheit - Variante:
                                          Artikelnummer, Bezeichnung, Mengeneinheit und Farbe aus der Lagerver-
                                          waltung.
                                      •   Breite, Höhe:
                                          Maße aus der Lagerverwaltung.
                                      •   Inhalt:
                                          Anzahl der Blätter in einer Kiste.
                                      •   Ges. Bestand:
                                          Bestand des Lagerartikels aller Lagerorte.
                                      •   Min. Bestand:
                                          Menge des festgelegten Mindestbestands.
                                      •   Best. Menge:
                                          Festgelegte Bestellmenge.

                                      Lagerorte
                                      •   Ident:
                                          Kisten-ID (manuelle Buchung oder aus dem Wareneingang).
                                      •   Lagerort:
                                          Lagerort in der Reihenfolge von Ebene 1 bis 4.
                                      •   Lagerbestand:
                                          Aktueller Bestand am Lagerort.
                                      •   Lief.-Ident:
                                          Kisten-ID des Lieferanten (nur wenn diese im Wareneingang miterfasst
                                          wurde).
1.10 / 12-2019




                 A+W Business Kistenmanagement                                                                K-77
                 Lagerverwaltung                                                                          Softwarereferenz




                                          Lagerverwaltung – Preise
                                          Lagerwirtschaft > Lagerverwaltung > Register Preise




                 Abb. K-50   Lagerverwaltung – Preise


                                          In diesem Register werden die aktuellen Preise eines Lagerartikels angezeigt.
                                          Bei der Aktualisierung werden Aufträge, Bestellungen und Lagerumbuchun-
                                          gen berücksichtigt.

                                             Voraussetzung
                                             Der durchschnittliche Einkaufspreis (Durchschnitts-EK) wird nur dann be-
                                             rechnet und angezeigt, wenn in den Firmendaten die Checkbox Durch-
                                             schnitts-Einkaufspreis ermitteln aktiviert ist.

                                              Stammdaten, “Durchschnitts EK: Der Durchschnittspreis für den Einkauf wird in
                                               folgenden Fällen neu berechnet:” auf Seite B-957
                                          Die Felder in den Übersichten sind ausführlich zum Register Lagerartikel be-
                                          schrieben.
                                           “Lagerverwaltung – Lagerartikel” auf Seite K-74

                                          Einkaufspreise
1.10 / 12-2019




                                          Niedrigster Preis Der niedrigste Preis, zu dem der Artikel eingekauft wurde.

                                          Höchstpreis Der höchste Preis, zu dem der Artikel eingekauft wurde.



                 K-78                                                                 A+W Business Kistenmanagement
                 Softwarereferenz                                                                  Lagerverwaltung




                                      Letzter Preis Der jüngste Preis, zu dem der Artikel eingekauft wurde.

                                      Lagerwert In dieser Spalte werden die aktuellen Lagerwerte angezeigt. Sie
                                      ergeben sich aus dem jeweiligen Preis und der Menge.

                                      Berechnung des geschnittenen Preises (Durchschnitts-EK)
                                      Mit der Wahl der Option bestimmen Sie, welche Lagermaße in dieser Über-
                                      sicht bei der Berechnung berücksichtigt werden. Die Einstellung ist nur bei
                                      Scheiben mit unterschiedlichen Lagermaßen sinnvoll.
                                      •   Nur dieser Artikel:
                                          Bei der Berechnung wird nur der angezeigte Artikel in der gewählten Ab-
                                          messung berücksichtigt. Die EK-Historie des aktuellen Artikels wird ange-
                                          zeigt.
                                      •   Alle Abmessungen:
                                          Bei der Berechnung werden alle Abmessungen des angezeigten Glases
                                          berücksichtigt. Die EK-Historie aller Abmessungen des Artikels wird ange-
                                          zeigt.
                                      Der Durchschnitts-EK wird für jeden Wareneingang errechnet, unabhängig
                                      davon, wie er gebucht wurde. Warenabgänge reduzieren lediglich den Be-
                                      stand. Die Liste wird durch die Archivierung und durch die Rechnungskontrolle
                                      reduziert.
                                      Der erste Datensatz zeigt den Anfangsbestand und den ursprünglichen Preis.
                                      Darunter werden Zu- und Abgänge (negatives Vorzeichen) aufgeführt. Beim
                                      Zugang durch eine Lagerbestellung sind außerdem die Bestellnummer und
                                      die Bestellposition angezeigt.
                                      Der Durchschnitts-EK wird bei der Erfassung oder Änderungen von Bestellun-
                                      gen aktualisiert. Er wird unter Berücksichtigung der gesamten Menge ermit-
                                      telt.

                                          Beispiel:

                                          100 Stück      auf Lager             à 15,00 €               1500,00 €

                                           40 Stück      neue Einbuchung       à 18,00 €       +        720,00 €

                                                                                               =      2200,00 €
                                                                                                      ========
                                          2200,00/140 Stück = 15,86 €



                                      In die Berechnung fließen auch automatische Zuschläge ein, die in Bestellun-
                                      gen aufgeführt sind, z. B. Energie- oder Transportzuschlag.
1.10 / 12-2019




                 A+W Business Kistenmanagement                                                                K-79
                 Lagerverwaltung                                                               Softwarereferenz




                                   Übersicht Die jeweiligen Durchschnittspreise werden als Historie darge-
                                   stellt. Auf diese Weise können Sie die Preisentwicklung leicht nachverfolgen.
                                   Angezeigt werden:
                                   •   Datum:
                                       Datum der letzten Aktualisierung.
                                   •   Menge [ME]:
                                       Ab- oder zugebuchte Menge und Mengeneinheit.
                                   •   Preis/PE:
                                       EK-Preis pro Preiseinheit zum Zeitpunkt der Buchung.
                                   •   Bestand [ME]:
                                       Bestand zum anzeigten Datum. Wenn der Durchschnitts-EK für alle Ab-
                                       messungen angezeigt wird, wird der Bestand immer in qm angezeigt.
                                   •   Geschnittener Preis / PE:
                                       Durchschnittspreis pro Preiseinheit zum Zeitpunkt der Buchung.
                                   •   Bestellung / Pos.:
                                       Nummer der Bestellung und der Bestellposition.
                                   •   Lagerwert:
                                       Lagerwert zum angezeigten Datum (Berechnung: EK-Preis * Bestand).
                                   •   Typ:
                                       Art von Buchung, die den jeweiligen Eintrag verursacht hat.

                                   Einbeziehen in Gesamt-EK Sie können festlegen, ob der Artikel in die Be-
                                   rechnung des gesamten Durchschnittspreises aller Ausprägungen dieses Ar-
                                   tikels einbezogen werden soll.
                                   ☐ Der Artikel wird bei der Berechnung des Durchschnittspreises nicht berück-
                                   sichtigt.
                                   ☑ Der Artikel wird in die Berechnung mit einbezogen.

                                   Geschnittener Preis Aktueller Durchschnittspreis. Je nach der Option zur
                                   Berechnung des Durchschnitts-EKs gilt die Anzeige für den aktuellen Artikel
                                   oder für alle Abmessungen des Artikels.

                                       Aktualisierung der Anzeige
                                       Die Anzeige der Durchschnittspreise wird bei der Archivierung und bei der
                                       Rechnungskontrolle für den jeweiligen Lagerartikel aktualisiert. Damit
                                       bleibt die Anzeige übersichtlicher.
                                       A+W Business geht davon aus, dass nach diesen Vorgängen die Preise
                                       nicht mehr geändert werden. Wenn Sie die Preise dennoch nach einem der
                                       Vorgänge ändern, fließen diese Änderungen nicht in die Berechnung des
                                       Durchschnittspreises ein.
1.10 / 12-2019




                 K-80                                                        A+W Business Kistenmanagement
                 Softwarereferenz                                                                    Lagerverwaltung




                                          Lagerverwaltung – Zusatz
                                          Lagerwirtschaft > Lagerverwaltung > Register Zusatz




                 Abb. K-51   Lagerverwaltung – Zusatz


                                          In diesem Register werden Reservierungen zu dem markierten Lagerartikel
                                          angezeigt.
                                          Die Felder in den Übersichten sind ausführlich zum Register Lagerartikel be-
                                          schrieben.
                                           “Lagerverwaltung – Lagerartikel” auf Seite K-74

                                          Reservierung
                                          Die Felder in diesem Bereich sind kundenspezifisch freigeschaltet.

                                          Kunde Nummer und Name des Kunden, für den der markierte Lagerartikel
                                          reserviert ist.

                                          Voll gesperrt Zur Zeit nicht genutzt.

                                          Exklusive Reservierungen Zur Zeit nicht genutzt.

                                          Lieferant
1.10 / 12-2019




                                          Lieferant Nummer und Name des Lieferanten, bei dem der Lagerartikel be-
                                          stellt wird.


                 A+W Business Kistenmanagement                                                                   K-81
                 Lagerverwaltung                                                               Softwarereferenz




                                   Bemerkung

                                   Produktbezogen, Lagerortbezogen Sie können zu jedem Lagerartikel und
                                   zu jedem Lagerort weitere Angaben eintragen, z. B. wann und vom welchem
                                   Lieferanten die Gläser/Kisten geliefert wurden, um die älteren Lieferungen zu-
                                   erst zu verwerten.
1.10 / 12-2019




                 K-82                                                        A+W Business Kistenmanagement
                 Softwarereferenz                                                               Lagerbewegung




                                      Lagerbewegung
                                      Lagerwirtschaft > Lagerbewegung
                                      Sie können Ab- und Zugänge von Lagerartikeln manuell buchen, Bestands-
                                      zahlen korrigieren, Lagerorte umbuchen und Kisten auflösen.
                                      In diesem Kapitel finden Sie Informationen zu folgenden Themen:
                                      •   “Menü Optionen” auf Seite K-83
                                      •   “Lagerbewegung” auf Seite K-83


                                      Menü Optionen
                                      Lagerwirtschaft > Lagerbewegung
                                      Folgende Einträge werden angezeigt:
                                      •   Protokoll beim Beenden:
                                          Beim Beenden des Dialogs wird automatisch die Lagerhistorie angezeigt.
                                      •   Bestand > 0:
                                          Nur Lagerartikel mit einem Bestand größer 0 werden angezeigt.


                                      Lagerbewegung
                                      Lagerwirtschaft > Lagerbewegung
                                      Zu- und Abgänge der Lagerartikel werden automatisch gebucht: bei Waren-
                                      eingängen durch Lieferung, bei Warenabgängen durch Aufträge. Im Dialog
                                      Lagerbewegung können Sie Zu- oder Abgänge manuell buchen, z. B. um Be-
                                      standsmengen zu korrigieren.
                                      Im Dialog Lagerbewegung finden Sie folgende Register:
                                      •   Lagerbewegung – Abgang, Zugang
                                      •   Lagerbewegung – Umbuchung
                                      •   Lagerbewegung – Blattanzahl
                                      •   Lagerbewegung – Aufbruch
1.10 / 12-2019




                 A+W Business Kistenmanagement                                                             K-83
                 Lagerbewegung                                                               Softwarereferenz




                                 Lagerbewegung – Abgang, Zugang
                                 Lagerwirtschaft > Lagerbewegung > Register Abgang, Register Zugang




                                 Abb. K-52     Lagerbewegung – Abgang, Zugang


                                 In den Registern Abgang und Zugang können Sie manuell Ab- und Zugänge
                                 buchen. Sie können einen bestimmten Lagerartikel auswählen und die ent-
                                 sprechenden Daten eingeben. Wenn Sie sich alle Lagerartikel anzeigen las-
                                 sen, können Sie den gewünschten Artikel in der Liste Lagerorte markieren.
                                 Die Felder im Bereich Bestandsveränderung werden dann freigeschaltet.
                                  Tutorial, “Lagerverwaltung für Kisten” auf Seite K-49
                                 Wenn Sie die Option Protokoll beim Beenden aktiviert haben, wird automa-
                                 tisch die Lagerhistorie mit dem Register Tabelle angezeigt, wenn Sie den
                                 Dialog schließen.

                                    Zugang von Kisten manuell erfassen
                                    Da jede Kiste mit einer eigenen ID geführt wird, können Sie Zugänge von
                                    Kisten nur über den Wareneingang oder in der Lagerverwaltung erfassen.
                                    In der Lagerverwaltung legen Sie dazu die Kiste als neuen Lagerartikel an.
1.10 / 12-2019




                 K-84                                                         A+W Business Kistenmanagement
                 Softwarereferenz                                                                Lagerbewegung




                                      Lagerprodukt

                                      Produkt Nummer und Bezeichnung des Lagerartikels.

                                      Ident Nr. Über die Identifikationsnummer können Sie nur Lagerabgänge ver-
                                      buchen. Zugänge von Kisten müssen Sie in der Lagerverwaltung definieren,
                                      damit Sie eine neue ID eintragen können.

                                      Inhalt Wenn Sie eine Kiste ausgewählt haben, wird deren Inhalt angezeigt.
                                      Wenn eine Kiste mit Identnummer ausgeliefert oder geöffnet werden soll, die
                                      bereits einem Auftrag zugeordnet ist, wird eine Meldung angezeigt. Dadurch
                                      wird verhindert, dass durch den anschließenden Druck des Lieferscheins oder
                                      der Rechnung ein negativer Bestand entsteht.

                                      Lagerort Lagerort, der dem Lagerartikel zugeordnet wurde.

                                          Lagerort <k.A.>
                                          Auch wenn Sie eigene Lagerorte hinterlegt haben, bleiben die Lagerorte
                                          <k.A.> erhalten und können bebucht werden.

                                      Durchschnitts EK Der Durchschnitts-EK wird nur angezeigt, wenn die
                                      Funktion in den Stammdaten aktiviert ist.
                                       Stammdaten, “Einkaufspreis ermitteln” auf Seite B-957

                                      Bestandsveränderung

                                      Menge Eingabe die Menge in Stück, die ab- oder zugebucht werden soll.
                                      Wenn Sie mit einer manuellen Abbuchung den Mindestbestand unterschrei-
                                      ten, wird eine Warnmeldung angezeigt.

                                      Breite, Höhe Diese Felder werden nur bei Lagermaßen mit der Mengenein-
                                      heit qm gefüllt.

                                      Bewertungspreis Eingabe des EK-Preises, zu dem der Warenzugang ge-
                                      liefert wurde.

                                      Buchungsdatum Das aktuelle Tagesdatum wird automatisch angezeigt. Es
                                      kann überschrieben werden.

                                      Bemerkung Sie können eine Bemerkung eingetragen oder aus der Kombo-
                                      box auswählen. Die Bemerkung wird in der Lagerhistorie angezeigt.
                                      Über die Schaltfläche können Sie der Liste eine neue Bemerkung hinzufügen.
                                       “Bemerkung (Lagerbewegung)” auf Seite K-89

                                      Lagerorte
                                      •   Farbe:
                                          Die Farbe wird nur bei Varianten angezeigt.
                                      •   Breite, Höhe:
1.10 / 12-2019




                                          Die Maße werden nur angezeigt, wenn das Produkt als Lagermaß oder
                                          Kiste angelegt ist.




                 A+W Business Kistenmanagement                                                              K-85
                 Lagerbewegung                                                                  Softwarereferenz




                                 •   Inhalt:
                                     Bei Lagerartikeln und Lagermaßen wird der Wert 1 angezeigt, bei Kisten
                                     die Anzahl der Blätter.
                                 •   Lagerort:
                                     Lagerort in der Reihenfolge von Ebene 1 bis 4.
                                 •   Ident Nr.:
                                     Kisten-ID (manuelle Buchung oder aus dem Wareneingang).
                                 •   Bestand:
                                     Aktueller Bestand
                                 •   ME:
                                     Mengeneinheit, mit der das Produkt im Lager geführt wird.
                                 •   Lief-Ident:
                                     Kisten-ID des Lieferanten.


                                 Lagerbewegung – Umbuchung
                                 Lagerwirtschaft > Lagerbewegung > Register Umbuchung




                                 Abb. K-53    Lagerbewegung – Umbuchung


                                 In diesem Register buchen Sie Lagerartikel an einen anderen Lagerort. Beim
                                 Umbuchen eines Lagerorts wird immer der gesamte Bestand eines Lageror-
                                 tes an einen anderen Lagerort umgebucht.
                                  Tutorial, “So buchen Sie einen Lagerort um” auf Seite K-65
                                 Die Felder in den Bereichen Lagerprodukt und Lagerorte sind zum Register
                                 Abgang beschrieben.
1.10 / 12-2019




                                  “Lagerbewegung – Abgang, Zugang” auf Seite K-84




                 K-86                                                        A+W Business Kistenmanagement
                 Softwarereferenz                                                                          Lagerbewegung




                                      Lagerort

                                      Lagerort Anzeige des aktuellen Lagerorts. Sie können einen anderen Lager-
                                      ort zuweisen. In der Kombobox werden alle hinterlegten Lagerorte aufgelistet.

                                         Lagerort <k.A.>
                                         Auch wenn Sie eigene Lagerorte hinterlegt haben, bleiben die Lagerorte
                                         <k.A.> erhalten und können bebucht werden.


                                      Lagerbewegung – Blattanzahl
                                      Lagerwirtschaft > Lagerbewegung > Register Blattanzahl




                                      Abb. K-54     Lagerbewegung – Blattanzahl


                                      In diesem Register korrigieren Sie den Inhalt von Kisten.
                                       Tutorial, “So korrigieren Sie die Blattanzahl einer Kiste” auf Seite K-66
                                      Die Felder in den Bereichen Lagerprodukt und Lagerorte sind zum Register
                                      Abgang beschrieben.
                                       “Lagerbewegung – Abgang, Zugang” auf Seite K-84

                                      Inhaltsänderung

                                      Inhalt Nur wenn Sie eine Kiste mit ID ausgewählt haben, wird die Anzahl der
                                      Blätter angezeigt, die in der Kiste vorhanden sein sollten. Diesen Wert können
                                      Sie korrigieren.
1.10 / 12-2019




                 A+W Business Kistenmanagement                                                                      K-87
                 Lagerbewegung                                                                Softwarereferenz




                                 Lagerbewegung – Aufbruch
                                 Lagerwirtschaft > Lagerbewegung > Register Aufbruch




                                 Abb. K-55     Lagerbewegung – Aufbruch


                                 In diesem Register lösen Sie Kisten auf, damit die einzelnen Blätter für die
                                 Produktion zur Verfügung stehen. Bei diesem Vorgang wird die Kiste aus dem
                                 Bestand ausgebucht und die Anzahl der Blätter werden dem Bestand des La-
                                 germaßes zugebucht.
                                  Tutorial, “So lösen Sie eine Kiste auf” auf Seite K-67

                                    Kisteninhalt an einen anderen Lagerort buchen
                                    Wenn Sie eine Kiste aufbrechen, wird der Inhalt an denselben Lagerort ge-
                                    bucht, an dem die Kiste steht. Wenn Sie den Inhalt umbuchen wollen, müs-
                                    sen Sie diesen am alten Lagerort ausbuchen und anschließend am neuen
                                    Lagerort zubuchen.

                                 Die Felder in den Bereichen Lagerprodukt und Lagerorte sind zum Register
                                 Abgang beschrieben.
                                  “Lagerbewegung – Abgang, Zugang” auf Seite K-84

                                 Kistenaufbruch
                                 Wenn eine Kiste mit Identnummer ausgeliefert oder geöffnet werden soll, die
                                 bereits einem Auftrag zugeordnet ist, wird eine Meldung angezeigt. Dadurch
                                 wird verhindert, dass durch den anschließenden Druck des Lieferscheins oder
1.10 / 12-2019




                                 der Rechnung ein negativer Bestand entsteht.

                                 Anzahl Kisten Anzahl der Kisten, die aufgebrochen werden sollen.



                 K-88                                                          A+W Business Kistenmanagement
                 Softwarereferenz                                                               Lagerbewegung




                                      Abweichender Inhalt Nur wenn Sie eine Kiste ausgewählt haben, wird die
                                      Anzahl der Blätter angezeigt. Sie können diesen Wert korrigieren.


                                      Bemerkung (Lagerbewegung)
                                      Lager > Lagerbewegung > [Bemerkung]




                                      Abb. K-56   Bemerkung zur Lagerbewegung


                                      In diesem Dialog hinterlegen Sie Bemerkungen, die im Dialog Lagerbewe-
                                      gung zur Auswahl angeboten werden. Wenn Sie die erste Zeile leer lassen,
                                      können Sie eine zugewiesene Bemerkung auch wieder entfernen.
1.10 / 12-2019




                 A+W Business Kistenmanagement                                                            K-89
                 Suche                                                              Softwarereferenz




                         Suche
                         Lagerwirtschaft > Suche
                         Sie können den Lagerbestand nach einzelnen Lagerartikeln oder nach Wa-
                         rengruppen abfragen.

                             Filter setzen
                             Wenn keine Filter gesetzt sind, werden keine Daten angezeigt.

                         Der Dialog ist ausführlich im Part Verkauf beschrieben.
                          Verkauf, “Lagerinfo” auf Seite C-741
                         Im Dialog Lagersuche finden Sie folgende Register:
                         •   Lagersuche – Lagersuche
                         •   Lagersuche – Zukünftiger Lagerbestand
1.10 / 12-2019




                 K-90                                             A+W Business Kistenmanagement
                 Softwarereferenz                                                                              Suche




                                         Lagersuche – Lagersuche
                                         Lagerwirtschaft > Suche > Register Lagersuche




                 Abb. K-57   Lagersuche – Lagersuche


                                         In diesem Register können Sie sich die aktuellen Bestände, die reservierten
                                         Mengen und die zukünftigen Bestände zu Lagerartikeln anzeigen lassen.
                                          Tutorial, “Lagerführungsmodus und Reservierung” auf Seite K-12

                                         Auswahl
                                         Die Felder sind nur im Auswahlmodus freigeschaltet.

                                         Produkt Produktnummer, unter der das Produkt in den Stammdaten erfasst
                                         ist.

                                         Art Produktart, der das Produkt in den Stammdaten zugeordnet ist.

                                         Gruppe Produktgruppe, der das Produkt in den Stammdaten zugeordnet ist.

                                         Identnr. Identifikationsnummer, unter der der Lagerartikel im Lager erfasst
1.10 / 12-2019




                                         wurde, z. B. für eine Kiste.




                 A+W Business Kistenmanagement                                                                  K-91
                 Suche                                                                 Softwarereferenz




                         Kateg. Wenn in Ihrem Unternehmen Lagerkategorien definiert sind, können
                         diese zum Filtern eingesetzt werden.
                          Stammdaten, “Lagerkategorien” auf Seite B-739

                         Farbe (Farb-)/ Varianten, die zu dem markierten Produkt erfasst sind.

                         WGR von, bis Zur Suche können Sie auch Warengruppen oder Warengrup-
                         penbereiche eintragen. In der Übersicht werden dann alle Produkte der ge-
                         wählten Warengruppen angezeigt.

                         Dicke / Breite / Höhe Diese Angaben werden aus der Lagerverwaltung
                         übernommen. Breite und Höhe werden nur angezeigt, wenn die markierte Po-
                         sition als Lagermaß oder Kiste mit den entsprechenden Angaben erfasst wur-
                         de.

                         Lagerort Wenn Sie mit mehreren Lagerorten arbeiten, wird der Lagerort der
                         markierten Position mit allen definierten Ebenen angezeigt.
                          Stammdaten, “Lagerdefinition” auf Seite B-737

                         Lief. Ident Identifikationsnummer der Lieferung aus der Lagerverwaltung.
                         Sie ist nicht identisch mit der Angabe in der Spalte Ident in der Übersicht.

                         Bemerkung Information, die zur markierten Position bei der Lieferung hin-
                         terlegt wurde.

                         Inhalt von, bis Im Auswahlmodus kann der Inhalt als Suchkriterium angege-
                         ben werden, z. B. alle Kisten mit einem Inhalt von 50 Stück. Inhalt = 1 bedeutet
                         immer Lagermaß.

                         Verfügbarkeit Anzeige der vorrätigen Stückzahlen.

                         Filteroptionen
                         Wenn keine Filter gesetzt sind, werden keine Bestände angezeigt. Der Filter
                         ist gesetzt, wenn die jeweilige Checkbox markiert ist. Folgende Filter stehen
                         zur Wahl:
                         •   Lagerware:
                             Lagerartikel sollen angezeigt werden.
                         •   Kisten (Inhalt > 1):
                             Kisten mit einem Inhalt > 1 sollen angezeigt werden.
                         •   Lagertafeln (Inhalt = 1):
                             Lagermaße sollen angezeigt werden. Die Anzeige der Anzahl (= 1) dient
                             zur Unterscheidung von Kisten mit identischen Größen.
                         •   Kisten nach Lagerort und Lieferant gruppieren:
                             Pro Lagerort und Lieferant wird nur eine Zeile angezeigt.
                         •   Artikel ohne Abmessung:
                             Auch Lagerartikel ohne Abmessungen sollen angezeigt werden.
                         •   Keine Kisten mit Identnummer:
1.10 / 12-2019




                             Kisten, die mit eine ID im Wareneingang erfasst wurden, sollen nicht ange-
                             zeigt werden.




                 K-92                                               A+W Business Kistenmanagement
                 Softwarereferenz                                                                             Suche




                                      •   Mindestmenge > 0:
                                          Nur die Lagerartikel, deren Mindestmenge größer als 0 definiert wurde, sol-
                                          len angezeigt werden.
                                      •   Bestand > 0:
                                          Nur Lagerartikel mit einem Bestand sollen angezeigt werden.
                                      •   Bestand = 0:
                                          Nur Lagerartikel ohne Bestand sollen angezeigt werden.
                                      •   Bestand < 0:
                                          Nur die Lagerartikel sollen angezeigt werden, zu denen Reservierungen
                                          vorliegen, aber kein Bestand.

                                      Druckoptionen
                                      Sie können die Sortierung für den Druck der Übersicht bestimmen. Mit der
                                      Wahl der Option werden die entsprechenden Checkboxen freigeschaltet. Sie
                                      können dann zusätzlich festlegen, wo eine Zwischensumme gedruckt werden
                                      soll.
                                      Folgende Einträge werden angezeigt:
                                      •   Gruppierung nach Produktnummern:
                                          Die Checkbox Zwischensumme n. Warengruppe wird freigeschaltet.
                                      •   Gruppierung nach Produktart/Produktgruppe gruppieren:
                                          Die Checkbox Zwischensummen. Warenobergrp. wird freigeschaltet.
                                      •   Gruppierung nach Warengruppen:
                                          Die Checkbox Zwischensumme n. Warenhauptgrp. wird freigeschaltet.

                                      Übersicht
                                      In der Übersicht werden alle Produkte angezeigt, die mit der Suche ausge-
                                      wählt wurden. Die Spalten zeigen die Details zu den gelagerten Produkten an.
                                      Die reservierten Mengen werden aktualisiert, sobald eine entsprechende Po-
                                      sition im Auftrag gespeichert wurde. Mit dem Druck des Lieferscheins werden
                                      die Angaben in der Spalte Bestand aktualisiert.
                                      Die Einträge in der Trefferliste sind mit folgenden Farben gekennzeichnet:
                                      • Schwarze Schrift:
                                          Lagerartikel mit Mengenführung
                                      • Blaue Schrift:
                                          Lagerartikel ohne Mengenführung
                                      • Rote Schrift:
                                          – Kein Lagerartikel: Artikel, die nicht im Lager geführt werden.
                                          – Dies gilt auch für Produkte, die nicht mehr verfügbar sind oder mit ne-
                                              gativen Beständen angezeigt werden. Ein negativer Bestand entsteht,
                                              wenn der Bestand und die bestellte Menge abzüglich der reservierten
                                              Menge <= 0 sind.

                                      Summen
                                      Die Summen des ausgewählten Produkts werden angezeigt. Wenn Sie eine
1.10 / 12-2019




                                      WGR mit verschiedenen Produkten ausgewählt haben, werden die Summen
                                      des markierten Produkts angezeigt.




                 A+W Business Kistenmanagement                                                                 K-93
                 Suche                                                                                 Softwarereferenz




                                          Lagersuche – Zukünftiger Lagerbestand
                                          Lagerwirtschaft > Suche > Register Zukünftiger Lagerbestand




                 Abb. K-58   Lagersuche – Zukünftiger Lagerbestand


                                          In diesem Register können Sie prüfen, ob die Wiederbeschaffungszeiten für
                                          ein bestimmtes Produkt ausreichen, um einen Auftrag termingerecht auslie-
                                          fern zu können. Die Farbe Rot zeigt an, dass die Termine nicht eingehalten
                                          werden können. Gelb zeigt an, dass die Wiederbeschaffungszeit ausreicht,
                                          sofern die Bestellungen termingerecht eintreffen.
                                          Die Wiederbeschaffungszeit ergibt sich aus der Lieferzeit, die in der Lieferan-
                                          tenkartei für den Artikel hinterlegt ist, und aus den Tourentagen des Lieferan-
                                          ten, die in der Tourenverwaltung hinterlegt sind.

                                          Vorschau bis
                                          Die Vorschau beginnt immer mit dem aktuellen Tagesdatum. Die Anzahl der
                                          Tage für die Vorschau stellen Sie in den Firmendaten ein, z. B. 14 Tage.
                                          • In der oberen Übersicht werden die Daten in einer Zeile pro gewähltem
                                             Produkt aufgelistet.
                                          • In der mittleren Übersicht werden die aktuellen Bestände pro Tag wieder-
1.10 / 12-2019




                                             gegeben.
                                          • In der unteren Übersicht werden Details zum gewählten Produkt angezeigt.




                 K-94                                                               A+W Business Kistenmanagement
                 Softwarereferenz                                                                             Suche




                                      Die Zeilen sind rot, wenn die Produktion nicht möglich ist, weil die Reservie-
                                      rungen den Bestand überschreiten.
                                      Um die Performance zu erhöhen, können Sie die Anzeige der Vorschau durch
                                      folgende Einstellungen einschränken:
                                      •   Im Dialog Produktverwaltung > Register Lager/Einkauf > Checkbox keine
                                          Verfügbarkeitsprüfung können Sie bestimmte Artikel aus der Lagervor-
                                          schau und der Verfügbarkeitsprüfung herausnehmen, indem Sie die Ver-
                                          fügbarkeitsprüfung für diese Artikel ausschalten.
                                      •   Im Dialog Firmendaten können Sie einstellen, über welchen Zeitraum die
                                          Vorschau dargestellt werden soll.
                                      •   Im Dialog Lagerverwaltung können Sie mehrere Lagermaße miteinander
                                          verknüpfen, damit die Bestandsprüfung nur für den definierten Lager-
                                          Hauptartikel durchgeführt wird.
                                           “Hauptartikel” auf Seite K-75
1.10 / 12-2019




                 A+W Business Kistenmanagement                                                                 K-95
                 Lagerbestellung                                                               Softwarereferenz




                                   Lagerbestellung
                                   Lagerwirtschaft > Lagerbestellung
                                   In diesem Dialog können Sie alle vorgeschlagenen Lagerbestellungen prüfen
                                   und an den Einkauf übergeben.
                                   In diesem Kapitel finden Sie Informationen zu folgenden Themen:
                                   •   “Menüs im Bestellpool” auf Seite K-96
                                   •   “Bestellpool” auf Seite K-99


                                   Menüs im Bestellpool
                                   Über die Menüs können Sie automatisch die Datumsfelder aktualisieren las-
                                   sen und zusätzlich andere Dialoge öffnen.
                                   In diesem Kapitel finden Sie Informationen zu folgenden Themen:
                                   •   “Menü Funktionen” auf Seite K-96
                                   •   “Menü Optionen” auf Seite K-97


                                   Menü Funktionen
                                   Lagerwirtschaft > Lagerbestellung > Menü Funktionen
                                   Über dieses Menü können Sie andere Dialoge öffnen, ohne die Bestellüber-
                                   gabe zu schließen. Folgende Einträge werden angezeigt:
                                   •   Lieferant/Liefertermin ändern:
                                       Öffnet den Dialog Lieferant und Liefertermin ändern.
                                        “Lieferant und Liefertermin ändern” auf Seite C-662
                                   •   Markierungsoptionen:
                                       Öffnet den Dialog Markierungsoptionen.
                                        “Markierungsoptionen” auf Seite C-663
                                   •   Lieferantenpreise:
                                       Öffnet den Dialog Preisvergleich.
                                        “Preisvergleich” auf Seite C-664
1.10 / 12-2019




                 K-96                                                           A+W Business Kistenmanagement
                 Softwarereferenz                                                                  Lagerbestellung




                                      Menü Optionen
                                      Lagerwirtschaft > Lagerbestellung > Menü Optionen
                                      Über dieses Menü können Sie die Standardeinstellung des Dialoges bestim-
                                      men. Sie können die Optionen aktivieren oder deaktivieren. Die Einstellung
                                      wird nicht zurückgesetzt, wenn Sie den Dialog schließen.

                                          Aktivierte Optionen nach dem Öffnen des Dialogs
                                          Bitte beachten Sie, dass geänderte Optionen erst beim nächsten Öffnen
                                          des Dialogs wirksam werden.
                                          Wenn durch eine aktivierte Option eine Prüfung gestartet wurde, kann sich
                                          das Öffnen eines Dokuments verzögern. Der Grad der Verzögerung hängt
                                          von der Leistungsfähigkeit des Rechners ab.
                                          Die folgenden Beschreibungen stellen die aktivierte Option dar.

                                      Gruppe Übergabe
                                      •   Auftragsbezogene Übergabe:
                                          Die Bestellungen werden pro Auftrag übergeben. Wenn diese Option nicht
                                          aktiviert ist, können Sammelbestellungen erzeugt werden.
                                      •   Bestellnummer = Auftragsnummer:
                                          Diese Option ist nur freigeschaltet, wenn die Option Auftragsbezogene
                                          Übergabe aktiviert ist.
                                      •   Bestellpool pro Mitarbeiter:
                                          Pro Mitarbeiter kann ein eigener Bestellpool angelegt werden.

                                      Gruppe Liefertermin
                                      •   Lieferterminprüfung:
                                          Der Liefertermin wird automatisch geprüft. Ändern Sie einen Liefertermin,
                                          der nicht an einem Tourentag liegt, wird eine entsprechende Meldung an-
                                          gezeigt.
                                      •   Lieferantentour berücksichtigen:
                                          Wenn die Bestellung auf einen Liefertermin fällt, der nicht an einem Tou-
                                          rentag liegt, wird eine entsprechende Meldung angezeigt. Dazu müssen
                                          die Lieferantentouren in den Stammdaten hinterlegt werden.
                                           Stammdaten, “Touren” auf Seite B-862
                                      •   Vorlauftage mit Kombiwarengruppen ermitteln:
                                          Wenn in den Kombiwarengruppen Vorlauftage hinterlegt sind, sollen diese
                                          zur Berechnung des Liefertermins herangezogen werden.
                                           Stammdaten, “Vorlauftage” auf Seite B-568
1.10 / 12-2019




                 A+W Business Kistenmanagement                                                                K-97
                 Lagerbestellung                                                               Softwarereferenz




                                   Gruppe Produktbezeichnung
                                   •   Produktbezeichnungen aus Lieferantenkartei:
                                       Die Bezeichnung der bestellten Produkte wird aus der Lieferantenkartei
                                       übernommen.
                                   •   Produktbezeichnungen aus Basisdaten (interne Best.):
                                       Für interne Bestellungen wird die Bezeichnung der bestellten Produkte aus
                                       den Produktstammdaten übernommen.

                                   Gruppe Sonstige
                                   •   Keine Kostenrückschreibung:
                                       Die Kosten werden nicht in die EK-Preise des Auftrags zurückgeschrieben.
                                   •   Maßzuschläge berücksichtigen:
                                       Bei der Bestellung sollen die Maßzuschläge mit übergeben werden.
                                   •   Druckkennzeichen für Bearbeitungen immer setzen:
                                       In der Bestellung sollen Bearbeitungen immer gedruckt werden. Wenn die
                                       Option deaktiviert ist, werden die Druckkennzeichen unverändert aus dem
                                       Auftrag in die Bestellung übernommen.
                                   •   Statistikwarengruppe aus dem Auftrag:
                                       Die Angabe zur Statistikwarengruppe wird aus dem Auftrag übernommen,
                                       wenn für Auftrag und Bestellung unterschiedliche Statistikwarengruppen
                                       definiert sind.
                                   •   Geschäftsart aus dem Auftrag:
                                       Die Geschäftsart wird aus dem Auftrag übernommen, wenn für Auftrag und
                                       Bestellung unterschiedliche Geschäftsarten definiert sind.
                                   •   AV-Bereich aus dem Auftrag:
                                       Der AV-Bereich wird aus dem Auftrag übernommen, wenn für Auftrag und
                                       Bestellung unterschiedliche AV-Bereiche definiert sind.
                                   •   Fachberater = Erfasser bei Neuanlage:
                                       In der Bestellung wird automatisch der Name des Mitarbeiters eingetragen,
                                       der sich in A+W Business angemeldet hat.
                                   •   Statusänderung erfragen:
                                       Die Abfrage zur Änderung des Status wird angezeigt.
                                   •   Wiederholte Übergabe nur bis Sperrstatus:
                                       Bestellungen können mehrfach übergeben werden, allerdings nur, bis der
                                       Sperrstatus erreicht ist.

                                   Gruppe Erweitert
                                   •   Einstellungen:
                                       Öffnet den Dialog Erweiterte Einstellungen, um Angaben zum Druck von
                                       Texten und Dateianhängen festzulegen.
1.10 / 12-2019




                 K-98                                                        A+W Business Kistenmanagement
                 Softwarereferenz                                                                         Lagerbestellung




                                          Bestellpool
                                          Lagerwirtschaft > Lagerbestellung




                 Abb. K-59   Lagerbestellung


                                          In diesem Dialog können Sie alle vorgeschlagenen Bestellungen für Artikel se-
                                          hen, deren Mindestbestand unterschritten wurde. Die Bestellmenge wird nach
                                          der Menge berechnet, die im Dialog Lagerverwaltung festgelegt ist.
                                          Mit der Übergabe werden die Bestellungen angelegt und können gedruckt und
                                          versendet werden.
                                           Tutorial, “Lagerbestellung von Kisten” auf Seite K-50
                                           Tutorial, “Manuelle und automatische Lagerbestellung” auf Seite K-42

                                          Lagerort

                                          Warenhaus, Gang, Regal, Fach Sie können die Anzeige auf einzelne La-
                                          gerorte einschränken. Bedenken Sie dabei, dass auch auf den Lagerort
                                          <k.A.> Lagerartikel gebucht sein können. Wenn Sie die Auswahl nicht ein-
                                          schränken, werden Bestellvorschläge zu allen Artikeln angezeigt, deren Min-
                                          destbestand unterschritten ist.
1.10 / 12-2019




                                          Die Bezeichnung der Lagerorte kann in den Stammdaten geändert werden.




                 A+W Business Kistenmanagement                                                                     K-99
                 Lagerbestellung                                                                    Softwarereferenz




                                   Übersicht
                                   In der Übersicht werden die Daten zu den Bestellvorschlägen angezeigt. Sie
                                   können einen anderen Lieferanten auswählen und sich einen Preisvergleich
                                   anzeigen lassen.
                                   •   Lieferant:
                                       Der Lieferant wird aus der Lieferantenkartei übernommen. Wenn kein Lie-
                                       ferant eingetragen ist oder wenn Ihnen Lieferschwierigkeiten Ihres Stan-
                                       dard-Lieferanten bekannt sind, können Sie den Namen ändern.
                                   •   Artikel/Farbe:
                                       Nummer und ggf. Variante des Produkts, das bestellt werden soll.
                                   •   Ident-Nr.:
                                       Kisten-ID (manuelle Buchung oder aus dem Wareneingang)
                                   •   Lagerort:
                                       Lagerort, an dem der Bestand des Lagerartikels unterschritten ist.
                                   •   Menge:
                                       Menge, die bestellt werden soll. Die Standard-Bestellmenge wird so oft
                                       multipliziert, bis der Mindestbestand überschritten ist. Sie können den Wert
                                       direkt in der Übersicht überschreiben.
                                   •   Breite, Höhe:
                                       Maße der Scheibe, die bestellt werden soll.
                                   •   Inhalt:
                                       Der Inhalt wird nur bei Kisten angezeigt.
                                   •   Anlief.-Lief.:
                                       Der Liefertermin des Lieferanten wird aus den Angaben in der Lieferanten-
                                       kartei errechnet. Wenn Ihnen Lieferschwierigkeiten Ihres Standard-Liefe-
                                       ranten bekannt sind, können Sie den Termin ändern.
                                    Verkauf, “Lieferant und Liefertermin ändern” auf Seite C-662
                                    Verkauf, “Preisvergleich” auf Seite C-664

                                   Position für Die Bestellvorschläge sind in unterschiedlichen Farben darge-
                                   stellt:
                                   • Rot: interner Auftrag:
                                      Interne Aufträge sind Produktionsaufträge, die erzeugt werden, um den La-
                                      gerbestand aufzufüllen. Der Vorschlag wird automatisch erzeugt, wenn in
                                      der Lieferantenkartei für das Produkt die entsprechende Option aktiviert ist.
                                   • Blau: Anfrage:
                                      Bestellanfragen an einen Lieferanten, um z. B. Preise und Liefertermine zu
                                      erfragen.
                                   • Grün: Liefertermin für Auftr./Best. gefährdet:
                                      Als Liefertermin wird automatisch das aktuelle Tagesdatum eingesetzt.
                                      Damit ist die Lieferung i. d. R. nicht termingerecht möglich. Wenn Sie das
                                      Datum ändern, wechselt die Schriftfarbe für den Eintrag zu Schwarz.

                                   Ziel-Nummernverwalter

                                   Mitarbeiter Name des Mitarbeiters, der sich in A+W Business angemeldet
1.10 / 12-2019




                                   hat oder der den Nummernverwalter eingerichtet hat. Wenn Sie einen neuen
                                   Nummernverwalter anlegen, können Sie diesen einem bestimmten Mitarbeiter
                                   zuweisen.



                 K-100                                                         A+W Business Kistenmanagement
                 Softwarereferenz                                                              Lagerbestellung




                                      Name Name des Nummernverwalters, in den die Bestellungen übergeben
                                      werden sollen. Wenn Sie einen neuen Namen eintragen, wird ein neuer Num-
                                      mernverwalter angelegt.

                                      Ziel-Nummernkreis

                                      Mandant Wenn Sie für Ihre Mandanten gesonderte Nummernkreise einge-
                                      richtet haben, können Sie den gewünschten Mandanten auswählen.

                                      AV-Bereich Wenn Sie mit AV-Bereichen arbeiten, können Sie die Bestellung
                                      einem bestimmten AV-Bereich zuordnen.
1.10 / 12-2019




                 A+W Business Kistenmanagement                                                          K-101
                 Kisten – Ein- und Ausgang                                                          Softwarereferenz




                                        Kisten – Ein- und Ausgang
                                        Vollständige Beschreibungen von Wareneingang und Warenausgang finden
                                        Sie in den Parts Fertigung und Einkauf.
                                        In diesem Kapitel finden Sie Informationen zu folgenden Themen:
                                        •    “Wareneingang (Kisten)” auf Seite K-102
                                        •    “Einstellungen (ID)” auf Seite K-113
                                        •    “Warenausgang Kisten” auf Seite K-114


                                        Wareneingang (Kisten)
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

                                              “Firmendaten” auf Seite K-18
                                        In diesem Dialog finden Sie folgende Register:
                                        •    “Wareneingang – Auswahl” auf Seite K-103
                                        •    “Wareneingang – Komplett” auf Seite K-105
                                        •    “Wareneingang – Positionsweise” auf Seite K-107
                                        •    “Wareneingang – Identnummer” auf Seite K-110
                                        •    “Wareneingang – Protokoll (Identnummern)” auf Seite K-112
1.10 / 12-2019




                 K-102                                                            A+W Business Kistenmanagement
                 Softwarereferenz                                                          Kisten – Ein- und Ausgang




                                         Wareneingang – Auswahl
                                         Dokumente > Bestellung > Wareneingang > Wareneingang > Register Aus-
                                         wahl




                 Abb. K-60   Wareneingang – Auswahl


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
1.10 / 12-2019




                 A+W Business Kistenmanagement                                                                  K-103
                 Kisten – Ein- und Ausgang                                                           Softwarereferenz




                                        •    Nach Lieferanten:
                                             Das Eingabefeld für die Lieferantennummer wird freigeschaltet. Im Regis-
                                             ter Komplett werden alle Bestellungen beim gewählten Lieferanten ange-
                                             zeigt.
                                        •    Nach Lieferscheinnummer / Lieferavis, Gesamtliefermenge:
                                             Das Eingabefeld für die Nummer des Lieferscheins oder des Lieferavis und
                                             das Feld für die Gesamtmenge werden freigeschaltet. Wurde ein Lieferavis
                                             importiert, müssen die tatsächlich gelieferten Mengen eingetragen werden.
                                        •    Nach Anliefertermin des Lieferanten:
                                             Das Eingabefeld für den Liefertermin wird freigeschaltet. Im Register Kom-
                                             plett werden alle Bestellungen angezeigt, die zum gewählten Termin ange-
                                             liefert werden sollen.
                                        •    Nach Nummernverwalter:
                                             Die Kombobox zur Auswahl des Nummernverwalters wird freigeschaltet.
                                             Im Register Komplett werden alle Bestellungen im gewählten Nummern-
                                             verwalter angezeigt.
                                        •    Nach Scanner / Dokument:
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
1.10 / 12-2019




                 K-104                                                             A+W Business Kistenmanagement
                 Softwarereferenz                                                              Kisten – Ein- und Ausgang




                                         Wareneingang – Komplett
                                         Dokumente > Bestellung > Wareneingang > Wareneingang > Register Kom-
                                         plett




                 Abb. K-61   Wareneingang – Komplett


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
1.10 / 12-2019




                 A+W Business Kistenmanagement                                                                   K-105
                 Kisten – Ein- und Ausgang                                                          Softwarereferenz




                                        Dokumente
                                        Mit den Schaltflächen können Sie alle oder einige Dokumente markieren oder
                                        die Markierung entfernen.
                                        In der Übersicht werden alle Bestellungen angezeigt, die den Suchkriterien im
                                        Register Auswahl entsprechen. Der vollständige Wareneingang wird für die
                                        Dokumente erfasst, bei denen die Checkbox komplett buchen markiert ist.
                                        •    Bestell-Nr.:
                                             Nummer der Bestellung.
                                        •    Komplett buchen:
                                             Eine Bestellung kann als komplett gebucht werden, wenn alle Positionen
                                             vollständig geliefert wurden.
                                             ☐ Der Wareneingang ist nicht vollständig. Es stehen noch Lieferungen
                                             aus.
                                             ☑ Der Wareneingang ist vollständig und die Bestellung soll als komplett
                                             verbucht werden.
                                        •    Status:
                                             Aktueller Status. Der Status wird nach der Erfassung des Wareneingangs
                                             umgesetzt.
                                        •    Lieferant:
                                             Nummer und Name des Lieferanten.
                                        •    Anlief.-Term. d. Lieferant:
                                             Anliefertermin des Lieferanten. Der Termin wird aus der Bestellung oder
                                             der AB übernommen. Wenn Sie den Wareneingang erfasst haben, wird der
                                             Termin auf das aktuelle Tagesdatum oder das von Ihnen gewählte Datum
                                             umgesetzt.
                                        •    Enthält Kisten:
                                             Anzeige der Bestellungen, in denen Kisten enthalten sind. Die Markierung
                                             der Checkbox kann nicht geändert werden.

                                        Zugehörige Aufträge
                                        In der Übersicht werden nur die referenzierten Aufträge angezeigt, die zu der
                                        ausgewählten Bestellung gehören. Wenn mehrere Bestellungen ausgewählt
                                        sind, bleibt die Liste leer.

                                        Anliefertermin bei Kunde Das Datum wird aus dem referenzierten Auftrag
                                        übernommen. Sie können es überschreiben, wenn der ursprüngliche Termin
                                        nicht eingehalten werden kann.
1.10 / 12-2019




                 K-106                                                            A+W Business Kistenmanagement
                 Softwarereferenz                                                         Kisten – Ein- und Ausgang




                                         Wareneingang – Positionsweise
                                         Dokumente > Bestellung > Wareneingang > Wareneingang Kiste > Register
                                         Positionsweise




                 Abb. K-62   Wareneingang – Positionsweise


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
1.10 / 12-2019




                 A+W Business Kistenmanagement                                                                K-107
                 Kisten – Ein- und Ausgang                                                              Softwarereferenz




                                        Über-/Unterlieferung akzeptieren Die Stückzahl der Lieferung kann sich
                                        von der Bestellung unterscheiden. Sie können die abweichenden Stückzahlen
                                        akzeptieren und damit die Lieferung für die Position als komplett erfassen.
                                        ☐ Über- oder Untermengen werden nicht akzeptiert.
                                        ☑ Die eingegebene Stückzahl wird akzeptiert und die Position wird als kom-
                                        plett gebucht. Wenn ein Lagerartikel geliefert wurde, wird der Lagerbestand
                                        der gelieferten Menge entsprechend aktualisiert. Die geänderte Menge wird in
                                        die Bestellung zurückgeschrieben.

                                        Bestätigung

                                        AB-Lieferant Nummer der Auftragsbestätigung des Lieferanten für die mar-
                                        kierte Position.

                                        AB-Liefertermin Liefertermin für die Position.

                                        Positionen
                                        In der Übersicht werden die Positionen der gewählten Bestellung angezeigt.
                                        •    Pos:
                                             Nummer der Bestellposition.
                                        •    Komplett buchen:
                                             Eine Position kann als komplett gebucht werden, wenn die gesamte Stück-
                                             zahl geliefert wurde.
                                             ☐ Der Wareneingang ist nicht vollständig.
                                             ☑ Die Position soll als komplett verbucht werden.
                                        •    Auftr.Nr.:
                                             Auftragsnummer.
                                        •    Artikel:
                                             Bezeichnung des bestellten Produkts.
                                        •    Farbe:
                                             (Farb-) Varianten, die zu dem bestellten Produkt erfasst sind.
                                        •    Breite/Höhe:
                                             Maße der bestellten Position.
                                        •    Bestellt:
                                             Stückzahl der Bestellung für diese Position.
                                        •    Avisiert:
                                             Avisierte Stückzahl der Position.
                                        •    Geliefert:
                                             Menge, die für diese Position bereits geliefert wurde. Bei Teillieferungen ist
                                             dies die Summe der Stückzahlen, die bisher zu dieser Bestellung geliefert
                                             wurden.
                                        •    Eingang:
                                             Menge, die für die markierte Position geliefert wurde.
1.10 / 12-2019




                 K-108                                                               A+W Business Kistenmanagement
                 Softwarereferenz                                                        Kisten – Ein- und Ausgang




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
                                       “Wareneingang – Komplett” auf Seite K-105
1.10 / 12-2019




                 A+W Business Kistenmanagement                                                                K-109
                 Kisten – Ein- und Ausgang                                                              Softwarereferenz




                                         Wareneingang – Identnummer
                                         Dokumente > Bestellung > Wareneingang > Wareneingang > Register Ident-
                                         nummer




                 Abb. K-63   Wareneingang – Identnummer


                                         In diesem Register werden die Positionen einer Bestellung mit Kisten ange-
                                         zeigt. Dabei wird für jede Kiste einer Bestellposition eine Unterposition (virtu-
                                         elle Positionsnummer) erzeugt, der eine Kiste mit einer eigenen Identnummer
                                         (Identifikationsnummer, ID) zugewiesen werden kann. Die Vorgabe für die ID
                                         können Sie festlegen.
                                          “Einstellungen (ID)” auf Seite K-113

                                             Voraussetzung
                                             In den Firmendaten muss die Checkbox für die Vergabe von virtuellen Po-
                                             sitionsnummern markiert sein.

                                              Stammdaten, “Virtuelle Positionsnummern verwenden” auf Seite B-943

                                         Kistendaten

                                         Lieferanten-Identnummer Die Kisten-ID, die der Lieferant für diese Position
                                         der Lieferung vergeben hat. Wenn die Nummer eingegeben ist, wird im Feld
                                         Identnummer die automatische Kisten-ID angezeigt.
1.10 / 12-2019




                 K-110                                                              A+W Business Kistenmanagement
                 Softwarereferenz                                                        Kisten – Ein- und Ausgang




                                      Identnummer Die automatische Kisten-ID wird angezeigt, sobald Sie die
                                      Lieferanten-ID eingetragen haben. Für jede Kiste einer Bestellposition wird
                                      beim Erfassen des Wareneingangs eine eigene Kisten-ID erzeugt. Wenn z. B.
                                      5 Kisten mit Float 5 à 1200 x 800 mm bestellt und geliefert wurden, werden
                                      die IDs XXXX00001, XXXX00002, …, XXXX00005 vergeben. Die Vorgabe für
                                      XXXX können Sie selbst bestimmen.
                                       “Einstellungen (ID)” auf Seite K-113

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
                                      •   Pr./ME:
                                          EK-Preis pro Mengeneinheit wie im Bereich Kistendaten eingetragen.
                                      •   Pr. Einh.:
                                          Preiseinheit für den angezeigten Preis.
1.10 / 12-2019




                 A+W Business Kistenmanagement                                                                K-111
                 Kisten – Ein- und Ausgang                                                          Softwarereferenz




                                          Wareneingang – Protokoll (Identnummern)
                                          Dokumente > Bestellung > Wareneingang > Wareneingang > Register Proto-
                                          koll (Identnummern)




                 Abb. K-64   Wareneingang – Protokoll (Identnummern)


                                          In diesem Register können Sie sich einen Überblick über die vergebenen Kis-
                                          ten-IDs verschaffen.
1.10 / 12-2019




                 K-112                                                            A+W Business Kistenmanagement
                 Softwarereferenz                                                        Kisten – Ein- und Ausgang




                                      Einstellungen (ID)
                                      Dokumente > Bestellung > Wareneingang > Wareneingang > Menü Optionen
                                      > Gruppe Identnummernvergabe > Einstellungen




                                      Abb. K-65    Einstellungen


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

                                      Vorgabe Sie können einen Text (oder Zahlen) mit max. 15 Zeichen einge-
                                      ben, der durch XXXXX ergänzt wird. XXXXX steht für die automatisch verge-
                                      bene Nummer. Der Text wird so lange beibehalten, bis Sie ihn ändern.
                                      Wenn Sie von unterschiedlichen Lieferanten Kisten beziehen und diese ge-
                                      trennt kennzeichnen möchten, müssen Sie vor dem Erfassen des Warenein-
                                      gangs die Vorgabe jeweils entsprechend anpassen.
1.10 / 12-2019




                 A+W Business Kistenmanagement                                                                  K-113
                 Kisten – Ein- und Ausgang                                                         Softwarereferenz




                                         Warenausgang Kisten
                                         Fertigung > Lieferwesen > Warenausgang Kisten > Register Identnummern




                 Abb. K-66   Warenausgang von Kisten – Kiste ausbuchen


                                         In diesem Register können Sie eine Kiste reservieren oder aus dem Lagerbe-
                                         stand ausbuchen. Sie können nur Kisten reservieren, die beim Lagereingang
                                         mit einer Kisten-ID erfasst wurden.
                                          Tutorial, “Warenausgang Kisten” auf Seite E-148
1.10 / 12-2019




                 K-114                                                              A+W Business Kistenmanagement
Kistenmanagement              K

                        Partindex




                   A+W Business
                 Partindex                                                                          Index




                 Index
                 A                                          – Reservierung K-56
                 Aufbruch einer Kiste K-88                  – Reservierung prüfen K-56
                 Auftrag                                    – virtuelle Positionsnummer K-111
                 – Dummy-Kiste zuweisen K-56                – Warenausgang K-59
                 – intern K-43                              – Wareneingang K-103
                 – Stücklisten-Kiste K-36                   Kiste als Palette K-30
                                                            Kisten-ID K-56
                                                            – Einstellungen K-113
                 B
                 Bemerkung zur Lagerbewegung K-89
                 Bestellübergabe                            L
                 – Menü Funktionen K-96                     Lager
                 – Menü Optionen K-97                       – Lagerkategorie definieren K-22
                 Bestellung                                 Lagerabgang K-84
                 – automatisch K-50                         Lagerartikel
                 – Bestellmenge nach Bestandsprüfung K-42   – in Lagerverwaltung anlegen K-26
                 – Kiste erfassen K-52                      – Lagermaß K-25
                 – Lager K-96                               – Lagerort umbuchen K-65
                 – Mindestmenge und Bestellmenge K-50       Lagerbestand
                 – Vorschlag K-50                           – Reservierung K-56
                 Blattanzahl einer Kiste K-87               Lagerbestellung
                 Blattanzahl korrigieren K-66               – Bestellpool K-96
                                                            – Kiste K-103
                                                            – Prüfung bei automatischer Bestellung K-42
                 D
                                                            Lagerbestellung nach Bestandsprüfung K-42
                 Darstellungskonventionen   K-10
                                                            Lagerbewegung K-83
                                                            – Abgang, Zugang K-84
                 E                                          – Aufbruch K-88
                 Einstellungen                              – Bemerkung K-89
                 – Kisten-ID K-113                          – Blattanzahl K-87
                                                            – Optionen (Menü) K-83
                 F                                          – Umbuchung K-86
                 Firmendaten                                Lagerbuchung
                 – Einstellungen K-18                       – Ab-/Zugang manuell buchen K-63
                 – Lagerführungsmodus aktivieren   K-20     – Anwenderstatus K-21
                                                            – Bestand manuell ändern K-62
                                                            – Erfassungsstelle K-18, K-51
                 I
                                                            – Kiste K-49
                 Identnummer
                                                            – Kiste auflösen K-67
                 – Einstellungen K-113
                                                            – Kisteninhalt korrigieren K-66
                 – Kisten-ID K-110
                                                            – Lagerort ändern K-65
                                                            Lagerführungsmodus K-12
                 K                                          – in Firmendaten aktivieren K-20
                 Kiste                                      Lagermaß
                 – aufbrechen K-67                          – in Stammdaten anlegen K-25
                 – auflösen K-88                            – Lagerartikel K-25
                 – Buchung des Inhalts korrigieren K-66
1.10 / 12-2019




                                                            – Produktverwaltung K-13
                 – im Warenausgang erfassen K-56            Lagerort
                 – Kisten-ID K-110                          – Artikel umbuchen K-65
                 – komplexer Aufbau K-30


                 A+W Business Kistenmanagement                                                     K-117
                 Index                                                                              Partindex




                 Lagerverwaltung K-73                          Status
                 – Grundgedanken K-12                          – Lagerbuchung K-20
                 – Lagerartikel K-74                           – Zuordnungen für Lagerbuchung K-21
                 – Lagerartikel anlegen K-26                   Stückliste
                 – Preise K-78                                 – Kiste in der Lagerverwaltung K-35
                 – Stücklisten-Kiste K-35                      – Kiste in der Positionserfassung K-36
                 – Zusatz K-81                                 Suche (Lagerinfo) K-90
                 Lagerwirtschaft K-71
                 – Menü-Übersicht K-11                         U
                 Lagerzugang K-84                              Umbuchung von Lagerartikeln K-86
                 – durch Produktionsauftrag K-18, K-51         Unterposition
                 Lieferantenkartei K-13                        – Wareneingang Kiste K-110
                 – interner Kunde K-43
                 – Produktionsauftrag K-43
                 Lieferung                                     V
                 – Teilmenge K-108                             Virtuelle Positionsnummer   K-111


                 M                                             W
                 Menü                                          Warenausgang
                 – Funktionen (Bestellübergabe) K-96           – Kiste ausbuchen K-56
                 – Optionen (Bestellübergabe) K-97             – Kiste der Position zuweisen K-59
                                                               Wareneingang
                                                               – ID für Kiste K-110
                 O                                             – Kiste K-103
                 Optionen                                      – Teilmenge K-108
                 – Lagerbewegung    K-83                       – Unterposition (Kisten) K-110
                                                               – vollständig K-106
                 P
                 Palette als Kiste K-30                        Z
                 Preise                                        Zusatz
                 – Lagerverwaltung K-78                        – Lagerverwaltung   K-81
                 Preislisten
                 – für EK-Berechnung K-17
                 Produkt
                 – Lagermaß anlegen K-25
                 Produktionsauftrag
                 – Lagerzugang K-18, K-51
                 – Lieferantenkartei K-43

                 R
                 Reservierung
                 – Kiste K-56
                 – prüfen K-56
                 Reservierungen    K-12

                 S
                 Stammdaten
                 – Anwenderstatus für Lagerbuchung K-21
                 – Lagerkategorie definieren K-22
1.10 / 12-2019




                 – Lagermaß anlegen K-25
                 – Preislisten für EK-Berechnung prüfen K-17



                 K-118                                                      A+W Business Kistenmanagement

