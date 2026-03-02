---
description: "DE_HB_AWProduction_11"
---


# Softwarereferenz - Stammdaten

---
## Betriebsmittel der Auftragserfassung
In diesem Feld wird Ihnen das Betriebsmittel der Auftragserfassung angezeigt. Dieses Feld wird an die Auftragserfassung zurück gemeldet. D. h., wenn Sie den Eintrag ändern, wird das geänderte Betriebsmittel zurück gemeldet.

**Technische Info:** Datenbankfeld: Maschinennr

## Erläuterung der Felder im Bereich Rückmeldung von Buchungen

### Bearbeitungsrückmeldung
Diese Checkbox steuert, ob Rückmeldungen bezüglich der Bearbeitungen erfolgen oder nicht. Mögliche Werte sind:
- Es erfolgt keine Rückmeldung.
- Wird eine Scheibe auf eine Erfassungsstelle gebucht, dann wird der Bearbeitungsfortschritt scheibengenau als Änderungsmeldung in die Datei STSD*.ASC geschrieben.

### Gestellrückmeldung
Diese Checkbox steuert, ob Rückmeldungen bezüglich der Gestellbelegung erfolgen oder nicht. Mögliche Werte sind:
- Es erfolgt keine Rückmeldung.
- Wird ein Gestell auf eine Erfassungsstelle gebucht, dann wird die Gestellbelegung scheibengenau als Snapshot (Momentaufnahme) in die Datei STSG*.ASC geschrieben.

### Gestellbelegung an Gestellserver melden
Diese Checkbox steuert, ob die Gestellbelegung an den Gestellserver gemeldet werden soll oder nicht. Mögliche Werte sind:
- Es erfolgt keine Rückmeldung an den Gestellserver.
- Die Gestellbelegung wird an den Gestellserver zurück gemeldet.

### Einheitenrückmeldung (STSU*.asc)
Über diese Checkbox ist es möglich, im A+W Business eine Zuordnung der A+W Production-Etiketten zur A+W Business-Auftragspositionen vorzunehmen. Mögliche Werte sind:
- Es erfolgt keine Rückmeldung.
- Wird eine Einheit auf eine Erfassungsstelle gebucht, dann wird der Bearbeitungsfortschritt scheibengenau als Änderungsmeldung in die Datei STSU*.ASC geschrieben.

### Produktionsrückmeldung
Diese Checkbox dient dazu, den aktuellen Auftragsstatus im A+W Business zu aktualisieren. Mögliche Werte sind:
- Es erfolgt keine Rückmeldung.
- Der aktuelle Auftragsstatus im A+W Business wird aktualisiert.

### Ergänzende Informationen
- ⇨ Tutorial, "Erfassungsstellen" auf Seite H-923
- ⇨ Tutorial, "Fehlergestell (Error-Rack)" auf Seite H-924
- ⇨ Tutorial, "Erfassungsstelle Lkw" auf Seite H-929
- ⇨ "Zustände" auf Seite H-1008
- ⇨ "Erfassungsstellen-Typen" auf Seite H-997

---
*A+W Production Betriebsdatenerfassung*
*H-1001*
---

# Stammdaten - Gestelle
Stammdaten > BDE > Gestelle

**Abb. H-5 Gestelle**
