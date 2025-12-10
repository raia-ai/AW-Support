---
description: "Error messages and solutions from A+W Enterprise (German) handbook"
---

# A+W Enterprise (German) - Error Messages & Solutions

**Source:** Extracted from de-hb-awenterprise.md  
**Product:** A+W Enterprise (German)  
**Language:** German

This document contains error messages, warnings, and their solutions extracted from the complete product handbook.

---

## Issue 1

```
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
```

---

## Issue 2

```
            Der Inhalt der Dokumentation dient nur der Information und kann jederzeit
            ohne Vorankündigung geändert werden.
            Bei der Zusammenstellung von Texten und Abbildungen wurde mit größter
            Sorgfalt vorgegangen. Trotzdem können Fehler nicht vollständig ausge-
            schlossen werden. Die A+W Software GmbH übernimmt keine Haftung für
            Fehler oder Ungenauigkeiten, es sei denn, diese beruhen auf vorsätzlichem
            oder grobfahrlässigem Handeln.
            Die Beschreibungen in dieser Dokumentation beruhen auf der vollen Ausbau-
            stufe von A+W Enterprise.


```

---

## Issue 3

```
 Hintergrund-Kontrollen ................................... D-1050               Lieferterminänderungs-Protokoll .................... D-1232
Wiedervorlagen ................................................ D-1051           Modellkatalog ................................................. D-1233
Modifikations-Funktionen im Verkauf ............... D-1054                       Modell-Maßangaben ...................................... D-1234
 Vorgangsänderung ........................................ D-1055                Zahlungsverwaltung ....................................... D-1236
                                                                                 Zahlungsplan .................................................. D-1238
Softwarereferenz ............................................ D-1059             Fehlerinformationssystem .............................. D-1240
Übersicht .......................................................... D-1065      Produktionsmonitor ........................................ D-1242
 Menü Verkauf ................................................. D-1066          Technische Werte ............................................. D-1243
 Zusatzmenü ................................................... D-1068           Leistungserklärung ......................................... D-1243
 Infomenü ........................................................ D-1074        Auftragserfassung – Technische Werte .......... D-1244
Suchfunktionen ................................................ D-1076          Stückliste .......................................................... D-1252
```

---

## Issue 4

```
                          systemen. Standardisiert oder individuell können z.B. FIBU, KORE und Cont-
                          rolling Systeme angebunden werden. Auch eine Kopplung mit dem
                          Gestellpool Europe ist möglich
                          Welche Funktionen und Funktionalitäten im Einzelnen zur Verfügung stehen,
                          hängt von der individuellen Konfiguration des A+W Enterprise-Systems ab.
                          Zusätzliche Module können problemlos jederzeit nachträglich integriert wer-
                          den. A+W Enterprise kann als kleines, schlankes System beginnen und nach
                          und nach zum Vollsystem ausgebaut werden.



```

---

## Issue 5

```

                          Eingangs- und Ausgangsschnittstellen
                          Neben der manuellen Erfassung bietet A+W Enterprise auch verschiedene
                          Auftragseingangsschnittstellen, um Kundenaufträge direkt aus deren EDV-
                          System zu übernehmen. Damit werden Erfassungszeiten und etwaige Einga-
                          befehler reduziert, die Kundenbindung dagegen erhöht.
                          Aufträge können mittels der A+W Standardschnittstelle oder individuellen
                          Kundenschnittstellen automatisch entgegen genommen werden.
                          Auch ein lieferantenseitiger Datentransfer kann mit A+W Enterprise erreicht
                          werden. Unter der Voraussetzung, dass sich beim jeweiligen Lieferanten
                          ebenfalls ein A+W Enterprise-System im Einsatz befindet, können auf beque-
```

---

## Issue 6

```


                       Fehlmengenkontrolle
                       Mithilfe der Fehlmengenkontrolle können Sie prüfen, ob alle Stückzahlen einer
                       Position bzw. eines Vorgangs verpackt sind und für den Versand bereitstehen.
                       Gegebenenfalls können Sie die Mengen ändern, wenn z. B. Barcodes fehler-
                       haft eingelesen wurden. Sie können einen Lieferschein erst dann erstellen,
                       wenn die gesamte Stückzahl eines Vorgangs als Verpackt gemeldet ist.


                       Lieferschein
```

---

## Issue 7

```
                     Technische Info: Toggle-Feld, DB-Feld: mp.objlimitpruef

                     Firmenlimit Dieses Feld kommt nur zum Tragen, wenn das Feld Limitprü-
                     fung auf J gesetzt ist. Überschreitet ein Auftragswert zuzüglich der offenen
                     Posten und des offenen Auftragsbestandes das an dieser Stelle hinterlegte
                     Firmenlimit, so erfolgt eine Warnung.
                     Technische Info: Numerisches Feld, DB-Feld: mp.firmlimit

                     MWST Auswahl des Mehrwertsteuerkennzeichens. Die benötigten Steuer-
                     schlüssel werden im Menü Steuertypen (Schlüssel > System > Steuern) hin-
                     terlegt.
```

---

## Issue 8

```

                     Abb. B-228    Beispiel für Einbaupositionen


                     Ist die Einbauposition für VSG-Folien nicht angegeben, weist A+W Enterprise
                     darauf hin und es führt zu einem Fehler in der Vorgangserfassung.
                     In der Systemeinstellung kann konfiguriert werden, dass die Stückliste ohne
                     Korrektur nicht verlassen werden darf.
                     Dieses Feld wird im Stücklisteneditor angezeigt.
                     Technische Info: Numerisches Feld, DB-Feld: strukt.pos

```

---

## Issue 9

```
                    Austausch und Bearbeitungen gelten. Das PLKZ selbst enthält keine Preise.
                    •   Das PLKZ ist durch eine Nummer, eine Bezeichnung und eine Währung
                        definiert.
                    •   Die PLKZ werden verwendet, um Preislisten zu sortieren.
                    •   Die Nummerierung ist aufsteigend.
                    Damit die Suche nach einem Preis fehlerfrei funktioniert, sollten Sie Num-
                    mernkreise für die einzelnen Preislisten/Glasarten festlegen, z. B. 1000 - 1999
                    für Float, 2000 - 2999 für Gussglas usw.

                            D                                 E

```

---

## Issue 10

```
                       welches PLKZ zur Preisberechnung herangezogen werden soll.
                       Über die Preislistensteuerung wird eingestellt, aus welcher Preisliste ein Preis
                       gezogen wird, wenn in der zugeordneten Preisliste kein Preis gefunden wur-
                       de.
                       Wenn in der Vorgangsverwaltung im Sinne der eingestellten PLKZ-Logik kein
                       Preis gefunden wird, wird eine Fehlermeldung ausgegeben.
                       In fast allen Dialogen, die zur Preisfindung herangezogen werden, können Sie
                       ein PLKZ angeben, ab dem der Preis gilt. Die Ab-PLKZ-Logik gilt für alle Dia-
                       loge getrennt, in denen ein Ab-PLKZ angegeben werden kann.
                       Die Ab-PLKZ-Logik kann in Einzelfällen übersteuert werden. Dazu steht der
                       Dialog Preislistensteuerung zur Verfügung:
```

