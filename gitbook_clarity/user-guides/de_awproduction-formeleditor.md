---
description: "DE AWProduction Formeleditor"
---



# DE AWProduction Formeleditor

Formeleditor              R




                          deutsch




               A+W Production
                                                                                                           Vorspann




                                        Vorspann
                                        In diesem Teil der Dokumentation finden Sie editorische Notizen.


                                        Revisionsübersicht
                                        Part
                                        Version / Datum

                                        1.00 / 01-2004           Ersterstellung

                                        1.01 / 07-2013           Layout an CI 2013 angepasst.

                                        1.02 / 01-2017           Produkt- und Firmennamen angepasst.



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
                                        © 2017, A+W Software GmbH, alle Rechte, auch des Nachdrucks, der Her-
                                        stellung von Kopien und der Übersetzung, bleiben vorbehalten.
                                        Die Dokumentation darf nur gemäß dem Lizenzvertrag ganz oder in Teilen ko-
1.02 / 01-2017




                                        piert, in einem Archivierungssystem gespeichert oder in irgendeiner anderen
                                        Form übertragen werden. Ohne die vorherige schriftliche Genehmigung der




                 A+W Production Formeleditor                                                                   R-3
                 Vorspann




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
1.02 / 01-2017




                 R-4                                                       A+W Production Formeleditor
                                                                                                                                                            Inhalt




                                        Inhalt
                                        Vorspann ................................................................................................................ R-3
                                         Revisionsübersicht .............................................................................................. R-3
                                         Editorial ............................................................................................................... R-3

                                        Funktionsprinzip                                                                                                    R-7
                                        Der Formel-Editor ................................................................................................... R-9
                                         Ziele des Formeleditors ....................................................................................... R-9
                                         Elemente des Formeleditors: Stufe I ................................................................... R-9
                                            Formel ............................................................................................................ R-10
                                            Vergleich ........................................................................................................ R-11
                                            Bedingung ...................................................................................................... R-11
                                              Verknüpfung von Elementar - Bedingungen ............................................... R-13
                                            Menge ............................................................................................................ R-14
                                            Zuweisung ...................................................................................................... R-15
                                         Elemente des Formeleditors: Stufe II ................................................................ R-15
                                            Formel ............................................................................................................ R-15
                                            Vergleich ........................................................................................................ R-16
                                            Bedingung ...................................................................................................... R-16
                                            Menge ............................................................................................................ R-18
                                            Zuweisung ...................................................................................................... R-18
                                         Elemente des Formeleditors: Stufe III ............................................................... R-19
                                            Menge ............................................................................................................ R-19
                                        Notation Formula.dll .............................................................................................. R-21
                                         Syntax ............................................................................................................... R-21
                                            ASSIGNMENT ............................................................................................... R-21
                                            FORMULA ..................................................................................................... R-21
                                            CONDITIONS ................................................................................................ R-21
                                            CONDITION (Vergleich) ................................................................................ R-21
                                            SET ................................................................................................................ R-22
                                         Funktion ............................................................................................................. R-22
                                            ASSIGNMENT ............................................................................................... R-22
                                            FORMULA ..................................................................................................... R-23
                                            CONDITIONS ................................................................................................ R-23
                                            CONDITION ................................................................................................... R-24
                                            SET ................................................................................................................ R-24
                                         Ergebnisprüfung ................................................................................................ R-25
                                        Übersicht der betroffenen Dialoge ........................................................................ R-26

                                        Bedienung                                                                                                        R-27
                                        Bedingungen für Abstellplätze .............................................................................. R-29
                                        Bedingungen für Orga-Gruppen ........................................................................... R-32
                                        Modus für Gruppenbildung ................................................................................... R-35
                                        Bedingungen für Fertigungsabschnitte ................................................................. R-37
                                        Weitere Beispiele .................................................................................................. R-40

                                        Softwarereferenz                                                                                                 R-43
                                        Formel-Editor ........................................................................................................ R-45
                                          Auswahl Bedingungen ....................................................................................... R-46
                                          Bedingungen - Erzeuger ................................................................................... R-48
1.02 / 01-2017




                                          Bedingung ......................................................................................................... R-50
                                          Name der Bedingung ........................................................................................ R-52




                 A+W Production Formeleditor                                                                                                                  R-5
                 Inhalt




                           Info .................................................................................................................... R-53
                             Invertieren ...................................................................................................... R-53
                             Übergebene Menge ....................................................................................... R-54
                           Eingabe Zahlenwert .......................................................................................... R-54
                           Auswahl Mengen ............................................................................................... R-56
                           Mengen - Erzeuger ............................................................................................ R-58
                           Name der Menge ............................................................................................... R-61
                           Info .................................................................................................................... R-62
                           Auswahl Formeln ............................................................................................... R-63
                           Formel - Editor ................................................................................................... R-65
                           Auswahl Zuweisung .......................................................................................... R-68
                           Zuweisung - Editor ............................................................................................ R-69

                          Partindex                                                                                                         R-71
1.02 / 01-2017




                 R-6                                                                                 A+W Production Formeleditor
Formeleditor                 R

                 Funktionsprinzip




               A+W Production
                 Funktionsprinzip                                                                    Der Formel-Editor




                                        Der Formel-Editor
                                        Den Formeleditor finden Sie in A+W Production in den folgenden Bereiche:
                                        •   Organisation
                                        •   Maschinenzuordnung
                                        •   Etiketten/Skizzen/Biegertexte.
                                        Den Formeleditor gibt es in verschiedenen Stufen. Je komplexer die Formel
                                        aufgebaut ist, je höher ist die Stufe.
                                        Die Dokumentation zum Formeleditor wurde deshalb wie folgt unterteilt:
                                        •   “Elemente des Formeleditors: Stufe I” auf Seite R-9
                                        •   “Elemente des Formeleditors: Stufe II” auf Seite R-15
                                        •   “Elemente des Formeleditors: Stufe III” auf Seite R-19


                                        Ziele des Formeleditors
                                        Im Bereich der Organisation ist das Ziel des Formeleditors das Erstellen von
                                        Bedingungen zur Trennung von beliebigen Eigenschaften eines Produktes auf
                                        die dafür vorgesehenen Abstellplätze.
                                        Im Bereich der MZO ist es das Ziel, Bedingungen zur Lokalisierung von Ma-
                                        schinen in Abhängigkeit der Bearbeitung und Eigenschaften eines Produktes
                                        zu erstellen.
                                        Das Ziel des Formeleditors im Bereich Etiketten ist das Erstellen von Bedin-
                                        gungen zur Auswahl des notwendigen Etikettenlayouts in Bezug auf die Pro-
                                        dukteigenschaften.


                                        Elemente des Formeleditors: Stufe I
                                        Im Formeleditor gibt es die folgenden Elemente:
                                        •   “Formel” auf Seite R-10
                                        •   “Vergleich” auf Seite R-11
                                        •   “Bedingung” auf Seite R-11
                                        •   “Menge” auf Seite R-14
                                        •   “Zuweisung” auf Seite R-15
1.02 / 01-2017




                 A+W Production Formeleditor                                                                     R-9
                 Der Formel-Editor                                                              Funktionsprinzip




                                     Formel
                                     In der einfachsten Form besteht eine Formel aus einem Ausdruck, in dem die
                                     erlaubten Eigenschaften der Objekte (Properties), Konstanten, andere For-
                                     meln sowie einige Operatoren vorkommen können. Die möglichen Operatoren
                                     sind die Grundrechenarten +, -, * und / nebst Klammern. Darüber hinaus gibt
                                     es noch die String-Operatoren:
                                     @LEFT : Syntax STRING @LEFT ANZAHL = STRING
                                     @RIGHT : Syntax STRING @RIGHT ANZAHL = STRING
                                     @MID : Syntax STRING @MID INDEX = STRING ; der Index ist 0-basiert
                                     Alle diese Operatoren dürfen nahezu beliebig gemischt werden.
                                     Die Formel wirkt genau auf ein Teil.




                                          Eingabefeld für Formel


                                       Dieser Teil wird nicht
                                             verwendet


                                     Abb. R-1     Formel-Editor


                                     Beispiele:
                                     $TEILETYP
                                     $MENGE * ($DICKE+1000)
                                     ($BEARB1TEXT @MID $TEILETYP) @RIGHT ($DICKE/1000)
1.02 / 01-2017




                 R-10                                                             A+W Production Formeleditor
                 Funktionsprinzip                                                                     Der Formel-Editor




                                        Vergleich
                                        Ein Vergleich besteht aus 1-2 Formeln und einer sogenannten Vergleichsvor-
                                        schrift. Dabei ist zu beachten, dass nur dann genau eine Formel verwendet
                                        werden darf, wenn die Vergleichsvorschrift Nur Formel 1 verwendet wird. In
                                        diesem Fall ist der Vergleich erfüllt, wenn das Ergebnis der Formel 1 eine Zahl
                                        größer Null oder ein nicht leerer String ist. Ansonsten ist der Vergleich erfüllt,
                                        wenn der Ausdruck FORMEL 1 VORSCHRIFT FORMEL 2 wahr ist.
                                        Für die Formel 2 muss für einfache Konstanten eine Formel nicht angelegt
                                        werden. In diesem Fall aktivieren Sie die Radiotaste Wert und geben die ge-
                                        wünschte Konstante dort ein.




                                        Abb. R-2     Vergleich


                                        Beispiele
                                        Formel Teiletyp = Wert 1
                                        Formel Bin Iso Nur Formel 1
                                        Formel 3fache Breite < Formel Höhe
                                        Formel Dicke = Wert 3 mm


                                        Bedingung




                                        Abb. R-3     Bedingung mit Und-Verknüpfung
1.02 / 01-2017




                                        Eine Bedingung muss erfüllt werden, damit die Zuordnung entsprechend des
                                        Formelwerkes vollzogen werden kann. Sie ist das oberste Glied innerhalb der
                                        Formelstruktur und besteht in der einfachsten Form aus einer Anzahl von Ver-
                                        gleichen. Die Anordnung der Vergleiche gibt an, wie die Ergebnisse der Ver-


                 A+W Production Formeleditor                                                                        R-11
                 Der Formel-Editor                                                                        Funktionsprinzip




                                     gleiche miteinander verknüpft werden müssen. Nebeneinander stehende
                                     Vergleiche werden durch UND verknüpft - übereinander stehende Vergleiche
                                     werden durch ODER verknüpft. Eine Bedingung ist immer dann erfüllt, wenn
                                     es möglich ist, einen horizontalen Weg von links nach rechts zu finden, der nur
                                     erfüllte Vergleiche berührt.

                                     Beispiele:


                                       Einfachste Form

                                          Bedingung        "Ist ESG"


                                                                                        "nur Formel 1"
                                                           "Teiletyp ESG"
                                            Formel                          Vergleich


                                                                            Mögliche Operationen:
                                                           "$T_ESG"         Nur Formel, gleich,
                                          Eigenschaft
                                                                            ungleich, kleiner,
                                                                            kleiner gleich, größer,
                                      Elementarbedingung                    größer gleich



                                     Abb. R-4      Schematische Darstellung einer Bedingung


                                     Die Bedingung Ist ESG ist erfüllt, wenn die Formel Teiletyp ESG mit der Eigen-
                                     schaft des DB-Feldes T_ESG aus der Pool_Teile den Wert Eins enthält (be-
                                     dingt durch die Operation Nur Formel).




                                                                              A
                                                                              B



                                                                              C



                                     A Formel
                                     B Vergleich
                                     C Elementarbedingung
                                     Abb. R-5      Bedingungen - Erzeuger
1.02 / 01-2017




                 R-12                                                                         A+W Production Formeleditor
                 Funktionsprinzip                                                                           Der Formel-Editor




                                        Beispiele:

                                        Verknüpfung von Elementar - Bedingungen



                                           Bedingung           Freie Form mit Bearbeitung



                                                 Formel        Vergleich       Wert          Formel      Vergleich

                                               Modellnummer        =            99         Bearbeitung   Nur Formel 1



                                                Property                                    Property

                                               Modell_Nr                                   Bearbeitung



                                                Formel         Vergleich       Wert

                                               Modellnummer        =            98


                                                Property
                                               Modell_Nr




                                         Oder - Verknüpfung
                                                                                         Und - Verknüpfung

                                        Abb. R-6           Schematische Darstellung einer Verknüpfung von Elementar-Bedingun-
                                                           gen
1.02 / 01-2017




                                        Abb. R-7           Verknüpfung von Elementar-Bedingungen




                 A+W Production Formeleditor                                                                            R-13
                 Der Formel-Editor                                                                                                      Funktionsprinzip




                                     Menge


                                                   Wird nicht verwendet



                                     Abb. R-8      Mengen - Erzeuger


                                     Eine Menge besteht aus der Vorschrift, wie aus dem Startteil (Stückliste) die
                                     Endmenge gebildet werden soll. Dabei dürfen die folgenden Vorschriften be-
                                     liebig miteinander kombiniert werden.
                                      Softwarereferenz, “Mengen - Erzeuger” auf Seite R-58
                                     Dabei kann Teil auch für eine Bearbeitung stehen.


                                                                                                                             Implizite Bearb.
                                                                                                                                 Isolieren
                                                                                                                              Keine Freigabe
                                                                                                  ISO
                                                                                                Freigabe
                                                                                                 Teil 0




                                                                                           Implizite Bearb.
                                                                                              Verbinden
                                                                   Gießharz                 Keine Freigabe                   Wärmeschutz
                                                                   Freigabe                                                  Keine Freigabe
                                                                 Teil 01000000                                               Teile 02000000


                                      Bedingung: Ist ESG
                                                                 Implizite Bearb.                         Implizite Bearb.
                                                                      Härten                                   Härten
                                                                  Keine Freigabe                           Keine Freigabe

                                                       ESG                                ESG
                                                    Freigabe                           Freigabe
                                                  Teil 1010000                       Teil 1020000



                                                                 Explizite Bearb.      Explizite Bearb.              Explizite Bearb.
                                                                    Säumen               Siebdruck                      Säumen
                                                                 Keine Freigabe           Freigabe                   Keine Freigabe


                                                     Float                               Float
                                                Keine Freigabe                      Keine Freigabe
                                                Teile 01010100                      Teile 01020100

                                     Abb. R-9      Schematische Darstellung einer Menge


                                     Somit ergibt sich z.B. aus der Bedingung Ist ESG und der Menge Parent alle
                                     End- und Zwischenprodukte, welche aus ein oder mehreren ESGs gefertigt
1.02 / 01-2017




                                     werden.




                 R-14                                                                                       A+W Production Formeleditor
                 Funktionsprinzip                                                                Der Formel-Editor




                                        Zuweisung
                                        In der einfachsten Form besteht eine Zuweisung aus einer Objekt-Eigenschaft
                                        (Property) und einer Formel. Das Ergebnis der Formel wird der Eigenschaft
                                        des Objektes zugewiesen.

                                        Beispiel:
                                            ZUSCHLAGSDICKE = Formel 2mm
                                            ABSTELLBREITE = Höhe


                                        Elemente des Formeleditors: Stufe II
                                        Im Formeleditor gibt es die Elemente:
                                        •   “Formel” auf Seite R-15
                                        •   “Vergleich” auf Seite R-16
                                        •   “Bedingung” auf Seite R-16
                                        •   “Menge” auf Seite R-18
                                        •   “Zuweisung” auf Seite R-18


                                        Formel
                                        Die Formel enthält nun eine Menge nebst Operationsanweisung. Ohne die
                                        Menge wirkt die Formel direkt auf zu untersuchende Objekt. Wenn eine Men-
                                        ge angegeben ist, so wird aus dem zu untersuchenden Objekt eine Menge ge-
                                        bildet, wobei das Objekt das Startobjekt der Menge ist. Die Formel wird nun
                                        für jedes Objekt der Endmenge ausgewertet und die Ergebnisse davon ge-
                                        mäß der Operation verknüpft. Enthält die Endmenge keine Objekte, so wird
                                        ein long-Wert -1 zurückgegeben.

                                        Beispiele:
                                            $DICKE ; Menge Alle Basisteile; SUMME Gesamtdicke
                                            1 ; Menge Alle Bearbeitungen ; SUMME  Anzahl aller Bearbeitungen
                                        Erlaubte Operationen sind Summe, Mittelwert, Und-Verknüpfung, Oder-Ver-
                                        knüpfung, Minimum und Maximum.




                                        Abb. R-10    Formel
