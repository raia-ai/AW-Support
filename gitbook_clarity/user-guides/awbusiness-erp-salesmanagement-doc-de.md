---
description: "DE_AWBusiness_Verkauf_4_3"
---


# Kompletterfassung von Dokumenten bis Faktura

---
## Formularverwaltung

Die Einstellung in der Formularverwaltung lässt folgende Möglichkeiten zu:

- **0 - Kein Druck:**
  Im Formulardruck werden die Angaben aus dem Dokument übernommen:
    - **0 - Kein Druck:** Preise werden nicht gedruckt.
    - **1 - Alle Preise:** Preise werden pro Auftragsposition gedruckt.
    - **2 - Nur Summen:** Nur die Positionssummen werden gedruckt.
- **1 - Alle Preise:**
  Die Einstellungen aus dem Dokument werden ignoriert. Die Preise werden pro Auftragsposition gedruckt.
- **2 - Nur Summen:**
  Im Formulardruck werden die Angaben aus dem Dokument übernommen:
    - **0 - Kein Druck:** Preise werden nicht gedruckt.
    - **1 - Alle Preise:** Preise werden pro Auftragsposition gedruckt.
    - **2 - Nur Summen:** Nur die Positionssummen werden gedruckt.

*(Seite C-201)*

---

### Einstellungen für den Preisdruck

Der Druck der Preise wird von der Formularverwaltung und von der Einstellung im Dokument gesteuert.

| Einstellungen | Druck |
| :--- | :--- |
| **Dokument** | **Formularverw.** | **Positionspreise** | **Summenpreise** |
| 0 | 0 | - | X |
| 1 | 0 | X | X |
| 2 | 0 | - | X |
| 0 | 1 | X | X |
| 1 | 1 | X | X |
| 2 | 1 | X | X |
| 0 | 2 | - | X |
| 1 | 2 | - | X |
| 2 | 2 | - | X |

**Legende:**
**Dokumente**
- 0 = Kein Druck
- 1 = Alle Preise
- 2 = Nur Summen

**Formularverwaltung**
- 0 = Standard (Dokument entscheidet)
- 1 = Preise immer drucken
- 2 = Preise immer drucken (Summenmodus)

- = kein Druck, X = Druck

> **Beispiel**
> Wenn im Dokument Summen drucken (2) eingestellt ist und in der Formularverwaltung Standard (0), werden nur Summenpreise gedruckt, jedoch keine Positionspreise.

*(Seite C-202)*

---

## Dokument drucken

In dieser Einheit lernen Sie, wie Sie Dokumente drucken. Die hinterlegten Formulare werden dem Druckmodus entsprechend zur Auswahl angeboten. In diesem Beispiel wird eine Rechnung gedruckt. Mit demselben Ablauf drucken Sie auch Auftragsbestätigungen, Lieferscheine, Fertigungsscheine usw.

> **Druck von Sammelrechnungen**
> Prüfen Sie vor dem Druck einer Sammelrechnung die Sortierreihenfolge in dem Nummernverwalter, in dem sich die Rechnungen befinden. Der Druck von Sammelrechnungen wird unterbrochen, wenn sich eines der Kriterien für Sammelrechnungen unterscheidet.

### So drucken Sie eine Rechnung

1.  Wählen Sie Dokumente > Auftrag > Druck Auftrag.