---

## Issue 11

```

                                Keine Ab-PLKZ-Logik
                                Die Ab-PLZK-Logik wird bei Matrizen nicht angewendet. Darum muss für
                                jede Matrixnummer in allen relevanten Preislistenkennzeichen (PLKZ) eine
                                separate Matrix definiert werden. Wenn keine Matrix vorhanden ist, wird im
                                Auftrag eine Fehlermeldung angezeigt.

                             Die Nummer für eine neue Matrix wird als Schlüssel im Dialog Matrizen ange-
                             legt.
                              “Matrizen” auf Seite C-698
                             Eine neue Matrix können Sie entweder über die Definition der Grenzwerte an-
```

---

## Issue 12

```
             Wenn die Umgebungsvariable ISOAUST_ABPLKZ entsprechend konfiguriert
             ist und die Austauschpreise gezogen werden, können folgende Meldungen
             angezeigt werden:
             • Eine Meldung mit dem PLKZ wird angezeigt, aus dem der Austauschpreis
                 gezogen wurde.
             • Eine Fehlermeldung wird angezeigt, weil kein Austauschpreis in den aus-
                 gewählten PLKZs gefunden werden konnte. Der Austauschpreis wird nicht
                 zur Berechnung herangezogen und auf 0 gesetzt.
             Technische Info: numerisches Feld, DB-Feld: isoaust.pkz

             Feldbeschreibungen
```

---

## Issue 13

```


            So können Sie den Auftrag zwischenspeichern
              Besonders bei größeren Aufträgen mit mehreren Positionen oder bei auf-
              wändigen Erfassungen ist ratsam den betroffenen Auftrag zwischenzu-
              speichern. Der Vorteil an dieser Stelle ist, sofern ein Problem auftritt, wird
              bei einem Neustart auf den gesicherten Zustand zurückgegriffen.
           1 Erfassen Sie einen Auftragskopf bis zu der Stelle, an der Ihnen die Siche-
             rung sinnvoll erscheint. Es muss jedoch mindestens eine Position vollstän-
             dig erfasst werden, damit die Schaltfläche Sichern automatisch aktiviert
             wird.
```

---

## Issue 14

```
             ben.
           3 Sofern ein Auftrag vollständig erfasst und gespeichert wird, wird das
             kauf.still=-3 gesetzt und der Auftrag wird dem Hintergrundprozess intauf
             zur weiteren Bearbeitung vorgelegt. Alternativ kann der erfasste Auftrag
             auch in den Freischaltpool gestellt werden.
           4 Im Falle, dass die Erfassung durch ein technisches Problem abgebrochen
             wurde, so dass anschließend A+W Enterprise neue gestartet werden
             muss, bietet das Programm folgende Möglichkeit:
              •   Beim Starten der Auftragserfassung bekommen Sie einen Hinweis,
                  dass noch Vorgänge existieren, deren Erfassung noch nicht abge-
                  schlossen ist.
```

---

## Issue 15

```
                         In der Regel wird der Auftragserfasser (kauf.eusr) über die Änderung infor-
                         miert. Wenn Sie den E-Mail-Versand konfigurieren, bekommt der Mitarbeiter
                         eine E-Mail.
                         Im Weiteren kann das System so konfiguriert werden, dass Auftragsänderun-
                         gen, die durch das System vorgenommen werden, wie z. B., Liefertermin-Ver-
                         schiebung, oder fehlerhafte Einlastung) nicht an den Auftragserfasser gehen,
                         sondern an den Mitarbeiter, der die letzte Änderung am Auftrag vorgenommen
                         hat. Dadurch wird die Informationskette übersichtlicher gestaltet.


                          So ändern Sie einen bestehenden Auftrag
```

---

## Issue 16

```

           Nutzen

           • Die Funktionen auf der Positionsebene dienen zur schnelleren und sicheren
             Auftragserfassung. Auf der Positionsebene werden einzelne Produkte erfasst, die
             der Kunde bestellt. Die Vermeidung von Erfassungsfehlern reduzieren mögliche
             Fehlproduktionen.


           Merke

```

---

## Issue 17

```

                         listennummer kann geändert werden. Sie können die Stückliste auch anzei-
                         gen und bearbeiten.
                          Stammdaten, “Stückliste” auf Seite B-485
                         Alle Änderungen an der Stückliste müssen sorgfältig durchgeführt werden.
                         Fehlerhafte Handlungen können zu weiteren Problemen bis hin zum Program-
                         mabsturz führen.
                         Das Kapitel Stücklisten bearbeiten umfasst folgende Informationen:
                          Verkauf, “Allgemeine Arbeitsschritte in der Stückliste” auf Seite D-1018
                          Verkauf, “Komplexe Handlungsschritte im Stücklisteneditor” auf Seite D-1020

```

---

## Issue 18

```
Tutorial                                                                                      Aufträge




                         sung im Hintergrund. Preisänderungen sind anschließend problemlos
                         möglich.
                          Softwarereferenz, “Preislose Erfassung” auf Seite D-1133
                         Sie haben die Möglichkeit, eine kundenindividuelle Abfrage von Preisen
                         durchzuführen, ohne dass ein Vorgang (Angebot, Auftrag) angelegt und abge-
                         speichert wird.
```

---

## Issue 19

```
                        Der Menüpunkt Kontrollen gliedert sich in die Untermenüpunkte Erfassungs-
                        und Hintergrundkontrolle.
                        Die Erfassungskontrolle präsentiert die bestehenden Aufträge in textueller
                        Form. Dabei werden vor allem die preisrelevanten Daten der jeweiligen Posi-
                        tionen detailliert dargestellt.
                        Die Hintergrundkontrolle beinhaltet ein Fehlerinformationssystem, das alle
                        Aufträge listet, bei denen Bearbeitungsfehler durch Hintergrundprozesse auf-
                        getreten sind. Zur Korrektur können Sie den betreffenden Auftrag direkt aufru-
                        fen und nachbearbeiten.
                         Softwarereferenz, “Recherche zu Vorgängen” auf Seite D-1445

```

---

## Issue 20

```
                        und Hintergrundkontrolle.
                        Die Erfassungskontrolle präsentiert die bestehenden Aufträge in textueller
                        Form. Dabei werden vor allem die preisrelevanten Daten der jeweiligen Posi-
                        tionen detailliert dargestellt.
                        Die Hintergrundkontrolle beinhaltet ein Fehlerinformationssystem, das alle
                        Aufträge listet, bei denen Bearbeitungsfehler durch Hintergrundprozesse auf-
                        getreten sind. Zur Korrektur können Sie den betreffenden Auftrag direkt aufru-
                        fen und nachbearbeiten.
                         Softwarereferenz, “Recherche zu Vorgängen” auf Seite D-1445


```

