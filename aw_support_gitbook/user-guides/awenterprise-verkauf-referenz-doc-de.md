---
description: "DE_AWEnterprise_Verkauf_4_7"
---


# Softwarereferenz: Preise und Konditionen

---
## Verkauf und Einkauf

### Staffelstufe
Preisstufe, aus der der Preis verwendet wird. Das Feld wird von der Preisberechnung nur ausgewertet, wenn für den relevanten Artikelpreis-vektor die Preisart 2 – Staffelstufe angegeben ist.
**Technische Info:** numerische Felder, DB-Felder: pokokon.flag1, pokokon.ekflag1

### TZ
Teuerungszuschlag in Prozent. Der Teuerungszuschlag wird auf den Men-geneinheitspreis aufgeschlagen. Wenn Sie den Wert 0 oder einen Wert <0 eintragen, wird kein Teuerungszuschlag berechnet.
**Technische Info:** numerische Felder, DB-Felder: pokokon.zu3, pokokon.zuk3

### Faktor
Faktor des Preiszuschlags in Prozent. Über den Faktor können Sie die Preisberechnung für den Artikel ändern, ohne alle Preise anpassen zu müssen, z. B. für Preiserhöhungen oder Rabatte. In der Regel wird mit einem Faktor ein Rabatt gewährt.
**Technische Info:** numerische Felder, DB-Felder: pokokon.zu4, pokokon.zuk4

### Scheibe €/qm
Preis pro Quadratmeter für die jeweilige Scheibe.
- **Verkauf:**
  Verkaufspreis pro Quadratmeter für die nebenstehende Scheibe.
  **Technische Info:** numerische Felder, DB-Felder: pokokon.zu6, pokokon.zu8, pokokon.zu10, pokokon.zu12, pokokon.zu14, pokokon.zu16, pokokon.zu18
- **Einkauf:**
  Einkaufspreis pro Quadratmeter für die nebenstehende Scheibe.
  **Technische Info:** numerische Felder, DB-Felder: pokokon.zuk6, pokokon.zuk8, pokokon.zuk10, pokokon.zuk12, pokokon.zuk14, pokokon.zuk16, pokokon.zuk18

### Zuschlag
Zuschlag, der auf den Preis erhoben wird. Im zweiten Feld geben Sie den Zuschlagstyp an. Der Zuschlagstyp gibt an, auf welchen Preis sich der Zuschlag bezieht:
- **WE/Stück:** Der Zuschlag wird als fester Betrag auf den Stückpreis der Position aufge-schlagen.
- **WE/GME:** Der Zuschlag wird auf den Preis pro Grundmengeneinheit aufgeschlagen, z. B. pro Quadratmeter.
- **Prozent:** Der Zuschlag wird als Prozentwert auf den Glasgrundpreis aufgeschlagen.
Dieses Feld wird nur im Bereich Verkauf angezeigt.
**Technische Info:** numerisches Feld, Toggle-Feld, DB-Felder: pokokon.zu19

### VK-Kantenbearbeitungen/TZ
Teuerungszuschlag für Kantenbearbeitungen auf den Verkaufspreis in Prozent. Wenn Sie den Wert 0 oder einen Wert <0 eintragen, wird kein Teuerungszuschlag berechnet.
**Technische Info:** numerisches Feld, DB-Feld: pokokon.zu20

### VK-Kantenbearbeitungen/Faktor
Faktor für Kantenbearbeitungen auf den Verkaufspreis in Prozent. In der Regel wird mit einem Faktor ein Rabatt gewährt.
**Technische Info:** numerisches Feld, DB-Feld: pokokon.zuk20

### VK-Eckenbearbeitungen/TZ
Teuerungszuschlag für Eckenbearbeitungen auf den Verkaufspreis in Prozent. Wenn Sie den Wert 0 oder einen Wert <0 eintragen, wird kein Teuerungszuschlag berechnet.
**Technische Info:** numerisches Feld, DB-Feld: pokokon.zu21

### VK-Eckenbearbeitungen/Faktor
Faktor für Eckenbearbeitungen auf den Verkaufspreis in Prozent. In der Regel wird mit einem Faktor ein Rabatt gewährt.
**Technische Info:** numerisches Feld, DB-Feld: pokokon.zuk21

### VK-Flächenbearbeitungen/TZ
Teuerungszuschlag für Flächenbearbeitungen auf den Verkaufspreis in Prozent. Wenn Sie den Wert 0 oder einen Wert <0 eintragen, wird kein Teuerungszuschlag berechnet.
**Technische Info:** numerisches Feld, DB-Feld: pokokon.zu22

### VK-Flächenbearbeitungen/Faktor
Faktor für Flächenbearbeitungen auf den Verkaufspreis in Prozent. In der Regel wird mit einem Faktor ein Rabatt gewährt.
**Technische Info:** numerisches Feld, DB-Feld: pokokon.zuk22

### EK alle Bearbeitungen/TZ
Teuerungszuschlag für alle Bearbeitungen auf den Einkaufspreis in Prozent. Wenn Sie den Wert 0 oder einen Wert <0 eintragen, wird kein Teuerungszuschlag berechnet.
**Technische Info:** numerisches Feld, DB-Feld: pokokon.zu23

### EK alle Bearbeitungen/Faktor
Faktor für alle Bearbeitungen auf den Einkaufspreis in Prozent. In der Regel wird mit einem Faktor ein Rabatt gewährt.
**Technische Info:** numerisches Feld, DB-Feld: pokokon.zuk23

### Zubehör/TZ
Teuerungszuschlag für Zubehörartikel auf den Einkaufs- und/oder Verkaufspreis in Prozent. Wenn Sie den Wert 0 oder einen Wert <0 eintragen, wird kein Teuerungszuschlag berechnet.
**Technische Info:** numerische Felder, DB-Felder: pokokon.zu24, pokokon.zuk24

### Zubehör/Faktor
Faktor für Zubehörartikel auf den Einkaufs- und/oder Verkaufspreis in Prozent. In der Regel wird mit einem Faktor ein Rabatt gewährt.
**Technische Info:** numerische Felder, DB-Felder: pokokon.zu25, pokokon.zuk25

### Fußzeile
In diesem Bereich werden die Bezeichnung des Artikels und das Kennzeichen der Warengruppe des Artikels angezeigt.

## Konditionen für Manuelle Preise

**Pfad:** Verkauf > Auftragserfassung > Register Positionen > Preisfeld von Positionsartikel mit Preismethode Manuelle Preise > <Shift> + <F9>

*Abb. D-127 Positionskonditionen – Konditionen Manuelle Preise*

In diesem Dialog werden die Preiskonditionen eines Positionsartikels angezeigt, dem die Preismethode Manuelle Preise in den Stammdaten zugeordnet ist. Sie können die Preiskonditionen bearbeiten.

> **Automatische Preismethodenänderung**
> Sie können auch für Positionsartikel mit einer anderen Preismethode einen Preis manuell festlegen. Die Preismethode für diesen Positionsartikel wird dann automatisch auf Manuelle Preise geändert.

### Preistyp
Angabe, worauf sich der Preis bezieht.
- **WE/Stück:** Der Preis gilt pro Stück.
- **WE/GME:** Der Preis gilt pro Grundmengeneinheit, z. B. pro Quadratmeter.
**Technische Info:** Toggle-Feld, DB-Feld: pokokon.flag2

Die folgenden Werte geben Sie für Verkaufs- und Einkaufspreise getrennt an.

### Preis
Grundpreis einer Glasscheibe. Der Preistyp wird aus dem vorherigen Feld herangezogen.
**Technische Info:** numerische Felder, DB-Felder: pokokon.zu1, pokokon.zuk1

### TZ
Teuerungszuschlag in Prozent. Der Teuerungszuschlag wird auf den Men-geneinheitspreis aufgeschlagen.
**Technische Info:** numerische Felder, DB-Felder: pokokon.zu2, pokokon.zuk2

### Faktor
Faktor des Preiszuschlags in Prozent. Über den Faktor können Sie die Preisberechnung für den Artikel ändern, ohne alle Preise anpassen zu müssen, z. B. für Preiserhöhungen oder Rabatte. In der Regel wird mit einem Faktor ein Rabatt gewährt.
**Technische Info:** numerische Felder, DB-Felder: pokokon.zu3, pokokon.zuk3

### Maßrundung
Maßrundung in Millimeter für die Preisberechnung des Artikels. Für die Preisberechnung werden die Kantenlängen in der Auftragsposition auf den nächsthöheren Wert in Millimeter aufgerundet, der durch die angegebene Maßrundung teilbar ist. In der Produktion werden diese Angaben nicht berücksichtigt.
**Technische Info:** numerische Felder, DB-Felder: pokokon.zu5, pokokon.zuk5

### Mindestberechnung
Wenn der Wert in der Auftragsposition kleiner ist als der Mindestberechnungswert, wird der Preis für diesen Wert berechnet. Bei z. B. einem Artikel, der als Fläche angegeben wird, wird die Mindestfläche in Quadratmeter als Mindestberechnungswert angegeben.
**Technische Info:** numerische Felder, DB-Felder: pokokon.zu5, pokokon.zuk5

## VSG-Austausch-/Zusatzpreise

**Pfad:** Verkauf > Auftragserfassung > Register Positionen > Preisfeld von VSG-Artikel > <Shift> + <F9> > <Shift> + <F10>

*Abb. D-128 VSG-Austausch-/Zusatzpreise*

In diesem Dialog werden die Konditionen der Austausch- und Zusatzpreise für die einzelnen Glasscheiben in einem VSG-Artikel angezeigt. Sie können die Preiskonditionen bearbeiten.

Die Werte für Verkauf, Einkauf und die Detailansicht der Austausch- und Zusatzpreise werden jeweils in einer eigenen Ansicht angezeigt.
- Mit `<F2>` wechseln Sie zwischen den Ansichten für Verkauf, Einkauf und der Detailansicht.

Der Dialog ist nur freigeschaltet, wenn in der gewählten Position VSG-Artikel erfasst sind.

### Verkauf und Einkauf

- **Artikel:** Artikelnummer.
  **Technische Info:** Anzeigefeld, numerisches Feld, DB-Feld: pokoaust.artnr
- **Austausch-/Zusatzliste, Bezeichnung:** Nummer der Austauschliste. Wenn eine Nummer angeben ist, wird die Bezeichnung im Klartext angezeigt.
  **Technische Info:** numerisches Feld, Anzeigefeld, DB-Felder: pokoaust.vkatinr, pokoaust.ekatlnr, xatl.bez
- **Min.ber.:** Mindestberechnung. Angabe der Mindestfläche in Quadratmeter, für die der Preis berechnet wird. Wenn die Fläche des Austauschglases in der Auftragsposition kleiner ist als die Mindestberechnungsfläche, dann wird der Preis für diese Mindestberechnungsfläche berechnet.
  **Technische Info:** numerisches Feld, DB-Felder: pokoaust.vkminber, pokoaust.ekminber
- **Faktor:** Faktor des Preiszuschlags in Prozent.
  **Technische Info:** numerisches Feld, DB-Felder: pokoaust.vkfaktor, pokoaust.ekfaktor
- **VK-Preis, EK-Preis:** Verkaufs- oder Einkaufspreis des Austauschglases.
  **Technische Info:** numerisches Feld, DB-Feld: pokoaust.vkmepreis, pokoaust.ekmepreis