1.02 / 01-2017




                 A+W Production Formeleditor                                                                  R-15
                 Der Formel-Editor                                                                 Funktionsprinzip




                                     Vergleich
                                     Üblicherweise besteht ein Vergleich aus 1-2 Formel und der Vorschrift. Alter-
                                     nativ darf ein Vergleich auch durch eine Bedingung ausgedrückt werden (dazu
                                     aktivieren Sie die Radiotaste Bedingungen). In diesem Fall ist der Vergleich
                                     erfüllt, wenn die zugewiesene Bedingung erfüllt ist. Diese Art der Verknüpfung
                                     von Bedingungen ist immer dann benutzt, wenn zwei oder mehr Bedingungen
                                     auf verschiedene Mengen angewendet werden.




                                     Abb. R-11    Vergleich


                                     Bedingung
                                     Zunächst kann eine Bedingung invertiert werden. D.h. die Bedingung ist er-
                                     füllt, falls das Resultat der Vergleiche nicht erfüllt ist und umgekehrt. Damit
                                     lässt sich einfach aus einer schon existierenden Bedingung die umgekehrte
                                     Bedingung erstellen. Die umgekehrte Bedingung enthält genau einen Ver-
                                     gleich, der die ursprüngliche Bedingung zugewiesen bekommt. Außerdem
                                     wird für die umgekehrte Bedingung die Eigenschaft invertieren ausgewählt. In
                                     der Statuszeile erscheint ein INV vor dem Namen der Bedingung.
                                     Die Vergleiche werden normaler Weise für das zu testende Objekt ausgewer-
                                     tet. Will man aber z.B. überprüfen, ob eins der Unterteile des Objekt einen be-
                                     stimmten Teiletyp/Bearbeitungstyp hat, so kann man dazu der Bedingung eine
                                     Menge zuweisen. Dann wird aus dem Objekt eine Menge gebildet, wobei das
                                     Objekt das Startobjekt der Menge ist. Dann wird die Bedingung für alle Teile
                                     der Endmenge ausgewertet. Nun muss man noch angeben wann die Bedin-
                                     gung erfüllt ist. Reicht es dazu aus, dass ein Teil der Endmenge die Bedingung
                                     erfüllt, so muss die Operation One ausgewählt werden. Ist die Bedingung da-
                                     gegen nur dann erfüllt, wenn alle Teile der Endmenge die Bedingung erfüllen,
                                     so ist die Operation All auszuwählen. Enthält die Endmenge keine Objekte, so
                                     ist die Bedingung nicht erfüllt.
1.02 / 01-2017




                 R-16                                                                A+W Production Formeleditor
                 Funktionsprinzip                                                               Der Formel-Editor




                                        Beispiele:
                                           Formel Teiletyp = Wert 125 ; Menge Alle Unterteile ; One
                                           Mit Bearbeitung vom Typ=125
                                           Formel T_ISO Nur Formel 1; Menge Kopfteil; One (oder All)
                                           Das Kopfteil ist ein ISO




                                                                             Mit Menge




                                        Abb. R-12    Bedingung
1.02 / 01-2017




                 A+W Production Formeleditor                                                               R-17
                 Der Formel-Editor                                                                     Funktionsprinzip




                                     Menge
                                     Die Mengendefinition enthält noch eine Bedingung. Dann werden aus der
                                     Endmenge alle Objekte entfernt, die diese Bedingung nicht erfüllen.

                                     Beispiel:
                                        ; Anychild ; Bedingung Bin Bearbeitung;
                                        -> Die Endmenge enthält nur die Bearbeitungen unter dem Startteil.
                                     Wenn eine Bedingung verwendet wird, so dürfen auch die beiden Vorschriften
                                     Up und Addup verwendet werden. Diese dürfen jeweils mit keiner anderen
                                     Vorschrift kombiniert werden.
                                     Unter Verwendung von Up besteht die Endmenge genau aus einem Teil. Da-
                                     bei werden vom Startteil ausgehend alle Oberteile des Startteils untersucht, ob
                                     das jeweilige Teil die Bedingung erfüllt. In der Endmenge befindet sich das
                                     letzte Teil, das die Bedingung erfüllt hat. Erfüllt ein Teil die Bedingung nicht, so
                                     wird die Iteration nach oben abgebrochen.
                                     Unter Verwendung von Addup kann die Endmenge aus mehr als einem Teil
                                     bestehen. Wie bei Up wird ebenfalls vom Startobjekt nach oben iteriert und die
                                     Iteration beendet, falls ein Teil die Bedingung nicht erfüllt. Aber die Endmenge
                                     enthält alle Teile, die die Bedingung erfüllt haben.

                                     Beispiele:
                                        ; Up ; Bedingung Bin keine Bearbeitung
                                        ; Addup ; Bedingung Bin nicht bestellt


                                     Zuweisung
                                     Auch die Zuweisung kann eine Menge enthalten. Dann wird für alle Objekte
                                     der Endmenge das jeweilige Ergebnis der Formel der jeweiligen Eigenschaft
                                     zugewiesen.

                                     Beispiel:
                                        ZUSCHLAGDICKE = Formel 2mm ; Menge Alle Zuschnittteile
1.02 / 01-2017




                 R-18                                                                   A+W Production Formeleditor
                 Funktionsprinzip                                                                     Der Formel-Editor




                                        Elemente des Formeleditors: Stufe III

                                        Menge
                                        Die Mengenbildung wird immer mit einer Startmenge aufgerufen. In den ein-
                                        fachen Fällen besteht die Startmenge aus genau einem Teil, dem Startteil. Im
                                        Dialog Mengen - Erzeuger kann man wie im Bedingungen - Erzeuger mehrere
                                        Elemente nebeneinander oder untereinander logisch anordnen. Die Elemente
                                        im Mengen - Erzeuger sind andere Mengen. Dabei wird aus übereinander ste-
                                        hende Mengen die Vereinigungsmenge gebildet und aus nebeneinander ste-
                                        henden Mengen die Schnittmenge.
                                        Zu beachten ist dabei, dass es für diese vorgelagerte Mengenbildung ein
                                        zweites Fenster gibt. Man schaltet zwischen dem ersten und dem zweiten
                                        Fenster mittels der Schaltfläche [+/-] um. Die Startmenge ergibt sich nun in-
                                        dem aus der Menge des ersten(+) Fensters alle Objekte der Menge des zwei-
                                        ten(-) Fensters entfernt.

                                        Beispiele:
                                        {Menge Oberteil oder selber ; Anychild + Self ; ; }
                                           1.Fenster (Plus): Menge Oberteil oder selber
                                           2.Fenster (Minus): leer
                                           Markiert sind Anychild und Self
                                        Damit erhält man das Oberteil und alle Unterteile des Oberteils. Sollte kein
                                        Oberteil existieren, so befindet sich in der Endmenge das Startteil und alle sei-
                                        ne Unterteile.
1.02 / 01-2017




                                        Abb. R-13    Mengen - Erzeuger




                 A+W Production Formeleditor                                                                       R-19
                 Der Formel-Editor                                                                Funktionsprinzip




                                     Damit erhält man die Endmenge mit allen Teilen, die das gleiche Oberteil ha-
                                     ben wie das Startteil.
                                     Soll die Iteration für Up oder Addup nicht beim Teil selber anfangen, sondern
                                     beim Oberteil, so bildet man zunächst aus dem Startteil die Startmenge via
                                     Menge Oberteil {;Parent;;} und verwendet diese in der gewünschten Menge
                                     mit der Vorschrift Up oder Addup.
                                     Einer Mengenbildung kann man ferner noch eine Formel zuweisen. In diesem
                                     Fall wird die Formel für alle Teile der Startmenge ausgewertet und die Ergeb-
                                     nisse gespeichert. Aus der Endmenge werden dann alle Teile entfernt, für die
                                     das Ergebnis der Formel nicht in der Ergebnismenge der Startmenge enthal-
                                     ten ist.

                                     Beispiel:
                                        ; All; ; Formel Teiletyp
                                        Damit erhält man alle Teile des Teilebaums mit dem gleichen Teiletyp wie
                                        das Startteil.
1.02 / 01-2017




                 R-20                                                              A+W Production Formeleditor
                 Funktionsprinzip                                                                 Notation Formula.dll




                                        Notation Formula.dll
                                        Syntax

                                        ASSIGNMENT
                                           Input: Object, UserSet
                                               PROPERTY = FORMULA ; SET [/USERSET]


                                        FORMULA
                                           Input: Object, UserSet
                                               [ formulaelements ; SET ; OP [/USERSET] ]
                                               OP ∈ {Summe, Mittelwert,Und,Oder, Minimum,Maximum}
                                               formulaelements = property , FORMULA ; + - * / ( ) 0..9 @LEFT
                                               @RIGHT @MID


                                        CONDITIONS
                                           Input: Object, UserSet
                                               ´ conditionelements ; SET ; OP [/N] [/USERSET] `
                                               OP ∈ {NULL,One,All}
                                               conditionelements =
                                               CONDITION(S)
                                               or
                                               (conditionelements OP conditionelements)    OP ∈ {Und,Oder}


                                        CONDITION (Vergleich)
                                           Input: Object, UserSet
                                               ´ FORMULA [OP FORMULA] ; ; `
                                               OP ∈ {=,!=,>,>=,<,<=}
1.02 / 01-2017




                 A+W Production Formeleditor                                                                    R-21
                 Notation Formula.dll                                                                 Funktionsprinzip




                                        SET
                                            Input; Set, UserSet
                                               { (setelements)[-(setelements)] ; OP ; CONDITIONS ; FORMULA [/
                                               USERSET] }
                                               Anmerkung: Der Teil ‚-(setelements)' wird nur verwendet, falls er nicht
                                               ‚empty' ist.
                                               OP ∈ {All,Master,Parent,Self;Child,Anychild,Bottom,Up,Addup}
                                               setelements =      'empty'
                                               or
                                               SET
                                               or
                                               (setelements OP setelements) OP ∈ {∩, ∪}


                                        Funktion

                                        ASSIGNMENT
                                        Der FORMULA und dem SET werden das UserSet übergeben.
                                        •   Ohne Set, ohne UserSet:
                                            Für das gegebene Object wird die FORMULA ausgewertet. Das Ergebnis
                                            der FORMULA wird der PROPERTY des Objects zugewiesen.
                                        •   Mit Set:
                                            Aus dem gegebenen Object wird mittels SET eine Menge erzeugt. Für je-
                                            des Element dieser Menge wird nun die FORMULA ausgewertet und das
                                            Ergebnis davon der PROPERTY des jeweiligen Objects zugewiesen.
                                        •   Mit UserSet:
                                            Für jedes Object im UserSet wird die FORMULA ausgewertet und das Er-
                                            gebnis davon der PROPERTY des jeweiligen Objects zugewiesen.
                                        •   Mit Set, mit UserSet:
                                            Nicht erlaubt, nicht möglich.
1.02 / 01-2017




                 R-22                                                                   A+W Production Formeleditor
                 Funktionsprinzip                                                                Notation Formula.dll




                                        FORMULA
                                        •   Dem SET und allen FORMULAs in den formulaelements werden das User-
                                            Set übergeben.
                                        •   Ohne Set, ohne UserSet:
                                            Für das gegebene Object werden alle formulaelements ausgewertet und
                                            daraus der komplette Ausdruck berechnet. Das Ergebnis wird als Multi-
                                            Value zurückgegeben.
                                        •   Mit Set:
                                            Aus dem gegebenen Object wird mittels SET eine Menge erzeugt. Für je-
                                            des Element dieser Menge werden alle formulaelements ausgewertet und
                                            daraus der komplette Ausdruck berechnet. Die Ergebnisse werden nun ge-
                                            mäß der Operation ausgewertet und das so erhaltene Gesamtergebnis als
                                            MultiValue zurückgegeben.
                                        •   Mit UserSet:
                                            Für jedes Element des UserSet werden alle formulaelements ausgewertet
                                            und daraus der komplette Ausdruck berechnet. Die Ergebnisse werden
                                            nun gemäß der Operation ausgewertet und das so erhaltene Gesamter-
                                            gebnis als MultiValue zurückgegeben.
                                        •   Mit Set, mit UserSet:
                                            nicht erlaubt, nicht möglich


                                        CONDITIONS
                                        Dem SET und allen CONDITION(S)s in den conditionelements werden das
                                        UserSet übergeben.
                                        •   Ohne Set, ohne UserSet:
                                            Für das gegebene Object werden alle conditionelements ausgewertet und
                                            daraus das komplette Ergebnis berechnet, das als BOOLEAN zurückgege-
                                            ben wird.
                                        •   Mit Set, (mit Operation != NULL):
                                            Aus dem gegebenen Object wird mittels SET eine Menge erzeugt. Für je-
                                            des Element dieser Menge werden alle conditionelements ausgewertet
                                            und daraus der komplette BOOLEAN-Ausdruck berechnet. Wenn nun die
                                            Operation = ONE ist, so gibt CONDITIONS TRUE zurück, falls für mindes-
                                            tens ein Element der komplette BOOLEAN-Ausdruck erfüllt ist, TRUE ist.
                                            Wenn aber die Operation = ALL ist, so gibt CONDITIONS TRUE zurück,
                                            falls für alle Elemente der komplette BOOLEAN-Ausdruck erfüllt ist, TRUE
                                            ist. Andernfalls wird jeweils FALSE zurückgegeben.
                                        •   Mit UserSet:
                                            Für jedes Element des UserSet werden alle conditionelements ausgewer-
                                            tet und daraus der komplette BOOLEAN-Ausdruck berechnet. Wenn nun
                                            die Operation = ONE ist, so gibt CONDITIONS TRUE zurück, falls für min-
                                            destens ein Element der komplette BOOLEAN-Ausdruck erfüllt ist, TRUE
                                            ist. Wenn aber die Operation = ALL ist, so gibt CONDITIONS TRUE zu-
                                            rück, falls für alle Elemente der komplette BOOLEAN-Ausdruck erfüllt ist,
                                            TRUE ist. Andernfalls wird jeweils FALSE zurückgegeben.
                                        •   Mit Set, mit UserSet:
1.02 / 01-2017




                                            nicht erlaubt, nicht möglich




                 A+W Production Formeleditor                                                                   R-23
                 Notation Formula.dll                                                                 Funktionsprinzip




                                        CONDITION
                                        Jeder FORMULA wird das UserSet übergeben.
                                        •   Beliebig:
                                            Für das gegebene Object werden beide FORMULAs, falls vorhanden, aus-
                                            gewertet.
                                        Sollte nur eine FORMULA vorhanden sein, so wird TRUE zurückgegeben,
                                        falls das Ergebnis der FORMULA verschieden von NULL (numerisches Resul-
                                        tat) ist oder aber für String-Resultate kein Leerstring ist. Ansonsten wird FAL-
                                        SE zurückgegeben. Sollten dagegen beide FORMULAs vorhanden sein, so
                                        werden die Ergebnisse der beiden gemäß der Operation verglichen. Sollte der
                                        Vergleich erfüllt werden, so wird TRUE zurückgegeben, ansonsten FALSE.


                                        SET
                                        Allen in den setelements enthaltenen SETs, der CONDITIONS und der FOR-
                                        MULA werden das UserSet übergeben.
                                        •   Ohne FORMULA, ohne UserSet:
                                            Für das gegebene Set werden alle setelements berechnet und daraus die
                                            vorläufige Menge A bestimmt. Für jedes Object dieser Menge A wird nun
                                            gemäß Operation eine Menge BA bestimmt und zur Menge B hinzugefügt.
                                            Aus dieser Menge B werden nun alle Objecte entfernt, die nicht die CON-
                                            DITIONS erfüllen. Als Ergebnis wird Menge B als RelatedSet zurückgege-
                                            ben.
                                        •   Mit FORMULA, ohne UserSet:
                                            Zunächst wie unter A, jedoch wird nicht Menge B zurückgegeben. Für je-
                                            des Object aus dem gegebenen Set wird die FORMULA ausgewertet. Die
                                            Ergebnisse werden in einem Array gespeichert. Danach wird für jedes Ob-
                                            ject in Menge B ebenfalls die FORMULA ausgewertet. Sollte das Ergebnis
                                            der FORMULA für ein Object aus Menge B im Array enthalten sein, so wird
                                            das jeweilige Object in Menge C eingefügt. Als Ergebnis wird Menge C als
                                            RelatedSet zurückgegeben.
                                        •   Ohne FORMULA, mit UserSet:
                                            Wie A, jedoch wird an Stelle der gegebenen Sets das UserSet zur Bildung
                                            der Menge A verwendet.
                                        •   Mit FORMULA, mit UserSet:
                                            Wie B, jedoch wird an Stelle der gegebenen Sets das UserSet zur Bildung
                                            der Menge A verwendet. Zur Bildung des Array dagegen wird weiterhin das
                                            gegebene Set verwendet.