---

## Issue 21

```
           Lieferterminänderungs-Protokoll ................................................................... D-1232
           Modellkatalog ................................................................................................ D-1233
           Modell-Maßangaben ..................................................................................... D-1234
           Zahlungsverwaltung ...................................................................................... D-1236
           Zahlungsplan ................................................................................................. D-1238
           Fehlerinformationssystem ............................................................................. D-1240
           Produktionsmonitor ....................................................................................... D-1242
         Technische Werte ............................................................................................. D-1243
           Leistungserklärung ........................................................................................ D-1243
           Auftragserfassung – Technische Werte ......................................................... D-1244
             Berechnete technische Werte .................................................................... D-1244
```

---

## Issue 22

```

    k       Listendruck                          “Listendruck” auf Seite D-1428

     l      Übersicht                            “Untermenü Übersicht” auf Seite D-1068

    m       Hintergrund-Kontrolle                “Fehlerinformationssystem” auf Seite D-1240

    n       Wiedervorlagen                       “Wiedervorlage” auf Seite D-1463

    o       Fertigmeldung                        “Fertigmeldung” auf Seite D-1464

```

---

## Issue 23

```
                         •   “Lieferterminänderungs-Protokoll” auf Seite D-1232
                         •   “Modellkatalog” auf Seite D-1233
                         •   “Modell-Maßangaben” auf Seite D-1234
                         •   “Zahlungsverwaltung” auf Seite D-1236
                         •   “Zahlungsplan” auf Seite D-1238
                         •   “Fehlerinformationssystem” auf Seite D-1240
                         •   “Produktionsmonitor” auf Seite D-1242




```

---

## Issue 24

```
                        wird geprüft, ob die importierten Daten und die Formatvorgaben für die zuge-
                        hörigen Felder im Kopfbereich übereinstimmen. Mit [Nein] können Sie die Fel-
                        der in der ersten Zeile bearbeiten. Mit <Ende> schließen Sie die Bearbeitung
                        ab und die importierten Daten werden geprüft.
                        Wenn die Daten die Vorgaben des jeweiligen Feldes erfüllen, wird vor der Po-
                        sition eine angewählte Checkbox angezeigt. Wenn die Daten fehlerhaft sind,


D-1222                                                                     A+W Enterprise Verkauf
Softwarereferenz                                                                   Vorgangsverwaltung

```

---

## Issue 25

```
Vorgangsverwaltung                                                                     Softwarereferenz




                     Fehlerinformationssystem
                     Verkauf > Hintergrund-Kontrolle > Datum eingeben > <F3>




```

---

## Issue 26

```
                     Verkauf > Hintergrund-Kontrolle > Datum eingeben > <F3>




                     Abb. D-80     Fehlerinformationssystem


                     In diesem Dialog werden bestimmte Bearbeitungsfehler durch den Hinter-
                     grundprozess INTAUF ab dem ausgewählten Datum angezeigt. Die Aufträge,
                     deren Bearbeitung fehlgeschlagen ist, werden in einer Tabelle aufgeführt.
```

---

## Issue 27

```


                     Abb. D-80     Fehlerinformationssystem


                     In diesem Dialog werden bestimmte Bearbeitungsfehler durch den Hinter-
                     grundprozess INTAUF ab dem ausgewählten Datum angezeigt. Die Aufträge,
                     deren Bearbeitung fehlgeschlagen ist, werden in einer Tabelle aufgeführt.
                     •    Mit <F3> starten Sie die Suche.
                     •    Mit den Pfeiltasten und <Bild runter>, <Bild hoch> navigieren Sie in der Ta-
                          belle.
```

---

## Issue 28

```
                     grundprozess INTAUF ab dem ausgewählten Datum angezeigt. Die Aufträge,
                     deren Bearbeitung fehlgeschlagen ist, werden in einer Tabelle aufgeführt.
                     •    Mit <F3> starten Sie die Suche.
                     •    Mit den Pfeiltasten und <Bild runter>, <Bild hoch> navigieren Sie in der Ta-
                          belle.
                     Die folgenden Fehler können angezeigt werden:

                     Fehlernummer Fehlertext                        Bedeutung

                     90                INTAUF fehlerhafter Aufruf   Die Bearbeitung durch INTAUF ist
                                                                    fehlerhaft. Für mehr Informationen
```

---

## Issue 29

```
                     •    Mit <F3> starten Sie die Suche.
                     •    Mit den Pfeiltasten und <Bild runter>, <Bild hoch> navigieren Sie in der Ta-
                          belle.
                     Die folgenden Fehler können angezeigt werden:

                     Fehlernummer Fehlertext                        Bedeutung

                     90                INTAUF fehlerhafter Aufruf   Die Bearbeitung durch INTAUF ist
                                                                    fehlerhaft. Für mehr Informationen
                                                                    können Sie das INTAUF-Protokoll
                                                                    auswerten.
```

---

## Issue 30

```
                          belle.
                     Die folgenden Fehler können angezeigt werden:

                     Fehlernummer Fehlertext                        Bedeutung

                     90                INTAUF fehlerhafter Aufruf   Die Bearbeitung durch INTAUF ist
                                                                    fehlerhaft. Für mehr Informationen
                                                                    können Sie das INTAUF-Protokoll
                                                                    auswerten.

                     91                INTAUF Ladefehler            Das INTAUF konnte den Vorgang
```

---

## Issue 31

```
                     Die folgenden Fehler können angezeigt werden:

                     Fehlernummer Fehlertext                        Bedeutung

                     90                INTAUF fehlerhafter Aufruf   Die Bearbeitung durch INTAUF ist
                                                                    fehlerhaft. Für mehr Informationen
                                                                    können Sie das INTAUF-Protokoll
                                                                    auswerten.

                     91                INTAUF Ladefehler            Das INTAUF konnte den Vorgang
                                                                    nicht laden.
```

---

## Issue 32

```
                     90                INTAUF fehlerhafter Aufruf   Die Bearbeitung durch INTAUF ist
                                                                    fehlerhaft. Für mehr Informationen
                                                                    können Sie das INTAUF-Protokoll
                                                                    auswerten.

                     91                INTAUF Ladefehler            Das INTAUF konnte den Vorgang
                                                                    nicht laden.

                     92                INTAUF Schreibfehler         Das INTAUF konnte den Vorgang
                                                                    nicht speichern.

```

---

## Issue 33

```
                                                                    auswerten.

                     91                INTAUF Ladefehler            Das INTAUF konnte den Vorgang
                                                                    nicht laden.

                     92                INTAUF Schreibfehler         Das INTAUF konnte den Vorgang
                                                                    nicht speichern.

                     93                INTAUF x Versuche            Die Bearbeitung des Vorgangs
                                                                    wurde nach dem x-ten Fehlversuch
                                                                    abgebrochen.
```