- **Preistyp:** Angabe, worauf sich der Preis bezieht.
  - **WE/qm:** Der Preis gilt pro Quadratmeter.
  - **Prozent:** Der Zuschlag wird als Prozentwert auf den Glasgrundpreis berechnet.
  **Technische Info:** Toggle-Feld, DB-Feld: pokoaust.vkpreistyp, pokoaust.ekpreistyp

### Detailansicht

Die Felder in der Detailansicht entsprechen den Spalten in Verkauf und Einkauf. Zusätzlich werden die Felder für die Größenzuschläge jeweils für den Verkauf und Einkauf angezeigt. Der Zuschlagstyp gibt an, worauf sich der Zuschlag bezieht:
- **WE Wert:** Der Zu- oder Abschlag wird als fester Betrag auf den Verkaufs-/Einkaufspreis berechnet.
- **Prozent:** Der Zuschlag wird prozentual aus dem Verkaufs-/Einkaufspreis berechnet.

#### Kleinglaszuschlag
Preiszuschlag für Kleingläser, wenn die Fläche des Glases kleiner ist als der angegebene Grenzwert. Im zweiten Feld wählen Sie den Zuschlagstyp.
**Technische Info:** numerisches Feld, Toggle-Feld, DB-Felder: pokoaust.vkklzuschlag, pokoaust.vkklzutyp, pokoaust.ekklzuschlag, pokoaust.ekklzutyp

#### Überlängenzuschlag
Preiszuschlag für Überlängen, wenn eine Kantenlänge länger ist, als der angegebene Grenzwert. Im zweiten Feld wählen Sie den Zuschlagstyp.
**Technische Info:** numerisches Feld, Toggle-Feld, DB-Felder: pokoaust.vkuebzuschlag, pokoaust.vkuebzutyp, pokoaust.ekuebzuschlag, pokoaust.ekuebzutyp

#### Übergrößenzuschlag
Preiszuschlag für Übergrößen, wenn beide Glaskanten eine festgelegte Länge überschreiten. Im zweiten Feld wählen Sie den Zuschlagstyp.
**Technische Info:** numerisches Feld, Toggle-Feld, DB-Felder: pokoaust.vkuebgrzuschlag, pokoaust.vkuebgrzutyp, pokoaust.ekuebgrzuschlag, pokoaust.ekuebgrzutyp

## Positionskonditionen – Bearbeitungspreise (VK), (EK), Detailansicht

**Pfad:** Verkauf > Auftragserfassung > Register Positionen > Preisfeld von Positionsartikel mit Zusatz-Bearbeitung wählen > <Shift> + <F9>

*Abb. D-129 Positionskonditionen – Bearbeitungspreise (VK), (EK), Detailansicht*

In diesen Registern werden die Preiskonditionen für eine preisrelevante Bearbeitung angezeigt, je nachdem ob diese in der Positionsstückliste enthalten ist. Sie können die Preiskonditionen bearbeiten.

Die Bearbeitungspreise sind in Verkauf und Einkauf aufgeteilt. Außerdem gibt es eine Detailansicht, die für beide Register analog aufgebaut ist. In der Detailansicht werden mehr Werte des Bearbeitungspreises für die einzelne Bearbeitung angezeigt.

- Mit `<F5>` wechseln Sie in die Detailansicht.

Die Register sind nur freigeschaltet, wenn in der gewählten Position Zusatz-Bearbeitungen erfasst sind. Das Register Bearbeitungspreise (EK) ist nur aktiv, wenn die Beschaffungsart Bestellung oder Mitgelief. für die Position gewählt ist.

### Register Bearbeitungspreise (VK)

- **Artikel:** Bezeichnung der Bearbeitung.
  **Technische Info:** Anzeigefeld, DB-Feld: aufstrukt.artnr
- **Bre, Höh:** Anzahl der bearbeiteten Breiten und Höhen der Scheibe.
  **Technische Info:** numerische Felder, DB-Felder: poszu.panz1, poszu.panz2
- **Preistyp:** Angabe, worauf sich der Preis der Bearbeitung bezieht:
  - **WE/Stück:** Der Preis gilt pro Stück.
  - **WE/GME:** Der Preis gilt pro Grundmengeneinheit, z. B. pro Quadratmeter.
  - **Prozent:** Der Preis wird als Prozentwert vom Grundpreis des Kopfartikels berechnet.
  - **WE/qm:** Der Preis gilt pro Quadratmeter
  - **WE/lfm:** Der Preis gilt pro laufender Meter.
  **Technische Info:** Toggle-Feld, DB-Feld: poszu.part
- **Menge:** Menge der Bearbeitung pro Grundmengeneinheit.
  **Technische Info:** numerisches Feld, DB-Feld: poszu.pme
- **Faktor:** Verkaufspreis-Faktor des Bearbeitungspreiszuschlags in Prozent. Über den Faktor können Sie die Preisberechnung für den Artikel ändern, ohne alle Preise anpassen zu müssen, z. B. für Preiserhöhungen oder Rabatte. In der Regel wird mit einem Faktor ein Rabatt gewährt.
  **Technische Info:** numerisches Feld, DB-Feld: poszu.vkfaktor
- **TZ:** Verkaufspreis-Teuerungszuschlag für die Bearbeitung in Prozent. Der Teuerungszuschlag wird auf den Mengeneinheitspreis aufgeschlagen. Wenn Sie den Wert 0 oder einen Wert <0 eintragen, wird kein Teuerungszuschlag berechnet.
  **Technische Info:** numerisches Feld, DB-Feld: poszu.vktz
- **ModZu:** Modellzuschlag in Prozent.
  **Technische Info:** numerisches Feld, DB-Feld: poszu.vkmodzusch
- **VK-Preis:** Verkaufspreis der Bearbeitung.
  **Technische Info:** numerisches Feld, DB-Feld: poszu.ppme
- **Grp:** Nummer der Gruppierung. Die Bearbeitungen können unter einer Nummer gruppiert werden.
  **Technische Info:** numerisches Feld, DB-Feld: poszu.masflag

### Register Bearbeitungspreise (EK)
Die meisten Spalten sind zum Register Bearbeitungspreise (VK) beschrieben.
⇨ "Register Bearbeitungspreise (VK)" auf Seite D-308
Zusätzlich werden folgende Spalten angezeigt:

- **EK-Faktor:** Einkaufspreis-Faktor des Bearbeitungspreiszuschlags in Prozent. Über den Faktor können Sie die Preisberechnung für den Artikel ändern, ohne alle Preise anpassen zu müssen, z. B. für Preiserhöhungen oder Rabatte. In der Regel wird mit einem Faktor ein Rabatt gewährt.
  **Technische Info:** numerisches Feld, DB-Feld: poszu.ekfaktor
- **EK-TZ:** Einkaufspreis-Teuerungszuschlag für die Bearbeitung in Prozent. Der Teuerungszuschlag wird auf den Mengeneinheitspreis aufgeschlagen. Wenn Sie den Wert 0 oder einen Wert <0 eintragen, wird kein Teuerungszuschlag berechnet.
  **Technische Info:** numerisches Feld, DB-Feld: poszu.ektz
- **EK-ModZu:** Einkaufspreis-Modellzuschlag in Prozent.
  **Technische Info:** numerisches Feld, DB-Feld: poszu.ekmodzusch
- **EK-Preis:** Einkaufspreis der Bearbeitung.
  **Technische Info:** numerisches Feld, DB-Feld: poszu.ppmeek

### Bearbeitungspreise Detailansicht
Die meisten Felder in der Detailansicht sind zum Register Bearbeitungspreise (VK) beschrieben:
⇨ "Register Bearbeitungspreise (VK)" auf Seite D-308
Zusätzlich werden folgende Felder angezeigt:

**Maßrundung** Maßrundung pro Bearbeitung in der Mengeneinheit.
**Technische Info:** Anzeigefeld, DB-Feld: poszu.massrund

**Mindestberechnung** Angabe der mindest berechneten Mengeneinheit der Bearbeitung.
**Technische Info:** Anzeigefeld, DB-Feld: poszu.minber, poszu.minberek

**Grundpreis** Grundpreis einer preisrelevanten Bearbeitung für Verkauf und Einkauf. Der Grundpreis für den Verkauf entspricht dem Wert im Feld VK-Preis im Register Bearbeitungspreise (VK), der Grundpreis für den Einkauf dem Wert im Feld EK-Preis im Register Bearbeitungspreise (EK).
**Technische Info:** numerische Felder, DB-Felder: poszu.ppme, poszu.ppmeek

**Mindestpreis** Mindestpreis für die Bearbeitung.
**Technische Info:** numerisches Feld, DB-Feld: poszu.minpreis

**Fußzeile**
In diesem Bereich werden die Bezeichnung des Artikels und das Kennzeichen der Warengruppe des Artikels angezeigt.

## Positionskonditionen – Sprossenpreise

**Pfad:** Verkauf > Auftragserfassung > Register Positionen > Preisfeld von Positionsartikel mit Sprossen > <Shift> + <F9>

*Abb. D-130 Positionskonditionen – Sprossenpreise*

In diesem Register werden die Preiskonditionen für Sprossenpreise eines Positionsartikels angezeigt. Sie können die Preiskonditionen bearbeiten.
Das Register ist nur freigeschaltet, wenn in der gewählten Position Sprossen erfasst sind. Die Werte für Verkaufs- und Einkaufspreise werden in zwei eigenen Bereichen angezeigt.

### Verkauf und Einkauf

#### Sprossen-PKZ
Sprossenpreiskennzeichen aus der vordefinierten Preisliste der Sprossenberechnung.
**Technische Info:** numerisches Feld, DB-Feld: pokospro.vkpkz, pokospro.ekpkz

#### Sprossenberechnungsart
Berechnungsart der Sprossen. Die Sprossenberechnungsarten sind ausführlich an anderer Stelle beschrieben:
⇨ "Auftragssprossenpreise" auf Seite D-271
**Technische Info:** numerisches Feld, DB-Feld: pokospro.vkberart, pokospro.ekberart

#### Sprossen-Faktor
Faktor des Sprossenpreiszuschlags in Prozent. Über den Faktor können Sie die Preisberechnung für den Artikel ändern, ohne alle Preise anpassen zu müssen, z. B. für Preiserhöhungen oder Rabatte. In der Regel wird mit einem Faktor ein Rabatt gewährt.
**Technische Info:** numerisches Feld, DB-Feld: pokospro.vkfaktor, pokospro.ekfaktor

#### Sprossen-TZ
Sprossen-Teuerungszuschlag in Prozent. Der Teuerungszuschlag wird auf den Mengeneinheitspreis aufgeschlagen. Wenn Sie den Wert 0 oder einen Wert <0 eintragen, wird kein Teuerungszuschlag berechnet.
**Technische Info:** numerisches Feld, DB-Feld: pokospro.vktz, pokospro.ektz

#### Preis pro Feld
Sprossenpreis nach Anzahl der Felder, wenn im Sprossenaufbau Kreuzungspunkte vorhanden sind. Wenn z. B. zwei Sprossen senkrecht und zwei waagerecht das Fenster in neun Felder teilen, dann wird der Preis neunmal berechnet. Der Preis wird bei den Berechnungsarten Felder, Feld +LM, Feld+K+R und Spezial ausgewertet.
**Technische Info:** numerisches Feld, DB-Feld: pokospro.vkfeld, pokospro.ekfeld