1.02 / 01-2017




                 R-24                                                                   A+W Production Formeleditor
                 Funktionsprinzip                                                                Notation Formula.dll




                                        Beispiel:
                                        Es soll für eine Scheibe A und eine Menge an Scheiben die Gesamtmenge
                                        von allen Scheiben bestimmt werden, die die gleiche Tour wie Scheibe A ha-
                                        ben:
                                           [$MENGE ; { ; ; ; [$TOUR] /USERSET } ; SUM }
                                        Scheibe X soll nur am Abstellplatz hängen bleiben, falls es VSG ist und in der
                                        Menge aller Scheiben mindestens 150 VSGs enthalten sind:
                                           ´ (´[T_VSG;;]=[1;;];;` AND ´[$MENGE;{;;´´[T_VSG;;]==[1;;]`;;`;/USER-
                                           SET};SUM]`>=[150;;]`) ; ; `


                                        Ergebnisprüfung
                                        Um die Ergebnisse des Formelwerkes zu überprüfen, gibt es die Möglichkeit,
                                        sich die entsprechende Log-Datei anzeigen zu lassen. Um die Ergebnisprü-
                                        fung für die Feinplanung zu aktivieren, müssen Sie in A+W Production folgen-
                                        de Einstellung vornehmen:
                                        Stammdaten > Parameter > Modul Feinplanung > Specials > ViewFormula >
                                        Wert 1 eintragen

                                           Performance
                                           Die Anzeige der Berechnungen wirkt sich nachteilig auf die System-Perfor-
                                           mance aus!




                                        Abb. R-14    Log-Datei


                                        Die Log-Datei der Ergebnisprüfung finden Sie unter
                                           \<AlcimRootDir>\Log\(Name der Log-Datei der Feinplanung).LOG
1.02 / 01-2017




                 A+W Production Formeleditor                                                                    R-25
                 Übersicht der betroffenen Dialoge                                                        Funktionsprinzip




                                          Übersicht der betroffenen Di-
                                          aloge
                                          Die Übersicht zeigt Ihnen alle Dialoge, die Sie zur vollständigen Nutzung des
                                          Formeleditors benötigen. Die Verweise führen Sie in das Kapitel Softwarere-
                                          ferenz des Stammdatenbereichs. Dort finden Sie detaillierte Informationen zu
                                          den Dialogen mit ihren Feldern und Schaltflächen.

                                          Menü Stammdaten

                                          Menü-Eintrag                  Dialog/Funktion

                                          Der Formel-Editor ist nicht    “Auswahl Bedingungen” auf Seite R-46
                                          über einen Menü-Eintrag zu     “Bedingungen - Erzeuger” auf Seite R-48
                                          erreichen.                     “Bedingung” auf Seite R-50
                                          Wie Sie ihn erreichen, ist
                                                                         “Name der Bedingung” auf Seite R-52
                                          bei den jeweiligen Dialogen
                                          genau beschrieben              “Info” auf Seite R-62
                                                                         “Auswahl Formeln” auf Seite R-63
                                                                         “Formel - Editor” auf Seite R-65
                                                                         “Auswahl Zuweisung” auf Seite R-68
                                                                         “Zuweisung - Editor” auf Seite R-69

                                          Tab. R-1     Übersicht der betroffenen Dialoge
1.02 / 01-2017




                 R-26                                                                       A+W Production Formeleditor
Formeleditor               R

                     Bedienung




               A+W Production
                 Bedienung                                                              Bedingungen für Abstellplätze




                                        Bedingungen für Abstellplät-
                                        ze
                                        Hier wird Ihnen erklärt, wie Sie im Bereich Orga Bedingungen für Abstellplätze
                                        definieren, ändern oder löschen.


                                         So erstellen Sie eine Bedingung für einen Abstellplatz, die alle
                                          Scheiben mit einer Seitenlänge ab 1,20 m herausfiltert
                                        1 Öffnen Sie den Orga-Dialog über
                                           Stammdaten > Feinplanung > Orga
                                        2 Öffnen Sie das Register Produktionsreihenfolge
                                        3 Markieren Sie den Abstellplatz, für den Sie die Bedingung anlegen möch-
                                          ten
                                        4 Betätigen Sie die Schaltfläche [Neue Bedingung]. Es öffnet sich der Dialog
                                          Auswahl Bedingungen --1--
                                        5 Betätigen Sie die Schaltfläche [Neue Bedingung …]. Es öffnet sich der Di-
                                          alog Bedingungen Erzeuger
                                        6 Öffnen Sie im Menü Bedingungen den Menüpunkt Namen. Es öffnet sich
                                          der Dialog Name der Bedingung. Im Feld Neue Bezeichnung steht stan-
                                          dardmäßig Neue Bedingung. Vergeben Sie in diesem Feld einen spre-
                                          chenden Namen für die Bedingung. Beispiel: Große Scheibe. Schließen
                                          Sie den Dialog über die Schaltfläche [OK]
                                        7 Öffnen Sie im Menü Bedingungen den Menüpunkt Info. Es öffnet sich der
                                          Dialog Info. Vergeben Sie in diesem Feld eine eindeutige Beschreibung für
                                          die Bedingung. Beispiel: Dies ist eine Bedingung, die wahr ist, wenn eine
                                          Seite einer Scheibe länger als 1,20 m ist. Schließen Sie den Dialog über
                                          die Schaltfläche [OK]
                                        8 Öffnen Sie im Menü Teilbedingungen den Menüpunkt Hinzufügen (Spalte).
                                          Es erscheint eine neue Teilbedingung, die Sie konfigurieren können.
                                        9 Öffnen Sie die Kombobox (standardmäßig vorbelegt mit nur Formel 1) und
                                          wählen Sie >= (größer gleich)
                                        10 Aktivieren Sie die Radiotaste Wert. Es öffnet sich automatisch der Dialog
                                           Eingabe Zahlenwert. Da der neue Abstellplatz nur Scheiben über 1,20 auf-
                                           nehmen soll, aktivieren wir die Radiotaste Länge und geben im Bereich
                                           Neuer Wert 1200 mm ein. Schließen Sie den Dialog über die Schaltfläche
                                           [OK]. Der Wert erscheint dann im unteren Feld der Bedingung
                                        11 Klicken Sie jetzt in das obere Eingabefeld der Bedingung. Es öffnet sich au-
                                           tomatisch der Dialog Auswahl Formeln --1--. Hier wird definiert, auf was si-
                                           cher der im 2. Eingabefeld eingetragene Wert beziehen soll
                                        12 Betätigen Sie die Schaltfläche [Neue Formel …]. Es öffnet sich der Dialog
1.02 / 01-2017




                                           Formel-Editor. Im oberen linken Eingabefeld erfassen Sie einen möglichst
                                           sprechenden Namen für die Formel. Beispiel: Großes Maß.
                                            Softwarereferenz, “Eingabefeld oben” auf Seite R-66


                 A+W Production Formeleditor                                                                     R-29
                 Bedingungen für Abstellplätze                                                              Bedienung




                                         13 Aus dem Bereich Vorhandene Eigenschaften wählen Sie mit einem Dop-
                                            pelklick Gross Mass
                                             Softwarereferenz, “Vorhandene Eigenschaften” auf Seite R-67
                                         14 Schließen Sie den Dialog über die Schaltfläche [OK]. Sie befinden sich
                                            wieder im Dialog Bedingungen-Erzeuger.
                                            Die erstellte Bedingung sieht wie folgt aus:




                                            Abb. R-15    Bedingung: Abstellplatz für Scheiben >= 1200 mm


                                            Schließen Sie den Dialog entweder über das Menü Bedingungen > OK
                                            oder durch einen Klick auf   .
                                            Sie befinden sich wieder im Dialog Auswahl-Bedingungen --1--. Die erstell-
                                            te Bedingung Große Scheibe steht am Ende der Liste Vorhandene Bedin-
                                            gungen.


                                          So weisen Sie einem Abstellplatz eine Bedingung zu
                                         1 Öffnen Sie den Orga-Dialog über
                                            Stammdaten > Feinplanung > Orga
                                         2 Öffnen Sie das Register Produktionsreihenfolge
                                         3 Markieren Sie den Abstellplatz, dem Sie die Bedingung zuweisen möchten
                                         4 Betätigen Sie die Schaltfläche [Neue Bedingung]. Es öffnet sich der Dialog
                                           Auswahl Bedingungen --1--
                                         5 Aus der Liste der Vorhandenen Bedingungen markieren Sie die Bedin-
                                           gung, die dem Abstellplatz zugewiesen werden soll
                                         6 Verlassen Sie den Dialog über die Schaltfläche [OK]
                                         7 Die Bedingung wurde dem im Register Produktionsreihenfolge markierten
                                           Abstellplatz angehängt


                                          So löschen Sie eine dem Abstellplatz zugewiesene Bedingung
                                         1 Öffnen Sie den Orga-Dialog über
                                            Stammdaten > Feinplanung > Orga
                                         2 Öffnen Sie das Register Produktionsreihenfolge
1.02 / 01-2017




                                         3 Öffnen Sie den entsprechenden Abstellplatz durch eine Doppelklick
                                         4 Markieren Sie die Bedingung des Abstellplatzes, die gelöscht werden soll


                 R-30                                                                      A+W Production Formeleditor
                 Bedienung                                                            Bedingungen für Abstellplätze




                                        5 Betätigen Sie die Schaltfläche [Löschen]. Die Bedingung wird sofort ge-
                                          löscht

                                           Löschen
                                           Das Löschen erfolgt ohne Sicherheitsabfrage. Sollten Sie versehentlich et-
                                           was gelöscht haben, verlassen Sie das Register Produktionsreihenfolge
                                           über die Schaltfläche [Abbrechen]. Sie werden gefragt, ob die Änderungen
                                           ignoriert werden sollen. Diese Frage beantworten Sie mit [OK]. Der Orga-
                                           Dialog wird geschlossen. Wenn Sie ihn das nächste Mal öffnen, sind die
                                           Daten wieder vorhanden.
1.02 / 01-2017




                 A+W Production Formeleditor                                                                   R-31
                 Bedingungen für Orga-Gruppen                                                            Bedienung




                                       Bedingungen für Orga-Grup-
                                       pen
                                       Hier wird Ihnen erklärt, wie Sie im Bereich Orga Bedingungen für Orga-Grup-
                                       pen definieren, ändern oder löschen.


                                        So erstellen Sie eine Bedingung für eine Orga-Gruppe, die ISO mit
                                         Sprossen für einen zweiten Fertigungsabschnitt herausfiltert
                                       1 Öffnen Sie den Orga-Dialog über
                                          Stammdaten > Feinplanung > Orga
                                       2 Öffnen Sie das Register Produktionsreihenfolge
                                       3 Markieren Sie den Orga-Gruppe, für den Sie die Bedingung anlegen möch-
                                         ten
                                       4 Betätigen Sie die Schaltfläche [Neue Bedingung]. Es öffnet sich der Dialog
                                         Auswahl Bedingungen --1--
                                        Softwarereferenz, “Auswahl Bedingungen” auf Seite R-46
                                       5 Betätigen Sie die Schaltfläche [Neue Bedingung …]. Es öffnet sich der Di-
                                         alog Bedingungen Erzeuger
                                           Softwarereferenz, “Bedingungen - Erzeuger” auf Seite R-48
                                       6 Öffnen Sie im Menü Bedingungen den Menüpunkt Namen. Es öffnet sich
                                         der Dialog Name der Bedingung. Im Feld Neue Bezeichnung steht stan-
                                         dardmäßig Neue Bedingung. Vergeben Sie in diesem Feld einen spre-
                                         chenden Namen für die Bedingung. In unserem Beispiel: ISO Sprossen.
                                         Schließen Sie den Dialog über die Schaltfläche [OK]
                                           Softwarereferenz, “Name der Bedingung” auf Seite R-52
                                       7 Öffnen Sie im Menü Bedingungen den Menüpunkt Info. Es öffnet sich der
                                         Dialog Info. Vergeben Sie in diesem Feld eine eindeutige Beschreibung für
                                         die Bedingung. In unserem Beispiel: Position wurde dem Fertigungsab-
                                         schnitt 2 zugeordnet MZO_ROUTE_MAP.ROUTE =2. Schließen Sie den
                                         Dialog über die Schaltfläche [OK]
                                           Softwarereferenz, “Info” auf Seite R-53
                                       8 Öffnen Sie im Menü Teilbedingungen den Menüpunkt Hinzufügen (Spalte).
                                         Es erscheint eine neue Teilbedingung, die Sie konfigurieren können.
                                       9 Öffnen Sie die Kombobox (standardmäßig vorbelegt mit nur Formel 1) und
                                         wählen Sie == (gleich)
                                       10 Aktivieren Sie die Radiotaste Wert. Es öffnet sich automatisch der Dialog
                                          Eingabe Zahlenwert. Da das ISO Sprossen ausschließlich auf dem Ferti-
                                          gungsabschnitt 2 produziert wird, aktivieren wir die Radiotaste Ziffer und
                                          geben im Bereich Neuer Wert 2 ein. Schließen Sie den Dialog über die
1.02 / 01-2017




                                          Schaltfläche [OK]. Der Wert erscheint dann im unteren Feld der Bedingung
                                           Softwarereferenz, “Eingabe Zahlenwert” auf Seite R-54




                 R-32                                                                  A+W Production Formeleditor
                 Bedienung                                                             Bedingungen für Orga-Gruppen




                                        11 Klicken Sie jetzt in das obere Eingabefeld der Bedingung. Es öffnet sich au-
                                           tomatisch der Dialog Auswahl Formeln --1--. Hier wird definiert, auf was si-
                                           cher der im 2. Eingabefeld eingetragene Wert beziehen soll
                                            Softwarereferenz, “Auswahl Formeln” auf Seite R-63
                                        12 Betätigen Sie die Schaltfläche [Neue Formel …]. Es öffnet sich der Dialog
                                           Formel-Editor. Im oberen linken Eingabefeld erfassen Sie einen möglichst
                                           sprechenden Namen für die Formel. In unserem Beispiel: Fertigungsab-
                                           schnitt.
                                            Softwarereferenz, “Eingabefeld oben” auf Seite R-66
                                        13 Aus dem Bereich Vorhandene Eigenschaften wählen Sie mit einem Dop-
                                           pelklick Route. Im Bereich Formel erscheint $Route
                                            Softwarereferenz, “Vorhandene Eigenschaften” auf Seite R-67
                                        14 Schließen Sie den Dialog über die Schaltfläche [OK]. Sie befinden sich
                                           wieder im Dialog Bedingungen-Erzeuger.
                                           Die erstellte Bedingung sieht wie folgt aus:




                                           Abb. R-16    Bedingung: Fertigungsabschnitt = 2


                                           Schließen Sie den Dialog entweder über das Menü Bedingungen > OK
                                           oder durch einen Klick auf   .
                                           Sie befinden sich wieder im Dialog Auswahl-Bedingungen --1--. Die erstell-
                                           te Bedingung ISO Sprossen steht am Ende der Liste Vorhandene Bedin-
                                           gungen.
                                        15 Markieren Sie die Bedingung und betätigen Sie die Schaltfläche [Ok]. Die
                                           Bedingung wird der zuvor markierten Orga-Gruppe angehängt.
1.02 / 01-2017




                 A+W Production Formeleditor                                                                     R-33
                 Bedingungen für Orga-Gruppen                                                            Bedienung




                                        So weisen Sie einer Orga-Gruppe eine vorhandene Bedingung zu
                                       1 Öffnen Sie den Orga-Dialog über
                                          Stammdaten > Feinplanung > Orga
                                       2 Öffnen Sie das Register Produktionsreihenfolge
                                       3 Markieren Sie die Orga-Gruppe, der Sie die Bedingung zuweisen möchten
                                       4 Betätigen Sie die Schaltfläche [Neue Bedingung]. Es öffnet sich der Dialog
                                         Auswahl Bedingungen --1--
                                       5 Aus der Liste der Vorhandenen Bedingungen markieren Sie die Bedin-
                                         gung, die der Orga-Gruppe zugewiesen werden soll
                                       6 Verlassen Sie den Dialog über die Schaltfläche [OK]
                                       7 Die Bedingung wurde der im Register Produktionsreihenfolge markierten
                                         Orga-Gruppe angehängt


                                        So löschen Sie eine der Orga-Gruppe zugewiesene Bedingung
                                       1 Öffnen Sie den Orga-Dialog über
                                          Stammdaten > Feinplanung > Orga
                                       2 Öffnen Sie das Register Produktionsreihenfolge
                                       3 Öffnen Sie die entsprechenden Orga-Gruppe durch eine Doppelklick
                                       4 Markieren Sie die Bedingung der Orga-Gruppe, die gelöscht werden soll
                                       5 Betätigen Sie die Schaltfläche [Löschen]. Die Bedingung wird sofort ge-
                                         löscht

                                          Löschen
                                          Das Löschen erfolgt ohne Sicherheitsabfrage. Sollten Sie versehentlich et-
                                          was gelöscht haben, verlassen Sie das Register Produktionsreihenfolge
                                          über die Schaltfläche [Abbrechen]. Sie werden gefragt, ob die Änderungen
                                          ignoriert werden sollen. Diese Frage beantworten Sie mit [OK]. Der Orga-
                                          Dialog wird geschlossen. Wenn Sie ihn das nächste Mal öffnen, sind die
                                          Daten wieder vorhanden.
1.02 / 01-2017




                 R-34                                                                A+W Production Formeleditor
                 Bedienung                                                                Modus für Gruppenbildung




                                        Modus für Gruppenbildung
                                        Dieses Beispiel dient dazu, den Orga-Gruppen und den Abstellplätzen einen
                                        weiteren wählbaren Modus zur Gruppenbildung hinzuzufügen.


                                         So erstellen Sie eine Gruppierung nach Anzahl der Scheiben pro
                                          Kunde, d.h. es wird eine Gruppe pro Kunde erstellt und diese
                                          Gruppen nach der Zahl der in ihnen enthaltenen Scheiben sortiert.
                                          Zuerst produziert wird dann die Gruppe mit der größten Anzahl an
                                          Scheiben
                                        1 Öffnen Sie den Gruppierung/Sortierung-Dialog über
                                           Stammdaten > Feinplanung > Editor-Gruppierungen
                                        2 Betätigen Sie die Schaltfläche [Formeln …]. Es öffnet sich der Dialog Aus-
                                          wahl Formeln --1--
                                        3 Betätigen Sie die Schaltfläche [Neue Formel …]. Es öffnet sich der Dialog
                                          Formel-Editor
                                        4 Im linken oberen Eingabefeld erfassen Sie den Namen für die Formel der
                                          Gruppierung. In unserem Beispiel Menge der Scheiben pro Kunde
                                        5 Im Bereich Vorhandene Eigenschaften wählen Sie Menge mit einem Dop-
                                          pelklick aus. Im Bereich Formel erscheint $MENGE
                                        6 Betätigen Sie die Schaltfläche [Menge …]. Es öffnet sich der Dialog Aus-
                                          wahl Menge --1--
                                        7 Betätigen Sie die Schaltfläche [Neue Menge …], um eine neue Menge an-
                                          zulegen. Es öffnet sich der Dialog Mengen-Erzeuger. Wir beginnen die
                                          Mengen-Erzeugung mit einer gegebenen Menge und bekommen nach den
                                          Mengenoperationen, die wir hier durchführen, unsere gewünschte endgül-
                                          tige Menge. An den Formelinterpreter wird von der Feinplanung an Werten
                                          übergeben eine Position eines bestimmten Kunden, die Mengenkalkulati-
                                          on der Feinplanung und als weiteren Parameter alle Aufträge des aktuellen
                                          Laufs. Von uns muss nur noch die Kundennummer hinzugefügt werden.
                                        8 Öffnen Sie im Menü Menge den Menüpunkt Namen und geben einen neu-
                                          en, möglichst sprechenden Namen für die Menge ein. In unserem Beispiel
                                          Mengen Scheiben pro Kunde. Verlassen Sie den Dialog mit der Schalt-
                                          fläche [Ok]
                                        9 Aktivieren Sie im Menü Menge den Menüpunkt Übergebene Menge. Dies
                                          bewirkt, dass bei der Bildung der Menge nicht nur die Position, mit der wir
                                          in den Mengen-Erzeuger gekommen sind, selbst berücksichtigt wird, son-
                                          dern alle Positionen des Laufs
                                        10 Da die gewünschte Menge nicht alle Teile enthalten soll, sondern nur die
                                           Freigabeteile, aktivieren Sie in der im Dialog Mengen-Erzeuger die Check-
                                           box Master.
1.02 / 01-2017




                 A+W Production Formeleditor                                                                   R-35
                 Modus für Gruppenbildung                                                                 Bedienung




                                       11 Um unserer Menge die Kundennummer als Eigenschaft hinzuzufügen,
                                          wählen Sie im Menü Menge de Menüpunkt Formel aus. Es öffnet sich der
                                          Dialog Auswahl Formeln --2--. Betätigen Sie die Schaltfläche [Neue
                                          Formel …], um die Formel für die Kundennummer anzulegen. Es öffnet
                                          sich der Dialog Formel Editor.
                                       12 Geben Sie im oberen linken Eingabefeld den Namen für die Formel ein. In
                                          unserem Beispiel Kundennummer
                                       13 Wählen Sie im Bereich Vorhandene Eigenschaften die Kundennummer mit
                                          einem Doppelklick aus. Im Bereich Formel erscheint $Kundennummer.
                                       14 Betätigen Sie die Schaltfläche [Ok]. Sie kehren zurück in den Dialog Aus-
                                          wahl Formeln --2--. Die Liste enthält nun als letzten Eintrag die soeben an-
                                          gelegte Formel für die Kundennummer. Markieren Sie die Kundennummer
                                          in der Liste und betätigen Sie die Schaltfläche [Ok]. Sie kehren zurück in
                                          den Dialog Mengen-Erzeuger.
                                       15 In der Statuszeile des Mengen-Erzeuger können Sie auf der rechten Seite
                                          sehen, ob und wenn ja, welche Formel bei der Bildung der neuen Menge
                                          benutzt wird. In unserem Beispiel steht dort: Formel: Kundennummer
                                       16 Schließen Sie nun alle geöffneten Dialog mit der Schaltfläche [Ok], bis Sie
                                          wieder im Dialog Gruppierung/Sortierung angekommen sind
                                       17 Die Formel Menge der Scheiben pro Kunde ist jetzt in der Liste der Formeln
                                          enthalten. Markieren Sie die Formel und betätigen Sie die Schaltfläche
                                          [Hinzufügen]. Die Formel wird den Gruppierungen im Register Editor-Grup-
                                          pierung hinzugefügt. Sie steht Ihnen dann in den Einstellungen für die
                                          Orga-Gruppen und den Abstellplätzen jeweils im Bereich Bildung der
                                          Gruppen zur Verfügung.
1.02 / 01-2017




                 R-36                                                                 A+W Production Formeleditor
                 Bedienung                                                      Bedingungen für Fertigungsabschnitte




                                        Bedingungen für Fertigungs-
                                        abschnitte
                                        Hier wird Ihnen erklärt, wie Sie im Bereich MZO Bedingungen für Fertigungs-
                                        abschnitte definieren, ändern oder löschen.


                                         So erstellen Sie eine Bedingung für einen Fertigungsabschnitt, der
                                          alle Scheiben mit Sprossen herausfiltert
                                        1 Öffnen Sie den Dialog Fertigungsabschnitte über
                                           Stammdaten > MZO > Konfiguration
                                        2 Markieren Sie den Fertigungsabschnitt, für den Sie die Bedingung anlegen
                                          möchten
                                        3 Betätigen Sie die rechte Maustaste. Es öffnet sich das Kontext-Menü. Aus
                                          dem Kontext-Menü wählen Sie
                                           Bedingung des Fertigungsabschnitts > Neu
                                        4 Es öffnet sich der Dialog Auswahl Bedingungen --1--
                                        5 Betätigen Sie die Schaltfläche [Neue Bedingung …]. Es öffnet sich der Di-
                                          alog Bedingungen Erzeuger
                                        6 Öffnen Sie im Menü Bedingungen den Menüpunkt Namen. Es öffnet sich
                                          der Dialog Name der Bedingung. Im Feld Neue Bezeichnung steht stan-
                                          dardmäßig Neue Bedingung. Vergeben Sie in diesem Feld einen spre-
                                          chenden Namen für die Bedingung. In unserem Beispiel: Bin Sprossen-
                                          ISO. Schließen Sie den Dialog über die Schaltfläche [OK]
                                        7 Öffnen Sie im Menü Bedingungen den Menüpunkt Info. Es öffnet sich der
                                          Dialog Info. Vergeben Sie in diesem Feld eine eindeutige Beschreibung für
                                          die Bedingung. Beispiel: Diese Bedingung ist wahr, wenn die Position ein
                                          Sprossenflag hat. Schließen Sie den Dialog über die Schaltfläche [OK]
                                        8 Öffnen Sie im Menü Teilbedingungen den Menüpunkt Hinzufügen (Spalte).
                                          Es erscheint eine neue Teilbedingung, die Sie konfigurieren können.
                                        9 Die Kombobox ist standardmäßig vorbelegt mit nur Formel 1. Das bleibt in
                                          unserem Beispiel unverändert
                                        10 Die Radiotaste Normal ist standardmäßig aktiv. Es öffnet sich automatisch
                                           der Dialog Eingabe Zahlenwert. Das bleibt in unserem Beispiel ebenfalls
                                           unverändert
                                        11 Klicken Sie jetzt in das obere Eingabefeld der Bedingung. Es öffnet sich au-
                                           tomatisch der Dialog Auswahl Formeln --1--
                                        12 Betätigen Sie die Schaltfläche [Neue Formel …]. Es öffnet sich der Dialog
                                           Formel-Editor. Im oberen linken Eingabefeld erfassen Sie einen möglichst
                                           sprechenden Namen für die Formel. In unserem Beispiel: Sprossen
1.02 / 01-2017




                                            Softwarereferenz, “Eingabefeld oben” auf Seite R-66




                 A+W Production Formeleditor                                                                     R-37
                 Bedingungen für Fertigungsabschnitte                                                       Bedienung




                                         13 Aus dem Bereich Vorhandene Eigenschaften wählen Sie mit einem Dop-
                                            pelklick Pos_Sprossen_Flag. Im Bereich Formel erscheint
                                            $Pos_Sprossen_Flag
                                             Softwarereferenz, “Vorhandene Eigenschaften” auf Seite R-67
                                         14 Schließen Sie den Dialog über die Schaltfläche [OK]. Sie befinden sich im
                                            Dialog Auswahl Formeln --1--. Die soeben angelegte Formel ist bereits
                                            markiert.
                                         15 Schließen Sie den Dialog über die Schaltfläche [OK]. Sie befinden sich
                                            wieder im Dialog Bedingungen-Erzeuger.
                                            Die erstellte Bedingung sieht wie folgt aus:




                                            Abb. R-17    Bedingung: Bin ISO mit Sprosse


                                            Schließen Sie den Dialog entweder über das Menü Bedingungen > OK
                                            oder durch einen Klick auf   .
                                            Sie befinden sich wieder im Dialog Auswahl-Bedingungen --1--. Die erstell-
                                            te Bedingung Bin Sprossen ISO steht am Ende der Liste Vorhandene Be-
                                            dingungen.


                                          So weisen Sie einem Fertigungsabschnitt eine vorhandene
                                           Bedingung zu
                                         1 Öffnen Sie den Dialog Fertigungsabschnitt über
                                            Stammdaten > MZO > Konfiguration
                                         2 Markieren Sie den Fertigungsabschnitt, dem Sie die Bedingung zuweisen
                                           möchten
                                         3 Betätigen Sie die rechte Maustaste. Es öffnet sich das Kontext-Menü. Aus
                                           dem Kontext-Menü wählen Sie
                                            Bedingung des Fertigungsabschnitts > Neu
                                         4 Es öffnet sich der Dialog Auswahl Bedingungen --1--
                                         5 Aus der Liste der Vorhandenen Bedingungen markieren Sie die Bedin-
                                           gung, die dem Fertigungsabschnitt zugewiesen werden soll
                                         6 Verlassen Sie den Dialog über die Schaltfläche [OK]
                                         7 Die Bedingung wurde dem markierten Fertigungsabschnitt angehängt.
1.02 / 01-2017




                 R-38                                                                      A+W Production Formeleditor
                 Bedienung                                                    Bedingungen für Fertigungsabschnitte




                                         So löschen Sie eine dem Fertigungsabschnitt zugewiesene
                                          Bedingung
                                        1 Öffnen Sie den Dialog Fertigungsabschnitt über
                                           Stammdaten > MZO > Konfiguration
                                        2 Öffnen Sie den entsprechenden Fertigungsabschnitt durch einen Doppel-
                                          klick
                                        3 Markieren Sie die Bedingung des Fertigungsabschnitts, die gelöscht wer-
                                          den
                                        4 Betätigen Sie die rechte Maustaste. Es öffnet sich das Kontext-Menü. Aus
                                          dem Kontext-Menü wählen Sie Bedingung löschen
                                           Die Bedingung wird sofort gelöscht!

                                           Löschen
                                           Das Löschen erfolgt ohne Sicherheitsabfrage. Sollten Sie versehentlich et-
                                           was gelöscht haben, verlassen Sie den Dialog Fertigungsabschnitte über
                                           die Schaltfläche [Abbrechen]. Wenn Sie ihn das nächste Mal öffnen, sind
                                           die Daten wieder vorhanden.
1.02 / 01-2017




                 A+W Production Formeleditor                                                                   R-39
                 Weitere Beispiele                                                                Bedienung




                                     Weitere Beispiele
                                      So erstellen Sie eine Bedingung für ESG im ISO oder mit
                                       Bearbeitungen am Float
                                     1 Erster Schritt




                                        Abb. R-18   Erster Schritt


                                        Dabei wird in Formel Bin ESG einfach die Eigenschaft T_ESG zurückge-
                                        geben
                                     2 Nun die Überprüfung, ob das Teil im ISO eingebaut wird




                                        Abb. R-19   Prüfen
1.02 / 01-2017




                 R-40                                                            A+W Production Formeleditor
                 Bedienung                                                                          Weitere Beispiele




                                        3 Da ein Teil nicht gleichzeitig ESG und ISO sein kann, wird die in Schritt 2
                                          gezeigte Bedingung so nicht funktionieren. Daher …




                                           Abb. R-20    Abbildung


                                        4 Jetzt noch die Oder-Verknüpfung, ob eins der Unterteile eine Bearbeitung
                                          ist. Dazu wird eine weitere Bedingung erzeugt, die für alle Unterteile die
                                          Formel Bin Bearbeitung prüft.




                                           Abb. R-21    Bedingung
1.02 / 01-2017




                 A+W Production Formeleditor                                                                    R-41
                 Weitere Beispiele                                                                    Bedienung




                                      Die Bearbeitungen direkt unter mir
                                     1 Die Endmenge soll nur die Bearbeitungen unter dem Startteil enthalten, die
                                       nach den letzten erzeugenden Bearbeitungen unter dem Startteil erfolgen.
                                     2 Dazu wird zunächst die Menge aller Unterteile gebildet, die keine Bearbei-
                                       tungen sind.
                                     3 Menge Erzeugende Bearbeitungen unter mir = { ; ANYCHILD ; Bedin-
                                       gung Ist keine Bearbeitung ; }
                                     4 Mit Hilfe dieser Menge wird nun die Menge aller Teile und Bearbeitungen
                                       unterhalb des Startteils erzeugt, die man nicht haben will.
                                     5 Menge Unerwünschte Teile/Bearbeitungen unter mir = { Menge Erzeu-
                                       gende Bearbeitungen unter mir ; ANYCHILD+SELF ; ; }
                                     6 Die gewünschte Menge ergibt sich dann aus der Menge Alle Unterteile
                                       und der Menge Unerwünschte Teile/Bearbeitungen unter mir.
                                           { Menge Alle Unterteile - Menge Unerwünschte Teile/Bearbeitungen
                                           unter mir ; SELF ; ; }
1.02 / 01-2017




                 R-42                                                              A+W Production Formeleditor
Formeleditor                  R

                 Softwarereferenz




               A+W Production
                 Softwarereferenz                                                                    Formel-Editor




                                        Formel-Editor
                                        Der Formel-Editor kommt in A+W Production in den folgenden Bereichen zum
                                        Einsatz:
                                        •   Organisation
                                        •   Maschinenzuordnung
                                        •   Etiketten, Skizzen, Biegertexte
                                        Der Weg, wie einzelne Dialoge aufgerufen werden, ist bei den nachfolgenden
                                        Dialogbeschreibungen nochmals angegeben. Bestehen mehrere alternative
                                        Wege einen Dialog aufzurufen, so sind diese ebenfalls angegeben.
1.02 / 01-2017




                 A+W Production Formeleditor                                                                 R-45
                 Formel-Editor                                                             Softwarereferenz




                                 Auswahl Bedingungen
                                 Aufruf über

                                 Organisation
                                 Stammdaten > Feinplanung > Orga > Register Produktionsreihenfolge >
                                 Orga-Gruppe markieren > [Neue Bedingung]
                                 Stammdaten > Feinplanung > Orga > Register Produktionsreihenfolge > Ab-
                                 stellplatz markieren > [Neue Bedingung]

                                 Maschinenzuordnung
                                 Stammdaten > MZO > Konfiguration > Fertigungsabschnitt markieren > rechte
                                 Maustaste > Bedingung des Fertigungsabschnitts > Neu
                                 Stammdaten > MZO > Konfiguration > Bedingung des Fertigungsabschnitts
                                 markieren > rechte Maustaste > Bedingung editieren
                                 Stammdaten > MZO > Konfiguration > [Technologie] > [Neu] > [Neu]
                                 Stammdaten > MZO > Konfiguration > [Technologie] > [Ändern] > [Neu]/[Edi-
                                 tieren]

                                 Etiketten, Skizzen, Biegertexte
                                 Stammdaten > Etiketten / Skizzen / Biegertexte > Konfiguration … > Bedin-
                                 gung markieren > [Formel Editor]




                                 Abb. R-22   Auswahl Bedingungen --1--


                                 In diesem Dialog können für die Bereiche Organisation, Maschinenzuordnung
                                 und Etiketten, Skizzen, Biegertexte vorhandene Bedingungen ausgewählt,
                                 geändert oder neue Bedingungen angelegt werden.
1.02 / 01-2017




                 R-46                                                         A+W Production Formeleditor
                 Softwarereferenz                                                                           Formel-Editor




                                        Erläuterung der Felder

                                        Vorhandene Bedingungen Die Tabelle listet alle im System vorhandenen
                                        Bedingungen für die Bereiche Organisation, Maschinenzuordnung und Etiket-
                                        ten, Skizzen, Biegertexte. Die Inhalte sind für die jeweiligen Bereiche unter-
                                        schiedlich!

                                        Keine Bedingung Ist diese Checkbox aktiv, so liefert der Dialog als Ergeb-
                                        nis, dass Nichts als selektiert gilt.

                                        Beschreibung Das Feld enthält eine detaillierte Erläuterung zu der Bedin-
                                        gung. Dabei handelt es sich um den Text, den Sie im Feld Info erfassen.
                                         Softwarereferenz, “Info” auf Seite R-53

                                        Erläuterung der Schaltflächen

                                        Löschen Betätigen Sie diese Schaltfläche, wird die zuvor markierte Bedin-
                                        gung gelöscht. Die Löschung erfolgt in diesem Dialog ohne Sicherheitsabfra-
                                        ge. Sollten Sie jedoch versehentlich etwas gelöscht haben, kehren Sie in den
                                        ursprünglichen Dialog (Orga-Dialog, Etikettenart-Dialog, Skizzenart-Dialog,
                                        Biegertextart-Dialog, MZO-Dialog) zurück. Wenn Sie diesen dann über
                                        [Abbrechen] schließen, werden Sie gefragt, ob die durchgeführten Änderun-
                                        gen ignoriert werden sollen oder nicht.

                                        Neue Bedingung Betätigen Sie diese Schaltfläche, öffnet sich der Dialog
                                        Bedingungen - Erzeuger. Sie können dann eine neue Bedingung anlegen.
                                         Softwarereferenz, “Bedingungen - Erzeuger” auf Seite R-48

                                        Editieren Betätigen Sie diese Schaltfläche, öffnet sich für die markierte Be-
                                        dingung der Dialog Bedingungen - Erzeuger.
                                         Softwarereferenz, “Bedingungen - Erzeuger” auf Seite R-48


                                        Weitere Informationen zu Bedingungen
                                         Funktionsprinzip, “Elemente des Formeleditors: Stufe I” auf Seite R-9
                                         Funktionsprinzip, “Elemente des Formeleditors: Stufe II” auf Seite R-15
1.02 / 01-2017




                 A+W Production Formeleditor                                                                        R-47
                 Formel-Editor                                                              Softwarereferenz




                                 Bedingungen - Erzeuger
                                 Aufruf über

                                 Organisation
                                 Stammdaten > Feinplanung > Orga > Register Produktionsreihenfolge >
                                 Orga-Gruppe markieren > [Neue Bedingung] > [Neue Bedingung …] / [Editie-
                                 ren]
                                 Stammdaten > Feinplanung > Orga > Register Produktionsreihenfolge > Ab-
                                 stellplatz markieren > [Neue Bedingung] > [Neue Bedingung …] / [Editieren]

                                 Maschinenzuordnung
                                 Stammdaten > MZO > Konfiguration > Fertigungsabschnitt markieren > rechte
                                 Maustaste > Bedingung des Fertigungsabschnitts > Neu > [Neue
                                 Bedingung …] / [Editieren]
                                 Stammdaten > MZO > Konfiguration > Bedingung des Fertigungsabschnitts
                                 markieren > rechte Maustaste > Bedingung editieren > [Neue Bedingung …] /
                                 [Editieren]

                                 Etiketten, Skizzen, Biegertexte
                                 Stammdaten > Etiketten / Skizzen / Biegertexte > Konfiguration … > Bedin-
                                 gung markieren > [Formel-Editor] > [Neue Bedingung …] / [Editieren]




                                 Abb. R-23   Bedingungen - Erzeuger


                                 Im Bedingungen - Erzeuger können Sie entweder eine zuvor markierte Bedin-
1.02 / 01-2017




                                 gung ändern oder neue Bedingungen anlegen.
                                 Die nachfolgende Tabelle gibt eine Übersicht der Dialoge und Funktionen, die
                                 sich in den Menüs Bedingungen und Teilbedingungen befinden.


                 R-48                                                          A+W Production Formeleditor
                 Softwarereferenz                                                                            Formel-Editor




                                        Menü-Eintrag                 Dialog/Funktion

                                        Menü Bedingungen:
                                        Name                          “Name der Bedingung” auf Seite R-52

                                        Info                          “Info” auf Seite R-53

                                        Menge                         “Auswahl Mengen” auf Seite R-56

                                        Invertieren                   “Invertieren” auf Seite R-53

                                        Übergebene Menge              “Übergebene Menge” auf Seite R-54

                                        OK                            Tab. auf Seite R-49

                                        Abbruch                       Tab. auf Seite R-49

                                        Menü Teilbedingungen:
                                         Hinzufügen (Spalte)         Tab. auf Seite R-49

                                        Hinzufügen (Zeile)            Tab. auf Seite R-49

                                        Entfernen                     Tab. auf Seite R-49

                                        Tab. R-2      Übersicht der Dialoge in den Menüs Bedingungen und Teilbedingungen

                                        Der Weg, wie einzelne Dialoge aufgerufen werden, ist bei den nachfolgenden
                                        Dialogbeschreibungen nochmals angegeben. Bestehen mehrere alternative
                                        Wege, einen Dialog aufzurufen, so sind diese ebenfalls angegeben.

                                        Werkzeugleiste

                                        Werkzeug      Erläuterung

                                                      Die definierte Bedingung wird gespeichert und der Editor verlassen


                                                      Die definierte Bedingung wird verworfen und der Editor verlassen.


                                                      Es öffnet sich das Bearbeitungsfenster zum Definieren der
                                                      Bedingung. Bei zweimaligem Anklicken öffnen sich zwei Fenster
                                                      nebeneinander, die eine Und-Verknüpfung darstellen.
                                                       “Bedingung” auf Seite R-50

                                                      Es öffnet sich das Bearbeitungsfenster zum Definieren der
                                                      Bedingung. Bei zweimaligem Anklicken öffnen sich zwei Fenster
                                                      untereinander, die eine Oder-Verknüpfung darstellen.
                                                       “Bedingung” auf Seite R-50

                                                      Die selektierte Bedingung wird gelöscht.


                                        Tab. R-3      Werkzeugleiste im Bedingungen - Erzeuger
1.02 / 01-2017




                 A+W Production Formeleditor                                                                          R-49
                 Formel-Editor                                                              Softwarereferenz




                                 Erläuterung der Radiotasten

                                 All Die Bedingungen aller Teile einer Stückliste werden berücksichtigt. Bei
                                 dieser Einstellung wird z.B. auch eine Scheibe ohne Struktur einem Abstell-
                                 platz mit der Bedingung Struktur zugeordnet. wenn ihre Gegenscheibe struk-
                                 turiert ist.

                                 One Es werden nur die Eigenschaften der aktuellen Scheibe berücksichtigt.

                                 Null Die der Bedingung zugeordnete Menge wird nicht berücksichtigt.


                                 Bedingung
                                 Aufruf über

                                 Organisation
                                 Stammdaten > Feinplanung > Orga > Register Produktionsreihenfolge >
                                 Orga-Gruppe markieren > [Neue Bedingung] > [Neue Bedingung …] > Menü
                                 Teilbedingungen > Hinzufügen …
                                 Stammdaten > Feinplanung > Orga > Register Produktionsreihenfolge > Ab-
                                 stellplatz markieren > [Neue Bedingung] > [Neue Bedingung …] > Menü Teil-
                                 bedingungen > Hinzufügen …

                                 Maschinenzuordnung
                                 Stammdaten > MZO > Konfiguration > Fertigungsabschnitt markieren > rechte
                                 Maustaste > Bedingung des Fertigungsabschnitts > Neu > [Neue
                                 Bedingung …] > Menü Teilbedingungen > Hinzufügen …
                                 Stammdaten > MZO > Konfiguration > Fertigungsabschnitt öffnen > Vorhan-
                                 dene Bedingung markieren > rechte Maustaste > Bedingung editieren > [Neue
                                 Bedingung …] > Menü Teilbedingungen > Hinzufügen …

                                 Etiketten, Skizzen, Biegertexte
                                 Stammdaten > Etiketten / Skizzen / Biegertexte > Konfiguration … > Etiketten
                                 / Skizzen / Biegertext markieren > [Formel-Editor] > [Neue Bedingung …] >
                                 Menü Teilbedingungen > Hinzufügen …
1.02 / 01-2017




                                 Abb. R-24   Bedingung




                 R-50                                                          A+W Production Formeleditor
                 Softwarereferenz                                                                      Formel-Editor




                                        Oberes Eingabefeld Klicken Sie mit der Maus in das Feld, öffnet sich der Di-
                                        alog Auswahl Formeln. Sie können dort entweder eine bereits definierte For-
                                        mel auswählen oder eine neue Formel erstellen.
                                         Softwarereferenz, “Auswahl Formeln” auf Seite R-63

                                        Mittleres Auswahlfeld Öffnen Sie die Kombobox und wählen Sie den ge-
                                        wünschten Operator aus. Mögliche Werte:
                                        • nur Formel 1
                                        • == gleich
                                        • != ungleich
                                        • < kleiner
                                        • <= kleiner gleich
                                        • > größer
                                        • >= größer gleich

                                        Unteres Eingabefeld Klicken Sie mit der Maus in das Feld, öffnet sich ent-
                                        weder der Dialog Auswahl Formeln, der Dialog Eingabe Zahlenwert oder der
                                        Dialog Auswahl Bedingungen. Welcher Dialog sich öffnet, hängt davon ab,
                                        welche Radiotaste (Normal, Wert, Bedingungen) aktiv ist. Ist die Radiotaste
                                        Normal aktiv, öffnet sich der Dialog Auswahl Formeln. Sie können dort entwe-
                                        der eine bereits definierte Formel auswählen oder eine neue Formel erstellen.
                                        Ist die Radiotaste Wert aktiv, öffnet sich der Dialog Eingabe Zahlenwert. Ge-
                                        ben Sie dann den gewünschten Wert ein. Ist die Radiotaste Bedingungen ak-
                                        tiv, öffnet sich der Dialog Auswahl Bedingungen. Sie können dort entweder
                                        eine bereits definierte Bedingung auswählen oder eine neue Bedingung er-
                                        stellen.
                                         Softwarereferenz, “Auswahl Formeln” auf Seite R-63
                                         Softwarereferenz, “Eingabe Zahlenwert” auf Seite R-54
                                         Softwarereferenz, “Auswahl Bedingungen” auf Seite R-46

                                        Normal Aktivieren Sie diese Radiotaste und klicken anschließend in das un-
                                        tere Eingabefeld, öffnet sich der Dialog Auswahl Formeln.
                                         Softwarereferenz, “Auswahl Formeln” auf Seite R-63

                                        Wert Aktivieren Sie diese Radiotaste, öffnet sich der Dialog Eingabe Zahlen-
                                        wert.
                                         Softwarereferenz, “Eingabe Zahlenwert” auf Seite R-54

                                        Bedingungen Aktivieren Sie diese Radiotaste und klicken anschließend in
                                        das untere Eingabefeld, öffnet sich der Dialog Auswahl Bedingungen --2 --.


                                        Weitere Informationen zu der Bedingung
                                         “Elemente des Formeleditors: Stufe I” auf Seite R-9
                                         “Elemente des Formeleditors: Stufe II” auf Seite R-15
1.02 / 01-2017




                 A+W Production Formeleditor                                                                   R-51
                 Formel-Editor                                                              Softwarereferenz




                                 Name der Bedingung
                                 Aufruf über

                                 Organisation
                                 Stammdaten > Feinplanung > Orga > Register Produktionsreihenfolge >
                                 Orga-Gruppe markieren > [Neue Bedingung] > [Neue Bedingung …] > Menü
                                 Bedingungen > Name
                                 Stammdaten > Feinplanung > Orga > Register Produktionsreihenfolge > Ab-
                                 stellplatz markieren > [Neue Bedingung] > [Neue Bedingung …] > Menü Be-
                                 dingungen > Name

                                 Maschinenzuordnung
                                 Stammdaten > MZO > Konfiguration > Fertigungsabschnitt markieren > rechte
                                 Maustaste > Bedingung des Fertigungsabschnitts > Neu > [Neue
                                 Bedingung …] > Menü Bedingungen > Name
                                 Stammdaten > MZO > Konfiguration > Fertigungsabschnitt öffnen > Vorhan-
                                 dene Bedingung markieren > rechte Maustaste > Bedingung editieren > [Neue
                                 Bedingung …] > Menü Bedingungen > Name

                                 Etiketten, Skizzen, Biegertexte
                                 Stammdaten > Etiketten / Skizzen / Biegertexte > Konfiguration … > Etiketten
                                 / Skizzen / Biegertext markieren > [Formel-Editor] > [Neue Bedingung …] >
                                 Menü Bedingungen > Name




                                 Abb. R-25   Name der Bedingung


                                 In diesem Dialog vergeben Sie einen sprechenden Namen für die Bedingun-
                                 gen. Der Name wird in der Statuszeile des Dialogs Bedingungen - Erzeuger
                                 angezeigt.

                                 Erläuterung der Felder

                                 Alte Bezeichnung Wenn für eine Bedingung noch keine Bezeichnung verge-
                                 ben wurde, steht in diesem Feld standardmäßig neue Bedingung. Wurde be-
                                 reits eine Bezeichnung vergeben, steht diese dann dort, im Beispiel oben
                                 >2300.
1.02 / 01-2017




                                 Neue Bezeichnung Geben Sie in diesem Feld die Bezeichnung für die Be-
                                 dingung ein. Sie kann jederzeit überschrieben werden. Die eingetragene Be-
                                 zeichnung erscheint in Statuszeile des Bedingungen - Erzeuger.


                 R-52                                                          A+W Production Formeleditor
                 Softwarereferenz                                                                        Formel-Editor




                                        Info
                                        Aufruf über

                                        Organisation
                                        Stammdaten > Feinplanung > Orga > Register Produktionsreihenfolge >
                                        Orga-Gruppe markieren > [Neue Bedingung] > [Neue Bedingung …] > Menü
                                        Bedingungen > Info
                                        Stammdaten > Feinplanung > Orga > Register Produktionsreihenfolge > Ab-
                                        stellplatz markieren > [Neue Bedingung] > [Neue Bedingung …] > Menü Be-
                                        dingungen > Info

                                        Maschinenzuordnung
                                        Stammdaten > MZO > Konfiguration > Fertigungsabschnitt markieren > rechte
                                        Maustaste > Bedingung des Fertigungsabschnitts > Neu > [Neue
                                        Bedingung …] > Menü Bedingungen > Info
                                        Stammdaten > MZO > Konfiguration > Fertigungsabschnitt öffnen > Vorhan-
                                        dene Bedingung markieren > rechte Maustaste > Bedingung editieren > [Neue
                                        Bedingung …] > Menü Bedingungen > Info

                                        Etiketten, Skizzen, Biegertexte
                                        Stammdaten > Etiketten / Skizzen / Biegertexte > Konfiguration … > Etiketten
                                        / Skizzen / Biegertext markieren > [Formel-Editor] > [Neue Bedingung …] >
                                        Menü Bedingungen > Info




                                        Abb. R-26    Info zur Bedingung


                                        In diesem Bereich können Sie den Inhalt der Bedingung beschreiben. Der Text
                                        erscheint im Dialog Auswahl Bedingungen im Bereich Beschreibung.


                                        Invertieren
                                        Zunächst kann eine Bedingung invertiert werden. D.h. die Bedingung ist er-
                                        füllt, falls das Resultat der Vergleiche nicht erfüllt ist und umgekehrt. Damit
                                        lässt sich einfach aus einer schon existierenden Bedingung die umgekehrte
                                        Bedingung erstellen. Die umgekehrte Bedingung enthält genau einen Ver-
                                        gleich, der die ursprüngliche Bedingung zugewiesen bekommt. Außerdem
                                        wird für die umgekehrte Bedingung die Eigenschaft invertieren ausgewählt. In
                                        der Statuszeile erscheint ein INV vor dem Namen der Bedingung.
                                        Der Menüpunkt ist zu aktivieren bzw. zu deaktivieren.
1.02 / 01-2017




                 A+W Production Formeleditor                                                                     R-53
                 Formel-Editor                                                                Softwarereferenz




                                 Übergebene Menge
                                 Dieser Menüpunkt ist zu aktivieren bzw. zu deaktivieren. Ist er aktiv, wird bei
                                 der Bildung der Mengen nicht nur die Position, über die der Dialog Bedingun-
                                 gen - Erzeuger geöffnet wurde, berücksichtigt, sondern alle Positionen des
                                 Laufs.


                                 Eingabe Zahlenwert
                                 Aufruf über

                                 Organisation
                                 Stammdaten > Feinplanung > Orga > Register Produktionsreihenfolge >
                                 Orga-Gruppe markieren > [Neue Bedingung] > [Neue Bedingung …] > Menü
                                 Teilbedingungen > Hinzufügen > Radiotaste [Wert] aktivieren
                                 Stammdaten > Feinplanung > Orga > Register Produktionsreihenfolge > Ab-
                                 stellplatz markieren > [Neue Bedingung] > [Neue Bedingung …] > Menü Teil-
                                 bedingungen > Hinzufügen > > Radiotaste [Wert] aktivieren

                                 Maschinenzuordnung
                                 Stammdaten > MZO > Konfiguration > Fertigungsabschnitt markieren > rechte
                                 Maustaste > Bedingung des Fertigungsabschnitts > Neu > [Neue
                                 Bedingung …] > Menü Teilbedingungen > Hinzufügen > Radiotaste [Wert] ak-
                                 tivieren
                                 Stammdaten > MZO > Konfiguration > Fertigungsabschnitt öffnen > Vorhan-
                                 dene Bedingung markieren > rechte Maustaste > Bedingung editieren > [Neue
                                 Bedingung …] > Menü Teilbedingungen > Hinzufügen > Radiotaste [Wert] ak-
                                 tivieren

                                 Etiketten, Skizzen, Biegertexte
                                 Stammdaten > Etiketten / Skizzen / Biegertexte > Konfiguration … > Etiketten
                                 / Skizzen / Biegertext markieren > [Formel-Editor] > [Neue Bedingung …] >
                                 Menü Teilbedingungen > Hinzufügen > Radiotaste [Wert] aktivieren




                                 Abb. R-27    Eingabe Zahlenwert


                                 Dieser Dialog dient der Eingabe von Zahlenwerten. Durch das Aktivieren der
1.02 / 01-2017




                                 entsprechenden Radiotaste, können Sie darüber hinaus spezifizieren, ob es
                                 sich bei dem Zahlenwert um Ziffer, Dicke, Text, Länge oder SZR handelt.



                 R-54                                                           A+W Production Formeleditor
                 Softwarereferenz                                                                       Formel-Editor




                                        Erläuterung der Felder

                                        Alter Wert Wenn für eine Bedingung noch kein Wert vergeben wurde, steht
                                        in diesem Feld standardmäßig 0. Wurde bereits ein Wert vergeben, steht die-
                                        ser dann dort.

                                        Neuer Wert Geben Sie in diesem Feld den Wert für die Bedingung ein. Der
                                        Wert kann jederzeit überschrieben werden.

                                        Erläuterung der Radiotasten

                                        Ziffer Bezieht sich die Bedingung z.B. auf eine Stückzahl, aktivieren Sie die-
                                        se Radiotaste und geben im Feld Neuer Wert den entsprechende Ziffer ein.
                                        Bsp.:
                                        • Menge > 10
                                        • Glasart = 1700

                                        Dicke Bezieht sich die Bedingung auf eine Dicke, aktivieren Sie diese Radio-
                                        taste und geben im Feld Neuer Wert den entsprechende Dicke in mm ein.

                                        Text Bezieht sich die Bedingung auf einen Text, aktivieren Sie diese Radio-
                                        taste und geben im Feld Neuer Wert den entsprechenden Text ein.

                                        Länge Bezieht sich die Bedingung auf eine Länge, aktivieren Sie diese Ra-
                                        diotaste und geben im Feld Neuer Wert die entsprechende Länge ein.

                                        SZR Bezieht sich die Bedingung auf einen Scheibenzwischenraum, aktivie-
                                        ren Sie diese Radiotaste und geben im Feld Neuer Wert den entsprechende
                                        SZR ein.
1.02 / 01-2017




                 A+W Production Formeleditor                                                                    R-55
                 Formel-Editor                                                              Softwarereferenz




                                 Auswahl Mengen
                                 Aufruf über

                                 Organisation
                                 Stammdaten > Feinplanung > Orga > Register Produktionsreihenfolge >
                                 Orga-Gruppe markieren > [Neue Bedingung] > [Neue Bedingung …] > Menü
                                 Teilbedingungen > Hinzufügen > mit der Maus in das erste Eingabefeld der
                                 Teilbedingung klicken > [Neue Formel …] > [Menge …]
                                 Stammdaten > Feinplanung > Orga > Register Produktionsreihenfolge > Ab-
                                 stellplatz markieren > [Neue Bedingung] > [Neue Bedingung …] > Menü Teil-
                                 bedingungen > Hinzufügen > mit der Maus in das erste Eingabefeld der
                                 Teilbedingung klicken > [Neue Formel …] > [Menge …]

                                 Maschinenzuordnung
                                 Stammdaten > MZO > Konfiguration > Fertigungsabschnitt markieren > rechte
                                 Maustaste > Bedingung des Fertigungsabschnitts > Neu > [Neue
                                 Bedingung …] > Menü Teilbedingungen > Hinzufügen > mit der Maus in das
                                 erste Eingabefeld der Teilbedingung klicken > [Neue Formel …] > [Menge …]
                                 Stammdaten > MZO > Konfiguration > Fertigungsabschnitt öffnen > Vorhan-
                                 dene Bedingung markieren > rechte Maustaste > Bedingung editieren > [Neue
                                 Bedingung …] > Menü Teilbedingungen > Hinzufügen > mit der Maus in das
                                 erste Eingabefeld der Teilbedingung klicken > [Neue Formel …] > [Menge …]

                                 Etiketten, Skizzen, Biegertexte
                                 Stammdaten > Etiketten / Skizzen / Biegertexte > Konfiguration … > Etiketten
                                 / Skizzen / Biegertext markieren > [Formel-Editor] > [Neue Bedingung …] >
                                 Menü Teilbedingungen > Hinzufügen > mit der Maus in das erste Eingabefeld
                                 der Teilbedingung klicken > [Neue Formel …] > [Menge …]




                                 Abb. R-28   Auswahl Mengen


                                 In diesem Dialog können für die Bereiche Organisation, Maschinenzuordnung
1.02 / 01-2017




                                 und Etiketten, Skizzen, Biegertexte vorhandene Mengen ausgewählt, geän-
                                 dert oder neue Mengen angelegt werden.



                 R-56                                                          A+W Production Formeleditor
                 Softwarereferenz                                                                       Formel-Editor




                                        Erläuterung der Felder

                                        Vorhandene Mengen Die Tabelle listet alle im System vorhandenen Mengen
                                        für die Bereiche Organisation, Maschinenzuordnung und Etiketten, Skizzen,
                                        Biegertexte. Die Inhalte sind für die jeweiligen Bereiche unterschiedlich!

                                        Keine Menge Ist diese Checkbox aktiv, so liefert der Dialog als Ergebnis,
                                        dass Nichts als selektiert gilt.

                                        Beschreibung Das Feld enthält eine detaillierte Erläuterung zu der Menge.
                                        Dabei handelt es sich um den Text, den Sie im Feld Info erfassen.
                                         “Info” auf Seite R-53

                                        Erläuterung der Schaltflächen

                                        Löschen Betätigen Sie diese Schaltfläche, wird die zuvor markierte Menge
                                        gelöscht. Die Löschung erfolgt in diesem Dialog ohne Sicherheitsabfrage.
                                        Sollten Sie jedoch versehentlich etwas gelöscht haben, kehren Sie in den ur-
                                        sprünglichen Dialog (Orga-Dialog, Etikettenart-Dialog, Skizzenart-Dialog, Bie-
                                        gertextart-Dialog, MZO-Dialog) zurück. Wenn Sie diesen dann über
                                        [Abbrechen] schließen, werden Sie gefragt, ob die durchgeführten Änderun-
                                        gen ignoriert werden sollen oder nicht.

                                        Neue Menge Betätigen Sie diese Schaltfläche, öffnet sich der Dialog Men-
                                        gen - Erzeuger. Sie können dann eine neue Menge anlegen.
                                         “Mengen - Erzeuger” auf Seite R-58

                                        Editieren Betätigen Sie diese Schaltfläche, öffnet sich für die markierte Men-
                                        ge der Dialog Mengen - Erzeuger.
                                         “Mengen - Erzeuger” auf Seite R-58
1.02 / 01-2017




                 A+W Production Formeleditor                                                                    R-57
                 Formel-Editor                                                              Softwarereferenz




                                 Mengen - Erzeuger
                                 Aufruf über

                                 Organisation
                                 Stammdaten > Feinplanung > Orga > Register Produktionsreihenfolge >
                                 Orga-Gruppe markieren > [Neue Bedingung] > [Neue Bedingung …] > Menü
                                 Teilbedingungen > Hinzufügen > mit der Maus in das erste Eingabefeld der
                                 Teilbedingung klicken > [Neue Formel …] > [Menge …] > [Neu Menge …] /
                                 [Editieren]
                                 Stammdaten > Feinplanung > Orga > Register Produktionsreihenfolge > Ab-
                                 stellplatz markieren > [Neue Bedingung] > [Neue Bedingung …] > Menü Teil-
                                 bedingungen > Hinzufügen > mit der Maus in das erste Eingabefeld der
                                 Teilbedingung klicken > [Neue Formel …] > [Menge …] > [Neu Menge …] /
                                 [Editieren]

                                 Maschinenzuordnung
                                 Stammdaten > MZO > Konfiguration > Fertigungsabschnitt markieren > rechte
                                 Maustaste > Bedingung des Fertigungsabschnitts > Neu > [Neue
                                 Bedingung …] > Menü Teilbedingungen > Hinzufügen > mit der Maus in das
                                 erste Eingabefeld der Teilbedingung klicken > [Neue Formel …] > [Menge …]
                                 > [Neu Menge …] / [Editieren]
                                 Stammdaten > MZO > Konfiguration > Fertigungsabschnitt öffnen > Vorhan-
                                 dene Bedingung markieren > rechte Maustaste > Bedingung editieren > [Neue
                                 Bedingung …] > Menü Teilbedingungen > Hinzufügen > mit der Maus in das
                                 erste Eingabefeld der Teilbedingung klicken > [Neue Formel …] > [Menge …]
                                 > [Neu Menge …] / [Editieren]

                                 Etiketten, Skizzen, Biegertexte
                                 Stammdaten > Etiketten / Skizzen / Biegertexte > Konfiguration … > Etiketten
                                 / Skizzen / Biegertext markieren > [Formel-Editor] > [Neue Bedingung …] >
                                 Menü Teilbedingungen > Hinzufügen > mit der Maus in das erste Eingabefeld
                                 der Teilbedingung klicken > [Neue Formel …] > [Menge …] > [Neu Menge …]
                                 / [Editieren]
1.02 / 01-2017




                 R-58                                                          A+W Production Formeleditor
                 Softwarereferenz                                                                        Formel-Editor




                                        Abb. R-29     Mengen - Erzeuger


                                        Im Mengen - Erzeuger können Sie entweder eine zuvor markierte Menge än-
                                        dern oder neue Menge anlegen.
                                        Die nachfolgende Tabelle gibt eine Übersicht der Dialoge und Funktionen, die
                                        sich in den Menüs Menge und Teilmengen befinden.

                                        Menü-Eintrag                Dialog/Funktion

                                        Menü Menge:
                                        Name                         “Name der Menge” auf Seite R-61

                                        Info                         “Info” auf Seite R-62

                                        Bedingung                    “Auswahl Bedingungen” auf Seite R-46

                                        Formel                       “Auswahl Formeln” auf Seite R-63

                                        OK                           Tab. auf Seite R-60

                                        Abbruch                      Tab. auf Seite R-60

                                        Menü Teilmengen:
                                        Hinzufügen (Spalte)          Tab. auf Seite R-60

                                        Hinzufügen (Zeile)           Tab. auf Seite R-60

                                        Entfernen                    Tab. auf Seite R-60

                                        Wechsel                      Tab. auf Seite R-60

                                        Tab. R-4      Übersicht der Dialoge in den Menüs Menge und Teilmengen
1.02 / 01-2017




                                        Der Weg, wie einzelne Dialoge aufgerufen werden, ist bei den nachfolgenden
                                        Dialogbeschreibungen nochmals angegeben. Bestehen mehrere alternative
                                        Wege, einen Dialog aufzurufen, so sind diese ebenfalls angegeben.


                 A+W Production Formeleditor                                                                    R-59
                 Formel-Editor                                                                    Softwarereferenz




                                 Werkzeugleiste

                                 Werkzeug      Erläuterung

                                               Die definierte Menge wird gespeichert und der
                                               Editor verlassen

                                               Die definierte Menge wird verworfen und der
                                               Editor verlassen.

                                               Es öffnet sich das Bearbeitungsfenster zum
                                               Definieren der Menge. Bei zweimaligem
                                               Anklicken öffnen sich zwei Fenster
                                               nebeneinander, die eine Und-Verknüpfung
                                               darstellen.

                                               Es öffnet sich das Bearbeitungsfenster zum
                                               Definieren der Menge. Bei zweimaligem
                                               Anklicken öffnen sich zwei Fenster
                                               untereinander, die eine Oder-Verknüpfung
                                               darstellen.
                                                “Bedingung” auf Seite R-50

                                               Die selektierte Menge wird gelöscht.


                                               Dient dem Umschalten zwischen dem ersten
                                               und dem zweiten Fenster.

                                 Tab. R-5      Werkzeugleiste im Mengen - Erzeuger

                                 Erläuterung der Checkboxen

                                 All Alle Teile des Teilebaums, in dem das Startteil enthalten ist.

                                 Master Das oberste Teil des Teilebaums (Kopfteil), in dem das Startteil ent-
                                 halten ist.

                                 Parent Das Teil, das sich im Teilebaum direkt über dem Startteil befindet.

                                 Self Das Startteil.

                                 Child Alle direkten Unterteile des Startteils.

                                 Anychild Alle Unterteile des Startteils, auch die indirekten.

                                 Bottom Alle Basisteile, die sich unter dem Startteil befinden.

                                 Up Unter Verwendung von Up besteht die Endmenge genau aus einem Teil.
                                 Dabei werden vom Startteil ausgehend alle Oberteile des Startteils untersucht,
                                 ob das jeweilige Teil die Bedingung erfüllt. In der Endmenge befindet sich das
                                 letzte Teil, das die Bedingung erfüllt hat. Erfüllt ein Teil die Bedingung nicht, so
                                 wird die Iteration nach oben abgebrochen
1.02 / 01-2017




                 R-60                                                                 A+W Production Formeleditor
                 Softwarereferenz                                                                            Formel-Editor




                                        Addup Unter Verwendung von Addup kann die Endmenge aus mehr als ei-
                                        nem Teil bestehen. Wie bei Up wird ebenfalls vom Startobjekt nach oben ite-
                                        riert und die Iteration beendet, falls ein Teil die Bedingung nicht erfüllt. Aber
                                        die Endmenge enthält alle Teile, die die Bedingung erfüllt haben.


                                        Weitere Informationen
                                         Funktionsprinzip, “Elemente des Formeleditors: Stufe III” auf Seite R-19



                                        Name der Menge
                                        Aufruf über

                                        Organisation
                                        Stammdaten > Feinplanung > Orga > Register Produktionsreihenfolge >
                                        Orga-Gruppe markieren > [Neue Bedingung] > [Neue Bedingung …] > Menü
                                        Teilbedingungen > Hinzufügen > mit der Maus in das erste Eingabefeld der
                                        Teilbedingung klicken > [Neue Formel …] > [Menge …] > [Neu Menge …] /
                                        [Editieren] > Menü Menge > Name
                                        Stammdaten > Feinplanung > Orga > Register Produktionsreihenfolge > Ab-
                                        stellplatz markieren > [Neue Bedingung] > [Neue Bedingung …] > Menü Teil-
                                        bedingungen > Hinzufügen > mit der Maus in das erste Eingabefeld der
                                        Teilbedingung klicken > [Neue Formel …] > [Menge …] > [Neu Menge …] /
                                        [Editieren] > Menü Menge > Name

                                        Maschinenzuordnung
                                        Stammdaten > MZO > Konfiguration > Fertigungsabschnitt öffnen > Vorhan-
                                        dene Bedingung markieren > rechte Maustaste > Bedingung editieren > [Neue
                                        Bedingung …] > Menü Teilbedingungen > Hinzufügen > mit der Maus in das
                                        erste Eingabefeld der Teilbedingung klicken > [Neue Formel …] > [Menge …]
                                        > [Neu Menge …] / [Editieren] > Menü Menge > Name
                                        Stammdaten > MZO > Konfiguration > Fertigungsabschnitt öffnen > Vorhan-
                                        dene Bedingung markieren > rechte Maustaste > Bedingung editieren > [Neue
                                        Bedingung …] > Menü Teilbedingungen > Hinzufügen > mit der Maus in das
                                        erste Eingabefeld der Teilbedingung klicken > [Neue Formel …] > [Menge …]
                                        > [Neu Menge …] / [Editieren] > Menü Menge > Name

                                        Etiketten, Skizzen, Biegertexte
                                        Stammdaten > Etiketten / Skizzen / Biegertexte > Konfiguration … > Etiketten
                                        / Skizzen / Biegertext markieren > [Formel-Editor] > [Neue Bedingung …] >
                                        Menü Teilbedingungen > Hinzufügen > mit der Maus in das erste Eingabefeld
                                        der Teilbedingung klicken > [Neue Formel …] > [Menge …] > [Neu Menge …]
                                        / [Editieren] > Menü Menge > Name
1.02 / 01-2017




                 A+W Production Formeleditor                                                                         R-61
                 Formel-Editor                                                              Softwarereferenz




                                 Abb. R-30   Name der Menge


                                 In diesem Dialog vergeben Sie einen sprechenden Namen für die Menge. Der
                                 Name wird in der Statuszeile des Dialogs Mengen - Erzeuger angezeigt.

                                 Felder

                                 Alte Bezeichnung Wenn für eine Menge noch keine Bezeichnung vergeben
                                 wurde, steht in diesem Feld standardmäßig neue Menge. Wurde bereits eine
                                 Bezeichnung vergeben, steht diese dann dort, im Beispiel oben 1, wenn Breite
                                 < Höhe.

                                 Neue Bezeichnung Geben Sie in diesem Feld die Bezeichnung für die Be-
                                 dingung ein. Sie kann jederzeit überschrieben werden. Die eingetragene Be-
                                 zeichnung erscheint in Statuszeile des Bedingungen - Erzeuger.


                                 Info
                                 Aufruf über

                                 Organisation
                                 Stammdaten > Feinplanung > Orga > Register Produktionsreihenfolge >
                                 Orga-Gruppe markieren > [Neue Bedingung] > [Neue Bedingung …] > Menü
                                 Teilbedingungen > Hinzufügen > mit der Maus in das erste Eingabefeld der
                                 Teilbedingung klicken > [Neue Formel …] > [Menge …] > [Neu Menge …] /
                                 [Editieren] > Menü Menge > Info
                                 Stammdaten > Feinplanung > Orga > Register Produktionsreihenfolge > Ab-
                                 stellplatz markieren > [Neue Bedingung] > [Neue Bedingung …] > Menü Teil-
                                 bedingungen > Hinzufügen > mit der Maus in das erste Eingabefeld der
                                 Teilbedingung klicken > [Neue Formel …] > [Menge …] > [Neu Menge …] /
                                 [Editieren] > Menü Menge > Info

                                 Maschinenzuordnung
                                 Stammdaten > MZO > Konfiguration > Fertigungsabschnitt öffnen > Vorhan-
                                 dene Bedingung markieren > rechte Maustaste > Bedingung editieren > [Neue
                                 Bedingung …] > Menü Teilbedingungen > Hinzufügen > mit der Maus in das
                                 erste Eingabefeld der Teilbedingung klicken > [Neue Formel …] > [Menge …]
                                 > [Neu Menge …] / [Editieren] > Menü Menge > Info
1.02 / 01-2017




                 R-62                                                          A+W Production Formeleditor
                 Softwarereferenz                                                                     Formel-Editor




                                        Stammdaten > MZO > Konfiguration > Fertigungsabschnitt öffnen > Vorhan-
                                        dene Bedingung markieren > rechte Maustaste > Bedingung editieren > [Neue
                                        Bedingung …] > Menü Teilbedingungen > Hinzufügen > mit der Maus in das
                                        erste Eingabefeld der Teilbedingung klicken > [Neue Formel …] > [Menge …]
                                        > [Neu Menge …] / [Editieren] > Menü Menge > Info

                                        Etiketten, Skizzen, Biegertexte
                                        Stammdaten > Etiketten / Skizzen / Biegertexte > Konfiguration … > Etiketten
                                        / Skizzen / Biegertext markieren > [Formel-Editor] > [Neue Bedingung …] >
                                        Menü Teilbedingungen > Hinzufügen > mit der Maus in das erste Eingabefeld
                                        der Teilbedingung klicken > [Neue Formel …] > [Menge …] > [Neu Menge …]
                                        / [Editieren] > Menü Menge > Info




                                        Abb. R-31   Info zur Menge


                                        In diesem Bereich können Sie den Inhalt der Bedingung beschreiben. Der Text
                                        erscheint im Dialog Auswahl Mengen im Bereich Beschreibung.


                                        Auswahl Formeln
                                        Aufruf über

                                        Organisation
                                        Stammdaten > Feinplanung > Orga > Register Produktionsreihenfolge >
                                        Orga-Gruppe markieren > [Neue Bedingung] > [Neue Bedingung …] > Menü
                                        Teilbedingungen > Hinzufügen > mit der Maus in das erste Eingabefeld der
                                        Teilbedingung klicken
                                        Stammdaten > Feinplanung > Orga > Register Produktionsreihenfolge > Ab-
                                        stellplatz markieren > [Neue Bedingung] > [Neue Bedingung …] > Menü Teil-
                                        bedingungen > Hinzufügen > mit der Maus in das erste Eingabefeld der
                                        Teilbedingung klicken

                                        Maschinenzuordnung
                                        Stammdaten > MZO > Konfiguration > Fertigungsabschnitt öffnen > Vorhan-
                                        dene Bedingung markieren > rechte Maustaste > Bedingung editieren > [Neue
                                        Bedingung …] > Menü Teilbedingungen > Hinzufügen > mit der Maus in das
                                        erste Eingabefeld der Teilbedingung klicken
                                        Stammdaten > MZO > Konfiguration > Fertigungsabschnitt öffnen > Vorhan-
                                        dene Bedingung markieren > rechte Maustaste > Bedingung editieren > [Neue
1.02 / 01-2017




                                        Bedingung …] > Menü Teilbedingungen > Hinzufügen > mit der Maus in das
                                        erste Eingabefeld der Teilbedingung klicken




                 A+W Production Formeleditor                                                                   R-63
                 Formel-Editor                                                              Softwarereferenz




                                 Etiketten, Skizzen, Biegertexte
                                 Stammdaten > Etiketten / Skizzen / Biegertexte > Konfiguration … > Etiketten
                                 / Skizzen / Biegertext markieren > [Formel-Editor] > [Neue Bedingung …] >
                                 Menü Teilbedingungen > Hinzufügen > mit der Maus in das erste Eingabefeld
                                 der Teilbedingung klicken




                                 Abb. R-32    Auswahl Formeln


                                 In diesem Dialog können für die Bereiche Organisation, Maschinenzuordnung
                                 und Etiketten, Skizzen, Biegertexte vorhandene Formeln ausgewählt, geän-
                                 dert oder neue Formeln angelegt werden.

                                 Felder

                                 Vorhandene Formeln Die Tabelle listet alle im System vorhandenen For-
                                 meln für die Bereiche Organisation, Maschinenzuordnung und Etiketten, Skiz-
                                 zen, Biegertexte.

                                 Keine Formel Ist diese Checkbox aktiv, so liefert der Dialog als Ergebnis,
                                 dass Nichts als selektiert gilt.

                                 Beschreibung Das Feld enthält eine detaillierte Erläuterung zu der Formel.
                                 Dabei handelt es sich um den Text, den Sie im Feld Beschreibung erfassen.
                                  “Beschreibung” auf Seite R-66

                                 Schaltflächen

                                 Löschen Betätigen Sie diese Schaltfläche, wird die zuvor markierte Formel
                                 gelöscht. Die Löschung erfolgt in diesem Dialog ohne Sicherheitsabfrage.
                                 Sollten Sie jedoch versehentlich etwas gelöscht haben, kehren Sie in den ur-
                                 sprünglichen Orga-Dialog zurück. Wenn Sie diesen dann über
                                 [Abbrechen] schließen, werden Sie gefragt, ob die durchgeführten Änderun-
                                 gen ignoriert werden sollen oder nicht.

                                 Neue Formel Betätigen Sie diese Schaltfläche, öffnet sich der Dialog Formel
                                 - Editor. Sie können dann eine neue Formel anlegen.
1.02 / 01-2017




                                  “Formel - Editor” auf Seite R-65




                 R-64                                                          A+W Production Formeleditor
                 Softwarereferenz                                                                            Formel-Editor




                                        Editieren Betätigen Sie diese Schaltfläche, öffnet sich für die markierte For-
                                        mel der Dialog Formel - Editor.
                                         “Formel - Editor” auf Seite R-65


                                        Weitere Informationen zu den Formeln
                                         Funktionsprinzip, “Elemente des Formeleditors: Stufe I” auf Seite R-9
                                         Funktionsprinzip, “Elemente des Formeleditors: Stufe II” auf Seite R-15
                                         Funktionsprinzip, “Elemente des Formeleditors: Stufe III” auf Seite R-19



                                        Formel - Editor
                                        Aufruf über

                                        Organisation
                                        Stammdaten > Feinplanung > Orga > Register Produktionsreihenfolge >
                                        Orga-Gruppe markieren > [Neue Bedingung] > [Neue Bedingung …] > Menü
                                        Teilbedingungen > Hinzufügen > mit der Maus in das erste Eingabefeld der
                                        Teilbedingung klicken > [Neue Formel …]
                                        Stammdaten > Feinplanung > Orga > Register Produktionsreihenfolge > Ab-
                                        stellplatz markieren > [Neue Bedingung] > [Neue Bedingung …] > Menü Teil-
                                        bedingungen > Hinzufügen > mit der Maus in das erste Eingabefeld der
                                        Teilbedingung klicken > [Neue Formel …]

                                        Maschinenzuordnung
                                        Stammdaten > MZO > Konfiguration > Fertigungsabschnitt öffnen > Vorhan-
                                        dene Bedingung markieren > rechte Maustaste > Bedingung editieren > [Neue
                                        Bedingung …] > Menü Teilbedingungen > Hinzufügen > mit der Maus in das
                                        erste Eingabefeld der Teilbedingung klicken > [Neue Formel …]
                                        Stammdaten > MZO > Konfiguration > Fertigungsabschnitt öffnen > Vorhan-
                                        dene Bedingung markieren > rechte Maustaste > Bedingung editieren > [Neue
                                        Bedingung …] > Menü Teilbedingungen > Hinzufügen > mit der Maus in das
                                        erste Eingabefeld der Teilbedingung klicken > [Neue Formel …]
1.02 / 01-2017




                 A+W Production Formeleditor                                                                         R-65
                 Formel-Editor                                                              Softwarereferenz




                                 Etiketten, Skizzen, Biegertexte
                                 Stammdaten > Etiketten / Skizzen / Biegertexte > Konfiguration … > Etiketten
                                 / Skizzen / Biegertext markieren > [Formel-Editor] > [Neue Bedingung …] >
                                 Menü Teilbedingungen > Hinzufügen > mit der Maus in das erste Eingabefeld
                                 der Teilbedingung klicken > [Neue Formel …]




                                 Abb. R-33    Formel - Editor


                                 In diesem Dialog können Sie neue Formeln erstellen. Eine Formel in ihrer ein-
                                 fachsten Art ist lediglich ein Feld der Datenbank. Im Bereich Vorhandene Ei-
                                 genschaften finden Sie eine Liste der Datenbankfelder. Markieren Sie eines
                                 der Datenbankfelder, erscheint im grauen Bereich darunter die Erklärung des
                                 Feldinhaltes. Es können natürlich auch viel kompliziertere Formeln erstellt
                                 werden, mehrere Felder verknüpft, bzw. eine oder mehrere der schon vorhan-
                                 denen Formeln benutzt werden.

                                 Felder

                                 Eingabefeld oben Geben Sie in diesem Feld einen möglichst sprechenden
                                 Namen für die Formel ein.

                                 Beschreibung In diesem Feld geben Sie eine möglichst detaillierte Beschrei-
                                 bung zu der Formel an.

                                 Formel In diesem Feld wird das für die Formel benötigte Datenbankfeld ein-
                                 getragen. D.h. Sie suchen sich im Bereich Vorhandene Eigenschaften das
                                 entsprechende Datenbankfeld aus und klicken doppelt darauf. Das Daten-
                                 bankfeld wird dann automatisch in den Bereich Formel übertragen.

                                 Menge Betätigen Sie diese Schaltfläche, öffnet sich der Dialog Auswahl Men-
                                 gen. Dort können Sie dann eine bereits vorhandene Menge auswählen oder
                                 eine neue Menge erstellen.
1.02 / 01-2017




                                  Softwarereferenz, “Auswahl Mengen” auf Seite R-56




                 R-66                                                           A+W Production Formeleditor
                 Softwarereferenz                                                                            Formel-Editor




                                        Übergebene Menge Checkbox. Ist die Checkbox aktiv, wird bei der Bildung
                                        der Mengen nicht nur die Position, über die der Dialog Auswahl Mengen ge-
                                        öffnet wurde, berücksichtigt, sondern alle Positionen des Laufs. Nur bei akti-
                                        vierter Checkbox sind die Radiotasten im Bereich Operation ebenfalls aktiv.

                                        Radiotasten im Bereich Operation
                                        Die Radiotasten in diesem Bereich sind nur aktiv, wenn die Checkbox Über-
                                        gebene Menge aktiv ist. D.h. wenn der Formel eine Menge zugeweisen wurde.
                                        Dann wird zunächst für alle Teile dieser Menge die Formel ausgewertet. Die
                                        Ergebnisse der Formel werden wie folgt verarbeitet:

                                        Summe (Wert) Summe aller Ergebnisse

                                        Mittelwert Summe/Anzahl Ergebnisse

                                        Und-Verknüpfung Die ergebnisse werden durch logisches Und verknüpft

                                        Oder-Verknüpfung Die Ergebnisse werden durch logisches Oder verknüpft

                                           Und-/Oder-Verknüpfungen
                                           Und-/Oder-Verknüpfungen machen nur richtig Sinn, wenn Formeln als Er-
                                           gebnis 0 oder 1 liefern!

                                        Minimum Kleinstes Ergebnis

                                        Maximum Größtes Ergebnis

                                        Anzahl Resultate Anzahl der verschiedenen Ergebnisse

                                        Felder

                                        Vorhandene Eigenschaften Die Tabelle listet Datenbankfelder für die Berei-
                                        che Organisation, Maschinenzuordnung und Etiketten, Skizzen, Biegertexte.
                                        Wird ein Feld markiert, erscheint unterhalb eine Erklärung des Feldinhaltes.

                                           Vorhandene Eigenschaften (Properties)
                                           Objekteigenschaften (Properties) innerhalb der Orga sind aus Perfor-
                                           mance-Gründen fest verdrahtet und können nicht ohne Programmände-
                                           rung erweitert werden. Objekteigenschaften (Properties) innerhalb der
                                           MZO und Etiketten können dynamisch über das Script DBInit erweitert wer-
                                           den.

                                        Vorhandene Formeln Die Tabelle listet alle im System vorhandenen For-
                                        meln für die Bereiche Organisation, Maschinenzuordnung und Etiketten, Skiz-
                                        zen, Biegertexte.


                                        Weitere Informationen zum Formel-Editor
                                         Funktionsprinzip, “Elemente des Formeleditors: Stufe I” auf Seite R-9
1.02 / 01-2017




                                         Funktionsprinzip, “Elemente des Formeleditors: Stufe II” auf Seite R-15
                                         Funktionsprinzip, “Elemente des Formeleditors: Stufe III” auf Seite R-19




                 A+W Production Formeleditor                                                                         R-67
                 Formel-Editor                                                               Softwarereferenz




                                 Auswahl Zuweisung
                                 Stammdaten > Feinplanung > Zuweisungen




                                 Abb. R-34    Auswahl Zuweisung


                                 In diesem Dialog können Sie nur für den Bereich der Orga vorhandene Zuwei-
                                 sungen auswählen, ändern oder neue Zuweisungen anlegen.

                                 Felder

                                 Vorhandene Zuweisungen Die Tabelle listet alle im System vorhandenen
                                 Zuweisungen für den Bereich der Orga.

                                 Keine Zuweisung Ist diese Checkbox aktiv, so liefert der Dialog als Ergeb-
                                 nis, dass Nichts als selektiert gilt.

                                 Beschreibung Das Feld enthält eine detaillierte Erläuterung zu der Zuwei-
                                 sung. Dabei handelt es sich um den Text, den Sie im Feld Info erfassen.
                                  Softwarereferenz, “Info” auf Seite R-53

                                 Schaltflächen

                                 Löschen Betätigen Sie diese Schaltfläche, wird die zuvor markierte Zuwei-
                                 sung gelöscht. Die Löschung erfolgt in diesem Dialog ohne Sicherheitsabfra-
                                 ge. Sollten Sie jedoch versehentlich etwas gelöscht haben schließen Sie den
                                 Dialog über [Abbrechen]. Die Änderungen werden ignoriert.

                                 Neue Zuweisung Betätigen Sie diese Schaltfläche, öffnet sich der Dialog Zu-
                                 weisung - Editor. Sie können dann eine neue Bedingung anlegen.
                                  Softwarereferenz, “Zuweisung - Editor” auf Seite R-69

                                 Editieren Betätigen Sie diese Schaltfläche, öffnet sich für die markierte Zu-
                                 weisung der Dialog Zuweisung - Editor.
                                  Softwarereferenz, “Zuweisung - Editor” auf Seite R-69
1.02 / 01-2017




                 R-68                                                             A+W Production Formeleditor
                 Softwarereferenz                                                                      Formel-Editor




                                        Zuweisung - Editor
                                        Stammdaten > Feinplanung > Zuweisungen > [Neue Zuweisung …]




                                        Abb. R-35   Zuweisung - Editor


                                        In diesem Dialog können Sie eine Zuweisung definieren. In der einfachsten
                                        Form besteht eine Zuweisung aus einer Objekt-Eigenschaft (Property) und ei-
                                        ner Formel. Das Ergebnis der Formel wird der Eigenschaft des Objektes zu-
                                        gewiesen. Die Zuweisung kann jedoch auch eine Menge enthalten. Dann wird
                                        für alle Objekte der Endmenge das jeweilige Ergebnis der Formel der jeweili-
                                        gen Eigenschaft zugewiesen.

                                        Felder

                                        Eingabefeld oben In diesem Feld vergeben Sie einen sprechenden Namen
                                        für die Zuweisung. Haben Sie den Dialog Zuweisung - Editor über die Schalt-
                                        fläche [Neue Zuweisung …] geöffnet, steht in diesem Feld standardmäßig
                                        neue Zuweisung. Haben Sie den Dialog über die Schaltfläche [Editieren] ge-
                                        öffnet, steht in dem Feld der Name der Zuweisung, die Sie bearbeiten möch-
                                        ten.

                                        Eigenschaft Wenn Sie die Kombobox öffnen, werden Ihnen die Datenbank-
                                        felder, die im Bereich der Feinplanung änderbar sind, angezeigt. Nachdem Sie
                                        das gewünschte Datenbankfeld ausgewählt haben, erscheint im grauen Be-
                                        reich rechts neben der Kombobox die Erklärung des Feldinhaltes.

                                           Vorhandene Eigenschaften (Properties)
                                           Objekteigenschaften (Properties) innerhalb der Feinplanung sind aus Per-
                                           formance-Gründen fest verdrahtet und können nicht ohne Programmände-
                                           rung erweitert werden.

                                        Wichtige Zuweisungen:
                                        • Abstellbreite: Wird für eine eventuell verwendete Gestellbelegung verwen-
                                          det. Im Normalfall ist diese Eigenschaft mit der Breite der Scheibe belegt.
                                        • Bewertung: Im Normalfall mit 100 belegt. Dient innerhalb der Optimierung
                                          dazu Scheiben auf mehrere Lagerplatten zu verteilen. Je kleiner der Wert
1.02 / 01-2017




                                          umso stärker ist diese Verschmierung. Damit kann zum Beispiel erreicht
                                          werden, dass für große Schieben nicht alle Schieben einer Einheit auf ei-
                                          nem Lagerblatt liegen.


                 A+W Production Formeleditor                                                                   R-69
                 Formel-Editor                                                                    Softwarereferenz




                                 •   Dickendifferenz: Für Auffüller kann hiermit eingestellt werden, um wie stark
                                     sich die Glasdicke durch das Auffüllen ändern darf.
                                 •   Gruppennummer: Ist per Standard mit 0 belegt. Sollten innerhalb der Fein-
                                     planung Fertigungsgruppen via dieser Gruppennummer gebildet werden,
                                     so ist diese Eigenschaft zunächst mit der geeigneten Formel zu belegen.
                                 •   Kiste: Ist frei verfügbar.
                                 •   Zuschlagdicke: Ist per Standard mit 0 mm belegt. Hiermit lässt sich errei-
                                     chen, dass beim Abstellen auf A-Böcke eine größere Dicke für eine Schei-
                                     be berücksichtigt wird als dies durch ihre Glasdicke der Fall ist. Zum
                                     Beispiel wird dies verwendet für Scheiben mit Siebdruck. Um den Sieb-
                                     druck zu schützen wird nach jeder Scheibe ein Stück Pappe mit einer Dicke
                                     von X mm davor gestellt. Diesen Wert weißt man hier der Zuschlagdicke
                                     zu. Damit dies nur für Scheiben mit Siebdruck erfolgt muss natürlich die
                                     Menge entsprechend gewählt sein.

                                 Formel … Wenn Sie diese Schaltfläche betätigen, öffnen Sie den Dialog
                                 Auswahl Formeln.
                                  Softwarereferenz, “Auswahl Formeln” auf Seite R-63

                                 Grau hinterlegtes Feld Wenn Sie über die Schaltfläche [Formel …] eine sol-
                                 che ausgewählt haben, erhalten Sie in diesem Feld den Namen der Formel
                                 angezeigt.

                                 Menge … Wenn Sie diese Schaltfläche betätigen, öffnen Sie den Dialog Aus-
                                 wahl Mengen. Er dient sowohl dazu für weitere Teile (nicht nur dem aktuellen
                                 Teil) die Zuweisung durchzuführen, als auch nur für bestimmte Teile die Zu-
                                 weisung anwendung zu dürfen
                                  Softwarereferenz, “Auswahl Mengen” auf Seite R-56

                                 Übergebene Menge Checkbox. Ist die Checkbox aktiv, wird bei der Bildung
                                 der Mengen nicht nur die Position, über die der Dialog Auswahl Mengen ge-
                                 öffnet wurde, berücksichtigt, sondern alle Positionen des Laufs.

                                 Grau hinterlegtes Feld Wenn Sie über die Schaltfläche [Menge …] eine sol-
                                 che ausgewählt haben, erhalten Sie in diesem Feld den Namen der Menge
                                 angezeigt.


                                 Weitere Informationen zu der Zuweisung
                                  Funktionsprinzip, “Elemente des Formeleditors: Stufe I” auf Seite R-9
                                  Funktionsprinzip, “Elemente des Formeleditors: Stufe II” auf Seite R-15
1.02 / 01-2017




                 R-70                                                              A+W Production Formeleditor
Formeleditor                R

                      Partindex




               A+W Production
                 Partindex                                                      Inhalt




                 Inhalt
                 Symbols                         – Neue Zuweisung R-68
                 ´Zuweisung                      – Vorhandene Zuweisung R-68
                 – Stufe II R-18
                                                 B
                 A                               Bedingung
                 Addup                           – Bedingungen R-51
                 – Mengen Erzeuger R-61          – Bedinungen-Erzeuger R-50
                 All                             – Invertieren R-53
                 – Bedinungen-Erzeuger R-50      – Mittleres Auswahlfeld R-51
                 – Mengen Erzeuger R-60          – Normal R-51
                 Alte Bezeichnung                – Oberes Eingabefeld R-51
                 – Name der Bedingung R-52       – Stufe I R-11
                 – Name der Menge R-62           – Stufe II R-16
                 Alter Wert                      – Übergebene Menge R-54
                 – Eingabe Zahlenwert R-55       – Unteres Eingabefeld R-51
                 Anychild                        – Wert R-51
                 – Mengen Erzeuger R-60          Bedingungen
                 Anzahl Resultate                – Bedingung R-51
                 – Formel Editor R-67            Bedingungen-Erzeuger
                 Auswahl Bedingungen             – All R-50
                 – Beschreibung R-47             – Bedingung R-50
                 – Dialog R-46                   – Dialog R-48
                 – Editieren R-47                – Menü R-49
                 – Keine Bedingung R-47          – Null R-50
                 – Löschen R-47                  – One R-50
                 – Neue Bedingung R-47           – Werkzeugleiste R-49
                 – Vorhandene Bedingungen R-47   Beschreibung
                 Auswahl Formeln                 – Auswahl Bedingungen R-47
                 – Beschreibung R-64             – Auswahl Formeln R-64
                 – Dialog R-63                   – Auswahl Mengen R-57
                 – Editieren R-65                – Auswahl Zuweisung R-68
                 – Keine Formel R-64             – Formel Editor R-66
                 – Löschen R-64                  Bottom
                 – Neue Formel R-64              – Mengen Erzeuger R-60
                 – Vorhandene Formeln R-64
                 Auswahl Mengen                  C
                 – Beschreibung R-57             Child
                 – Dialog R-56                   – Mengen Erzeuger R-60
                 – Editieren R-57
                 – Keine Menge R-57
                                                 D
                 – Löschen R-57
                                                 Dialog
                 – Neue Menge R-57
                                                 – Auswahl Bedingungen R-46
                 – Vorhandene Menge R-57
                                                 – Auswahl Formeln R-63
                 Auswahl Zuweisung
                                                 – Auswahl Mengen R-56
                 – Beschreibung R-68
                                                 – Auswahl Zuweisung R-68
1.02 / 01-2017




                 – Dialog R-68
                                                 – Bedinungen-Erzeuger R-48
                 – Editieren R-68
                                                 – Eingabe Zahlenwert R-54
                 – Keine Zuweisung R-68
                                                 – Formel Editor R-65
                 – Löschen R-68


                 A+W Production Formeleditor                                    R-73
                 Inhalt                                                              Partindex




                 – Info R-53, R-62                 – Dialog R-53, R-62
                 – Mengen Erzeuger R-58            Invertieren
                 – Name der Bedingung R-52         – Bedingung R-53
                 – Name der Menge R-61
                 – Zuweisung Editor R-69           K
                                                   Keine Bedingung
                 E                                 – Auswahl Bedingungen R-47
                 Editieren                         Keine Formel
                 – Auswahl Bedingungen R-47        – Auswahl Formeln R-64
                 – Auswahl Formeln R-65            Keine Menge
                 – Auswahl Mengen R-57             – Auswahl Mengen R-57
                 – Auswahl Zuweisung R-68          Keine Zuweisung
                 Eigenschaft                       – Auswahl Zuweisung R-68
                 – Zuweisung Editor R-69
                 Einabefeld oben                   L
                 – Zuweisung Editor R-69           Länge
                 Eingabe Zahlenwert                – Eingabe Zahlenwert R-55
                 – Alter Wert R-55                 Löschen
                 – Dialog R-54                     – Auswahl Bedingungen R-47
                 – Länge R-55                      – Auswahl Formeln R-64
                 – Neuer Wert R-55                 – Auswahl Mengen R-57
                 – SZR R-55                        – Auswahl Zuweisung R-68
                 – Text R-55
                 – Ziffer R-55
                 Eingabefeld oben                  M
                 – Formel Editor R-66              Master
                                                   – Mengen Erzeuger R-60
                                                   Maximum
                 F                                 – Formel Editor R-67
                 Formel                            Menge
                 – Formel Editor R-66              – Formel Editor R-66
                 – Stufe I R-10                    – Stufe I R-14
                 – Stufe II R-15                   – Stufe II R-18
                 – Zuweisung Editor R-70           – Stufe III R-19
                 Formel Editor                     – Zuweisung Editor R-70
                 – Anzahl Resultate R-67           Mengen Erzeuger
                 – Beschreibung R-66               – Addup R-61
                 – Dialog R-65                     – All R-60
                 – Eingabefeld oben R-66           – Anychild R-60
                 – Formel R-66                     – Bottom R-60
                 – Maximum R-67                    – Child R-60
                 – Menge R-66                      – Dialog R-58
                 – Minimum R-67                    – Master R-60
                 – Mittelwert R-67                 – Menü R-59
                 – Oder-Verknüpfung R-67           – Parent R-60
                 – Summe R-67                      – Self R-60
                 – Übergebene Menge R-67           – Up R-60
                 – Und-Verknüpfung R-67            – Werkzeugleiste R-60
                 – Vorhandene Eigenschaften R-67   Menü
                 – Vorhandene Formeln R-67
1.02 / 01-2017




                                                   – Bedinungen-Erzeuger R-49
                                                   – Mengen Erzeuger R-59
                 I                                 Minimum
                 Info                              – Formel Editor R-67


                 R-74                                              A+W Production Formeleditor
                 Partindex                                                   Inhalt




                 Mittelwert                     T
                 – Formel Editor R-67           Text
                 Mittleres Auswahlfeld          – Eingabe Zahlenwert R-55
                 – Bedingung R-51
                                                U
                 N                              Übergebene Menge
                 Name der Bedingung             – Bedingung R-54
                 – Alte Bezeichnung R-52        – Formel Editor R-67
                 – Dialog R-52                  – Zuweisung Editor R-70
                 – Neue Bezeichnung R-52        Und-Verknüpfung
                 Name der Menge                 – Formel Editor R-67
                 – Alte Bezeichnung R-62        Unteres Eingabefeld
                 – Dialog R-61                  – Bedingung R-51
                 – Neue Bezeichnung R-62        Up
                 Neue Bedingung                 – Mengen Erzeuger R-60
                 – Auswahl Bedingungen R-47
                 Neue Bezeichnung
                                                V
                 – Name der Bedingung R-52
                                                Vergleich
                 – Name der Menge R-62
                                                – Stufe I R-11
                 Neue Formel
                                                – Stufe II R-16
                 – Auswahl Formeln R-64
                                                Vorhandene Bedingungen
                 Neue Menge
                                                – Auswahl Bedingungen R-47
                 – Auswahl Mengen R-57
                                                Vorhandene Eigenschaften
                 Neue Zuweisung
                                                – Formel Editor R-67
                 – Auswahl Zuweisung R-68
                                                Vorhandene Formeln
                 Neuer Wert
                                                – Auswahl Formeln R-64
                 – Eingabe Zahlenwert R-55
                                                – Formel Editor R-67
                 Normal
                                                Vorhandene Menge
                 – Bedingung R-51
                                                – Auswahl Mengen R-57
                 Null
                                                Vorhandene Zuweisung
                 – Bedinungen-Erzeuger R-50
                                                – Auswahl Zuweisung R-68

                 O                              W
                 Oberes Eingabefeld
                                                Werkzeugleiste
                 – Bedingung R-51
                                                – Bedinungen-Erzeuger R-49
                 Oder-Verknüpfung
                                                – Mengen Erzeuger R-60
                 – Formel Editor R-67
                                                Wert
                 One
                                                – Bedingung R-51
                 – Bedinungen-Erzeuger   R-50

                                                Z
                 P
                                                Ziffer
                 Parent
                                                – Eingabe Zahlenwert R-55
                 – Mengen Erzeuger   R-60
                                                Zuweisung
                                                – Stufe I R-15
                 S                              Zuweisung Editor
                 Self                           – Dialog R-69
                 – Mengen Erzeuger R-60         – Eigenschaft R-69
                 Summe                          – Eingabefeld oben R-69
1.02 / 01-2017




                 – Formel Editor R-67           – Formel R-70
                 SZR                            – Menge R-70
                 – Eingabe Zahlenwert R-55      – Übergebene Menge R-70


                 A+W Production Formeleditor                                 R-75
                 Inhalt                     Partindex
1.02 / 01-2017




                 R-76     A+W Production Formeleditor