---

## Issue 34

```
                                                                    abgebrochen.

                     100               INTAUF Preisdifferent        Der eigene VK-Preis und der EK-
                                                                    DFÜ-Preis sind unterschiedlich.

                     Tab. D-4      Fehleranzeige




D-1240                                                                         A+W Enterprise Verkauf
```

---

## Issue 35

```



                         Kopfbereich

                         Anzeigen ab Datum Startdatum, ab dem nach Fehlern gesucht wird.
                         Technische Info: Datumsfeld

                         Trefferliste
                         In der Trefferliste werden folgende Felder angezeigt:
                         •   Auftrag:
```

---

## Issue 36

```
                         Technische Info: Datumsfeld

                         Trefferliste
                         In der Trefferliste werden folgende Felder angezeigt:
                         •   Auftrag:
                             Nummer des Auftrags, in dem der Fehler aufgetreten ist.
                             Technische Info: Anzeigefeld, DB-Feld: kauferr.auftrnr
                         •   Zähl.:
                             Subnummer, z. B. bei Rechnungen oder Lieferscheinen.
                             Technische Info: Anzeigefeld, DB-Feld: kauferr.subnr
                         •   Vorgang:
```

---

## Issue 37

```
                             Technische Info: Anzeigefeld, DB-Feld: kauferr.subnr
                         •   Vorgang:
                             Art des Vorgangs.
                             Technische Info: Anzeigefeld, DB-Feld: kauferr.vorgang
                         •   Err:
                             Nummer des aufgetretenen Fehlers.
                             Technische Info: Anzeigefeld, DB-Feld: kauferr.errno
                         •   Fehlertext:
                             Informationstext zum aufgetretenen Fehler.
                             Technische Info: Anzeigefeld, DB-Feld: kauferr.txt
                         •   Datum:
```

---

## Issue 38

```
                             Art des Vorgangs.
                             Technische Info: Anzeigefeld, DB-Feld: kauferr.vorgang
                         •   Err:
                             Nummer des aufgetretenen Fehlers.
                             Technische Info: Anzeigefeld, DB-Feld: kauferr.errno
                         •   Fehlertext:
                             Informationstext zum aufgetretenen Fehler.
                             Technische Info: Anzeigefeld, DB-Feld: kauferr.txt
                         •   Datum:
                             Datum, an dem der Fehler aufgetreten ist.
                             Technische Info: Anzeigefeld, DB-Feld: kauferr.datum
```

---

## Issue 39

```
                             Technische Info: Anzeigefeld, DB-Feld: kauferr.vorgang
                         •   Err:
                             Nummer des aufgetretenen Fehlers.
                             Technische Info: Anzeigefeld, DB-Feld: kauferr.errno
                         •   Fehlertext:
                             Informationstext zum aufgetretenen Fehler.
                             Technische Info: Anzeigefeld, DB-Feld: kauferr.txt
                         •   Datum:
                             Datum, an dem der Fehler aufgetreten ist.
                             Technische Info: Anzeigefeld, DB-Feld: kauferr.datum
                         •   Zeit:
```

---

## Issue 40

```
                             Technische Info: Anzeigefeld, DB-Feld: kauferr.errno
                         •   Fehlertext:
                             Informationstext zum aufgetretenen Fehler.
                             Technische Info: Anzeigefeld, DB-Feld: kauferr.txt
                         •   Datum:
                             Datum, an dem der Fehler aufgetreten ist.
                             Technische Info: Anzeigefeld, DB-Feld: kauferr.datum
                         •   Zeit:
                             Uhrzeit, zu der der Fehler aufgetreten ist.
                             Technische Info: Anzeigefeld, DB-Feld: kauferr.zeit
                         Wenn Sie eine Zeile markieren, können Sie mit <F3> den entsprechenden
```

---

## Issue 41

```
                             Technische Info: Anzeigefeld, DB-Feld: kauferr.txt
                         •   Datum:
                             Datum, an dem der Fehler aufgetreten ist.
                             Technische Info: Anzeigefeld, DB-Feld: kauferr.datum
                         •   Zeit:
                             Uhrzeit, zu der der Fehler aufgetreten ist.
                             Technische Info: Anzeigefeld, DB-Feld: kauferr.zeit
                         Wenn Sie eine Zeile markieren, können Sie mit <F3> den entsprechenden
                         Auftrag im Anzeigemodus öffnen.


```

---

## Issue 42

```

                            Anz1=2 – in der Breite werden 2 Kanten bearbeitet.
                            Anz1=1 – in der Höhe wird 1 Kante bearbeitet.

                         Die Felder Anz1 und Anz2 sind für Glasartikel jedoch nicht änderbar, da sonst
                         die fehlerhafte Übergabe an die Produktion erfolgen kann.
                         Technische Info: numerische Felder, DB-Felder: aufstrukt.anzahl1,
                         aufstrukt.anzahl2

                         Br., Hö. Anzahl der Breiten und Höhen der Scheibe, die bearbeitet werden.
                         Die Felder werden bei Kantenbearbeitungen alternativ zu den Feldern Anz1,
```

---

## Issue 43

```
            Dialog zur Angabe der Mandantennummer (Hausnummer). In dem Protokoll
            werden nur die Vorgänge zum ausgewählten Haus angezeigt.

               Lieferscheinprotokoll zu dem aktuellen Tag
               Ein Lieferscheinprotokoll wird zu dem aktuellen Tag erzeugt. Wenn die
               Fehlermeldung angezeigt wird, dass die Datei leer oder nicht lesbar ist,
               dann wurde an diesem Tag noch kein Lieferschein erzeugt.




```

---

## Issue 44

```
                         [Int.Auft.] Verzweigt zu einem internen Auftrag mit eigener Auftragsnummer
                         für die Produktion, wenn dieser existiert und das System entsprechend konfi-
                         guriert ist. Die internen Aufträge können nur erzeugt werden, wenn die Umge-
                         bungsvariable VORGANGSSTATUS_ADHOCSQL aktiv ist und Sie eine
                         eigene Ad-Hoc-SQL eingebunden haben. Wenn die Variable nicht gesetzt ist,
                         wird eine entsprechende Fehlermeldung angezeigt.




A+W Enterprise Verkauf                                                                       D-1431
```

---

## Issue 45

```
                          links angezeigt.
                          Die Schaltflächen sind zum Register Vorgang beschrieben:
                           “Vorgangsinformationen – Vorgang” auf Seite D-1430
                          Zusätzlich wird folgende Schaltfläche angezeigt:

                          [Info] Zeigt die Fehlermeldung aus der Produktion zu der gewählten Position
                          an. Die Schaltfläche ist nur aktiv, wenn zu der gewählten Position eine Fehler-
                          meldung existiert.


                          Vorgangsinformationen – Einkauf
```

---

## Issue 46