#### Preis pro Feld 2
Sprossenpreis nach Anzahl der Felder, wenn im Sprossenaufbau keine Kreuzungspunkte vorhanden sind. Wenn z. B. vier Sprossen senkrecht und keine waagerecht das Fenster in fünf Felder teilen, dann wird der Preis fünfmal berechnet. Der Preis wird bei den Berechnungsarten Felder, Feld +LM, Feld+K+R und Spezial ausgewertet.
**Technische Info:** numerisches Feld, DB-Feld: pokospro.vk2feld, pokospro.ek2feld

#### Preis pro Laufmeter
Preis pro laufendem Meter der Sprosse. Der Preis wird bei den Berechnungsarten LM, LM+K+R, LM+K, LM+R, Feld+LM und Spezial ausgewertet.
**Technische Info:** numerisches Feld, DB-Feld: pokospro.vklaufm, pokospro.eklaufm

#### Preis pro Rand
Preis pro Randverbindung. Der Preis wird bei den Berechnungsarten R, LM+K+R, LM+R, K+R, Feld+K+R und Spezial ausgewertet.
**Technische Info:** numerisches Feld, DB-Feld: pokospro.vkrand, pokospro.ekrand

#### Preis pro Kreuz
Preis pro Kreuzungspunkt. Der Preis wird bei den Berechnungsarten K, K+R, LM+K, LM+K+R, K oder LM, Feld+K+R und Spezial ausgewertet.
**Technische Info:** numerisches Feld, DB-Feld: pokospro.vkkreuz, pokospro.ekkreuz

#### Prozent
Preis als Prozentwert auf den Preis des Kopfartikels. Der Preis wird bei der Berechnungsart Prozent ausgewertet.
**Technische Info:** numerisches Feld, DB-Feld: pokospro.vkprozent, pokospro.ekprozent

#### Qm-Preis
Preis pro Quadratmeter. Der Preis wird bei der Berechnungsart qm-Preis ausgewertet.
**Technische Info:** numerisches Feld, DB-Feld: pokospro.vkqmpreis, pokospro.ekqmpreis

#### Stückpreis
Preis pro Sprossenkonstruktion. Der Preis wird bei der Berechnungsart Stück ausgewertet.
**Technische Info:** numerisches Feld, DB-Feld: pokospro.vkstueckprs, pokospro.ekstueckprs

#### Mindestlaufmeter
Mindestlänge der Sprosse in Meter, die für den Preis berechnet wird. Wenn die Sprosse weniger Laufmeter misst, als die Mindestlaufmeter, dann wird der Preis für die Mindestlaufmeter berechnet. Der Preis wird bei der Berechnungsart LM ausgewertet.
**Technische Info:** numerisches Feld, DB-Feld: pokospro.vkminlm, pokospro.ekminlm

#### Mindestfeldanzahl
Anzahl der Sprossenfelder, für die der Preis mindestens berechnet wird. Der Preis wird bei der Berechnungsart Felder ausgewertet.
**Technische Info:** numerisches Feld, DB-Feld: pokospro.vkminfeld, pokospro.ekminfeld

#### Sprossen Faktor 2
Faktor des Sprossenpreiszuschlags in Prozent für die zweite Sprosse. Über den Faktor können Sie die Preisberechnung für den Artikel ändern, ohne alle Preise anpassen zu müssen, z. B. für Preiserhöhungen oder Rabatte. In der Regel wird mit einem Faktor ein Rabatt gewährt.
**Technische Info:** numerisches Feld, DB-Feld: pokospro.vkfaktor2, pokospro.ekfaktor2

#### Preis pro Feld (2.Sprosse)
Sprossenpreis nach Anzahl der Felder für die zweite Sprosse, wenn im Sprossenaufbau Kreuzungspunkte vorhanden sind. Der Preis wird bei den Berechnungsarten Felder, Feld +LM, Feld+K+R und Spezial ausgewertet.
**Technische Info:** numerisches Feld, DB-Feld: pokospro.vkfeld2, pokospro.ekfeld2

#### Preis pro Feld 2 (2.Sprosse)
Sprossenpreis nach Anzahl der Felder für die zweite Sprosse, wenn im Sprossenaufbau keine Kreuzungspunkte vorhanden sind. Der Preis wird bei den Berechnungsarten Felder, Feld +LM, Feld+K+R und Spezial ausgewertet.
**Technische Info:** numerisches Feld, DB-Feld: pokospro.vk2feld2, pokospro.ek2feld2

#### Preis pro Laufmeter (2.Sprosse)
Preis pro laufendem Meter für die zweite Sprosse. Der Preis wird bei den Berechnungsarten LM, LM+K+R, LM+K, LM+R, Feld+LM und Spezial ausgewertet.
**Technische Info:** numerisches Feld, DB-Feld: pokospro.vklaufm2, pokospro.eklaufm2

#### Preis pro Rand (2.Sprosse)
Preis pro Randverbindung für die zweite Spros-se. Der Preis wird bei den Berechnungsarten R, LM+K+R, LM+R, K+R, Feld+K+R und Spezial ausgewertet.
**Technische Info:** numerisches Feld, DB-Feld: pokospro.vkrand2, pokospro.ekrand2

#### Mindestlaufmeter (2.Sprosse)
Mindestlänge der zweiten Sprosse in Meter, die für den Preis berechnet wird. Wenn die Sprosse weniger Laufmeter misst, als die Mindestlaufmeter, dann wird der Preis für die Mindestlaufmeter berech-net. Der Preis wird bei der Berechnungsart LM ausgewertet.
**Technische Info:** numerisches Feld, DB-Feld: pokospro.vkminlm2, pokospro.ekminlm2

### Fußzeile
In diesem Bereich werden die Bezeichnung des Artikels und das Kennzeichen der Warengruppe des Artikels angezeigt.

## Produktionskostenkalkulation

**Pfad:** Verkauf > Auftragserfassung > Register Positionen > Preisfeld > <Strg> + <F10>

In diesem Dialog werden die Ergebnisse der Kostenkalkulation angezeigt. Sie können die Werte teilweise bearbeiten.

In der Vorgangserfassung werden zunächst nur die Materialkosten angezeigt. Die Maschinen- und Personalkosten werden Ihnen erst angezeigt, wenn der Vorgang in ein Produktionssystem eingelastet wurde.

Der Dialog hat folgende Register:
- "Produktionskostenkalkulation - Übersicht" auf Seite D-314
- "Produktionskostenkalkulation - Details" auf Seite D-316

### Produktionskostenkalkulation – Übersicht

**Pfad:** Verkauf > Auftragserfassung > Register Positionen > Preisfeld > <Strg> + <F10> > Übersicht

*Abb. D-131 Produktionskostenkalkulation – Übersicht*

In diesem Register werden die Produktionskosten der gewählten Position angezeigt. Sie können die kalkulierte Menge und den Stückpreis der Positionen bearbeiten.

Wenn für einen Bearbeitungsartikel Maschinen- oder Personalkosten berechnet werden, dann wird die entsprechende Artikelnummer und -bezeichnung des Positionsartikels in der Registerüberschrift über der Tabelle angezeigt.

Mit `<F2>` wechseln Sie in die Detailansicht, in der Sie weitere Daten bearbeiten können.

> **Kalkulation erst nach Übermittlung an die Produktion**
> Je nach Systemkonfiguration werden Ihnen die Produktionskosten erst angezeigt, wenn Sie den Auftrag bereits an die Produktion übergeben haben. Wenn Sie den Auftrag noch nicht an die Produktion übergeben haben, werden nur die Materialkosten angezeigt.

#### Übersicht

- **Kostentyp:** Anzeige des Typs der Produktionskosten.
  - Materialkosten
  - interner DB
  - Montagekosten
  - Maschinenkosten
  - Personalkosten
  - Fixkosten
  - Zukauf
  **Technische Info:** Anzeigefeld, DB-Feld: poskost.satztyp
- **Artikel:** Anzeige der Artikelnummer.
  **Technische Info:** Anzeigefeld, DB-Feld: poskost.artnr
- **Kostenstelle:** Bezeichnung der Kostenstelle für statistische Auswertungen.
  **Technische Info:** alphanumerisches Feld, DB-Feld: poskost.kostenst
- **Phy. Menge:** Anzeige der physikalischen Positionsnenge (tatsächliche Menge), z. B. Glasfläche.
  **Technische Info:** Anzeigefeld, DB-Feld: poskost.phymenge
- **Kalk. Menge:** Anzeige der kalkulierten Positionsmenge, z. B. Glasfläche + Verschnitt.
  **Technische Info:** Anzeigefeld, DB-Feld: poskost.pme
- **ME-Preis:** Anzeige des Preises pro Mengeneinheit der Position.
  **Technische Info:** Anzeigefeld, DB-Feld: poskost.ppme
- **Stückpreis:** Preis pro Stück der Position.
  **Technische Info:** numerisches Feld, DB-Feld: poskost.stprs

#### Fußzeile
Summen der jeweiligen Satztypen. Folgende Abkürzungen werden angezeigt:
- **Mat.:** Materialkosten.
- **IntDB:** Interner Deckungsbeitrag.
- **Mont.:** Montagekosten.
- **Masch.:** Maschinenkosten.
- **Pers.:** Personalkosten.

### Produktionskostenkalkulation – Details

**Pfad:** Verkauf > Auftragserfassung > Register Positionen > Preisfeld > <Strg> + <F10> > Register Details

*Abb. D-132 Produktionskostenkalkulation - Details*

In diesem Register werden die Detaildaten der ermittelten Produktionskosten angezeigt. Sie können die Werte der gewählten Position bearbeiten und so die Produktionskosten neu kalkulieren.

Mit `<Bild hoch>`, `<Bild runter>` können Sie zwischen den einzelnen Kosten der aktuellen Position navigieren.

Wenn für einen Bearbeitungsartikel Maschinen- oder Personalkosten berechnet werden, dann wird die entsprechende Artikelnummer und -bezeichnung des Positionsartikels in der Registerüberschrift über der Tabelle angezeigt.

#### Details
Je nach Kostentyp werden verschiedene Felder angezeigt:

**Produktionsposition** Produktionspositionsnummer bei Produktionskosten. Bei bestellten Bearbeitungen wird hier die entsprechende Positionsnummer der Bestellung angezeigt, in der das Unterteilt bestellt ist.
**Technische Info:** Anzeigefeld, DB-Feld: poskost.plfdpos

**Kostentyp** Anzeige des Typs der Produktionskosten.
**Technische Info:** Anzeigefeld, DB-Feld: poskost.satztyp

**Manuelle Änderung** Angabe, ob die Werte überschrieben wurden. Wenn die Produktionskosten geändert werden, wird Manuell in dem Feld angezeigt. Sie können den Inhalt im Feld nicht bearbeiten.
**Technische Info:** Anzeigefeld, DB-Feld: poskost.manuell

**Beschaffungsart** Anzeige der Beschaffungsart des gewählten Artikels. Der Wert kann nur bei den Satztypen Maschinenkosten und Personalkosten bearbeitet werden.
- **Keine:** Keine Beschaffungsart, z. B. für Dienstleistungen.
- **Bestellung:** Artikel muss beim Lieferanten bestellt werden.
- **Lager:** Artikel wird dem Lager entnommen.
- **Produktion:** Artikel wird produziert.
- **Mitgelief.:** Artikel wird vom Kunden mitgeliefert, z. B. zur weiteren Bearbeitung.
- **n. verfüg.:** Artikel ist nicht verfügbar.
**Technische Info:** Toggle-Feld, DB-Feld: poskost.beschaffart

