---
description: "DE-HB-AWEnterprise_17"
---


# A+W Enterprise Einkauf
---
## Vorgangsverwaltung

**(CAD-Kennzeichen)** Kennzeichen, ob der Position eine CAD-Datei zugeordnet ist. Wenn eine CAD-Datei angehängt ist, wird das Kennzeichen CAD angezeigt. Bei S/N-Positionen wird der S/N-Code in Klammern hinter dem CAD-Kennzeichen angezeigt.
**Technische Info:** Anzeigefeld

**(Kostenstelle)** Bezeichnung der Kostenstelle, die der Position zugeordnet ist. Wenn der Position keine Kostenstelle zugeordnet ist, wird die marktpartnerspezifische Kostenstelle herangezogen. Wenn dem Marktpartner auch keine Kostenstelle zugeordnet ist, wird die Hauptkostenstelle herangezogen.
**Technische Info:** Anzeigefeld, DB-Feld: kpos.kostenst

**(Sprossenkennzeichen)** Kennzeichen, ob in der Position Sprossen erfasst sind.
*   **S:** In der Position sind Sprossen erfasst. Der Sprossenaufbau wurde nicht bearbeitet.
*   **E:** In der Position sind Sprossen erfasst. Der Sprossenaufbau wurde im Editor bearbeitet.
*   **(Kein Kennzeichen):** In der Position sind keine Sprossen erfasst.
**Technische Info:** Anzeigefeld

**(Kopfartikel, Artikel)** Bezeichnung des Kopfartikels. Bei Mehrfachgläsern werden neben dem Kopfartikel die Bezeichnungen der einzelnen Gläser angezeigt.
**Technische Info:** Anzeigefelder, DB-Feld: aufstrukt.artbez1

**(Austausch-, Zusatzartikel, Anzahl1/Anzahl2)** Bezeichnung der Austausch- und Zusatzartikel und Anzahl der Artikel in der Stückliste. Austausch-artikel werden mit einem A, Zusatzartikel mit einem Z vor der Bezeichnung angezeigt. Hinter der Artikelbezeichnung wird angezeigt, wie oft für den Artikel der Wert Breite und wie oft der Wert Höhe berechnet werden muss.
**Technische Info:** Anzeigefelder, DB-Felder: aufstrukt.artbez1, aufstrukt.an-zahl1, aufstrukt.anzahl2

**(Sprossenaustausch-, Sprossenzusatzartikel, Anzahl1/Anzahl2)** Bezeichnung der Sprossenaustausch- und/oder Sprossenzusatzartikel und Anzahl der Sprossen in der Stückliste. Sprossenaustauschartikel werden mit einem A, Sprossenzusatzartikel mit einem Z vor der Bezeichnung angezeigt. Hinter der Sprossenbezeichnung wird die Anzahl der waagerechten und/oder senkrechten Sprossen angezeigt.
**Technische Info:** Anzeigefelder, DB-Felder: aufstrukt.artbez1, aufstrukt.an-zahl1, aufstrukt.anzahl2

## Register Positionen (Info-Bereich – Grafik, Technische Werte)

Im rechten Bereich im Register Positionen werden, abhängig von der System-konfiguration und den Einstellungen, eine der folgenden Informationen angezeigt:

*   Beschaffung, Warengruppe und Modell
*   Technische Werte
*   Verdeckte Maßangaben

Die Informationen werden zu der markiert Position angezeigt.