```
                          Die Schaltflächen sind zum Register Vorgang beschrieben:
                           “Vorgangsinformationen – Vorgang” auf Seite D-1430
                          Zusätzlich wird folgende Schaltfläche angezeigt:

                          [Info] Zeigt die Fehlermeldung aus der Produktion zu der gewählten Position
                          an. Die Schaltfläche ist nur aktiv, wenn zu der gewählten Position eine Fehler-
                          meldung existiert.


                          Vorgangsinformationen – Einkauf
                          Verkauf > Übersicht > Auftragsinformation > Auftragsnummer angeben
```

---

## Issue 47

```
                            Aufträge/Bestellungen – Filterdialog .......................................................... F-1783
                            Aufträge/Bestellungen – Trefferliste ........................................................... F-1784
                            Aufträge/Bestellungen – Trefferliste-Details ............................................... F-1785
                         Buchungsstatus ............................................................................................ F-1787
                            Buchungsstatus – Ungebucht .................................................................... F-1787
                            Buchungsstatus – Fehler ........................................................................... F-1789
                            Buchungsstatus – Inventur ........................................................................ F-1791
                            Buchungsstatus – Korrektur ....................................................................... F-1792
                         Lagerinformationen – Pickliste ...................................................................... F-1794
                         Lagerinformationen – Trefferliste ................................................................... F-1795
                         LVR-Status .................................................................................................... F-1796
```

---

## Issue 48

```

     i      Buchungsstatus                       Öffnet das Untermenü

    ia      Buchungsstatus - Ungebucht           “Buchungsstatus – Ungebucht” auf Seite F-1787

    ib      Buchungsstatus - Fehler              “Buchungsstatus – Fehler” auf Seite F-1789

    ic      Buchungsstatus - Inventur            “Buchungsstatus – Inventur” auf Seite F-1791

     j      Auftragsliste                        “Lagerinformationen – Pickliste” auf Seite F-1794

```

---

## Issue 49

```
                       In diesem Dialog können Sie die Suchkriterien festlegen, um sich die Buchun-
                       gen anzeigen zu lassen und zu korrigieren.
                       Um Buchungen korrigieren zu können, müssen zuerst Lagerdaten durch das
                       Lagerbuchungssystem angelegt worden sein. Sicherungs-Lagerdaten werden
                       nur angelegt, wenn Zeitpunkte zur automatischen Speicherung der Lagerda-
                       ten definiert werden, z. B. der 15. eines jeden Monats. Fehlerhafte Buchungs-
                       sätze dürfen nicht im Buchungssystem vorhanden sein.
                       Die Details der Übersicht können Sie sich in der Detailansicht anzeigen las-
                       sen.
                        “Buchungskorrektur – Details” auf Seite F-1731
                       Sie können folgende Tastaturbefehle ausführen:
```

---

## Issue 50

```


                       Buchungsstatus
                       Infosystem > Buchungsstatus
                       Im Buchungsstatus können Sie sich die Buchungsinformationen zu den La-
                       gern anzeigen lassen, die nicht gebuchten oder fehlerhaften Buchungssätze
                       enthalten oder Lager die sich gerade in der Inventur befinden. Im Dialog Bu-
                       chungsstatus – Korrektur können Sie die Daten für den Buchungsstatus korri-
                       gieren.
                       Zu diesem Dialog werden folgende Unterdialoge angezeigt:
                       •   Buchungsstatus – Ungebucht
```

---

## Issue 51

```
                       enthalten oder Lager die sich gerade in der Inventur befinden. Im Dialog Bu-
                       chungsstatus – Korrektur können Sie die Daten für den Buchungsstatus korri-
                       gieren.
                       Zu diesem Dialog werden folgende Unterdialoge angezeigt:
                       •   Buchungsstatus – Ungebucht
                       •   Buchungsstatus – Fehler
                       •   Buchungsstatus – Inventur
                       •   Buchungsstatus – Korrektur


                       Buchungsstatus – Ungebucht
```

---

## Issue 52

```
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
```

---

## Issue 53

```
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
```

---

## Issue 54

```
Softwarereferenz                                                              Informationssystem




                       Buchungsstatus – Fehler
                       Infosystem > Buchungsstatus > Fehler




```

---

## Issue 55

```




                       Buchungsstatus – Fehler
                       Infosystem > Buchungsstatus > Fehler




                       Abb. F-56    Buchungsstatus – Fehler
```

---

## Issue 56

```
                       Infosystem > Buchungsstatus > Fehler




                       Abb. F-56    Buchungsstatus – Fehler


                       In diesem Dialog können Sie sich Buchungsinformationen zu den Lagern an-
                       zeigen lassen, die fehlerhafte Buchungssätze enthalten. Im Dialog Buchungs-
                       status – Korrektur können Sie die Daten für den Buchungsstatus korrigieren.
```

---

## Issue 57

```

                       Abb. F-56    Buchungsstatus – Fehler


                       In diesem Dialog können Sie sich Buchungsinformationen zu den Lagern an-
                       zeigen lassen, die fehlerhafte Buchungssätze enthalten. Im Dialog Buchungs-
                       status – Korrektur können Sie die Daten für den Buchungsstatus korrigieren.
                       Sie können folgende Tastaturbefehle ausführen:
                       •   Mit <F5> können Sie den Dialog Buchungsstatus – Korrektur aufrufen.
                       •   Mit <F2> können Sie sich weitere Spalten anzeigen lassen.

```

---

## Issue 58

```
                           Nummer der Artikelfarbe.
                       •   Anzahl:
                           Anzahl der nicht gebuchten Artikel.
                       •   Status:
                           Nummer des Status der aktuellen Buchung, z. B. Lagerausgang.
                       •   Fehler:
                           Nummer für den Fehlerstatus. Der Fehlerstatus steht im Fußbereich im
                           Klartext.



```

---

## Issue 59

```
                       •   Anzahl:
                           Anzahl der nicht gebuchten Artikel.
                       •   Status:
                           Nummer des Status der aktuellen Buchung, z. B. Lagerausgang.
                       •   Fehler:
                           Nummer für den Fehlerstatus. Der Fehlerstatus steht im Fußbereich im
                           Klartext.




```

---

## Issue 60

```

                       Abb. F-57    Buchungsstatus – Inventur


                       In diesem Dialog können Sie sich Buchungsinformationen zu den Lager an-
                       zeigen lassen, die nicht gebuchten oder fehlerhaften Buchungssätze enthal-
                       ten oder Lager die sich gerade in der Inventur befinden. Im Dialog
                       Buchungsstatus – Korrektur können Sie die Daten für den Buchungsstatus
                       korrigieren.

                           Lager in Inventur
```

---

## Issue 61

```
                         Mitarbeiternummer des Mitarbeiters, der das Lager zur Inventur vorbereitet
                         hat.


                     Buchungsstatus – Korrektur
                     Infosystem > Buchungsstatus > Ungebucht, Fehler, Inventur > <F5>




                     Abb. F-58    Buchungsstatus – Korrektur
```