**Stückzahl** Artikelmenge in der Stückliste der Position. Bei den Produktionskosten entspricht die Stückzahl immer 1. Für Maschinenkosten wird in der Regel keine Stückzahl angezeigt.
**Technische Info:** Anzeigefeld, DB-Feld: poskost.menge

**Artikel** Nummer des Artikels, für den die Kosten ermittelt werden.
**Technische Info:** Anzeigefeld, DB-Feld: poskost.artnr

**Kopfartikel** Artikels, dem der gewählte Artikel als Unterteil angehängt ist. Wenn der Artikel selbst der Kopfartikel ist, bleibt das Feld leer.
**Technische Info:** Anzeigefeld, DB-Feld: poskost.refartnr

**Betriebsmittelnr.** Nummer des Betriebsmittels, das für die Berechnung herangezogen wird.
Dieses Feld wird nur beim Satztypen Maschinenkosten angezeigt.
**Technische Info:** numerisches Feld, DB-Feld: poskost.bmnr

**Produktionssubnr.** Personal-Betriebsmittelnummer. Sie können den Wert nicht bearbeiten.
Dieses Feld wird nur beim Satztypen Maschinenkosten angezeigt.
**Technische Info:** numerisches Feld, DB-Feld: poskost.psbmnr

**Arbeitsgangklasse** Nummer der Arbeitsgangklasse für die Produktionsplanung. In einer Arbeitsgangklasse können mehrere Arbeitsgänge zusammengefasst werden.
Dieses Feld wird nur bei den Satztypen Maschinenkosten und Personalkosten angezeigt.
**Technische Info:** numerisches Feld, DB-Feld: poskost.agknr

**Arbeitsgang** Nummer des Arbeitsgangs für die Produktionsplanung.
Dieses Feld wird nur bei den Satztypen Maschinenkosten und Personalkosten angezeigt.
**Technische Info:** numerisches Feld, DB-Feld: poskost.agnr

**Personalnummer** Personalklassennummer. Sie können den Wert nicht bearbeiten.
Dieses Feld wird nur beim Satztypen Personalkosten angezeigt.
**Technische Info:** numerisches Feld, DB-Feld: poskost.pknr

**Kostenstelle** Bezeichnung der Kostenstelle für statistische Auswertungen.
**Technische Info:** alphanumerisches Feld, DB-Feld: poskost.kostenst

**Grundmengeneinheit** Grundmengeneinheit, die dem Artikel in den Stammdaten zugewiesen wurde, z. B. Quadratmeter, Stück. Der Wert wird zur Berechnung des Stückpreises für die Satztypen Maschinenkosten und Personalkosten herangezogen. Sie können den Wert nicht bearbeiten.
Dieses Feld wird nur bei den Satztypen Maschinenkosten und Personalkosten angezeigt.
**Technische Info:** numerisches Feld, DB-Feld: poskost.lugme

**Variante** Anzeige der Variantennummer des Artikels.
**Technische Info:** numerisches Feld, DB-Feld: poskost.variante

**Menge/Physikalische** Physikalische Menge der Position (tatsächliche Menge), z B. Glasfläche, Arbeitsdauer. Die physikalische Menge dient als Berechnungsgrundlage für die kalkulatorische Menge und den Stückpreis. Das Feld entspricht der Spalte Phy. Menge im Register Übersicht.
**Technische Info:** numerisches Feld, DB-Feld: poskost.phymenge

**Verlust** Prozentualer Verlust der Position, z. B. Materialverlust, Zeitverlust. Der Prozentsatz des Verlusts wird auf die kalkulierte Menge gerechnet. Wenn Sie einen negativen Verlust angeben, wird die kalkulierte Menge geringer.
**Technische Info:** numerisches Feld, DB-Feld: poskost.verlust

**Menge/Kalkulation** Kalkulierte Menge der Position, z. B. Glasfläche + Verschnitt. Die kalkulierte Menge wird aus der physikalischen Menge inklusive Verlust berechnet:
`physikalische Menge + Verlust / 100 x physikalische Menge`
Das Feld entspricht der Spalte Kalk. Menge im Register Übersicht.
**Technische Info:** numerisches Feld, DB-Feld: poskost.pme

**Mengeneinheitspreis** Preis pro Grundmengeneinheit der Position. Der Mengeneinheitspreis wird zur Berechnung des Stückpreises herangezogen.
Das Feld entspricht der Spalte ME-Preis im Register Übersicht.
**Technische Info:** numerisches Feld, DB-Feld: poskost.ppme

**Stückpreis** Preis pro Stück der Position. Der Stückpreis berechnet sich aus Mengeneinheitspreis und der kalkulierten Mengen:
`Mengeneinheitspreis x kalkulierte Menge`
Bei den Satztypen Maschinenkosten und Personalkosten wird zusätzlich die Grundmengeneinheit zur Berechnung des Stückpreises herangezogen:
`Mengeneinheitspreis x kalkulierte Menge / Grundmengeneinheit`
**Technische Info:** numerisches Feld, DB-Feld: poskost.stkprs

**Datum** Erfassungsdatum der Position.
**Technische Info:** Datumsfeld, DB-Feld: poskost.datum

**Mengeneinheitspreis/Fertigmeldung** Preis pro Mengeneinheit bei Fertigmeldung.
**Technische Info:** numerisches Feld, DB-Feld: poskost.fppme

**Stückpreis/Fertigmeldung** Stückpreis bei Fertigmeldung in Eigenwährung.
**Technische Info:** numerisches Feld, DB-Feld: poskost.fstprs

**(Stückpreis) in Fremdwährung** Stückpreis in Fremdwährung.
**Technische Info:** numerisches Feld, DB-Feld: poskost.stkprsfw

**(Stückpreis/Fertigmeldung in Fremdwährung)** Stückpreis bei Fertigmeldung in Fremdwährung.
**Technische Info:** numerisches Feld, DB-Feld: poskost.fstkprsfw

#### Fußzeile
Die Fußzeile ist zum Register Übersicht beschrieben:
⇨ "Fußzeile" auf Seite D-315

## Preiskalkulation

**Pfad:** Verkauf > Preiskalkulation

*Abb. D-133 Preiskalkulation*

In diesem Dialog berechnen Sie die Verkaufspreise anhand der definierten Konditionen. Der berechnete Preis dient nur Informationszwecken und wird nicht gespeichert.

Die Steuerelemente sind zum Dialog Auftragserfassung beschrieben:
⇨ "Auftragserfassung" auf Seite D-82

## Freischaltung

Je nach Systemkonfiguration werden Aufträge bei der Erfassung nicht freigeschaltet, z. B. wenn der Erfasser nicht ausreichend Rechte hat, der Deckungsbeitrag unterschritten oder das Firmenlimit überschritten wird. Diese Aufträge müssen für die weitere Bearbeitung manuell freigeschaltet werden, um sie weiter an das System, also an Produktion, Einkauf, Versand, und Lager, zu übergeben.

In diesem Abschnitt sind folgende Dialoge erklärt:
- "Auftragsfreischaltung" auf Seite D-321
- "Autorisierung" auf Seite D-324

### Auftragsfreischaltung

**Pfad:** Verkauf > Auftragsfreischaltung > Freischaltung

*Abb. D-134 Auftragsfreischaltung*

In diesen Dialogen suchen und schalten Sie einen Auftrag zur weiteren Bearbeitung frei. Sie können einen Auftrag nur freischalten, wenn Sie die entsprechenden Rechte besitzen. Je nach Grund der Auftragssperrung werden unterschiedliche Rechte für die Auftragsfreischaltung benötigt.

Im Suchdialog Auftragsfreischaltung können Sie die Suche zur Freischaltung filtern:
- **Suchkriterien eingeben > [Start]:** Sie können Abteilung oder Erfasser und/oder Grund in dem vorgegebenen Haus wählen. Es werden alle Aufträge angezeigt, die den Kriterien entsprechen. Wenn Sie keine Kriterien angeben, werden in der Trefferliste alle alle nicht freigeschalteten Aufträge angezeigt.
- **[Individuell] > Grund eingeben > Haus, Erfasser angeben > [OK]:** Sie müssen zunächst einen Grund eingeben und können anschließend im Dialog Freischaltung das Haus und/oder den Erfasser wählen.

Im Dialog Auftragsfreischaltung werden alle Aufträge angezeigt, die den Suchkriterien entsprechen.
- Mit `<Shift> + <F5>` können Sie den markierten Auftrag in der Auftragserfassung öffnen.
- Mit `<Strg> + <F9>` können Sie alle Aufträge freischalten.
- Mit `<Shift> + <F9>` können Sie ab dem markierten Auftrag alle Aufträge freischalten.
- Mit `<Shift> + <F12>` öffnen Sie den Dialog Sperrgründe für die nicht erfolgte Freischaltung. In diesem Dialog werden die Gründe für die Sperrung des Auftrags angezeigt. Der Dialog wird nur angezeigt, wenn ein Auftrag aus mehr als einem Grund gesperrt ist.
- Mit `<F3>` schalten Sie die gewählten Aufträge frei.

#### Kopfzeile
In diesem Bereich werden die Suchkriterien angezeigt, die Sie festgelegt haben. Sie können die Suchkriterien nachträglich nicht mehr bearbeiten. Für eine neue Suche müssen Sie den Dialog schließen und neu aufrufen.

#### Übersicht
In diesem Bereich werden die Aufträge angezeigt, die den Suchkriterien entsprechen und freigeschaltet werden können. Sie können nur die Werte in den Spalten Frei und LSp bearbeiten. Die übrigen Spalten dienen der Information.

- **Auftrag:** Nummer des Auftrags, der noch nicht freigeschaltet ist.
  **Technische Info:** Anzeigefeld, DB-Feld: kauf.auftrnr
- **Frei:** Angabe über die Freischaltung des Auftrags. Wenn das Feld ausgegraut ist, dann ist die Freischaltung aus datentechnischen Gründen nicht möglich, oder Sie besitzen nicht die entsprechenden Rechte für die Freischaltung.
  - **NEIN:** Der Auftrag wird noch nicht freigeschaltet.
  - **JA:** Der Auftrag wird sofort freigeschaltet.
  - **NIE:** Der Auftrag wird nie freigeschaltet.
  - **VS:** Der Auftrag wird nur an die Versandsteuerung übergeben.
  **Technische Info:** Toggle-Feld, DB-Feld: kauf.tekap.kz
- **Kunde, Name:** Nummer und Name des Kunden aus dem Auftrag.
  **Technische Info:** Anzeigefelder, DB-Felder: kauf.kunr, mp.name
- **Termin:** Geplanter Liefertermin.
  **Technische Info:** Anzeigefeld, DB-Feld: kauf.Itideal
- **Abruf:** Angabe, ob der Auftrag nur bei Abruf geliefert wird.
  - **J:** Der Auftrag wird nur bei Anforderung durch den Kunden geliefert.
  - **N:** Der Auftrag wird standardmäßig geliefert.
  **Technische Info:** Anzeigefeld, DB-Feld: kauf.abrufkz
- **User, Abtnr:** Nummer und Abteilungsnummer des Auftrags-Erfassers.
  **Technische Info:** Anzeigefelder, DB-Felder: kauf.eusr, kauf.abtnr
- **Erfasst:** Datum der Auftragserfassung.
  **Technische Info:** Anzeigefeld, DB-Feld: kauf.edat
- **Haus:** Mandantennummer (Hausnummer), zu der der Auftrag zugeordnet ist.
  **Technische Info:** Anzeigefeld, DB-Feld: kauf.hausnr
- **LSp:** Limit-Sperre. Angabe, ob der Auftrag gesperrt ist. Sie können Aufträge nur freischalten, wenn Sie die entsprechenden Rechte besitzen. Sie benötigen spezielle Rechte, wenn Sie Aufträge freischalten wollen, die das Firmenlimit oder das Allgemeines Kredit-Versicherungslimit (AKV-Limit) überschritten haben.
  - **J:** Die Limit-Sperre ist aktiv. Das Feld Frei wird gesperrt und der Wert automatisch auf NEIN gesetzt.
  - **N:** Die Limit-Sperre ist deaktiviert. Der Auftrag kann freigeschaltet werden.
  **Technische Info:** Toggle-Feld, DB-Feld: kauf.limsperre
- **Bemerkung:** Zusatz-Information zum Auftrag.
  **Technische Info:** Anzeigefeld, DB-Feld: kauf.lusperrmodus
- **Info:** Anzeige, ob Auftrags-Informationen hinterlegt sind. Wenn in der Spalte ein I angezeigt wird, sind Informationen für den Auftrag hinterlegt. Mit `<F5>` öffnen Sie den Dialog Anmerkungen mit den hinterlegten Informationen.
  **Technische Info:** Anzeigefeld

### Autorisierung

**Pfad:** Verkauf > Auftragsfreischaltung > Autorisierung

*Abb. D-135 Autorisierung*

In diesem Dialog autorisieren Sie einen Mitarbeiter, einen Auftrag freizuschalten, selbst wenn dieser Auftrag das Kreditlimit überschreitet. Die maximale Höhe der Überschreitung legen Sie fest, indem Sie den neuen Wert entsprechend erhöhen oder einen Wert im Feld Maximale Werterhöhung eintragen.

Die Funktionen sind von den Einstellungen in den Stammdaten und der jeweiligen Systemkonfiguration und abhängig. Für kundenindividuelle Anpassungen kontaktieren Sie Ihren Ansprechpartner der A+W Software GmbH.

**Vorgang** Nummer und Art des Vorgangs. Wenn Sie eine Nummer angegeben haben, wird die Vorgangsart im Klartext angezeigt.
**Technische Info:** Pflichtfeld, numerisches Feld, DB-Feld: kauffrei.auftrnr

**Laufende Änderungsnr.** Nummer des Änderungsvorgangs. Die aktuelle Änderungsnummer wird automatisch eingetragen. Sie können eine kleinere Änderungsnummer angeben, um den entsprechenden Änderungsstand einzusehen.
**Technische Info:** numerisches Feld, DB-Feld: kauffrei.aendernr

> **Erhöhung der Änderungsnummer**
> Sie können nur den jeweils letzten Änderungsstand bearbeiten, ohne dass die Änderungsnummer erhöht wird. Wenn Sie einen weiter zurückliegenden Änderungsstand abrufen und bearbeiten, werden die Änderungen unter einer neuen Änderungsnummer gespeichert.

**Kunde** Kundenname aus dem Vorgang. Wenn Sie die Vorgangs-Nummer angegeben haben, wird der Kunde im Klartext angezeigt.
**Technische Info:** Anzeigefeld, DB-Feld: kauf.kunr

**Autorisierter Mitarbeiter** Nummer und Name des Mitarbeiters, für den die Autorisierung eingerichtet wird. Wenn Sie eine Nummer angegeben haben, wird der Name des Mitarbeiters im Klartext angezeigt.
**Technische Info:** Pflichtfeld, numerisches Feld, DB-Feld: kauffrei.aendmanr

**Alter Wert** Alter Nettototal-Wert des Vorgangs. Als Wert wird immer der aktuelle Nettototal-Wert des Vorgangs herangezogen.
**Technische Info:** numerisches Feld

**Neuer Wert** Obergrenze für den neuen Nettototal-Wert des Vorgangs. Der Wert muss höher sein, als der alte Nettototal-Wert. Der Wert ist abhängig vom Feld Maximale Werterhöhung:
- Wenn das Feld Maximale Werterhöhung leer ist und Sie einen neuen Nettototal-Wert angeben, wird im Feld Maximale Werterhöhung automatisch die Differenz zwischen altem und neuem Nettototal-Wert angezeigt.
- Wenn im Feld Maximale Werterhöhung bereits ein Wert steht und Sie einen neuen Nettototal-Wert angeben, wird der Wert im Feld Maximale Werterhöhung automatisch an den neuen Wert angepasst.
**Technische Info:** numerisches Feld

**Maximale Werterhöhung** Maximale Erhöhung der Kosten, die den alten Nettototal-Wert des Auftrags übersteigt. Der Wert ist abhängig vom Feld Neuer Wert:
- Wenn das Feld Neuer Wert leer ist und Sie einen neuen Maximalwert angeben, wird im Feld Neuer Wert automatisch die Differenz zwischen altem und neuem Nettototal-Wert angezeigt.
- Wenn im Feld Neuer Wert bereits ein Wert steht und Sie einen neuen Maximalwert angeben, wird der Wert im Feld Neuer Wert an den neuen Wert angepasst.
**Technische Info:** numerisches Feld, DB-Feld: kauffrei.maxpreisdiff

#### Fußbereich
**Mitarbeiter** Anzeige des Namens des autorisierenden Mitarbeiters.
**Technische Info:** Anzeigefeld, DB-Feld: kauffrei.automanr

**Datum** Anzeige des Datums, an dem die Autorisierung freigeschaltet wurde. Standardmäßig wird das aktuelle Datum angezeigt.
**Technische Info:** Anzeigefeld

## Lieferung

Standardmäßig werden Lieferscheine im Modul Versandsteuerung erfasst und verwaltet, weil die Buchungen von verpackten und fertigen Produkten aus anderen Modulen bzw. Programmen automatisch an die Versandsteuerung weitergeleitet werden. Wenn das Modul Versandsteuerung nicht konfiguriert ist, können Sie die Lieferscheine im Modul Verkauf erstellen.

Je nach Konfiguration können Sie zu einem Auftrag einen Lieferplan erstellen. Im Lieferplan können Sie den Auftrag in Teillieferungen aufteilen. Für jede (Teil-)Lieferung eines Auftrags wird ein Lieferschein erstellt. Der Lieferschein dient zum Nachweis der Auftragsabwicklung für die Logistik und Spedition und zur Auskunft für den Kunden. Je nach Art der Lieferungen unterscheidet das System zwischen Komplett- und Teillieferscheinen. Sie können Lieferscheine automatisch oder manuell erstellen und bearbeiten.

Die Funktionen sind von den Einstellungen in den Stammdaten und der jeweiligen Systemkonfiguration und abhängig.

Für kundenindividuelle Anpassungen kontaktieren Sie Ihren Ansprechpartner der A+W Software GmbH.

In diesem Abschnitt sind folgende Dialoge erklärt:
- "Lieferplan" auf Seite D-327
- "Lieferinformation – Details der Auslieferung" auf Seite D-329
- "Lieferscheine (automatisch)" auf Seite D-333
- "Lieferscheine (manuell)" auf Seite D-335
- "Lieferscheinprotokoll" auf Seite D-337

### Lieferplan

**Pfad:** Verkauf > Auftragserfassung > Positionsebene > <F4> > Lieferplan

*Abb. D-136 Lieferplan*

In diesem Dialog erfassen Sie den Lieferplan. Sie können für einen Auftrag mehrere Teillieferungen festlegen. Wenn Sie einen Lieferschein erzeugen, werden die Daten aus dem Lieferplan herangezogen und ausgewertet. Sie können einen Lieferschein für einen Auftrag erst dann erzeugen, wenn die Erfassung der Positionen abgeschlossen ist.

#### Übersicht
- **Pos.:** Nummer der Position aus dem Auftrag.
  **Technische Info:** Anzeigefeld, DB-Feld: lieferplan.posnr
- **Lief.:** Nummer der (Teil-)Lieferung.
  **Technische Info:** Pflichtfeld, numerisches Feld, DB-Feld: liefplan.subnr
- **Lieferdatum:** Voraussichtlicher Termin der (Teil-)Lieferung.
  **Technische Info:** Datumsfeld, DB-Feld: liefplan.ltplan
- **Ankunftstag:** Voraussichtlicher Ankunftstag der (Teil-)Lieferung.
  **Technische Info:** Anzeigefeld, DB-Feld: liefplan.ankunft
- **Artikel:** Bezeichnung des Artikels.
  **Technische Info:** Anzeigefeld, DB-Feld: liefplan.artbez1
- **Route:** Nummer der Route der (Teil-)Lieferung.
  **Technische Info:** Pflichtfeld, numerisches Feld, DB-Feld: liefplan.route
- **Gesamt:** Gesamt-Stückzahl der bestellten Position aus dem Auftrag.
  **Technische Info:** numerisches Feld, DB-Feld: liefplan.geslief
- **Gelief:** Bereits ausgelieferte Menge aus der Position des Auftrags.
  **Technische Info:** numerisches Feld, DB-Feld: liefplan.geliefert
- **Verpackt:** Stückzahl der verpackten Position des Auftrags.
  **Technische Info:** numerisches Feld, DB-Feld: liefplan.gespack
- **Geplant:** Geplante Stückzahl der Position, die in dieser (Teil-)Lieferung ausgeliefert werden soll.
  **Technische Info:** Pflichtfeld, numerisches Feld, DB-Feld: liefplan.zuliefern

#### Details
Das Register Details wird zurzeit nicht genutzt.

### Lieferinformation – Details der Auslieferung

**Pfad:** Verkauf > Auftragserfassung > Kopf-, Fußbereich > <F4> > Lieferinformation

*Abb. D-137 Details der Auslieferung*

In diesem Dialog werden die Details der Auslieferung angezeigt, z. B die Route und der geplante Liefertermin. Die verschiedenen Lieferinformationen sind besonders wichtig, wenn sich Produktions- und Auslieferungshaus unterscheiden.

Einige Felder in den Bereichen Produktions- und Auslieferungshaus können nur vorbelegt werden, wenn Sie mit interner Mandantentrennung arbeiten und die Via-Plant-Logik aktiv ist.

Die Felder in diesem Dialog werden vom System vorbelegt. In der Regel müssen Sie die Felder nicht bearbeiten.

#### Produktionshaus
- **Lieferadresscode, Lieferadressname:** Code und Name der gespeicherten Lieferadresse des Produktionshauses.
  **Technische Info:** alphanumerische Felder, DB-Felder: kauf.lort, kauf.lort
- **Versandart:** Nummer und Bezeichnung der Versandart. Wenn eine Nummer angegeben wird, wird die Bezeichnung der Versandart im Klartext angezeigt.
  **Technische Info:** numerisches Feld, Anzeigefeld, DB-Feld: kauf.versandartvia
- **gepl.Liefertermin:** Datum der geplanten Auslieferung im Produktionshaus. Das Datum gibt an, an welchem Tag die Lieferung das Produktionshaus voraussichtlich verlässt.
  **Technische Info:** Datumsfeld, DB-Feld: kauf.ltplan