---

## Issue 62

```


                     In diesem Dialog können Sie die Daten des Buchungsstatus der folgenden Di-
                     aloge korrigieren:
                     •   Buchungsstatus – Ungebucht
                     •   Buchungsstatus – Fehler
                     •   Buchungsstatus – Inventur

                     Rumpfbereich

                     Artikel Artikelnummer und Artikelbezeichnung.
```

---

## Issue 63

```

                       Artikel Artikelbezeichnung.

                       Lager Lagerbezeichnung.

                       Fehler Fehlerstatus im Klartext.

                       Status Status der aktuellen Buchung im Klartext, z. B. Lagerausgang.



```

---

## Issue 64

```

                       Abb. F-69    Lager-Preiskorrektur


                       In diesem Dialog können Sie den Durchschnittspreis für eingekaufte Lagerar-
                       tikel korrigieren. Fehlerhafte Preisbuchungen für Lagerartikel verfälschen den
                       Durchschnittspreis in der Statistik und können nur über den Höchstpreis und
                       den Niedrigstpreis korrigiert werden.

                       Artikel Artikelnummer.

```

---

## Issue 65

```
                      die Sicherung auch für andere Tage festlegen: gültige Einstellungen sind
                      zwischen 1 und 31, wobei 31 immer der letzte Tag im Monat ist und wird
                      automatisch an den Monat angepasst (28(29), 30 oder 31).

                      Zu dem Zeitpunkt der Sicherung dürfen keine Lagerinventuren und keine
                      fehlerhafte Buchungen offen sein, ansonsten kann die Sicherung nicht
                      durchgeführt werden. Im Erfolgsfall sowie auch im Fehlerfall kann ein zu-
                      ständige Mitarbeiter per E-Mail über das Ergebnis informiert werden. Bitte
                      sprechen Sie einen A+W Mitarbeiter für die korrekte Systemeinstellung
                      dieser Funktion an.

```

---

## Issue 66

```
                      zwischen 1 und 31, wobei 31 immer der letzte Tag im Monat ist und wird
                      automatisch an den Monat angepasst (28(29), 30 oder 31).

                      Zu dem Zeitpunkt der Sicherung dürfen keine Lagerinventuren und keine
                      fehlerhafte Buchungen offen sein, ansonsten kann die Sicherung nicht
                      durchgeführt werden. Im Erfolgsfall sowie auch im Fehlerfall kann ein zu-
                      ständige Mitarbeiter per E-Mail über das Ergebnis informiert werden. Bitte
                      sprechen Sie einen A+W Mitarbeiter für die korrekte Systemeinstellung
                      dieser Funktion an.

                   Datum Datum der letzten Sicherung.
```

---

## Issue 67

```
    Workflow
1 Menü Buchung > Eingang wählen.                                Buchung prüfen:
     Dialog Lagereingang wird geöffnet.                        7 Menü Infosystem > Buchungsstatus > Ungebucht: Nicht
                                                                 gebuchte Buchungen.
2 Artikel und Lager wählen.
                                                               8 Menü Infosystem > Buchungsstatus > Fehler: Fehlerhaf-
3 Artikelvariante, Artikelmenge und Einkaufspreis pro
                                                                 te Buchungen.
  Stück oder pro Mengeneinheit eingeben.
                                                               9 Menü Infosystem > Historie > Filterkriterium eingeben >
     Gesamtpreis der Position wird angezeigt.
```

---

## Issue 68

```
    Workflow
1 Menü Buchung > Ausgang wählen.                                Buchung prüfen:
     Dialog Lagerausgang wird geöffnet.                        7 Menü Infosystem > Buchungsstatus > Ungebucht: Nicht
                                                                 gebuchte Buchungen.
2 Artikel und Lager wählen.
                                                               8 Menü Infosystem > Buchungsstatus > Fehler: Fehlerhaf-
3 Artikelvariante und Artikelmenge in Stückzahl oder Men-
                                                                 te Buchungen.
  geneinheit eingeben.
                                                               9 Menü Infosystem > Historie > Filterkriterium eingeben >
     Gesamtpreis der Position wird angezeigt.
```

---

## Issue 69

```
    Workflow
1 Menü Buchung > Facheingang wählen.                            Buchung prüfen:
     Dialog Fachlagereingang wird geöffnet.                    7 Menü Infosystem > Buchungsstatus > Ungebucht: Nicht
                                                                 gebuchte Buchungen.
2 Artikel und Lager wählen.
                                                               8 Menü Infosystem > Buchungsstatus > Fehler: Fehlerhaf-
3 Artikelvariante, Artikelmenge und Einkaufspreis pro
                                                                 te Buchungen.
  Stück oder pro Mengeneinheit eingeben.
                                                               9 Menü Infosystem > Historie > Filterkriterium eingeben >
     Gesamtpreis der Position wird angezeigt.
```

---

## Issue 70

```
    Workflow
1 Menü Buchung > Fachausgang wählen.                            Buchung prüfen:
     Dialog Fachlagerausgang wird geöffnet.                    7 Menü Infosystem > Buchungsstatus > Ungebucht: Nicht
                                                                 gebuchte Buchungen.
2 Artikel und Lager wählen.
                                                               8 Menü Infosystem > Buchungsstatus > Fehler: Fehlerhaf-
3 Artikelvariante und Artikelmenge in Stückzahl oder Men-
                                                                 te Buchungen.
  geneinheit eingeben.
                                                               9 Menü Infosystem > Historie > Filterkriterium eingeben >
     Gesamtpreis der Position wird angezeigt.
```

---

## Issue 71

```
    Workflow
1 Menü Buchung > Kisteneingang wählen.                          Buchung prüfen:
     Dialog Kistenlagereingang wird geöffnet.                  8 Menü Infosystem > Buchungsstatus > Ungebucht: Nicht
                                                                 gebuchte Buchungen.
2 Artikel und Kistenlager wählen.
                                                               9 Menü Infosystem > Buchungsstatus > Fehler: Fehlerhaf-
3 Artikelvariante wählen.
                                                                 te Buchungen.
4 Kistenbezeichnung und Verpackungsart eingeben.
                                                               10 Menü Infosystem > Historie > Filterkriterium eingeben >
5 Artikelmenge und Artikelpreis des Lieferanten eingeben.         <F3>.
```

---

## Issue 72

```
1 Menü Buchung > Kistenausgang wählen.                             Kisten werden vom Lager abgebucht.
     Dialog Kistenlagerausgang wird geöffnet.                   Buchung prüfen:
2 Artikel und Kistenlager wählen.                              8 Menü Infosystem > Buchungsstatus > Ungebucht: Nicht
                                                                 gebuchte Buchungen.
3 Kiste mit der entsprechenden Artikelvariante wählen und
  <F4> drücken.                                                9 Menü Infosystem > Buchungsstatus > Fehler: Fehlerhaf-
                                                                 te Buchungen.
     Zusatzmenü wird angezeigt.
                                                               10 Menü Infosystem > Historie > Filterkriterium eingeben >
4 Menü Kisten > Kiste abbuchen wählen.
                                                                  <F3>.
```