- **Route:** Nummer der Route, über die ausgeliefert wird.
  **Technische Info:** Pflichtfeld, numerisches Feld, DB-Feld: kauf.routenr
- **Fahrtzeit:** Voraussichtliche Fahrtdauer zum Auslieferungshaus. Wenn eine Route angegeben ist, für die eine Fahrtzeit hinterlegt ist, wird die Fahrtzeit im Klartext angezeigt. Sie kann sich auf den Liefertermin auswirken.
  **Technische Info:** Anzeigefeld
- **Routentage:** Anzeige der Wochentage, an denen die gewählte Route gefahren wird. Wenn eine Route angegeben ist, werden die zugehörigen Routentage aus den Stammdaten herangezogen und im Klartext angezeigt.
  **Technische Info:** Anzeigefeld
- **Region:** Anzeige der Versandregion. Mehrere Auslieferungsrouten können zu einer Versandregion zusammengefasst werden, wenn das System entsprechend konfiguriert ist. Die Versandregion wird zu der entsprechenden via Route aus den Stammdaten herangezogen. Das Feld ist vorbelegt, wenn das Modul Regionalrouten konfiguriert ist und der aktuellen Route eine Versandregion zugeordnet ist. Zudem müssen Sie mit interner Mandantentrennung arbeiten und die Via-Plant-Logik muss aktiv sein.
  **Technische Info:** Anzeigefeld, DB-Feld: route.region
- **via Haus:** Nummer des Auslieferungshauses, über das die Lieferung versendet wird. Das Auslieferungshaus legen Sie im Kopfbereich im Feld Route mit `<F5>` fest.
  **Technische Info:** Anzeigefeld, DB-Feld: kauf.vsvia
- **Haus:** Anzeige der Mandantennummer (Hausnummer), in der der Auftrag angelegt wird.
  **Technische Info:** Anzeigefeld, DB-Feld: kauf.hausnr
- **Tonnage:** Anzeige der Nutzlast des Fahrzeugs in Kilogramm. Dieses Feld ist frei konfigurierbar.
  **Technische Info:** Anzeigefeld
- **Kalender:** Anzeige, ob der Kalender bei der Lieferterminbestimmung herangezogen wird. Sie können in den Routenstammdaten für jede Route festlegen, ob der Kalender ausgewertet wird.
  - Der Kalender wird bei der Lieferterminbestimmung berücksichtigt.
  - Der Kalender wird bei der Lieferterminbestimmung nicht berücksichtigt.
  **Technische Info:** Checkbox

#### Auslieferungshaus
Dieser Bereich wird nur angezeigt, wenn Sie mit interner Mandantentrennung arbeiten und die Via-Plant-Logik aktiv ist.

- **Lieferadresscode, Lieferadressname:** Code und Name der Lieferadresse des Auslieferungshaus.
  **Technische Info:** alphanumerische Felder, DB-Felder: kauf.lort, kauf.lort
- **Versandart:** Nummer der Versandart, z. B. LKW. Wenn eine Nummer ausgewählt ist, wird die Bezeichnung der Versandart im Klartext angezeigt.
  **Technische Info:** Anzeigefeld, DB-Feld: kauf.versandartvia
- **Ankunft in via Haus:** Datum, an dem die Lieferung voraussichtlich im Auslieferungshaus ankommt.
  **Technische Info:** Anzeigefeld
- **Handlingszeit:** Handlings-Zeit, um die Lieferung im Auslieferungshaus auf- oder abzuladen.
  **Technische Info:** numerisches Feld
- **Route:** Nummer der Route, über die an den Kunden ausgeliefert wird. Die Route muss in den Stammdaten als via Route für das Auslieferungshaus angelegt sein:
  ⇨ Stammdaten, "Routen" auf Seite J-193
  **Technische Info:** Plichtfeld, numerisches Feld, DB-Feld: kauf.routenr
- **Fahrtzeit:** Anzeige der Fahrtdauer zum Auslieferungshaus. Wenn eine Route angegeben ist, für die eine Fahrtzeit hinterlegt ist, wird die Fahrtzeit im Klartext angezeigt.
  **Technische Info:** Anzeigefeld
- **Routentage:** Anzeige der Wochentage, an denen die gewählte Route gefahren wird. Wenn eine Route angegeben ist, werden die zugehörigen Routentage aus den Stammdaten herangezogen und im Klartext angezeigt.
  **Technische Info:** Anzeigefeld
- **Region:** Anzeige des Länderkennzeichens mit Benennung der Versandregion.
  **Technische Info:** Anzeigefeld
- **Tonnage:** Anzeige der Nutzlast des Fahrzeugs in Kilogramm. Dieses Feld ist frei konfigurierbar.
  **Technische Info:** Anzeigefeld

#### Kunde
- **Gepl.LiefTerm:** Geplantes Lieferdatum vom Auslieferungshaus zum Kunden.
  **Technische Info:** Anzeigefeld, DB-Feld: kauf.ltplan
- **Kalender:** Anzeige, ob der Kalender bei der Lieferterminbestimmung herangezogen wird. Sie können in den Routenstammdaten für jede Route festlegen, ob der Kalender ausgewertet wird.
  - Der Kalender wird bei der Lieferterminbestimmung berücksichtigt.
  - Der Kalender wird bei der Lieferterminbestimmung nicht berücksichtigt.
  **Technische Info:** Checkbox
- **Wunschtermin:** Gewünschter Liefertermin des Kunden.
  **Technische Info:** Datumsfeld, DB-Feld: kauf.Itideal
- **Ankunftstag:** Datum, an dem die Lieferung voraussichtlich beim Kundeneintrifft. Der Ankunftstag wird anhand des Liefertermins, der Fahrtdauer und der Routentage errechnet.
  **Technische Info:** Anzeigefeld
- **Terminstatus:** Statuskennzeichen, ob der Wunschtermin des Kunden und der berechnete Ankunftstermin der Lieferung übereinstimmen.
  **Technische Info:** Anzeigefeld

| Symbol | Statuskennzeichen | Bedeutung |
| :--- | :--- | :--- |
| (grün) | grün | Der voraussichtliche Liefertermin entspricht exakt dem Wunschtermin des Kunden. |
| (gelb) | gelb | Der voraussichtliche Liefertermin liegt vor dem Wunschtermin des Kunden. |
| (rot) | rot | Der voraussichtliche Liefertermin liegt nach dem Wunschtermin des Kunden. |
*Tab. D-12 Terminstatus*

#### Kalenderausschnitt
Der Kalenderausschnitt zeigt einen Ausschnitt von drei Wochen um den Wunschtermin des Kunden. Alle Termine, z. B. geplanter Liefertermin, Kundenwunschtermin, Liefertermin im Produktionshaus usw., die in diesem Zeitraum liegen, werden an den entsprechenden Tagen angezeigt. Sie können sich auf den Kalendertagen Informationen über den jeweiligen Termin als Tooltipp anzeigen lassen.

### Lieferscheine (automatisch)

**Pfad:** Verkauf > Lieferscheine > Automatische Freigabe

*Abb. D-138 Lieferscheine (automatisch)*

In diesem Dialog erzeugen Sie Lieferscheine als Begleitdokumente für die Auftragsauslieferung. Sie können in diesem Dialog auch Rechnungen erzeugen und Vorgänge abschließen.

> **Inkonsistenz mit der Versandsteuerung**
> Wenn das Modul Versandsteuerung in Ihrem System konfiguriert ist, sollten Sie die Lieferscheine nur in der Versandsteurung erstellen. Das System ist standardmäßig nicht für die Erstellung von Lieferscheinen im Modul Verkauf konfiguriert.
> Lieferscheine im Verkauf zu erstellen, kann zu Inkonsistenzen mit der Versandsteuerung führen, da die Statusbuchungen, wie z. B. verpackte oder fertig gemeldete Mengen, nur in der Versandsteuerung auf dem aktuellen Stand sind.
> Für kundenindividuelle Anpassungen kontaktieren Sie Ihren Ansprechpartner der A+W Software GmbH.

- **Freigabe:** Angabe der Freigabe-Art für den gewählten Vorgang.
  - **Lieferschein:** Für den gewählten Vorgang wird ein Lieferschein erzeugt.
  - **Rechnung:** Für den gewählten Vorgang wird eine Rechnung erzeugt. Sie können eine Rechnung nur für Vorgänge erzeugt, zu denen bereits ein Lieferschein existiert.
  - **LS + Rechnung:** Für den gewählten Vorgang werden Lieferschein und Rechnung erzeugt.
  - **Vorgang abschließen:** Der gewählte Vorgang wird abgeschlossen. Änderungen am Vorgang werden nicht mehr an das System weitergegeben.
- **Hnr:** Mandantennummer (Hausnummer).
- **Vorgang:** Vorgangsnummer. Bei Lieferscheinerzeugung geben Sie die Nummer des Auftrags, bei Rechnungserzeugung die Nummer des Lieferscheins an. Die Auftrags- und die Lieferscheinnummer sind identisch. Für den Lieferschein können Sie zusätzlich die Subnummer bei Teillieferungen angeben.
- **Subnr:** Subnummer des Vorgangs, z. B. vom Teillieferschein. Die Subnummer muss für die Erzeugung eines Lieferscheins angegeben werden.
- **Grp:** Versandgruppe. Lieferscheine können in der Versandplanung einer Versandgruppe zugeordnet werden. Die Versandgruppen werden in den Systemstammdaten hinterlegt. Die Versandgruppe dient als zusätzliches Kennzeichen für die Toursperre.
- **Lieferschein:** Angabe, ob ein Lieferschein oder Teillieferschein existiert. Existiert bereits ein Lieferschein, dann steht in diesem Feld die Angabe existiert.
- **Rechnung:** Rechnungsnummer.
- **Kundennr.:** Kundennummer.
- **Kunde:** Kundenname.
- **Datum:** Erfassungsdatum des Vorgangs.
- **Valuta:** Frist der Wertstellung in Tagen.
- **Er.:** Erzeugen. Angabe, ob die Lieferscheine und/oder Rechnungen erzeugt werden sollen.
  - Ja, erzeugen.
  - ☐ Nicht erzeugen.

Mit `<F2>` werden die folgenden Felder angezeigt:
- **Betrag:** Höhe des Nettototal-Betrags.
- **Erf.:** Mitarbeiternummer des Vorgangserfassers.
- **Erfasser:** Name des Vorgangserfassers.
- **Belegdatum:** Entspricht dem Feld Datum.

#### Fußzeile
Kundenname und die Höhe des Nettototal-Betrags werden angezeigt.

### Lieferscheine (manuell)

**Pfad:** Verkauf > Lieferscheine > Manuelle Lieferscheine

*Abb. D-139 Lieferscheine (manuell)*

In diesem Dialog erzeugen und bearbeiten Sie Lieferscheine manuell. Lieferscheine erzeugen Sie nur dann manuell, wenn Sie Korrekturen in den Auftragsdaten vornehmen müssen, z. B. bei einer abweichenden Liefermenge.

Wenn das Modul Versandsteuerung in Ihrem System konfiguriert ist, sollten Sie die Lieferscheine nur in der Versandsteurung erzeugen. Das System ist standardmäßig nicht für die Erzeugung von Lieferscheinen im Modul Verkauf konfiguriert.

> **Inkonsistenz mit der Versandsteuerung**
> Lieferscheine im Verkauf zu erzeugen, kann zu Inkonsistenzen mit der Versandsteuerung führen, da die Statusbuchungen, wie z. B. verpackte oder fertig gemeldete Mengen, nur in der Versandsteuerung auf dem aktuellen Stand sind.
> Für kundenindividuelle Anpassungen kontaktieren Sie Ihren Ansprechpartner der A+W Software GmbH.

Die Felder und Register sind zum Dialog Auftragserfassung beschrieben:
⇨ "Auftragserfassung" auf Seite D-82

Zusätzliche werden folgende Felder angezeigt:

#### Kopfbereich
**Auftrag** Nummer des Auftrags und Subnummer. Subnummern vergeben Sie für Teil-Lieferscheine. Mit `<TAB>` wird die nächste freie Subnummer automatisch vergeben. Wenn zu einem Auftrag bereits Lieferscheine erfasst sind, können Sie die Subnummer eingeben und den bereits erstellten Lieferschein aufrufen.

#### Register Allgemein
**Erhalten** Positionsmenge, die bereits mit vorherigen Lieferscheinen ausgeliefert worden ist.

**Gelief.** Menge der Artikel, die mit dem ausgewählten Lieferschein ausgeliefert werden.

### Lieferscheinprotokoll

**Pfad:** Verkauf > Lieferscheine > Protokoll

*Abb. D-140 Lieferscheinprotokoll*

In diesem Dialog wird das Lieferscheinprotokoll angezeigt. Alle Vorgänge zu den Lieferscheinen sind mit der Angabe des Datums und der Zeit vermerkt.

Wenn Sie mit interner Mandantentrennung arbeiten, öffnet sich zunächst ein Dialog zur Angabe der Mandantennummer (Hausnummer). In dem Protokoll werden nur die Vorgänge zum ausgewählten Haus angezeigt.

> **Lieferscheinprotokoll zu dem aktuellen Tag**
> Ein Lieferscheinprotokoll wird zu dem aktuellen Tag erzeugt. Wenn die Fehlermeldung angezeigt wird, dass die Datei leer oder nicht lesbar ist, dann wurde an diesem Tag noch kein Lieferschein erzeugt.

## Rechnungen

Um Kundenaufträge abzurechnen, werden Rechnungen erzeugt und an die Finanzbuchhaltung (FIBU) übergeben.
Sie können die Rechnungen automatisch oder manuell erstellen. Eine Rechnung kann erst automatisch erstellt werden, wenn ein Lieferschein existiert.

In diesem Abschnitt sind folgende Dialoge erklärt:
- "Rechnungen (automatisch)" auf Seite D-339
- "Positionsinfo" auf Seite D-342
- "Rechnungen (manuell)" auf Seite D-344
- "Thekenrechnung" auf Seite D-345
- "Rechnungen buchen" auf Seite D-346
- "Abschlagsrechnung (automatisch)" auf Seite D-348
- "Abschlagsrechnung (manuell)" auf Seite D-350
- "Schlussrechnung (automatisch)" auf Seite D-351
- "Schlussrechnung (manuell)" auf Seite D-352
- "Rechnungsprotokoll" auf Seite D-353

### Rechnungen (automatisch)

**Pfad:** Verkauf > Rechnungen > Automatische Freigabe

*Abb. D-141 Rechnungen (automatisch)*

In diesem Dialog erstellen Sie Rechnungen zu Vorgängen und übergeben sie an die FIBU. Sie können die Vorgänge importieren, zu denen Rechnungen erzeugt werden können, oder Sie können die Vorgangsnummern manuell angeben.

Mit `<Strg> + <F8>` importieren Sie die Daten aller Vorgänge, für die eine Rechnung erzeugt werden kann. Die Daten werden über eine frei konfigurierbare SQL-Abfrage importiert. Die Anzahl der importierten Daten ist von der jeweiligen SQL-Abfrage abhängig. Sie können die Abfrage nutzen, die standardmäßig von A+W konfiguriert ist oder eine kundenspezifische SQL-Abfrage für den Datenimport festlegen.

Für kundenindividuelle Anpassungen kontaktieren Sie Ihren Ansprechpartner der A+W Software GmbH.

In der Fußzeile wird der Kundenname und der Gesamtbetrag aus dem Auftrag angezeigt, für den eine Rechnung erstellt wird.

Wenn Sie eine Rechnung noch nicht gebucht haben, können Sie im Dialog Rechnungen zusätzliche Informationen einsehen und die Rechnung bearbeiten, z. B. um Korrekturen vorzunehmen.
⇨ "Rechnungen (manuell)" auf Seite D-344

In diesem Dialog können Sie zusammen mit der Rechnung auch gleichzeitig den Lieferschein erzeugen oder den Vorgang abschließen.
Mit `<F3>` werden die Rechnungen zu den ausgewählten Aufträgen vom System erzeugt.

#### Register Vorgänge

- **Freigabe:** Angabe, welche Dokumente Sie für den Vorgang freigeben, der im Feld Vorgang angegeben ist.
  - **Rechnung:** Für den Vorgang wird die Rechnung erzeugt.
  - **LS + Rechnung:** Für den Vorgang werden der Lieferschein und die Rechnung erzeugt.
  - **Vorgang abschließen:** Der Vorgang wird abgeschlossen, d. h. er kann nicht mehr bearbeitet werden.
  - **Lieferschein:** Für den Vorgang wird der Lieferschein erzeugt.
  **Technische Info:** Toggle-Feld, DB-Feld: kauf.vorgang
- **Hnr:** Anzeige der Mandantennummer (Hausnummer).
  **Technische Info:** Anzeigefeld, DB-Feld: kauf.hausnr
- **Vorgang:** Vorgangsnummer.
  **Technische Info:** Pflichtfeld, numerisches Feld, DB-Feld: kauf.auftrnr
- **Subnr:** Nummer des Teillieferscheins. Wenn das Dokument für eine Komplettlieferung erzeugt wird, wird eine 1 angezeigt.
  **Technische Info:** numerisches Feld, DB-Feld: kauf.subnr
- **Grp:** Versandgruppe. Lieferscheine können in der Versandplanung einer Versandgruppe zugeordnet werden. Die Versandgruppen werden in den Systemstammdaten hinterlegt. Die Versandgruppe dient als zusätzliches Kennzeichen für die Toursperre.
  **Technische Info:** numerisches Feld, DB-Feld: lapool.vsgruppe
- **Lieferschein:** Anzeige, ob ein Lieferschein oder Teillieferschein existiert. Wenn ein Lieferschein existiert, steht in diesem Feld der Eintrag existiert.
  **Technische Info:** Anzeigefeld
- **Rechnung:** Nummer des Rechnungsvorgangs, wenn eine Rechnung existiert.
  **Technische Info:** Anzeigefeld
- **Kundennr.:** Anzeige der Kundennummer.
  **Technische Info:** Anzeigefeld, DB-Feld: kauf.kunr
- **Kunde:** Anzeige des Kundennamens.
  **Technische Info:** Anzeigefeld, DB-Feld: mp.name
- **Belegdatum:** Datum der Rechnungserstellung oder Rechnungsbuchung. Standardmäßig wird das Feld mit dem aktuellen Datum vorbelegt. Für Rechnungen und Lieferscheine können Sie mit `<Strg> + <B>` zwischen Beleg- und Buchungsdatum wechseln. Über dem Spaltenkopf wird angezeigt, welches Datum gerade angezeigt wird.
  **Technische Info:** Pflichtfeld, Datumsfeld, DB-Feld: kauf.edat
- **Valuta:** Frist zur Wertstellung in Tagen bis maximal 99 Tage.
  **Technische Info:** Anzeigefeld, DB-Feld: kauf.valuta
- **Er.:** Erzeugen. Angabe, ob die gewählten Dokumente erzeugt werden sollen.
  - Ja, erzeugen.
  - Nicht erzeugen.
  **Technische Info:** Checkbox

Mit `<F2>` wechseln Sie zum Register Information zum Vorgang.

#### Register Information zum Vorgang
Die Spalten sind zum Register Vorgänge beschrieben:
⇨ "Register Vorgänge" auf Seite D-340
Zusätzlich werden folgende Spalten angezeigt:
- **Betrag:** Anzeige der Höhe des Rechnungsbetrages.
  **Technische Info:** Anzeigefeld, DB-Feld: kauf.nettototal
- **Erf., Erfasser:** Anzeige der Erfassernummer und des Erfassernamens.
  **Technische Info:** Anzeigefelder, DB-Felder: kauf.eust, mitarb.maname

#### Fußzeile
In der Fußzeile werden der Kundenname und der Rechnungsbetrag aus dem Vorgang angezeigt.

Mit `<F5>` öffnen Sie den Dialog Positionen, in dem weitere Details zu den Rechnungspositionen angezeigt werden.
⇨ "Positionsinfo" auf Seite D-342

### Positionsinfo

**Pfade:**
- Verkauf > Rechnungen > Automatische Freigabe > Werte angeben > `<F5>`
- Verkauf > Rechnungen buchen > Werte angeben > `<F5>`
- Verkauf > Abschlagsrechnung, Schlussrechnung > Automatische Freigabe > Werte angeben > `<F5>`
- Verkauf > Gutschriften > Gutschriften buchen > Werte angeben > `<F5>`

*Abb. D-142 Positionsinfo*

In diesem Dialog werden die Details zu den einzelnen Positionen aus der automatischen Rechnungs- oder Gutschrifterstellung angezeigt.

#### Register PositionsInfo I
- **Vorgang:** Vorgangsnummer.
  **Technische Info:** numerisches Feld, DB-Feld: kauf.auftrnr
- **Pos:** Nummer der Position im Vorgang.
  **Technische Info:** numerisches Feld, DB-Feld: kpos.lfdpos
- **Artikel, Bezeichnung:** Nummer und Bezeichnung des Artikels.
  **Technische Info:** numerisches Feld, alphanumerisches Feld, DB-Felder: kpos.artnr, kpos.artbez1
- **F:** Anzeige, ob die Position fakturiert ist.
  **Technische Info:** Anzeigefeld, DB-Feld: kauf.fakturakz
- **Menge:** Anzahl der Einheiten der Position.
  **Technische Info:** numerisches Feld, DB-Feld: kpos.menge
- **Breite:** Breite der erfassten Glasscheibe in der Position in Millimetern.
  **Technische Info:** numerisches Feld, DB-Feld: kpos.laenge
- **Höhe:** Höhe der erfassten Glasscheibe in der Position in Millimetern.
  **Technische Info:** numerisches Feld, DB-Feld: kpos.breite
- **Stückpreis:** Preis pro Einheit der Position.
  **Technische Info:** numerisches Feld, DB-Feld: kpos.nstpreis
- **Pos. Preis:** Preis der kompletten Position.
  **Technische Info:** numerisches Feld, DB-Feld: kpos.npospreis

Mit `<F2>` wechseln Sie zum Register PositionsInfo II.

#### Register PositionsInfo II
Die Spalten sind zum Register PositionsInfo I beschrieben:
⇨ "Register PositionsInfo I" auf Seite D-342
Zusätzlich werden folgende Spalten angezeigt:
- **Mod:** Modellnummer für den Positionsartikel.
  **Technische Info:** numerisches Feld, DB-Feld: kpos.modnr
- **gelief.:** Anzahl der Einheiten, die bereits ausgeliefert wurden.
  **Technische Info:** numerisches Feld, DB-Feld: kpos.geslief