---

## Issue 73

```
     gaben im Fußbereich wechseln.                              werden.
•    Mit <Strg> + <E> die Einzelblattinformationen bearbei-      Buchungskorrektur buchen
     ten.

    Workflow
1 Menü Buchung > Kisteneingang wählen.                          10 Menü Infosystem > Buchungsstatus > Fehler: Fehlerhaf-
                                                                   te Buchungen.
     Dialog Kistenlagereingang wird geöffnet.
                                                                11 Menü Infosystem > Historie > Filterkriterium eingeben >
2 Artikel und Einzelblattkistenlager wählen.
                                                                   <F3>.
```

---

## Issue 74

```
1 Menü Buchung > Kistenausgang wählen.                            6 Mit [OK] führen Sie die Buchung aus.
     Dialog Kistenlagerausgang wird geöffnet.                      Buchung prüfen:
2 Artikel und Einzelblattkistenlager wählen.                      7 Menü Infosystem > Buchungsstatus > Ungebucht: Nicht
                                                                    gebuchte Buchungen.
3 Variante wählen.
                                                                  8 Menü Infosystem > Buchungsstatus > Fehler: Fehlerhaf-
4 Mit <Strg> + <E> in die Einzelblattinformationen wech-
                                                                    te Buchungen.
  seln.
                                                                  9 Menü Infosystem > Historie > Filterkriterium eingeben >
5 Mit <F7> einzelne Positionen löschen.
```

---

## Issue 75

```
    Workflow
1 Menü Buchung > Gestelleingang wählen.                         Buchung prüfen:
     Dialog Gestelllagereingang wird geöffnet.                 9 Menü Infosystem > Buchungsstatus > Ungebucht: Nicht
                                                                 gebuchte Buchungen.
2 Entweder Artikel und Gestelllager oder das Gestell wäh-
  len.                                                         10 Menü Infosystem > Buchungsstatus > Fehler: Fehlerhaf-
                                                                  te Buchungen.
3 Artikelvariante wählen.
                                                               11 Menü Infosystem > Historie > Filterkriterium eingeben >
4 Gestell wählen oder neues Gestell anlegen.
                                                                  <F3>.
```

---

## Issue 76

```
    Workflow
1 Menü Buchung > Gestellausgang wählen.                             Artikel werden vom Gestelllager abgebucht.
     Dialog Gestelllagerausgang wird geöffnet.                   Buchung prüfen:
2 Entweder Artikel und Gestelllager wählen oder das Ge-         10 Menü Infosystem > Buchungsstatus > Ungebucht: Nicht
  stell.                                                           gebuchte Buchungen.
3 Register Auftragsbezogen wählen.                              11 Menü Infosystem > Buchungsstatus > Fehler: Fehlerhaf-
                                                                   te Buchungen.
4 Variante auf dem Gestell wählen.
                                                                12 Menü Infosystem > Historie > Filterkriterium eingeben >
5 Buchungsmenge der Variante in Mengeneinheit einge-
                                                                   <F3>.
```

---

## Issue 77

```
    Workflow
1 Menü Buchung > Gestellausgang wählen.                             Artikel werden vom Gestelllager abgebucht.
     Dialog Gestelllagerausgang wird geöffnet.                   Buchung prüfen:
2 Entweder Artikel und Gestelllager wählen oder das Ge-         10 Menü Infosystem > Buchungsstatus > Ungebucht: Nicht
  stell.                                                           gebuchte Buchungen.
3 Register Umbuchung wählen.                                    11 Menü Infosystem > Buchungsstatus > Fehler: Fehlerhaf-
                                                                   te Buchungen.
4 Variante auf dem Gestell wählen.
                                                                12 Menü Infosystem > Historie > Filterkriterium eingeben >
5 Buchungsmenge der Variante in Mengeneinheit einge-
                                                                   <F3>.
```

---

## Issue 78

```
    Workflow
1 Menü Buchung > Ausgang (Auftragsbezogen) wählen.              Buchung prüfen:
     Dialog Lagerausgang (Auftragsbezogen) wird geöffnet.      7 Menü Infosystem > Buchungsstatus > Ungebucht: Nicht
                                                                 gebuchte Buchungen.
2 Auftrag wählen.
                                                               8 Menü Infosystem > Buchungsstatus > Fehler: Fehlerhaf-
     Positionen des Auftrags werden angezeigt.
                                                                 te Buchungen.
3 Position des Auftrags zum Ausbuchen wählen.
                                                               9 Menü Infosystem > Historie > Filterkriterium eingeben >
4 Stückzahl des Artikels eingeben.                               <F3>.
```

---

## Issue 79

```
    Workflow
1 Menü Buchung > Stapeleingang wählen.                        Buchung prüfen:
     Dialog Stapellagereingang wird geöffnet.                7 Menü Infosystem > Buchungsstatus > Ungebucht: Nicht
                                                               gebuchte Buchungen.
2 Stapellager und Lieferant wählen.
                                                             8 Menü Infosystem > Buchungsstatus > Fehler: Fehlerhaf-
3 Mit <Shift> + <F8> eine neue Stapelnummer anlegen.
                                                               te Buchungen.
4 Artikelvariante, Artikelmenge und Einkaufspreis pro
                                                             9 Menü Infosystem > Historie > Filterkriterium eingeben >
  Stück oder pro Mengeneinheit eingeben.
```

---

## Issue 80

```
     Dialog Stapellageränderung wird geöffnet.               Artikel des Stapels werden in das Ziellager gebucht.
2 Filterkriterien eingeben.                               Buchung prüfen:
     Vorhandene Stapel werden angezeigt.                 11 Menü Infosystem > Buchungsstatus > Ungebucht: Nicht
                                                            gebuchte Buchungen.
3 Stapel wählen und neue Gesamtmenge im Feld Anzahl
  eingeben.                                              12 Menü Infosystem > Buchungsstatus > Fehler: Fehlerhaf-
                                                            te Buchungen.
4 Buchung mit <Ende> bestätigen.
                                                         13 Menü Infosystem > Historie > Filterkriterium eingeben >
     Stapel wird auf die eingegebene Menge gesetzt.
                                                            <F3>.
```

---

## Issue 81

```
    Workflow
1 Menü Buchung > Korrektur wählen.                             Buchungen prüfen:
     Dialog Buchungskorrektur wird geöffnet.                  6 Menü Infosystem > Buchungsstatus > Ungebucht: Nicht
                                                                gebuchte Buchungen.
2 Filterkriterien eingeben.
                                                              7 Menü Infosystem > Buchungsstatus > Fehler: Fehlerhaf-
     Trefferliste der Suche wird angezeigt.
                                                                te Buchungen.
3 Mengen / Anzahl und / oder Preis in den Spalten korrigie-
                                                              8 Menü Infosystem > Historie > Filterkriterium eingeben >
  ren.
```