- **(Feld ohne Bezeichnung):** Anzeige, ob die Position fakturiert ist.
  **Technische Info:** Anzeigefeld, DB-Feld: kauf.fakturakz
- **berech.:** Anzahl der Einheiten, die bereits fakturiert wurden.
  **Technische Info:** numerisches Feld, DB-Feld: kpos.gesberech
- **SZR 1,SZR 2:** Breite des Scheibenzwischenraums in Millimeter. Bei einem Mehrfachisolierglas wird im SZR1 der erste und im SZR2 der zweiten Scheibenzwischenraum angezeigt.
  **Technische Info:** numerische Felder, DB-Felder: kpos.szr, kpos.szr2

### Rechnungen (manuell)

**Pfad:** Verkauf > Rechnungen > Manuelle Rechnung

*Abb. D-143 Rechnungen (manuell)*

In diesem Dialog können Sie Rechnungen bearbeiten oder erstellen. Anschließend können Sie die Rechnungen an die FIBU übergeben, wenn das System entsprechend konfiguriert ist.

Wenn Sie eine manuelle Abschlags- oder Schlussrechnung erstellen möchten, können Sie diese auch direkt im entsprechenden Menüpunkt auswählen. Um z. B. eine Abschlagsrechnung manuell zu erstellen, wählen Sie im Menüpfad bei Abschlagsrechnungen die Manuelle Rechnung aus.

Die Felder sind zum Dialog Auftragserfassung beschrieben:
⇨ "Auftragserfassung" auf Seite D-82
Zusätzlich werden die folgenden Felder angezeigt:

#### Kopfbereich
**Rech-Nr.** Rechnungsnummer. Wenn Sie eine Rechnung anlegen, wird vom System eine temporäre Nummer für die Rechnung erstellt. Nach Abschluss der Rechnungserstellung vergibt das System eine endgültige Rechnungsnummer. Auf diese Weise werden die Rechnungen fortlaufend durchnummeriert. Wenn Sie eine vorhandene Rechnungsnummer angeben, wird die entsprechende Rechnung geöffnet.
Die Rechnungen werden in der Datenbanktabelle kauf unter vorgang mit dem Wert 7, mit ihrer endgültig vergebenen Rechnungsnummer gespeichert.
**Technische Info:** numerisches Feld, DB-Feld: kauf.auftrnr

> **Rechnungen mit Bezug erfassen**
> In der Regel werden Rechnungen immer mit Bezug auf einen Vorgang, z. B. einen Lieferschein oder einen Auftrag, erfasst. Sie können die Vorgangsnummer, für den Sie die Rechnung ausstellen wollen, in dem Feld Bezug im Kopfbereich angeben.

#### Register Allgemein
**Berech** Positionsmenge, die berechet werden soll. Das Feld ist bei einer manuellen Rechnung standardmäßig mit dem Wert Menge aus dem Vorgang vorbelegt. Sie können den Wert verringern.
**Technische Info:** numerisches Feld, DB-Feld: kpos.berechnet

#### Fußbereich
Wenn zu dem Bezugsvorgang bereits eine Rechnung erzeugt wurde, dann wird im Feld **Fakturasaldo** der Rechnungsbetrag aus allen Rechnungen angezeigt, die für diesen Vorgang bereits erfasst wurden.

### Thekenrechnung

**Pfad:** Verkauf > Rechnungen > Thekenrechnung

*Abb. D-144 Thekenrechnung*

In diesem Dialog wickeln Sie das Thekengeschäft ab, für Kunden, die ihre Ware selbst abholen und direkt bezahlen. Bei einem Thekengeschäft erfassen Sie die Auftragsdaten und die Rechnung und der Lieferschein werden sofort im Anschluss erstellt.

Die Felder sind zum Dialog Auftragserfassung beschrieben:
⇨ "Auftragserfassung" auf Seite D-82

### Rechnungen buchen

**Pfad:** Verkauf > Rechnungen > Rechnungen buchen

*Abb. D-145 Rechnungen buchen*

In diesem Dialog buchen Sie Rechnungen, die noch nicht an die FIBU übergeben worden sind. In der Regel werden Rechnungen nach dem Erzeugen automatisch gebucht.

In Ausnahmefällen kann die Rechnung auch nachträglich gebucht werden. In der Rechnungserfassung wird je nach Konfiguration beim Erzeugen der Rechnung eine Abfrage angezeigt, ob die Rechnung gebucht werden soll. Wenn Sie die Abfrage mit [Nein] beantworten, können Sie diese ungebuchte Rechnung im Dialog Rechnungen buchen importieren und nachträglich buchen.

Mit `<Strg> + <F8>` importieren Sie die Daten aller Rechnungen, die in dem festgelegten Zeitraum erzeugt worden sind.

In der Fußzeile wird der Kundenname und der Gesamtbetrag aus dem Auftrag angezeigt, für den die Rechnung gebucht wird.

Mit `<F3>` werden die ausgewählten Rechnungen gebucht.

#### Register Verkaufs-Rechnung
- **Rechnung:** Rechnungsnummer. Wenn Sie eine Nummer angeben, werden in die übrigen Spalten die entsprechenden Werte eingetragen.
  **Technische Info:** Pflichtfeld, numerisches Feld
- **Subnr.:** Anzeige der Subnummer für Teilrechnungen.
  **Technische Info:** Anzeigefeld, DB-Feld: kauf.subnr
- **Fremdnummer:** Anzeige der Vorgangsnummer, die vom Kunden vorgegeben wird. Für Aufträge aus einem anderen Haus steht in diesem Feld die Auftragsnummer des sendenden Hauses.
  **Technische Info:** Anzeigefeld, DB-Feld: kauf.exaufnr
- **Auftrag:** Anzeige der Auftragsnummer.
  **Technische Info:** Anzeigefeld, DB-Feld: kauf.auftrnr
- **Belegdatum:** Anzeige des Datums der Rechnungserstellung.
  **Technische Info:** Anzeigefeld, DB-Feld: kauf.edat
- **Buch.datum:** Anzeige des Datums der Rechnungsbuchung. Standardmäßig ist das aktuelle Datum eingegeben. Wenn Sie ein anderes Buchungsdatum angeben wollen, müssen Sie das neue Datum in das Feld eingeben, die Eingabe bestätigen und das neue Datum nochmals eingeben. Das Datum wird erst nach der zweiten Eingabe in das Feld übernommen.
  **Technische Info:** Datumsfeld, DB-Feld: kauf.bdat
- **Bu.:** Angabe, ob die Rechnung gebucht werden soll.
  - Die Rechnung wird gebucht.
  - Die Rechnung wird nicht gebucht.
  **Technische Info:** Checkbox

#### Register Information zum Vorgang
Das Register Information zum Vorgang ist nur in den Dialogen Rechnungen (automatisch) und Lieferscheine (automatisch) freigeschaltet:
- ⇨ "Rechnungen (automatisch)" auf Seite D-339
- ⇨ "Lieferscheine (automatisch)" auf Seite D-333

### Abschlagsrechnung (automatisch)

**Pfad:** Verkauf > Rechnungen > Abschlagsrechnung > Automatische Freigabe

*Abb. D-146 Abschlagsrechnung (automatisch)*

In diesem Dialog erstellen Sie die Abschlagsrechnungen für Aufträge anhand eines entsprechenden Zahlungsplans. Wenn es für den aktuellen Tag Aufträge gibt, für die ein Zahlungsplan existiert, dann können Sie die Aufträge mit `<Strg> + <F8>` importieren. Sie können die Auftragsnummern auch manuell eingeben oder mit `<F9>` nach Aufträgen suchen.

In der Fußzeile wird der Kundenname und der Gesamtbetrag aus dem Auftrag angezeigt, für den eine Abschlagsrechnung erstellt wird.

Mit `<F3>` werden die Abschlagsrechnungen zu den ausgewählten Aufträgen vom System erzeugt.

- **Auftrag:** Auftragsnummer.
  **Technische Info:** Pflichtfeld, numerisches Feld, DB-Feld: kauf.auftrnr
- **Haus:** Anzeige der Mandantennummer (Hausnummer).
  **Technische Info:** Anzeigefeld, DB-Feld: kauf.hausnr
- **Betrag:** Abschlagsbetrag aus dem Zahlungsplan.
  **Technische Info:** numerisches Feld, DB-Feld: zahlplan.betrag
- **Lieferschein:** Anzeige, ob ein Lieferschein oder Teillieferschein existiert. Wenn ein Lieferschein existiert, steht in diesem Feld der Eintrag existiert.
  **Technische Info:** Anzeigefeld
- **Datum:** Anzeige des Termins für die Fälligkeit des Abschlagsbetrags.
  **Technische Info:** Anzeigefeld, DB-Feld: zahlplan.ztplan
- **Ko.:** Kontrolliert. Anzeige, ob die Rechnung bereits kontrolliert wurde. Je nach Konfiguration kann eine Rechnung nur erstellt werden, wenn diese bereits vom autorisierten Mitarbeiter kontrolliert wurde.
  - Die Rechnung wurde kontrolliert und kann erzeugt werden.
  - Die Rechnung wurde noch nicht kontrolliert. Je nach Konfiguration kann die Rechnung nicht erzeugt werden.
  **Technische Info:** Checkbox, Anzeigefeld
- **Er.:** Erzeugen der Abschlagsrechnung, wenn Sie die Rechnungserstellung mit `<F3>` auslösen.
  - Abschlagsrechnung erstellen.
  - Keine Abschlagsrechnung erstellen.
  **Technische Info:** Checkbox

#### Register Information zum Vorgang
Das Register Information zum Vorgang ist nur in den Dialogen Rechnungen (automatisch) und Lieferscheine (automatisch) freigeschaltet:
- ⇨ "Rechnungen (automatisch)" auf Seite D-339
- ⇨ "Lieferscheine (automatisch)" auf Seite D-333

### Abschlagsrechnung (manuell)

**Pfad:** Verkauf > Rechnungen > Abschlagsrechnung > Manuelle Rechnung

*Abb. D-147 Abschlagsrechnung (manuell)*

In diesem Dialog können Sie manuell Abschlagsrechnungen erstellen.
Wenn es zu dem Auftrag einen Zahlungsplan gibt, erscheint ein Hinweis mit der Frage, ob die Termine zu dem Zahlungsplan angezeigt werden sollen. Wenn Sie bestätigen, dann können Sie einen Termin aus dem Zahlungsplan auswählen.

Manuelle Abschlagsrechnungen werden wie manuellen Rechnungen erfasst. Die Dialoge Abschlagsrechnung (manuell) und Rechnungen (manuell) sind weitgehend analog aufgebaut.

Im Positionsbereich wird eine neue Position in der letzten Zeile angezeigt. Sie listet den Abschlag mit dem Betrag aus dem Zahlungsplan auf.

Die Felder sind zum Dialog Rechnungen (manuell) beschrieben:
⇨ "Rechnungen (manuell)" auf Seite D-344:
Zusätzlich werden die folgenden Felder angezeigt:

#### Fußbereich
Der Gesamtbetrag des Auftrags wird im Feld **Auftragswert** angezeigt. Wenn zu dem Bezugsvorgang bereits eine Rechnung erzeugt wurde, wird der Gesamtbetrag der Rechnung, auf die Bezug genommen wird, im Feld **Fakturasaldo** angezeigt.