---

## Issue 82

```
                                         einsehen.

• Aufträge / Bestellungen einsehen     • Informationen zu auftrags- und bestellbezogenen
                                         Buchungen einsehen.

• Buchungsstatus einsehen              • Nicht gebuchte oder fehlerhafte Buchungen einsehen
                                         und korrigieren.
                                       • Übersicht für alle Lager in Inventur aufrufen.

• Dispositiven Lagerbestand einsehen   • Bestellten, verplanten und verfügbaren Lagerbestand
                                         einsehen.
```

---

## Issue 83

```




    Ziel der Handlung
•    Nicht gebuchte oder fehlerhafte Buchungen einsehen      •   Übersicht für alle Lager in Inventur aufrufen.
     und korrigieren.

    Voraussetzungen


```

---

## Issue 84

```
    Voraussetzungen



    Zusatzinfo
Informationen zum Buchungsstatus für fehlerhafte Daten-      folgenden Dialogen aufgelistet: Infosystem > Buchungssta-
sätze und für die Inventur werden in der gleichen Weise in   tus > Fehler, Inventur.

    Workflow
1 Menü Infosystem > Buchungsstatus > Ungebucht wäh-          3 Daten korrigieren.
  len.
```

---

## Issue 85

```



    Zusatzinfo
Informationen zum Buchungsstatus für fehlerhafte Daten-      folgenden Dialogen aufgelistet: Infosystem > Buchungssta-
sätze und für die Inventur werden in der gleichen Weise in   tus > Fehler, Inventur.

    Workflow
1 Menü Infosystem > Buchungsstatus > Ungebucht wäh-          3 Daten korrigieren.
  len.
                                                             4 Mit <Strg> + <F8> nach der Korrektur der Fehlerursache
```

---

## Issue 86

```
sätze und für die Inventur werden in der gleichen Weise in   tus > Fehler, Inventur.

    Workflow
1 Menü Infosystem > Buchungsstatus > Ungebucht wäh-          3 Daten korrigieren.
  len.
                                                             4 Mit <Strg> + <F8> nach der Korrektur der Fehlerursache
     Dialog Buchungsstatus für ungebuchte Datensätze wird      den Fehlerstatus zurücksetzen.
     geöffnet.
                                                             5 Mit <Shift> + <F8> den Lagerbucher aktivieren.
2 Mit <F5> die Detailansicht des ausgewählten Datensat-
                                                             6 Mit <Ende> Korrektur speichern.
```

---

## Issue 87

```

    Workflow
1 Menü Infosystem > Buchungsstatus > Ungebucht wäh-          3 Daten korrigieren.
  len.
                                                             4 Mit <Strg> + <F8> nach der Korrektur der Fehlerursache
     Dialog Buchungsstatus für ungebuchte Datensätze wird      den Fehlerstatus zurücksetzen.
     geöffnet.
                                                             5 Mit <Shift> + <F8> den Lagerbucher aktivieren.
2 Mit <F5> die Detailansicht des ausgewählten Datensat-
                                                             6 Mit <Ende> Korrektur speichern.
  zes öffnen.
```

---

## Issue 88

```


                      Funktionstest (F-Test) starten
                      <Strg> + <F4> > <Shift> + <F12> > <9> > [Nein]
                      Mit dieser Tastenfolge starten Sie den Funktionstest. Die Service-Techniker
                      benötigen die Protokollierung der Programmabläufe, um im Problemfall die
                      Fehlerquellen zu finden. Beachten Sie folgende Punkte zum Funktionstest:
                      •   Nur auf Anweisung der Service-Techniker einschalten.
                      •   Nach dem Start wird jede Aktion der Software protokolliert.
                      •   Verbraucht zusätzliche Rechenkapazität und zusätzliche Festspeicherka-
                          pazität.
```

---

## Issue 89

```

                      Funktionstest (F-Test) starten
                      <Strg> + <F4> > <Shift> + <F12> > <9> > [Nein]
                      Mit dieser Tastenfolge starten Sie den Funktionstest. Die Service-Techniker
                      benötigen die Protokollierung der Programmabläufe, um im Problemfall die
                      Fehlerquellen zu finden. Beachten Sie folgende Punkte zum Funktionstest:
                      •   Nur auf Anweisung der Service-Techniker einschalten.
                      •   Nach dem Start wird jede Aktion der Software protokolliert.
                      •   Verbraucht zusätzliche Rechenkapazität und zusätzliche Festspeicherka-
                          pazität.
                      •   Kann zusammen mit der Datenbankprotokollierung durchgeführt werden.
```

---

## Issue 90

```
– Verschiedenes E-1592             – offene Buchungen bearbeiten F-1729, F-1731
– Zahlungsoption E-1592            Buchungsprotokoll
Bestellkopplung A-24, A-30         – erstellen, für Verpackte Menge G-1960
Bestellpool A-34                   – Fertigwarenlager G-2004
Bestellte Bearbeitungen            Buchungsstatus
– Erfassen bzw. ändern B-364       – Fehler F-1789
Bestellung                         – Inventur F-1791
– Bestellart E-1622                – Korrektur F-1792
– Lieferant, erzeugen für E-1564   – nicht gebuchte Buchungssätze F-1787
– Position, erzeugen zur E-1568
– Position,Details zur E-1569      C
```

---

## Issue 91

```


A+W Enterprise                                                                  Z-2047
– Anmerkungstext D-1304                      – Grundpreise C-711
– Auftragsanzeige D-1461                     – Gussaustausch C-735
– Fehler D-1240                              – Gussklassen C-734
– Marktpartner D-1197                        – Matrix-Editor C-722
Informationssystem A-35                      – Matrizen umrechnen C-731
Infosystem                                   – Mindestpreis C-720
– Aufträge/Bestellungen F-1783, F-1784,      – Staffelpreise C-720
  F-1785                                     – Stammdaten C-710
```

---

## Issue 92

```
Informationssystem A-35                      – Matrizen umrechnen C-731
Infosystem                                   – Mindestpreis C-720
– Aufträge/Bestellungen F-1783, F-1784,      – Staffelpreise C-720
  F-1785                                     – Stammdaten C-710
– Bestandsprognose F-1800                    – SZR-Zuschläge C-743
– Buchungsstatus, Fehler F-1789              – UV-Abdeckung C-745
– Buchungsstatus, Inventur F-1791            iTOE
– Buchungsstatus, Korrektur F-1792           – Position bearbeiten D-1028, D-1031
– Buchungsstatus, nicht gebuchte             – Position erfassen D-1028, D-1031
  Buchungssätze F-1787                       iTOE - Austauschregeln B-359
– Dispositiver Bestand F-1798
```

---

