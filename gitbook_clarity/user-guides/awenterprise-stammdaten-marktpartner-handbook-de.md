---
description: "DE-HB-AWEnterprise_2"
---


# Marktpartner

---
## Softwarereferenz

liefern Ihnen die Zahlen rechts oberhalb der Treffermenge. Bsp.: Wenn in der Satzanzeige steht 1:100 (14873). Das bedeutet, dass es sich um den ersten Eintrag (der Treffermenge) von 100 geladenen (Zwischenspeicher) von insgesamt 14873 Einträgen handelt. Die Anzahl der zu ladenden Einträge (Zwischenspeicher) ist konfigurierbar.

**Schaltflächen zum Blättern**
Über die Schaltflächen |<, <<, >> und >| können Sie in der Treffermenge blättern. Mit der Schaltfläche >> blättern Sie seitenweise (16 Einträge) vor. Mit der Schaltfläche << blättern Sie seitenweise (16 Einträge) zurück. Mit der Schaltfläche >| springen Sie an das Ende des Zwischenspeichers (100. Eintrag) und mit |< an den Anfang des Zwischenspeichers (1. Eintrag).
Zum Laden weiterer Einträge, klicken Sie auf die Schaltfläche [Weitere Daten]. Dann wird wieder die konfigurierte Anzahl an Daten (in unserem Fall 100) in den Zwischenspeicher geladen.

### Erläuterung der Suchfelder

**Ab Nummer**
Eingabe einer Nummer, ab der gesucht werden soll.
> Technische Info: Numerisches Feld, DB-Feld: mp.mpnr

**Matchcode**
Eingabe des Matchcodes als Suchwert. Sie können den kompletten Matchcode eingeben oder nur einen Teil.
> Technische Info: Alphanumerisches Feld, DB-Feld: mp.mpmc

**Typ**
Anzeige des Marktpartnertyps nach dem gerade gesucht wird. Er wird entsprechend der Auswahl im Marktpartnerdialog vorbelegt und ist nicht änderbar.

**Name**
Eingabe des Namens als Suchwert. Sie können den kompletten Namen eingeben oder nur einen Teil (Groß-/Kleinschreibung wird nicht berücksichtigt).
> Technische Info: Numerisches Feld, DB-Feld: mp.name

**Vorname**
Eingabe des Vornamens als Suchwert. Sie können den kompletten Vornamen eingeben oder nur einen Teil.
> Technische Info: Alphanumerisches Feld, DB-Feld: mp.vname

**Straße**
Eingabe der Straße als Suchwert. Sie können die komplette Straße eingeben oder nur einen Teil.
> Technische Info: Alphanumerisches Feld, DB-Feld: mp.strasse

**Haus**
Auswahl und Eingabe der Hausnummer/Mandantennummer als Suchwert. Die Eingabe hier ist nur sinnvoll, wenn das erweiterte Mehrmandantensystem konfiguriert ist, da nur dann Marktpartner einem Mandanten zugeordnet werden können.
> Technische Info: Numerisches Feld, <F9>, DB-Feld: mp.hausnr

**Land**
Auswahl und Eingabe des Landes als Suchwert. Die entsprechenden Schlüssel können über das Menü Länder (Schlüssel > Marktpartner) vergeben werden.
> Technische Info: Alphabetisches Feld, <F9>, DB-Feld: mp.kfz

**PLZ**
Auswahl und Eingabe der Postleitzahl als Suchwert. Sie können die komplette Postleitzahl eingeben oder nur einen Teil.
> Technische Info: Numerisches Feld, <F9>, DB-Feld: mp.plz

**Ort**
Auswahl und Eingabe des Ortes als Suchwert. Sie können den kompletten Ort eingeben oder nur einen Teil.
> Technische Info: Alphabetisches Feld, <F9>, DB-Feld: mp.ort

**USt-Ident-Nr.**
Eingabe der Umsatzsteuer-Identifikationsnummer als Suchwert. Sie können die komplette Nummer eingeben oder nur einen Teil (Groß-/Kleinschreibung wird berücksichtigt).
> Technische Info: Numerisches Feld, DB-Feld: mp.steuernr

**Art**
Auswahl der Art als Suchwert:
- **aktiv:** Es werden nur aktive Marktpartner angezeigt.
- **stillgelegt:** Es werden nur stillgelegte Marktpartner angezeigt.
- **alle:** Es werden alle Marktpartner angezeigt.
> Technische Info: Alphabetisches Feld, <F9>, DB-Feld: mp.still

## Register Adresse

*Stammdaten > Marktpartner*

*Abb. B-9 Register Adresse*

In diesem Register erfassen und/oder bearbeiten Sie die Rechnungsadresse des Marktpartners. Das Register ist in eine linke und eine rechte Seite aufgeteilt. Die linke Seite enthält die Adressdaten des Marktpartners und ist während des gesamten Bearbeitungsvorgangs präsent. Die rechte Seite zeigt die Daten aus den anderen Registern bzw. weitere Optionen.

Mit `<F5>` öffnen Sie einen Dialog, in dem Sie Anmerkungstexte zu dem Marktpartner hinterlegen können.
-> "Marktpartner - Anmerkungstexte" auf Seite B-106

Mit `<Shift><F5>` öffnen Sie einen Dialog, in dem Sie Artikel-Anmerkungstexte zu dem Marktpartner hinterlegen können.
-> "Artikel - Anmerkungstexte" auf Seite B-386

Mit `<Shift><F9>` springen Sie in das Feld Matchcode.

> **Asiatische Installationen**
> Die asiatischen Installationen beinhalten zusätzliche Textfelder zur Eingabe von Adressen.

**Name**
Name des Marktpartners.
> Technische Info: Alphanumerisches Feld, DB-Feld: mp.name

**Vorname**
Vorname des Marktpartners an.
> Technische Info: Alphanumerisches Feld, DB-Feld: mp.vname

**Anrede**
Auswahl der Anrede, z, B. Herr oder Frau (Stammdaten > Schlüssel > Marktpartner > Anreden).
> Technische Info: <F9>, DB-Feld: mp.anrede

**z.Hd.**
zu Händen. Name des Postempfängers bei Firmenadressen.
> Technische Info: Alphabetisches Feld, DB-Feld: mp.zhd

**Zusatz**
Feld für Zusatz, z. B. die Branche.
> Technische Info: Alphabetisches Feld, DB-Feld: mp.branche

**Straße**
Straße zur Adresse.
> Technische Info: Alphanumerisches Feld, DB-Feld: mp.str

**PLZ, Fach**
Die dem Postfach entsprechende Postleitzahl sowie die Nummer des Postfachs.
> Technische Info: Alphanumerisches Feld, DB-Feld: mp.pfplz / mp.postfach

**PF Ort**
Der dem Postfach zugehörige Ort.
> Technische Info: Alphanumerisches Feld, DB-Feld: mp.pfort

**PLZ, Ort**
Die dem Ort entsprechende Postleitzahl und der Ort.
> Technische Info: Alphanumerisches Feld, DB-Feld: mp.plz / mp.ort

**KFZ Land**
KFZ-Länderkennzeichen und das entsprechende Land.
> Technische Info: Alphanumerisches Feld, DB-Feld: mp.kfzcode / mp.land
> "Länder" auf Seite B-204

**Entfer.**
Die Entfernung zwischen Ihrer Firma und dem Marktpartner in Kilometer. Wird in der Rabatt/ Zuschlagsberechnung verwendet (z B Transportzuschlag) als Staffelbasis.
> Technische Info: Numerisches Feld, DB-Feld: mp.kilometer

**Telefon**
Telefonnummer des Marktpartners (Nummer des Festanschlusses).
> Technische Info: Numerisches Feld, DB-Feld: mp.telefon

**Mobil**
Telefonnummer des Marktpartners (Nummer des Festanschlusses).
> Technische Info: Numerisches Feld, DB-Feld: mp.mobile

**Fax**
Faxnummer des Marktpartners. Mit dem Toggle-Feld dahinter steuern Sie, ob der Marktpartner die Dokumente per Fax haben möchte. Mögliche Werte: J/N. Wird im Formulardruck ausgewertet und ermöglicht bei entsprechender Konfiguration das automatische Faxen von Dokumenten zum Marktpartner.
> Technische Info: Numerisches Feld, DB-Feld: mp.faxnr

**E-Mail**
E-Mail-Adresse des Marktpartners. Mit `<F5>` können Sie mehrere E-Mail-Adressen hinterlegen. Wird im Formulardruck ausgewertet und ermöglicht bei entsprechender Konfiguration das automatische versenden von Dokumenten zum Marktpartner per E-Mail.
> Technische Info: Alphanumerisches Feld, DB-Feld: mp.email

**Webseite**
URL des Marktpartners. Mit `<F5>` starten Sie den Browser.
> Technische Info: Alphanumerisches Feld, DB-Feld: mp.website

**Sprache**
Auswahl der Sprache, in der der Kunde seine Dokumente erhält, z, B. Deutsch oder Englisch (Stammdaten > System > Sprachen). Entsprechend dieser Definition werden die Texte bei der Vorgangserfassung generiert und bei entsprechender Konfiguration die Ausdrucke für Marktpartner in der angegebenen Sprache erstellt.
> Technische Info: <F9>, DB-Feld: mp.sprkz

**Anmerkungen**
Diese Texte dienen in den verschiedensten Programmteilen als wichtiges Informationsmedium. So können die Einträge u. a. in der Auftragserfassung bei Auswahl des Kunden auf dem Bildschirm angezeigt werden. Es gibt zwei unterschiedliche Anmerkungstexte:
- `<F5>` startet den Dialog für allgemeine Anmerkungstexte des Marktpartners.
- `<Shift> <F5>` startet den Dialog für artikelbezogene Anmerkungstexte des Marktpartners.
> Technische Info: DB-Feld: memo.txt

**Ergänzende Informationen**
- "Marktpartner - Anmerkungstexte" auf Seite B-106
- "Artikel - Anmerkungstexte" auf Seite B-386

## Marktpartner - Anmerkungstexte

*Stammdaten > Marktpartner > F5*

*Abb. B-10 Marktpartner Anmerkungstexte*

In diesem Dialog können Sie Texte für Marktpartner hinterlegen, die in den verschiedensten Programmteilen als wichtiges Informationsmedium dienen. Oben im Dialog sehen Sie die Marktpartner-Nummer, für die der Text gilt.

> **Mehrsprachige Anmerkungstexte**
> Seit QR2209 können Sie in A+W Enterprise auch für Anmerkungen mehrsprachige Bezeichnungen hinterlegen. Diese Möglichkeit besteht jedoch nur, wenn Sie mit dem Modul Mehrsprachigkeit für Mitarbeiter innerhalb der internen Mandantentrennung arbeiten.

**Sprache**
Sprachkennzeichen.
> Technische Info: Numerisches Feld, DB-Feld: xsprbez.sprkz

Geben Sie den Text in dem freien Feld ein und speichern Sie diesen mit `<F3>`. Mit `<Shift><F9>` legen Sie den Info-Ort fest:
- **Stammdaten:** Der Text wird nur in den Stammdaten angezeigt.
- **Überall:** Der Text wird in den Stammdaten und in den Verkaufs- und Einkaufsvorgängen angezeigt.
- **VK-Auftrag:** Der Text wird im Verkaufsvorgang angezeigt.
- **EK-Auftrag:** Der Text wird im Einkaufsvorgang angezeigt.

Mit `<Shift><F10>` legen Sie die Priorität fest:
- **hoch:** Der Text wird automatisch an den festgelegten Info-Orten angezeigt, sobald nur eine Zeile die Prio-hoch hat.
- **niedrig:** Der Text wird nicht automatisch angezeigt, er muss bei der Vorgangserfassung über das Menü aufgerufen werden.
> Technische Info: Alphanumerisches Feld, DB-Feld: memo.txt

> **Priorität bei Info-Ort Stammdaten**
> Wenn Sie als Info-Ort Stammdaten gewählt haben, greift die Priorität niedrig nicht. Der Text wird immer in den Stammdaten des Marktpartners angezeigt.

## Register Identifikation

*Stammdaten > Marktpartner > Register Identifikation*

*Abb. B-11 Marktpartner - Register Identifikation*

In diesem Register erfassen und/oder bearbeiten Sie alle steuerlichen und provisionsmäßigen Daten des Marktpartners.

> **Linker Dialogteil**
> Während der Bearbeitung der rechten Dialogseite bleiben die Stammdaten des Kunden im linken Dialogteil weiterhin sichtbar. Sind Änderungen notwendig, müssen diese im Register Adresse vorgenommen werden.

**USt-Identnr.**
EG-Steuernummer, d. h. die Umsatzsteueridentnummer. Bei der Eingabe der USt-Identnr. erfolgt eine länderspezifische Prüfung. Diese Nummer wird vorwiegend in der FIBU-Übergabe verwendet.
> Technische Info: Alphanumerisches Feld, DB-Feld: mp.steuernr

**FA-Steuernr.**
Angabe zur Finanzamtssteuernummer, die vorwiegend in der FIBU-Übergabe verwendet wird. Es ist auch möglich, das System so zu konfigurieren, dass eine Erfassung von Gutschriften ohne FA-Steuernr nicht möglich ist.
> Technische Info: Alphanumerisches Feld, DB-Feld: mp.finstnr

**Firmierung**
Vollständiger Firmenname des Marktpartners, z. B. Schmidt GmbH & Co. KG.
> Technische Info: Alphanumerisches Feld, DB-Feld: mp.firmname

**Externe Liefnr.**
Falls der Marktpartner eine eigene Lieferantennummer vorgibt, können Sie diese hier hinterlegen. Das Feld wird vorwiegend in der FIBU-Übergabe verwendet.
> Technische Info: Alphanumerisches Feld, DB-Feld: mp.exlinr

**Externe Kundennr.**
Falls der Marktpartner eine eigene Kundennummer vorgibt, können Sie diese hier hinterlegen. Das Feld wird vorwiegend in der FIBU-Übergabe verwendet.
> Technische Info: Alphanumerisches Feld, DB-Feld: mp.extkundnr

**Externe Objektnr.**
Dieses Feld ist nur aktiv, wenn der Marktpartner vom Typ Objekt ist. Dann können Sie hier eine externe Objektnummer hinterlegen.
> Technische Info: Alphanumerisches Feld, DB-Feld: mp.extkundnr

**Liefnr.**
Auswahl der Lieferantennummer. Wenn es sich bei dem Marktpartner um einen Kunden handelt, der auch als Lieferant fungiert, dann können Sie hier die Lieferantennummer zuordnen. Das Feld wird vorwiegend in der FIBU-Übergabe verwendet.
> Technische Info: <F9>, DB-Feld: mp.lieflinr

**Matchcode**
Dieses Feld steht in Zusammenhang mit dem Feld Liefnr. und zeigt Ihnen den Matchcode des Lieferanten.
> Technische Info: Anzeige-Feld

**Div.-Marktp.**
Hier handelt es sich um einen Marktpartner, der nur einmal bestellt bzw. beliefert wird. Bei diesem Kunden kann im Gegensatz zu den anderen Kunden in der Vorgangserfassung, die Rechnungsadresse geändert werden:
- **Ja:** Bei dem Marktpartner handelt es sich um einen diversen Marktpartner.
- **Nein:** Der Marktpartner wird als permanenter Kunde geführt.
> Technische Info: Toggle-Feld, DB-Feld: mp.divers

**Provision**
Auswahl des Provisionsschlüssels. Steht die Höhe der Vertreterprovision in Abhängigkeit zum Kunden, muss hier ein numerischer Provisionsschlüssel eingegeben werden. Die Provisionssätze für die verschiedenen Schlüsselwerte werden im Menüpunkt Provisionskürzel (Stammdaten > Provisionen) hinterlegt. Das Feld ist nur bei entsprechender Systemkonfiguration verfügbar.
> Technische Info: <F9>, DB-Feld: mp.provnr

**Vertr. (Erlös)**
Auswahl des erlösmäßigen Vertreters. Für den hier eingetragenen Mitarbeiter werden dann die jeweiligen Provisionssätze gebucht und stehen zur Abrechnung bereit. Diese Angaben können später im Auftrag geändert werden. Voraussetzung für die Auswahlmenge ist die Funktionszuordnung Vertreter in den Mitarbeiter-Stammdaten. Bei erweiterter interner Mandatentrennung kann diese Angabe auch mandantengenau erfolgen.
> Technische Info: <F9>, DB-Feld: mp.vertrerloe

**Außendienst**
Auswahl des zuständigen Außendienstmitarbeiters. Diese Angaben werden in die Auftragserfassung übernommen und gegebenenfalls auf den kundenseitigen Papieren ausgegeben. Diese Angaben können später im Auftrag geändert werden.
> Technische Info: <F9>, DB-Feld: mp.aussenmanr

**Innendienst**
Auswahl des zuständigen Innendienstmitarbeiters. Diese Angaben werden in die Auftragserfassung übernommen und gegebenenfalls auf den kundenseitigen Papieren ausgegeben. Diese Angaben können später im Auftrag geändert werden.
> Technische Info: <F9>, DB-Feld: mp.innenmanr

**Sachbearbeiter**
Auswahl des zuständigen Mitarbeiters für die Auftragsbearbeitung. Er wird in den Auftrag übernommen und gegebenenfalls auf den kundenseitigen Papieren ausgedruckt. Diese Angaben können später im Auftrag geändert werden.
> Technische Info: <F9>, DB-Feld: mp.sachmanr

**Ergänzende Informationen**
- "Marktpartner - Anmerkungstexte" auf Seite B-106
- "Artikel - Anmerkungstexte" auf Seite B-386

## Register Bezüge

*Stammdaten > Marktpartner > Register Bezüge*

*Abb. B-12 Marktpartner - Register Bezüge*

In diesem Register erfassen und/oder bearbeiten Sie alle FIBU-technischen und ein Teil der preisrelevanten Daten des Marktpartners. Auf der rechten Seite werden Ihnen die Adressinformationen angezeigt.

### Erläuterung der Felder

**FIBU-Debitor**
Auswahl der FIBU-Debitorennummer. Sie ist ein Verweis auf den rechnungsempfangenden Kunden. Daher werden FIBU-Debitor und Kundennummer gleich sein. Im Falle einer zentralen Rechnungsverwaltung eines Unternehmens mit mehreren Zweigstellen muss der FIBU-Debitor mit der Kundennummer der Rechnungsstelle belegt werden, auf die dann die Rechnungen verbucht und ausgestellt werden.
> Technische Info: <F9>, DB-Feld: mp.stddebnr

**Statistik-Debitor**
Auswahl des Statistik-Debitors. Unabhängig vom FIBU-Debitor können die statistischen Umsätze auf andere Statistik-Debitoren kumuliert werden. Das könnte z. B. die Kundennummer einer auftraggebenden Zweigstelle sein. Die statistischen Daten geben dann Aufschluss über die Umsatzentwicklung der einzelnen Filialen.
> Technische Info: <F9>, DB-Feld: mp.statdebnr

**Konditions-Debitor**
Auswahl der Kundennummer, deren Konditionen für die erfassten Vorgänge gelten soll. Bei erweiterter interner Mandantentrennung kann der Konditions-Debitor auch mandantengenau erfolgen.
> Technische Info: <F9>, DB-Feld: mp.konddebnr

**AZ-Debitor**
Auswahl der Kundennummer. Analog gelten die Austausch-Zusatz-Regeln in der Vorgangserfassung, die für den Kunden hinterlegt wurden, der in diesem Feld vermerkt wurde.
> Technische Info: <F9>, DB-Feld: mp.azdebnr

**Debitor**
Auswahl, ob Debitor:
- **Ja:** Der Marktpartner ist ein Debitor.
- **Nein:** Der Marktpartner ist kein Debitor.
> Technische Info: <F9>, DB-Feld: mp.debitor

**Debitor-Hausnr.**
Ist nur aktiv, wenn das Feld Debitor den Eintrag Ja hat. Dann können Sie dem Debitor ein Haus zuordnen. Diese Angaben sind nur bei erweiterten internen Mandantentrennung relevant. Nähere Information darüber kann der A+W Enterprise-Konfigurationsanleitung entnommen werden.
> Technische Info: <F9>, DB-Feld: mp.debhausnr

**Kond. Branche**
Auswahl der Branche, z. B. Schreiner, Metallbau, etc. Die entsprechenden Konditionen werden im Menü Brance (Stammdaten > Schlüssel > Marktpartner > Branche) hinterlegt.
> Technische Info: <F9>, DB-Feld: mp.kbranche

**Wirtsch.-Raum**
Auswahl des Wirtschaftsraums, in dem sich der Marktpartner befindet, z. B. Frankreich, Niederlande, Belgien, etc.. Der Wirtschaftsraum wird sehr oft in die eigenen statistischen Auswertungen herangezogen.
> Technische Info: <F9>, DB-Feld: mp.kwrtraum

**Region**
Auswahl der Region, in der sich der Marktpartner befindet, z. B. Hessen, Niedersachsen, Bayern, etc.. Die Regionen werden im Menü Region / Bundesländer (Stammdaten > Schlüssel > Marktpartner > Region / Bundesländer) hinterlegt.
> Technische Info: <F9>, DB-Feld: mp.region

**Kostenstelle**
Auswahl der Kostenstelle des Marktpartners, z. B. Isolierglas, ESG, Gestelle, etc.. Kostenstellen sind sinnvolle betriebliche Bereiche (Abteilungen, Gruppen), die eingrenzbare Kosten verursachen. Die gewählte Kostenstelle kann später ausgewertet werden. Kostenstellen werden im Menü Kostenstellen (Stammdaten > Kostenstamm > Kostenstellen) hinterlegt.
> Technische Info: <F9>, DB-Feld: mp.kostenst

**Abteilung**
Auswahl einer Abteilung, z. B. Zuschnitt, Versand, etc..
> Technische Info: <F9>, DB-Feld: mp.abtnr

**Kalender**
Auswahl einer spezifischen Marktpartner-Kalendernummer.
> Technische Info: <F9>, DB-Feld: mp.kalnr

**Ergänzende Informationen**
- "Marktpartner - Anmerkungstexte" auf Seite B-106
- "Artikel - Anmerkungstexte" auf Seite B-386

## Register Auftrag

*Stammdaten > Marktpartner > Register Auftrag*

*Abb. B-13 Marktpartner - Register Auftrag*

In diesem Register werden alle auftragsbezogenen Informationen des Marktpartners hinterlegt. Auf der rechten Seite werden Ihnen die Adressinformationen angezeigt.

### Erläuterung der Felder

**Kantenschutz**
Auswahl des gewünschten Kantenschutzartikels, der bei ISO angebracht werden soll. Damit erfolgt automatisch ein entsprechender Eintrag bei den Kunden-Austausch-Zusatzregeln, die während der Auftragserfassung ausgewertet werden.
> Technische Info: <F9>, DB-Feld: mp.kantschutz

**Stdverglasg**
Auswahl der gewünschten Verglasungsartikels, der bei ISO angebracht werden soll. Damit erfolgt automatisch ein entsprechender Eintrag bei den Kunden-Austausch-Zusatzregeln, die während der Auftragserfassung ausgewertet werden.
> Technische Info: <F9>, DB-Feld: mp.stdverglas

**Verglasung**
Auswahl, wo die Verglasung angezeigt wird:
- In Position und Fuß ausweisen
- In Position einrechnen
- Nur im Fuß ausweisen
> Technische Info: Toggle-Feld, DB-Feld: mp.verglasung

**Objektzwang**
Definition, ob dem Kunden im Auftrag zwingend ein Objekt zugeordnet werden muss:
- **Ja:** Dem Kunden muss im Auftrag immer ein Objekt zugeordnet werden.
- **Nein:** Eine Objektzuordnung ist optional.
> Technische Info: Toggle-Feld, DB-Feld: mp.objmuss

**FremdnrZwang**
Definition, ob dem Kunden im Auftrag zwingend eine Fremdnummer zugeordnet werden muss:
- **Ja:** Dem Kunden muss im Auftrag immer eine Fremdnummer zugeordnet werden.
- **Nein:** Die Zuordnung einer Fremdnummer ist optional.
> Technische Info: Toggle-Feld, DB-Feld: mp.exaufmuss

**KommissZwang**
Definition, ob dem Kunden im Auftrag zwingend eine Kommission zugeordnet werden muss:
- **Ja:** Dem Kunden muss im Auftrag immer eine Kommission zugeordnet werden.
- **Nein:** Die Zuordnung einer Kommission ist optional.
> Technische Info: Toggle-Feld, DB-Feld: mp.kommmuss

**Maßheinheit**
Auswahl der Maßeinheit:
- Metrisch
- Imperial
Für die Nutzung der imperialen Maßeinheit muss das System entsprechend konfiguriert werden.
> Technische Info: Toggle-Feld, DB-Feld: mp.massystem

**Standard-SZR**
Hier können Sie den Wert für einen Standard-Rahmen in mm hinterlegen. Dieser Wert wird dann als Vorbelegung in der Auftragserfassung bei ISO-Positionen ohne fixen SZR verwendet.
Ist für einen ISO Artikel in den Artikelstammdaten ein nicht änderbarer SZR definiert, so wird der SZR des Artikels verwendet. Ist der SZR jedoch als änderbar definiert, wird der kundenindividuelle SZR verwendet.
Wenn der SZR in den Artikelstammdaten als änderbar definiert ist, ist auch der kundenindividuelle SZR ist in der Positionserfassung änderbar.
> Technische Info: Numerisches Feld, DB-Feld: mp.defszr

**min ISO ges. Stärke**
Hier können Sie die minimale Stärke einer gesamten ISO-Einheit hinterlegen.
> Technische Info: Numerisches Feld, DB-Feld: mp.minszr

**max ISO ges. Stärke**
Hier können Sie die maximale Stärke einer gesamten ISO-Einheit hinterlegen.
Minimale und maximale Stärke werden innerhalb der Restriktionsprüfung in der Auftragserfassung geprüft. Wenn ein Auftrag Positionen, die diese Restriktion nicht erfüllen, enthält, kann der Auftrag nur von berechtigten Mitarbeitern erfasst werden. Die weiteren Information kann der A+W Enterprise - EDV-Modulbeschreibung entnommen werden.
> Technische Info: Numerisches Feld, DB-Feld: mp.maxszr

**Mindestwert**
Hier können Sie einen Mindestauftragswert (Kunden) bzw. einen Mindestbestellwert (für Lieferanten) hinterlegen. Dieser Wert wird als Berechnungsgrundlage in den Auftrag übernommen. Ist der Auftragswert < Mindestwert, wird der Mindestwert berechnet.
Der Mindestauftragswert bzw. Mindestbestellwert müssen zwingend in Kundenwährung angegeben werden. Andernfalls, bei Währungsänderung im Auftrag, erfolgt keine Umrechnung des Mindestwertes.
> Technische Info: Numerisches Feld, DB-Feld: mp.relimwert

**Ergänzende Informationen**
- "Marktpartner - Anmerkungstexte" auf Seite B-106
- "Artikel - Anmerkungstexte" auf Seite B-386

## Register Lieferung

*Stammdaten > Marktpartner > Register Lieferung*

*Abb. B-14 Marktpartner - Register Lieferung*

In diesem Register werden alle Informationen, die die Lieferung an den Marktpartner betreffen, hinterlegt. Auf der rechten Seite werden Ihnen die Adressinformationen angezeigt.

### Erläuterung der Felder

**Std.-Route**
Auswahl der Route. Für die Versandplanung sollte jeder Kunde einer Route zugeordnet werden. Die Route wird in den Auftrag übernommen, die beim Bedarf geändert werden kann. Von dort aus wird die Route an das Versandsteuerungssystem weitergereicht. Im Menüpunkt Routen (Stammdaten > Schlüssel > System > Versand > Routen) werden die Routen hinterlegt.
> Technische Info: <F9>, DB-Feld: mp.routenr

**Route 2-4**
Definition von Alternativ-Routen, die verwendet werden können, wenn die Standard-Route nicht optimal zum Kundenwunschtermin passt. Bei der Lieferterminbestimmung im Auftrag wird dann berechnet, ob eine Alternativroute günstiger ist. Die Felder Route 2-4 sind nur dann änderbar, wenn das System nicht für Routen aus den Adressenstamm konfiguriert ist.
> Technische Info: <F9>, DB-Feld: mp.routenr2, routenr3, routenr4

**Ladefolge**
Definition der Ladefolge. Bei der Zusammenstellung einer Tour werden Auftragspositionen verschiedener Kunden auf ein Fahrzeug geladen. Die Reihenfolge der Beladung kann durch die Ladefolge vorgegeben werden. Der Eintrag erfolgt frei und wird im Versandsteuerungssystem angezeigt und kann auf den Ladepapieren ausgewertet werden. Über `<F9>` kann der Überblick verschaffen werden, welche Lagefolgen bereits vergeben wurden.
Bei Verwendung des Moduls OTR wird die Ladereihenfolge aus OTR übernommen werden.
> Technische Info: <F9>, DB-Feld: mp.routeposnr

**Versandart**
Auswahl der Versandart, z. B. LKW, Spedition, etc. Dieses Feld hat ausschließlich informativen Charakter für die Versandabteilung. Die Versandarten werden im Menü Verpackungsart (Stammdaten > Schlüssel > System > Versand > Versandart) angelegt.
> Technische Info: <F9>, DB-Feld: mp.versandart

**Verpackart**
Auswahl der Verpackungsart, z. B. Gestell, Kiste, Gitterbox, etc. Dieses Feld hat ausschließlich informativen Charakter für die Versandabteilung. Die Versandarten werden im Menü Verpackungsart (Stammdaten > Schlüssel > System > Versand > Verpackungsart) angelegt.
> Technische Info: <F9>, DB-Feld: mp.verpackart

**Lieferart**
Auswahl der Lieferbedingung, z. B. frei Haus, Selbstabholer, etc. Dieser Text ist für Ausdruck auf den Kundenpapieren vorgesehen. Die Lieferarten werden im Menü Verpackungsart (Stammdaten > Schlüssel > System > Versand > Lieferarten) angelegt.
> Technische Info: <F9>, DB-Feld: mp.lieferart

**Sammellieferschein**
Auswahl, ob für den Marktpartner ein Sammellieferschein möglich ist oder nicht:
- **Ja:** Ein Sammellieferschein ist möglich.
- **Nein:** Sammellieferschein ist nicht möglich.
> Technische Info: Toggle-Feld, DB-Feld: mp.Isammel

**Teillieferung möglich**
Auswahl, ob der Marktpartner Teillieferungen erlaubt oder nicht:
- **Ja:** Teillieferungen sind erlaubt.
- **Nein:** Teillieferungen sind nicht erlaubt.
> Technische Info: Toggle-Feld, DB-Feld: mp.teilliefkz

**Handlingszeit**
Ist der Zeitraum zwischen der Fertigstellung des Produktes und dem Tag der Auslieferung. Eine solche Zeit kann notwendig werden, wenn der Kunde bestimmte Vorgaben für die Kommissionierung seiner Ware trifft. Sie wird als Frist eingetragen und damit von der Termin- und Kapazitätsplanung berücksichtigt. Die Zeit kann in Tagen oder in Stunden eingegeben werden (konfigurierbar).
> Technische Info: Numerisches Feld, DB-Feld: mp.hzeit

**Anruf vor Auslieferung**
Auswahl, ob der Marktpartner vor der Auslieferung telefonisch kontaktiert werden soll oder nicht:
- **Ja:** Der Marktpartner möchte vor der Auslieferung angerufen werden.
- **Nein:** Ein Anruf ist nicht nötig.
> Technische Info: Toggle-Feld, DB-Feld: mp.anruf

**Fahrtdauer**
Hier können Sie die Fahrtdauer zum Marktpartner in Tagen hinterlegen. Dieser Wert wird dann bei der Kalkulation des Liefertermins mit berücksichtigt.
> Technische Info: Numerisches Feld, DB-Feld: mp.anfahrt

**Auslieferung via**
Auswahl, ob die Auslieferung über ein anderes Haus statt findet. Nähere Erläuterungen finden Sie in den Dokumenten zur via plant-Logik.
> Technische Info: <F9>, DB-Feld: mp.vsvia

**Typ der DFÜ**
Handelt es sich bei diesem Marktpartner um einen internen Kunden, so kann hier definiert werden, wie interne Bestellungen per DFÜ ausgetauscht werden. Die Einstellung hat insbesondere Auswirkungen darauf, wie die Adressen in den erzeugten Bestellungen und Aufträgen behandelt werden:
- **keine:** Es erfolgt keine automatische interne Bestellübertragung.
- **VKKopplung:** Aus dem Auftrag im Handelshaus werden die zu bestellenden Teile bestellt. Es wird ein Auftrag direkt im System des Lieferanten erzeugt.
- **EK 1:1:** Aus dem Auftrag im Handelshaus werden die zu bestellenden Teile bestellt. Dabei wird erst eine entsprechende Bestellung im Handelshaus erzeugt und aus dieser wird ein Auftrag direkt im System des Lieferanten erzeugt. Eine Bestellung enthält bei dieser Einstellung immer nur Bestellteile aus einem Auftrag.
- **EK 1:n:** Aus dem Auftrag im Handelshaus werden die zu bestellenden Teile bestellt. Dabei wird erst eine entsprechende Bestellung im Handelshaus erzeugt und aus dieser wird ein Auftrag direkt im System des Lieferanten erzeugt. Eine Bestellung kann dabei Bestellteile aus mehreren Aufträgen enthalten.
> Technische Info: <F9>, DB-Feld: mp.dfuetyp

**Direktbestellung**
Auswahl für Direktbestellung. Das Feld ist nur aktiv, wenn es sich bei dem Marktpartner und einen Lieferanten handelt. Damit steuern Sie, ob eine Bestellung bei diesem Lieferanten nach Auftragsfreischaltung sofort ausgelöst wird oder nicht:
- **Ja:** Bestellung wird sofort ausgelöst.
- **Nein:** Die Bestellung wird nicht sofort erzeugt, sondern wird zunächst in dem Bestellpool gestellt und kann später ausgelöst werden.
> Technische Info: Toggle-Feld, DB-Feld: mp.direktbestkz

**Lieferscheinübertragung**
Über diese Checkbox steuern Sie die automatische Lieferscheinübertragung:
- [x] Die Lieferscheinübertragung erfolgt automatisch per OpenTRANS.
- [ ] Es erfolgt keine Lieferscheinübertragung
> Technische Info: Toggle-Feld, DB-Feld: mp.liefdfuekz

**Ergänzende Informationen**
- "Marktpartner - Anmerkungstexte" auf Seite B-106
- "Artikel - Anmerkungstexte" auf Seite B-386

## Register Rechnung

*Stammdaten > Marktpartner > Register Rechnung*

*Abb. B-15 Marktpartner - Register Rechnung*

In diesem Register werden alle Informationen, die die Rechnung an den Marktpartner betreffen, hinterlegt. Auf der rechten Seite werden Ihnen die Adressinformationen angezeigt.

### Erläuterung der Felder

**Konto**
9stellige Kontonummer. Mit der Einführung der IBAN wird dieses Feld nicht mehr ausgewertet.
> Technische Info: Numerisches Feld, DB-Feld: mp.konto

**Rechnungsart**
Auswahl der gewünschten Rechnungsform vom Marktpartner:
- Einzelrechnung
- Deckblattrechnung
- Sammelrechnung (wöchentlich, 14-tägig, monatlich)
> Technische Info: Toggle-Feld, DB-Feld: mp.rechnungsart

**Sammelrechnungslimit**
Hier geben Sie ein, wie hoch das Rechnungslimit für die Sammelrechnungen ist.
> Technische Info: Numerisches Feld, DB-Feld: mp.srechlimit

**Sammelrechnungsart**
Auswahl des Turnus, in dem die Sammelrechnungen geschrieben werden:
- wöchentlich
- 14-tägig
- monatlich
> Technische Info: Toggle-Feld, DB-Feld: mp.srechart

**FIBU**
Falls die angebundene Finanzbuchhaltung die getrennte Übergabe verschiedener Zahlungsziele nicht erlaubt, kann dieses Feld alternativ mit einem beliebigen alphanumerischen Code versehen werden, der an die Finanzbuchhaltung übergeben wird. Die konkrete Nutzung der Felder ist maßgeblich vom verwendeten Fibu-System abhängig.
> Technische Info: Numerisches Feld, SELO (<F9>), DB-Feld: mp.fibukey

**Rechnungsübertragung**
Auswahl, ob die Rechnungsübertragung im openTRANS-Format möglich ist.
- [x]: Die Übertragung ist im openTRANS-Format möglich.
- [ ]: Die Übertragung ist nicht möglich.
> Technische Info: Toggle-Feld,

**Gestelle berechnen**
Auswahl, ob der Marktpartner Teillieferungen erlaubt oder nicht:
- **Ja:** Gestelle werden in Rechnung gestellt.
- **Nein:** Gestelle werden nicht in Rechnung gestellt.
> Technische Info: Toggle-Feld, DB-Feld: mp.gsfaktura

**Mietfreie Tage**
Wenn Sie Ihrem Kunden die Gestelle eine gewisse Anzahl von Tagen überlassen, an denen die Gestelle nichts kosten, können Sie hier diese Anzahl an Tagen eingeben.
> Technische Info: Numerisches Feld, DB-Feld: mp.gsmietfrei

**Ergänzende Informationen**
- "Marktpartner - Anmerkungstexte" auf Seite B-106
- "Artikel - Anmerkungstexte" auf Seite B-386

## Register Kundenspezifisch

*Stammdaten > Marktpartner > Register Kundenspezifisch*

*Abb. B-16 Marktpartner - Register Kundenspezifisch*

Das Register ist nur aktiv, wenn es sich bei dem Marktpartner um ein Objekt handelt und entsprechend konfiguriert ist. In diesem Register werden alle Informationen, die das Objekt betreffen zusammengefasst. Auf der rechten Seite werden Ihnen die Adressinformationen angezeigt.

### Erläuterung der Felder

**Vertr. (Erlös)**
Jedem Objekt kann ein Vertriebsmitarbeiter zugeordnet werden, der als erlösmäßiger Vertreter für alle am Objekt beteiligten Aufträge in die Vertreter-Provisionierung einfließt.
> Technische Info: <F9>, DB-Feld: mp.vertrerloe

**Kostenstelle**
Ob die Kostenstelle objektindividuell in der Auftragsbearbeitung ersetzt werden soll, ist von dem gewählten Kostenstellenverfahren abhängig. Falls eine objektbezogene Kostenstellenvergabe gewünscht ist, kann dieses von A+W eingerichtet werden.
> Technische Info: <F9>, DB-Feld: mp.kostenst

**Objektzwang**
Steht dieses Feld auf J, muss in der Auftragserfassung ein Objekt zwingend eingegeben werden.
> Technische Info: Toggle-Feld, DB-Feld: mp.kommmuss

**Limitprüfung**
Objektorientierte Limitprüfung:
- **Fibu-Debitor:** Limitprüfung bei Auftragserfassung.
- **MP-Objekt:** Objektorientierte Limitprüfung.
> Technische Info: Toggle-Feld, DB-Feld: mp.objlimitpruef

**Firmenlimit**
Dieses Feld kommt nur zum Tragen, wenn das Feld Limitprüfung auf J gesetzt ist. Überschreitet ein Auftragswert zuzüglich der offenen Posten und des offenen Auftragsbestandes das an dieser Stelle hinterlegte Firmenlimit, so erfolgt eine Warnung.
> Technische Info: Numerisches Feld, DB-Feld: mp.firmlimit

**MWST**
Auswahl des Mehrwertsteuerkennzeichens. Die benötigten Steuerschlüssel werden im Menü Steuertypen (Schlüssel > System > Steuern) hinterlegt.
> Technische Info: <F9>, DB-Feld: mp.mwst

**Skonto 1/2**
Auswahl der Skontogruppenschlüssel. Die benötigten Skontoschlüssel werden im Menü Skontogruppen (Schlüssel > System > Skontogruppen) hinterlegt.
> Technische Info: Toggle-Feld, DB-Feld: mp.skonto1/2

**Rechnungsart**
Auswahl der gewünschten Rechnungsform vom Objekt:
- Einzelrechnung
- Deckblattrechnung
- Sammelrechnung (wöchentlich, 14-tägig, monatlich)
> Technische Info: Toggle-Feld, DB-Feld: mp.rechnungsart

**Std-Route**
Eine etwaige Objektroute greift übersteuernd in die Auftragsbearbeitung ein und ersetzt die im Kundenstamm hinterlegte Kundenroute.
> Technische Info: Toggle-Feld, DB-Feld: mp.routenr

## Register Zahlung

*Stammdaten > Marktpartner > Register Zahlung*

*Abb. B-17 Marktpartner - Register Zahlung*

In diesem Register werden alle Informationen, die die Zahlungsoptionen bezüglich der Marktpartner betreffen, hinterlegt. Auf der rechten Seite werden Ihnen die Adressinformationen angezeigt.

### Erläuterung der Felder

**Skonto 1-3**
In den Skontofeldern können die kundenindividuellen Skonti als Schlüssel zugewiesen werden. Bis zu drei gestaffelte Skonti sind möglich, deren Laufzeit und Prozentsatz entsprechend variieren muss. Die benötigten Skontoschlüssel werden im Menü Skontogruppen (Schlüssel > System) hinterlegt.
> Technische Info: <F9>, DB-Feld: mp.skonto1-3

**Urlaub berücksichtigen**
Auswahl, ob sich die Skontodauer verlängert, wenn der Rechnungsempfänger Urlaub hat:
- Die Skontodauer verlängert sich.
- Die Skontodauer verlängert sich nicht.
Voraussetzung ist, dass der Kalender für den jeweiligen Rechnungsempfänger gepflegt wird.
> Technische Info: Toggle-Feld, DB-Feld: mp.htag_skonto_rel

**Zahlziel**
Hierunter versteht man den spätestmöglichen Zeitpunkt der Nettozahlung. Nach Ablauf des Zahlzieles beginnt die Mahnfrist. Die Eingabe erfolgt in Tagen.
> Technische Info: Numerisches Feld, DB-Feld: mp.zahlziel

**Valuta**
Die Valutierung in Tagen bestimmt den Beginn der Skontofristen und des Zahlungszieles ab Rechnungsdatum (zuzüglich Postweg).
> Technische Info: Numerisches Feld, DB-Feld: mp.valuta

**Merkmal**
Über die Schlüssel können Zahlungsmerkmale für Marktpartner vermerkt werden (Lastschrift, Abbuchung, etc.). Die Schlüssel werden im Menü Zahlungsmerkmal (Schlüssel > System) hinterlegt.
> Technische Info: <F9>, DB-Feld: mp.zahlngmerk

**Bonus**
Hier definieren Sie ob und in welcher Höhe sowie innerhalb welchen Zeitraumes der Kunde/Objekt einen Bonus erhält. Der Bonus wird nicht automatisch errechnet. Diese Angabe dient lediglich eigenen statistischen Anfragen. Die Bonusschlüssel werden im Menü Bonus (Schlüssel > System > Marktpartner) hinterlegt.
> Technische Info: <F9>, DB-Feld: mp.bonus

**Zahlungsverkehr**
Auswahl des Zahlungsverkehrs:
- Bankeinzug
- Vorauskasse
- Bei Lieferung
- Nach Vereinbarung
- Scheck
- Banklastschrift
> Technische Info: Toggle-Feld, DB-Feld: mp.azahlkz

> **Zahlungsfelder für Marktpartnertyp=Objekt**
> Bei entsprechender Systemkonfiguration können die Felder Skonto1-Zahlungsverkehr auch für Objekte hinterlegt werden. Diese Zahlungskonditionen werden anschließend im Block in den Auftrag übernommen, sofern das Objekt erfasst wird. Bleiben die betroffene Felder für Objekt leer, wird die Information aus dem Kundenstamm übernommen.

**Mahnung**
Auswahl, ob im Verzugsfall eine Mahnung erfolgen soll.
- [x] Der Kunde wird gemahnt.
- [ ] Der Kunde wird nicht gemahnt.
> Technische Info: Toggle-Feld, DB-Feld: mp.mahnkz

**Gemahnt**
Zur Information kann notiert werden, wie viele Mahnungen bereits an den Kunden/Objekt ergangen sind. Dieser Wert kann ggf. an die Fibu übermittelt werden.
> Technische Info: Numerisches Feld, DB-Feld: mp.mahnanz

**ltz. Schufa-Anfr.**
Hier können Sie das Datum der letzten Schufa-Anfrage eingeben.
> Technische Info: Datums-Feld, DB-Feld: mp.ltzschufa

**Teilfakt. möglich**
Auswahl, ob der Marktpartner Teilfakturierungen erlaubt oder nicht:
- **Ja:** Teilfakturierungen sind erlaubt.
- **Nein:** Teilfakturierungen sind nicht erlaubt.
> Technische Info: Toggle-Feld, DB-Feld: mp.teilfakkz

**Währung**
Das Mehrwährungssystem ist optional. Auswahl der Währung, in der der Marktpartner abgerechnet wird. Die Währungsschlüssel werden im Menü Währung (Stammdaten > Schlüssel > System) hinterlegt.
> Technische Info: <F9>, DB-Feld: mp.waehrung

**Kalkulat. in**
Das Mehrwährungssystem ist optional. Auswahl, in welcher Währung die Auftragsberechnung erfolgen soll:
- Eigenwährung der Firma
- Fremdwährung des Kunden, falls die Kundenwährung von der Eigenwährung der Firma abweicht, z. B. Kunde in der Schweiz.
> Technische Info: Toggle-Feld, DB-Feld: mp.waehrprs

**Ausdruck in**
Haben Sie im Feld Kalkulat. in die Auswahl Fremdwährung getroffen, dann steuern Sie hier, in welcher Währung die kundenseitigen Papiere ausgegeben werden sollen. Mögliche Werte sind:
- kalkulierte Währung
- Fremdwährung im Fuß
- Fremdwährung in Pos. und Fuß
- Kalk. Währung + Euro im Fuß
- Kalk. Währung + Euro in Pos. und Fuß
- Fremdwährung + Euro im Fuß
- Fremdwährung + Euro in Pos. und Fuß
> Technische Info: Numerisches Feld, DB-Feld: mp.waehrdru

> **Die Felder Kalkulation in und Ausdruck**
> Die Felder Kalkulation in und Ausdruck in sind nur zugänglich, wenn das Fremdwährungsmodul lizenziert und dem Kunden eine Währung zugeordnet wurde, die von der eigenen Währung abweicht.

## Register Ausdruck

*Stammdaten > Marktpartner > Register Ausdruck*

*Abb. B-18 Marktpartner - Register Ausdruck*

In diesem Register werden alle Informationen, die die Druckoptionen an den Marktpartner betreffen, hinterlegt. Auf der rechten Seite werden Ihnen die Adressinformationen angezeigt.

### Erläuterung der Felder

**Bruttopreis drucken**
Auswahl, ob der Bruttopreis ausgedruckt werden soll:
- Ja
- Nein
> Technische Info: Toggle-Feld, DB-Feld: mp.preisdrkz

**MP-Faktor drucken**
Auswahl, ob der Marktpartner-Faktor ausgedruckt werden soll:
- Ja
- Nein
> Technische Info: Toggle-Feld, DB-Feld: mp.rabdrkz

**Bearbeitungen drucken**
Mit diesem Feld steuern Sie, ob die Bearbeitungspreise bereits in der Vorgangserfassung in die zu druckenden Bearbeitungstexte generiert werden:
- Ja
- Nein
- P: Konfigurierbare Möglichkeit, die Preise für die Bearbeitungen nur dann in die Texte zu generieren, wenn diese vorhanden sind (Bearbeitungspreis > 0).
> Technische Info: Toggle-Feld, DB-Feld: mp.explbearbkz

**Zwischensumme**
Auswahl, ob eine kommissionsabhängige Zwischensumme gedruckt werden soll:
- Ja
- Nein
> Technische Info: Toggle-Feld, DB-Feld: mp.sumkomis

**AB mit Sprossen**
Auswahl, ob der Sprossenaufbau mit der Auftragsbestätigung gedruckt werden sollen:
- Ja
- Nein
> Technische Info: <F9>, DB-Feld: mp.sprossenab

**Bruttonettokennz.**
Auswahl für Brutto- oder Nettokennzeichen:
- **B:** Bruttokennzeichen
- **N:** Nettokennzeichen
> Technische Info: <F9>, DB-Feld: mp.brutnetkz

**Kundenind. Positionen**
Auswahl für kundenindividuelle Positionsbezeichnungen, falls im Kundenstamm ein entsprechender Hinweis existiert:
- **Pos.:** Für Kunden, die diese Kennzeichnung tragen, wird in der Auftragsbearbeitung das Kundenpositionsfeld zugeschaltet, um die gewünschte Kunden-Positionsbezeichnung einzugeben. Diese Angaben erscheinen auf allen kundenseitigen Papieren und Etiketten.
- **Typ:** Hierbei handelt es sich um die Möglichkeit der typisierten Erfassung, wie es häufig bei Leistungsverzeichnissen öffentlicher Ausschreibungen gefordert wird. Bei dieser Vorgehensweise wird jedem Produkt eine vorgegebenen Typenbezeichnung im Rahmen der Auftragserfassung zugeordnet. Der Ausdruck einer solchen Auftragsbestätigung weist im Positionsteil nur die jeweilige Typbezeichnung aus, während im Fuß des Dokuments die genaue Produktbeschreibung dargestellt wird.
- **Keine**
> Technische Info: Toggle-Feld, DB-Feld: mp.kndposkz

**Etikett**
Auswahl für Etikettentext. Die Schlüssel können über das Menü Etikettentexte (Stammdaten > Schlüssel > Marktpartner) vergeben werden.
> Technische Info: <F9>, DB-Feld: mp.etikett

**Etikett-Text**
Wenn es sich bei dem Marktpartner um ein Objekt handelt können Sie hier einen weiteren Text für Etiketten eingeben.
> Technische Info: <F9>, DB-Feld: mp.etitxt1

**Objekt-Kürzel**
Da auf Etiketten häufig nur wenig Platz zur Verfügung steht, kann auch das zweibuchstabige Objektkürzel auf dem Etikett ausgewiesen werden.
> Technische Info: Alphanumerisches Feld, DB-Feld: mp.etitxt2

**Preisdarstellung**
Auswahl für die Preisdarstellung auf den Papieren nach Wunsch des Marktpartners:
- kein Preis
- ME-Preis
- Stückpreis
- ME-+Stückpreis
> Technische Info: <F9>, DB-Feld: mp.prsdarst

**Textformeln**
Auswahl der Textformel.
> Technische Info: <F9>, DB-Feld: mp.artkennfrm

**Max. E-Mailgröße**
Maximale Größe der E-Mail mit Anhang in MByte. Beim E-Mail-Versand wird standardmäßig der Anhang in das zip-Format komprimiert. Durch eine Systemkonfiguration können Sie einstellen, ob der gesamte Anhang komprimiert wird, oder nur, wenn der Anhang die hier im Feld eingegebene E-Mailgröße überschreitet.
> Technische Info: <F9>, DB-Feld: mp.mailsize

## Register Limits

*Stammdaten > Marktpartner > Register Limits*

*Abb. B-19 Marktpartner - Register Limits*

In diesem Register werden alle Informationen, die die Limits bezüglich der Marktpartner betreffen, hinterlegt. Auf der rechten Seite werden Ihnen die Adressinformationen angezeigt.

### Erläuterung der Felder

**Limitprüfung via**
Auswahl der Limitprüfung:
- **Fibu-Debitor:** Die Limitprüfung erfolgt bei der Auftragserfassung für den entsprechenden Kunden (Fibu-Debitor).
- **MP-Objekt:** Die Limitprüfung erfolgt bei der Auftragserfassung, wenn dieses Objekt dem Auftrag zugeordnet ist und das System entsprechend konfiguriert ist.
> Technische Info: <F9>, DB-Feld: mp.objlimitpruef

**Firmenlimit**
Betrag in Eigenwährung bis zu dem die Firma dem Kunden Kredit gewährt. Bei entsprechender Konfiguration wird der Auftragswert zuzüglich der offenen Posten und der offenen Aufträge gegen das an dieser Stelle hinterlegte Firmenlimit geprüft.
> Technische Info: Numerisches Feld, DB-Feld: mp.firmlimit

**Versichert bis**
In diesem Feld kann das Ablaufdatum der Kreditlimit hinterlegt werden.
> Technische Info: Numerisches Feld, DB-Feld: mp.firmlimverfall

**AKV-Limit**
Betrag in Eigenwährung bis zu dem die Firma dem Kunden Kredit gewährt. Bei entsprechender Konfiguration wird der Auftragswert zuzüglich der offenen Posten und der offenen Aufträge gegen das an dieser Stelle hinterlegte AKV-Firmenlimit geprüft.
> Technische Info: Numerisches Feld, DB-Feld: mp.akvlimit

**Versichert bis**
In diesem Feld kann das Ablaufdatum der Versicherung hinterlegt werden.
> Technische Info: Numerisches Feld, DB-Feld: mp.limverfall

**Limitprüfung Auftrag**
Mit diesem Feld steuern Sie, was mit Aufträgen passiert, deren Auftragswert zuzüglich der offenen Posten und der offenen Aufträge das in den Feldern Firmenlimit und AKV-Limit hinterlegte Limit überschreitet. Verfügt der Mitarbeiter über entsprechende Rechte kann der Auftrag erfasst werden und landet anschließend in einem Freischaltpool (konfigurierbar). Aufträge, die sich im Freischaltpool befinden, können nur von autorisierten Personen freigegeben werden. Verfügt der Mitarbeiter nicht über diese Rechte, kann er den Auftrag nicht erfassen:
- **Firmen:** Es wird der im Feld Firmenlimit hinterlegte Wert verwendet.
- **AKV:** Es wird der im Feld AKV-Limit hinterlegte Wert verwendet.
- **AKV+Firmen:** Es werden die in den Feldern Firmenlimit und AKV-Limit hinterlegten Werte verwendet.
- **Keine:** Es erfolgt keine Limitprüfung.
> Technische Info: <F9>, DB-Feld: mp.limpruefkz

**Erfassungsstopp**
Mit diesem Feld steuern Sie, ob beim Erreichen des Limits ein Vorgang für diesen Marktpartner erfasst werden darf oder nicht.
- **Nur Angebot:** Beim Erreichen des Limits kann kein Angebot mehr erfasst werden. Aufträge können für diesen Marktpartner noch erfasst werden.
- **Nur Auftrag:** Beim Erreichen des Limits kann kein Auftrag mehr erfasst werden. Angebote können für diesen Marktpartner noch erfasst werden.
- **Auftrag+Angebot:** Beim Erreichen des Limits können weder Angebote noch Aufträge erfasst werden.
- **Nein:** Für diesen Marktpartner wurde kein Erfassungsstopp hinterlegt.
> Technische Info: Toggle-Feld, DB-Feld: mp.erfasstop

**Lieferstopp**
Mit diesem Feld steuern Sie, ob beim Erreichen des Limits ein Lieferschein für diesen Marktpartner gedruckt werden darf oder nicht.
- **Ja:** Beim Erreichen des Limits erfolgt keine Lieferung mehr.
- **Nein:** Beim Erreichen des Limits können Aufträge dennoch ausgeliefert werden.
> Technische Info: Toggle-Feld, DB-Feld: mp.lieferstop

**Fakturastopp**
Mit diesem Feld steuern Sie, ob beim Erreichen des Limits eine Rechnung für diesen Marktpartner gedruckt werden darf oder nicht.
- **Ja:** Beim Erreichen des Limits kann keine Rechnung mehr ausgestellt werden.
- **Nein:** Beim Erreichen des Limits können Rechnungen dennoch ausgestellt werden.
> Technische Info: Toggle-Feld, DB-Feld: mp.fakturastop

**MwSt**
Auswahl des Mehrwertsteuerkennzeichens. Die Steuerschlüssel werden im Menü Steuertypen (Stammdaten > Schlüssel > System > Steuern) hinterlegt.
> Technische Info: <F9>, DB-Feld: mp.mwst

**MwSt int.**
Interne Mehrwertsteuer. Das Feld ist nur aktiv, wenn es sich bei dem Marktpartner um einen Lieferanten handelt.
> Technische Info: <F9>, DB-Feld: mp.mwstint

## Register Bewertung

*Stammdaten > Marktpartner > Register Bewertung*

*Abb. B-20 Marktpartner - Register Bewertung*

In diesem Register können Sie die Zuverlässigkeit, Lieferzeit, Qualität, etc. bewerten. Auf der rechten Seite werden Ihnen die Adressinformationen angezeigt.

### Erläuterung der Felder

**Klasse**
Bewertung der Klasse. Die Bewertungsschlüssel werden im Menü Allgemein (Stammdaten > Schlüssel > Marktpartner > Qualitätsskala) hinterlegt.
> Technische Info: <F9>, DB-Feld: mp.qklass

**Zuverlässigkeit**
Bewertung der Zuverlässigkeit. Die Bewertungsschlüssel werden im Menü Allgemein (Stammdaten > Schlüssel > Marktpartner > Qualitätsskala) hinterlegt.
> Technische Info: <F9>, DB-Feld: mp.qzuverl

**Lieferzeit**
Bewertung der Lieferzeit. Die Bewertungsschlüssel werden im Menü Allgemein (Stammdaten > Schlüssel > Marktpartner > Qualitätsskala) hinterlegt.
> Technische Info: <F9>, DB-Feld: mp.qzeit

**Preise**
Bewertung der Preise. Die Bewertungsschlüssel werden im Menü Allgemein (Stammdaten > Schlüssel > Marktpartner > Qualitätsskala) hinterlegt.
> Technische Info: <F9>, DB-Feld: mp.qpreis

**Qualität**
Bewertung der Qualität. Die Bewertungsschlüssel werden im Menü Allgemein (Stammdaten > Schlüssel > Marktpartner > Qualitätsskala) hinterlegt.
> Technische Info: <F9>, DB-Feld: mp.qqual

**Service**
Bewertung des Services. Die Bewertungsschlüssel werden im Menü Allgemein (Stammdaten > Schlüssel > Marktpartner > Qualitätsskala) hinterlegt.
> Technische Info: F9>, DB-Feld: mp.qservice

**Beratung**
Bewertung der Beratung. Die Bewertungsschlüssel werden im Menü Allgemein (Stammdaten > Schlüssel > Marktpartner > Qualitätsskala) hinterlegt.
> Technische Info: <F9>, DB-Feld: mp.qberat

**Kulanzverhalten**
Bewertung des Kulanzverhaltens. Die Bewertungsschlüssel werden im Menü Allgemein (Stammdaten > Schlüssel > Marktpartner > Qualitätsskala) hinterlegt.
> Technische Info: <F9>, DB-Feld: mp.qkulanz

**Bonität**
Bewertung der Bonität. Die Bewertungsschlüssel werden im Menü Allgemein (Stammdaten > Schlüssel > Marktpartner > Qualitätsskala) hinterlegt.
> Technische Info: <F9>, DB-Feld: mp.qbonitaet

## Register Produktion

*Stammdaten > Marktpartner > Register Produktion*

*Abb. B-21 Marktpartner - Register Produktion*

Die Felder dieses Dialogs dienten der Übergabe an PMS. Mit Einführung von A+W Production hat sich die Produktionsübergabe geändert. Für weitere Informationen kontaktieren Sie bitte einen Mitarbeiter der A+W Software GmbH.

### Erläuterung der Felder

**Vorgabe der Produktionsfolge**
Auswahl, ob eine Produktionsfolge vorgegeben werden soll.
- **Ja:** Produktionsfolge soll vorgegeben werden
- **Nein:** Es wird keine Produktionsfolge vorgegeben.
> Technische Info: Toggle-Feld, DB-Feld: mp.prodfolge

**Gestellbeladung**
Dieses Kriterium bestimmt die Sortierreihenfolge auf einem Gestell, abhängig von z. B. von Position, SZR, HM (Hardmaß), etc.
> Technische Info: Toggle-Feld, DB-Feld: mp.gbelad

**Gestellgewicht (max)**
Das maximale Gestellgewicht kann eingegeben werden.
> Technische Info: F9>, DB-Feld: mp.gmaxgew

## Register Modifikation

*Stammdaten > Marktpartner > Register Modifikation*

*Abb. B-22 Marktpartner - Register Modifikation*

Dieses Register zeigt, wann und durch wen der Marktpartner angelegt wurde, wann und durch wen Änderungen vorgenommen wurden und wann der Marktpartner repliziert wurde. Auf der rechten Seite werden Ihnen die Adressinformationen angezeigt.

Im Bereich Replikationsdatum sehen Sie, an welche Häuser der Marktpartner repliziert wurde.

**Ergänzende Informationen**
- "Marktpartner - Anmerkungstexte" auf Seite B-106
- "Artikel - Anmerkungstexte" auf Seite B-386

## Register Privat

*Stammdaten > Marktpartner > Register Privat*

*Abb. B-23 Marktpartner Register Privat*

Für individuelle Auswertungen oder zusätzliche Kundeninformationen stehen zwei numerische und zwei alphanumerische Felder zur Verfügung. Auf Wunsch können diese mit einer eigenen Überschrift versehen und im System konfiguriert werden. Für kundenindividuelle Anpassungen kontaktieren Sie bitte einen Mitarbeiter der A+W Software GmbH.

**Ergänzende Informationen**
- "Marktpartner - Anmerkungstexte" auf Seite B-106
- "Artikel - Anmerkungstexte" auf Seite B-386

## Ansprechpartner

*Stammdaten > Marktpartner > <F4> > Kontaktdaten > Ansprechpartner*

*Abb. B-24 Hauptansprechpartner*

In diesem Dialog können Sie für einen Marktpartner verschiedene Ansprechpartner hinterlegen. Dabei können mit `<F6>` weitere Datensätze hinzugefügt werden.

Bei mehreren hinterlegten Ansprechpartnern wird mit `<F5>` ein Hauptansprechpartner bestimmt.

### Erläuterung der Felder

**Name**
Nachname des Ansprechpartners.
> Technische Info: Alphanumerisches Feld, DB-Feld: anspr.apname

**Vorname**
Vorname des Ansprechpartners.
> Technische Info: Alphanumerisches Feld, DB-Feld: anspr.apvname

**Anrede**
Auswahl der Anrede für den Ansprechpartner. Die entsprechenden Schlüssel können über das Menü Anreden (Stammdaten > Schlüssel > Marktpartner) vergeben werden.
> Technische Info: <F9>, DB-Feld: anspr.anrede

**Abteilung**
Abteilung des Ansprechpartners.
> Technische Info: Alphanumerisches Feld, DB-Feld: anspr.abteilung

**Position**
Position des Ansprechpartners.
> Technische Info: Alphanumerisches Feld, DB-Feld: anspr.position

**Geburtsdatum**
Geburtsdatum des Ansprechpartners.
> Technische Info: Numerisches Feld, DB-Feld: anspr.gebdat

**Telefon**
Telefonnummer des Ansprechpartners, z. B. +4964042051-0.
> Technische Info: Numerisches Feld, DB-Feld: anspr.telefon

**Fax**
Faxnummer des Ansprechpartners, z. B. +4964042051-877.
> Technische Info: Numerisches Feld, DB-Feld: anspr.telefax

**Mobil**
Mobilnummer des Ansprechpartners, z. B. +491777500000.
> Technische Info: Numerisches Feld, DB-Feld: anspr.telex

**E-Mail**
Mailadresse des Ansprechpartners.
> Technische Info: Numerisches Feld, DB-Feld: anspr.email

**Bemerkung**
Textuelle Bemerkungsfelder.
> Technische Info: Alphanumerisches Feld, DB-Feld: adr.text1-3

## Adressen

*Stammdaten > Marktpartner > <F4> > Kontaktdaten > Adressen*

*Abb. B-25 Adressen*

In diesem Dialog können Sie dem Marktpartner zusätzliche Adressen zuordnen. Die Rechnungsadresse ist die Hauptadresse und kann nicht verändert werden. Mit `<F6>` können weitere Datensätze hinzugefügt werden. Weicht die Lieferadresse von der Hauptanschrift ab, so ist der entsprechende Adresssatz mit `<F5>` als Standard-Anschrift zu bestimmen.

> **Löschen bzw. Reaktivieren einer Marktpartneradresse**
> Über diesen Dialog können Sie trotz der Verwendung der Adresse in anderen Modulen diese löschen. In ersten Schritt wird diese Adresse nur stillgelegt. In zweiten Schritt kann die Adresse gelöscht bzw. wieder aktiviert werden. Die Schaltfläche [Löschen] ändert sich in [Reaktivieren]. In beiden Fälle erfolgt eine Sicherheitsabfrage, ob die Aktion tatsächlich durchgeführt werden soll.

### Erläuterung der Felder

**Name**
Nachname, bzw. Firmenname.
> Technische Info: Alphanumerisches Feld, DB-Feld: adr.adrname

**Vorname**
Vorname.
> Technische Info: Alphanumerisches Feld, DB-Feld: adr.adrvname

**Anrede**
Anrede, z. B. Herr, Frau, Firma. Die Schlüssel werden im Menü Anreden (Stammdaten > Schlüssel > Marktpartner) hinterlegt.
> Technische Info: <F9>, DB-Feld: anspr.anrede

**z. Hd.**
Zu Händen von (Nachname, Vorname).
> Technische Info: Alphanumerisches Feld, DB-Feld: adr.zhd

**Zusatz**
Ermöglicht eine zusätzliche Adressinformation zur Ausgabe auf Kundenpapieren.
> Technische Info: Alphanumerisches Feld, DB-Feld: adr.branche

**Straße**
Straßenname.
> Technische Info: Alphanumerisches Feld, DB-Feld: adr.str

**PLZ, Fach**
Postleitzahl und das Postfach.
> Technische Info: numerisches/Alphanumerisches Feld, DB-Feld: adr.pfplz/ postfach

**PF Ort**
Postfach und Ort.
> Technische Info: numerisches/Alphanumerisches Feld, DB-Feld: adr.pfort

**PLZ, Ort**
Postleitzahl und der Ort.
> Technische Info: numerisches/Alphanumerisches Feld, DB-Feld: adr.plz/ort

**Versandregion**
Auswahl der Versandregion. Die entsprechenden Schlüssel können über das Menü Versandregionen (Stammdaten > Schlüssel > System > Versand) vergeben werden.
> Technische Info: <F9>, DB-Feld:DB-Feld: adr.vsregion

**KFZ Land**
Auswahl des Länder-Kfz-Kennzeichens. Die entsprechenden Schlüssel können über das Menü Länder (Stammdaten > Schlüssel > Marktpartner) vergeben werden.
> Technische Info: <F9>, DB-Feld: adr.kfzcode

**Entfernung**
Entfernung zur Lieferadresse in km.
> Technische Info: Numerisches Feld, DB-Feld: adr.kilometer

> **Hausspezifische Angaben zu Entfernung und Fahrtdauer**
> Angaben zu Entfernung und Fahrtdauer soll bei Verwendung interner Mandantentrennung pro Haus (Mandant) erfasst werden. Der Erfassungsdialog startet in solcher Konfiguration automatisch.
> -> "Hausspezifische Adressdaten" auf Seite B-144

**Fahrtzeit**
Dauer der Fahrtzeit zur Lieferadresse in Tagen.
> Technische Info: Numerisches Feld, DB-Feld: adr.fahrtzeit

> **Handlingszeit, Ankunftszeit und Anlieferstelle**
> Die Felder Handlingszeit, Ankunftszeit und Anlieferzeit sind nur bei entsprechenden Konfiguration freigeschaltet.

**Handlingszeit**
Ist der Zeitraum zwischen der Fertigstellung des Produktes und dem Tag der Auslieferung. Eine solche Zeit kann notwendig werden, wenn der Kunde bestimmte Vorgaben für die Kommissionierung seiner Ware trifft. Sie wird als Frist eingetragen und damit von der Termin- und Kapazitätsplanung berücksichtigt. Die Zeit kann in Tagen oder in Stunden eingegeben werden (konfigurierbar). Die Handlingszeit kann bei entsprechenden Konfiguration pro Lieferadresse hinterlegt werden.
> Technische Info: Numerisches Feld, DB-Feld: adr.handlingszeit

**Ankunftszeit**
Ankunftszeit in HH:MM bei Anlieferung der Ware.
> Technische Info: Numerisches Feld, DB-Feld: adr.ankunftszeit

**Anlieferstelle**
Platz, wo die Ware bei Anlieferung angefahren wird.
> Technische Info: Numerisches Feld, DB-Feld: adr.anlieferstelle

**Fax, Tel.**
Faxnummer und Telefonnummer der Adresse.
> Technische Info: numerisches/alphanumerisches Feld, DB-Feld: adr.fax/telefon

**E-Mail**
Mailadresse.
> Technische Info: Alphanumerisches Feld, DB-Feld: adr.email

**Std. Route**
Selo-Feld. Falls die Lieferadresse nicht über die im Kundenstamm hinterlegte Standard-Route erreicht werden kann, besteht die Möglichkeit, die Anschrift einer gesonderten Route zuzuordnen.
> Technische Info: <F9>, DB-Feld: adr.routenr

**Bemerkung**
Beliebige Informationen.
> Technische Info: Alphanumerisches Feld, DB-Feld: adr.text1

> **Adressenlogik**
> Zum Zeitpunkt der Auftragserfassung wird für den betreffenden Kunden in der Regeln die hinterlegte Standard-Lieferanschrift mit der zugehörigen Routennummer übernommen. Wurde dem Kunden eine Standardlieferanschrift mit eigener Routennummer hinterlegt, so wird die im Kundenstamm eingetragene Routennummer übersteuert. Es existieren diverse Abweichungen in dieser Funktion, diese sind meistens konfigurationsabhängig. Bei Fragen, bzw. um weitere Information zu erhalten, wenden Sie sich an den zuständigen A+W Software GmbH Mitarbeiter.

> **Neue Adressen im Auftrag und im A+W iQuote Vorgang**
> Neue Kundenadressen können in die Stammdaten übernommen werden. In der Auftragserfassung verwenden Sie die Taste `<F3>` dazu:
> Verkauf, "Neue Lieferadresse" auf Seite D-1192
> In einem A+W iQuote-Vorgang wird die neue Adresse standardmäßig in den Kundenstamm übernommen. Wenn diese Vorgehensweise nicht gewünscht ist, wenden Sie sich an A+W - Mitarbeiter, um die Konfiguration zu ändern.

## Hausspezifische Adressdaten

*Abb. B-26 Hausspezifische Adressdaten*

In diesem Dialog können Sie hausspezifische Adressdaten pro Haus hinterlegen. Dieser Dialog erscheint automatisch, wenn Sie die interne Mandantentrennung nutzen und im Dialog Adressen das Feld Entfernung betreten.
-> "Adressen" auf Seite B-140

### Erläuterung der Felder

**Haus**
Auswahl der Hausnummer.
> Technische Info: <F9>, DB-Feld: mdzu.hnr

**Name**
Der Hausbenennung wird im Klartext automatisch angezeigt, wenn Sie das Feld Haus verlassen.

**Entfernung**
Entfernung zur Lieferadresse in km für das aktuellen Haus.
> Technische Info: Numerisches Feld, DB-Feld: adr.kilometer

**Fahrtzeit**
Dauer der Fahrtzeit zur Lieferadresse in Tagen oder Stunden für das aktuellen Haus.
> Technische Info: Numerisches Feld, DB-Feld: adr.fahrtzeit

## Bankverbindungen

*Stammdaten > Marktpartner > <F4> > Kontaktdaten > Bankverbindungen*

*Abb. B-27 Bankverbindungen*

In diesem Dialog werden die marktpartnerspezifischen Bankverbindungen hinterlegt. Dabei können durch `<F6>` weitere Datensätze hinzugefügt werden. Existieren mehrere Bankverbindungen, ist die Hauptbankverbindung mit `<F5>` zu bestimmen.

### Erläuterung der Felder

**Bankname**
Name des Kreditinstituts.
> Technische Info: Alphanumerisches Feld, DB-Feld: bankv.bname

**Banksitz**
Sitz des Kreditinstituts.
> Technische Info: Alphanumerisches Feld, DB-Feld: bankv.sitz

**KFZ Land**
Selo-Feld. Das Länder Kfz-Kennzeichen.
> Technische Info: <F9>, DB-Feld: bankv.kfzcode

**BLZ**
Bankleitzahl des Kreditinstituts.
> Technische Info: Numerisches Feld, DB-Feld: bankv.blz

**Konto-Nr.**
Kontonummer bei dem Kreditinstitut.
> Technische Info: Numerisches Feld, DB-Feld: bankv.kontonr

**BIC**
Business Identifier Code.
> Technische Info: Alphanumerisches Feld, DB-Feld: bankv.bic

**IBAN**
Internationale Bank-Kontonummer.
> Technische Info: Alphanumerisches Feld, DB-Feld: bankv.iban

## E-Mailadressen

*Stammdaten > Marktpartner > <F4> > Kontaktdaten > E-Mailadressen*

*Abb. B-28 E-Mailadressen*

In diesem Dialog haben Sie die Möglichkeit, diverse E-Mailadressen zu hinterlegen. Die hinterlegten Daten werden in der zugehörigen Datenbank-Tabelle xemail gepflegt. Diese enthält die Angaben zur E-Mail-Versendung der Formulare. Hier können der MP-Typ, der Marktpartner, die Formularart, der Mitarbeiter bzw. die Abteilung und die E-Mail-Adressen eingegeben werden. Wird ein Mitarbeiter eingetragen, kann keine Abteilung eingetragen werden. Wird eine Abteilung eingegeben, kann kein Mitarbeiter hinterlegt werden. Es ist möglich Werte für einen Marktpartner und einen Mitarbeiter (bzw. eine Abteilung), für einen Marktpartner, eine Formularart und einen Mitarbeiter (bzw. eine Abteilung) oder nur für einen Marktpartner anzulegen. Genau in dieser Reihenfolge wird beim Versenden der Formulare auch die E-Mail-Adresse ermittelt, an die das zum Vorgang gehörige Formular versandt wird.

Die hier hinterlegten Daten beziehen sich immer auf den Vorgang, für den ein Formular versendet werden soll, d.h. die hier hinterlegte Mitarbeiternummer muss mit dem Vorgangserfasser übereinstimmen, damit die entsprechende E-Mail-Adresse ermittelt werden kann.

### Erläuterung der Felder

**Formular**
Wählen Sie das gewünschte Formular (Angebot, Rechnung, etc.) aus.
> Technische Info: <F9>, DB-Feld: xemail.formart

**Mitarb.**
Wählen Sie die gewünschte Mitarbeiter-Nummer aus. Wenn die E-Mail nicht an einen Mitarbeiters sondern an eine Abteilung gehen soll, dann lassen Sie dieses Feld leer und wählen im Feld Abteilung die entsprechende aus.
> Technische Info: <F9>, DB-Feld: xemail.manr

**Abteilung**
Wählen Sie die Abteilung aus, an die die E-Mail gehen soll. Haben Sie im Feld Mitarb. eine Mitarbeiter-Nummer eingetragen, können Sie in diesem Feld keine Angabe machen.
> Technische Info: <F9>, DB-Feld: xemail.abtnr

**E-Mail**
Geben Sie hier die entsprechende E-Mailadresse ein.
> Technische Info: Alphanumerisches Feld, DB-Feld: xemail.email

**S**
Handelt es sich bei der E-Mailadresse um eine für diese Formularart stillgelegte E-Mailadresse:
- **J:** Die Mail-Adresse ist für diese Formularart stillgelegt.
- **N:** Die Mail-Adresse ist für diese Formularart aktiv.
> Technische Info: Toggle-Feld, DB-Feld: xemail.still

**Ergänzende Informationen**
- "E-Mailadressen - Detail" auf Seite B-148

### E-Mailadressen - Detail

*Stammdaten > Marktpartner > <F4> > Kontaktdaten > E-Mailadressen > F2*

*Abb. B-29 E-Mailadresse*

In diesem Dialog werden Ihnen weitere Informationen für zu der ausgewählten E-Mailadresse angezeigt.

#### Erläuterung der Felder

**Partnertyp**
Das Feld wird mit dem Partnertyp vorbelegt, aus dem Sie das Kontextmenü geöffnet haben. Sie können den Typ ändern.
> Technische Info: Toggle-Feld

**Marktpart.**
Das Feld wird mit dem Marktpartner vorbelegt, aus dem Sie das Kontextmenü geöffnet haben. Sie können den Marktpartner ändern.
> Technische Info: <F9>, DB-Feld: xemail.mpnr

**Formular**
Das Feld wird mit dem Formular vorbelegt, das Sie im Dialog zuvor ausgewählt haben. Sie können das Formular ändern.
> Technische Info: <F9>, DB-Feld: xemail.formart

**Mitarbeiter**
Das Feld wird mit dem Mitarbeiter vorbelegt, den Sie im Dialog zuvor ausgewählt haben. Sie können den Mitarbeiter ändern.
> Technische Info: <F9>, DB-Feld: xemail.manr

**Abteilung**
Das Feld wird mit der Abteilung vorbelegt, die Sie im Dialog zuvor ausgewählt haben. Sie können die Abteilung ändern.
> Technische Info: <F9>, DB-Feld: xemail.abtnr

**E-Mail**
Das Feld wird mit der E-Mailadresse vorbelegt, die Sie im Dialog zuvor eingegeben haben. Sie können die Adresse ändern.
> Technische Info: Alphanumerisches Feld, DB-Feld: xemail.email

**E-Mail von**
Abweichende Absenderadresse bei Verwendung dieser E-Mail-adresse.
> Technische Info: Alphanumerisches Feld, DB-Feld: xemail.emailabs

**cc**
Zusätzliche CC-Adresse bei Verwendung dieser E-Mailadresse.
> Technische Info: Alphanumerisches Feld, DB-Feld: xemail.cc

**E-Mail**
Zusätzliche BCC-Adresse bei Verwendung dieser E-Mailadresse.
> Technische Info: Alphanumerisches Feld, DB-Feld: xemail.bcc

**Versandart**
Versandart des Dateianhangs:
- **0 (Standard):** Pro E-Mail eine PDF-Datei
- **1:** Pro E-Mail mehrere Dateianhänge verwenden
- **2:** Alle Dateianhänge zu einem PDF zusammenfassen.
> Technische Info: Alphanumerisches Feld, DB-Feld: xemail.bcc

**Passwort**
Hier können Sie ein Passwort vergeben.
> Technische Info: Alphanumerisches Feld, DB-Feld: xemail.passwort

**Stillgelegt**
Das Feld wird mit dem Flag vorbelegt, das Sie im Dialog zuvor eingestellt haben. Sie können das Flag ändern.
> Technische Info: Toggle-Feld, DB-Feld: xemail.still

## Rabatte

*Stammdaten > Marktpartner > <F4> > Rabatte*

*Abb. B-30 Rabatte*

Hier ordnen Sie dem ausgewählten Marktpartner Rabatte zu. Der Dialog wird an folgender Stelle im Schlüsselbereich ausführlich erläutert:
- "Rabatte" auf Seite B-228

Die Werte für die jeweilige Rabattmethode kann pro Marktpartner individuell vereinbart und geändert werden.

### Rabatte - Details

*Stammdaten > Marktpartner > <F4> > Rabatte > Details*

*Abb. B-31 Rabatte, Details*

Bei diesem Dialog handelt es sich um die Detail-Ansicht der Rabatte. Der Dialog wird an folgender Stelle ausführlich erläutert:
- "Rabatte - Details" auf Seite B-230

## Austausch-/Zusatzregeln

*Stammdaten > Marktpartner > <F4> > Austausch-/Zusatzregeln*

*Abb. B-32 Austausch-/Zusatzregeln*

Der Menüpunkt Austausch-/Zusatzregeln ermöglicht es, kundenspezifische Regeln, nach denen im Auftrag die Stückliste ergänzt bzw. Teile ausgetauscht werden sollen, für einzelne Artikel oder Artikeltypen zu hinterlegen.

Der Dialog wird an folgender Stelle ausführlich erläutert:
- "Austausch-/Zusatzregeln" auf Seite B-304
- "Austausch-/Zusatzregel - Details" auf Seite B-308
- "Austausch-/Zusatzregel - Testmodus" auf Seite B-310

## Gestelltypen

*Stammdaten > Marktpartner > <F4> > Gestelltypen*

*Abb. B-33 Gestelltypen*

In diesem Dialog legen Sie fest, auf welchen Gestellen die Ware einem Kunden vorzugsweise auszuliefern ist.
Bei Nutzung der prioritätsgesteuerten Packmitteloptimierung kann zusätzlich eine Priorität festgelegt werden, welcher Gestelltyp für den Kunden der wünschenswerteste und welcher eher ungünstig ist. Die Prioritätszahl kann zwischen 1 und 100 gewählt werden und legt damit die Rangfolge der Gestelle fest. Größere Werte bewirken eine Bevorzugung dieses Gestelltyps vor anderen mit niedrigeren Prioritätswerten.
Die hier hinterlegten Informationen nutzt die automatischen Gestellplanung, um den Auftrag unter Beachtung von Scheibengrößen und Limitierungen der Gestelltypen bestmöglich auf vom Kunden bevorzugte Gestelle zu verladen. Für die automatische Gestellplanung kann hier entweder der Gestelltyp oder die Hauptgruppe hinterlegt werden.

Mit `<F2>` erreichen Sie den Gestelltypen-Details Dialog.
- "Gestelltypen - Details" auf Seite B-154

### Erläuterung der Felder

**Typ**
Auswahl des Gestelltyps. Die Gestelltypen werden im Menüpunkt Gestelltypen (Logistik > Gestellverwaltung > Gestellstamm) hinterlegt. Nach der Auswahl des Gestelltypes wird die dazugehörige Bezeichnung in dem zweiten Feld dargestellt.
> Technische Info: <F9>, DB-Feld: kugest.gtypnr

**Hauptgruppe**
Auswahl der Hauptgruppe. Die Hauptgruppen werden im Menüpunkt Hauptgruppen (Logistik > Gestellverwaltung > Gestellstamm) hinterlegt. Nach der Auswahl der Hauptgruppe wird die dazugehörige Bezeichnung in dem letzten Feld dargestellt. Bei Verwendung der prioritätsgesteuerten Konfiguration ist die Eingabe der Hauptgruppe nicht möglich.
> Technische Info: <F9>, DB-Feld: kugest.gtypnr

**Priorität**
Gestellpriorität aus Sicht des Kunden. Das Feld ist nur bei kundenspezifischen Konfiguration sichtbar.
> Technische Info: Numerisches Feld, DB-Feld: kugest.prioritat

### Gestelltypen - Details

*Stammdaten > Marktpartner > <F4> > Gestelltypen > <F2>*

*Abb. B-34 Gestelltypen, F2*

In diesem Dialog können Sie einen kundenspezifischen Packmitteltext hinterlegen und definieren, ob dieser auf der Packmittelbestellung gedruckt werden soll.

Mit `<F2>` kehren Sie zurück in den Hauptdialog:
- "Gestelltypen" auf Seite B-153

#### Erläuterung der Felder

**Text**
Kundenspezifischer Packmitteltext.
> Technische Info: Alphanumerisches Feld, DB-Feld: kugest.kuspectxt/kuspectxt1

**Bestell-KZ**
Soll der Text auf der Bestellung gedruckt werden:
- Ja
- Nein.
> Technische Info: Toggle-Feld, DB-Feld: kugest.bestelldru/bestelldru1

## Konfigurierte MP-Felder

*Stammdaten > Marktpartner > <F4> > Konfigurierte MP-Felder*

*Abb. B-35 Konfigurierte MP-Felder*

In diesem Dialog wird jedes Feld kundenspezifisch konfiguriert und ausgewertet. Die Felder können unter dem Menüpunkt MP-Feldkonfiguration (Stammdaten > Feldkonfiguration) definiert werden.
- “MP-Feldkonfiguration" auf Seite B-502

Die Auswertung der Felder kann nur individuell gestaltet werden. Für weitere Informationen kontaktieren Sie bitte einen Mitarbeiter der A+W Software GmbH.

Die Daten in oben gezeigten Screenshot dienen an dieser Stelle nur als Beispiel.

## Vertreterzuordnung

*Stammdaten > Marktpartner > <F4> > Mitarbeiterzuordnung > Vertreterzuordnung*

*Abb. B-36 Mitarbeiterzuordnung*

In diesem Dialog ist es möglich, einem Kunden mehrere Vertreter (Mitarbeiter) zuzuordnen.
Die Auswahl erfolgt über `<F9>`. Zur Auswahl stehen nur die Mitarbeiter zur Verfügung, denen eine Vertreter-Funktion im Mitarbeiterstamm zugeordnet ist.
Mit `<F5>` kann ein Mitarbeiter als Hauptvertreter (= Außendienstmitarbeiter) festgelegt werden.

### Erläuterung der Felder

**Pers-Nr**
Auswahl der Mitarbeiternummer. Der Name wird im Feld Vertreter angezeigt.
> Technische Info: <F9>, DB-Feld: mitarbzu.manr

## Erfasserzuordnung

*Stammdaten > Marktpartner > <F4> > Mitarbeiterzuordnung > Erfasserzuordnung*

*Abb. B-37 Erfasserzuordnung*

In diesem Dialog ist es möglich, einem Kunden mehrere Erfasser (Mitarbeiter) zuzuordnen. Die Auswahl erfolgt über `<F9>`.

### Erläuterung der Felder

**Pers-Nr**
Auswahl der Mitarbeiternummer. Im Feld Erfasser wird Ihnen dann der Name angezeigt.
> Technische Info: <F9>, DB-Feld: mperfasszu.manr

**AB-Empfang**
Über dieses Feld steuern Sie, wie der Mitarbeiter Kopien der AB an den Kunden erhalten soll. Folgende Werte sind möglich:
- **nein:** Der Mitarbeiter erhält keine Kopie der AB.
- **per Email:** Der Mitarbeiter erhält die Kopie per E-Mail.
- **per Fax:** Der Mitarbeiter erhält die Kopie per Fax.
> Technische Info: Toggle-Feld, DB-Feld: mperfasszu.abflag

## Gruppenzuordnung

*Stammdaten > Marktpartner > <F4> > Gruppenzuordnung*

*Abb. B-38 Gruppenzuordnung*

In diesem Dialog kann ein Kunde über `<F9>` verschiedenen Gruppen zugeordnet werden. Die Pflege der Gruppen-Schlüssel erfolgt im Menü Gruppen (Stammdaten > Marktpartner).

Den verschiedenen Marktpartnergruppen können im Rahmen der Textverarbeitung (Stammdaten > Textverwaltung > Gruppentexte) diverse Texte zugeordnet werden, die auf den marktpartnerseitigen Papieren ihre Ausgabe finden. Damit kann beispielsweise die Marktpartnergruppe der Fensterbauer über die Einführung eines neuen Isolierglasproduktes informiert werden.

### Erläuterung der Felder

**Gruppe**
Auswahl des Gruppenschlüssels. Im Feld Bezeichnung wird Ihnen dann der Name angezeigt.
> Technische Info: <F9>, DB-Feld: grpzu.grpnr

**Klasse**
Gruppenklassifikation. Über die definierte Klasse können Sie statistische Auswertungen durchführen.
> Technische Info: Numerisches Feld, DB-Feld: grpzu.klasskz

## Objektzuordnung

*Stammdaten > Marktpartner > <F4> > Objektzuordnung*

*Abb. B-39 Objektzuordnung*

In diesem Dialog können einem Kunden ein oder mehrere Objekte, (z. B. Großbaustellen) zugeordnet werden. Die Objekte werden über `<F9>` angezeigt und über ihre Objektnummer eingetragen.

Mit `<F3>` öffnen Sie den Dialog für die kundenindividuellen Objekttexte, in dem Sie die Objekttexte zuweisen und bestimmen, auf welchen Papieren der Text gedruckt wird.

Mit `<F5>` definieren Sie das Standard-Objekt.

### Erläuterung der Felder

**Objekt**
Auswahl der Objektnummer. Im Feld Objektbezeichnung wird Ihnen der Name des Objekts angezeigt.
> Technische Info: <F9>, DB-Feld: okkond.objnr

**Ergänzende Informationen**
- "Objekttexte" auf Seite B-160

## Objekttexte

*Stammdaten > Marktpartner > <F4> > Objektzuordnung > <F3>*

*Abb. B-40 Objekttexte*

In diesem Dialog weisen Sie einen Objekttext zu und bestimmen, auf welchen Papieren der Text gedruckt wird.

### Erläuterung der Felder

**Datei**
Auswahl der Textdatei, in der die Texte gespeichert werden. Wenn Sie einen neuen Dateinamen eingeben, öffnet sich der Dialog Stammtexte, in dem Sie den neuen Text eingeben können.
> Technische Info: <F9>, DB-Feld: objtxtzu.datei

**Nr**
Über dieses Feld steuern Sie die Reihenfolge, in der die Objekttexte gedruckt werden.
> Technische Info: <F5>, DB-Feld: objtxtzu.lfdnr

**Druckposition**
Auswahl der Druckposition:
- Kopftext
- Fußtext
> Technische Info: Toggle-Feld, DB-Feld: objtxtzu.ludrupos

> **Formulare**
> Mit `<F5>` legen Sie fest, auf welchen Formulararten (Auftragsbestätigung, Rechnung, etc.) die Dateien in der hier angegebenen Reihenfolge gedruckt wird.

**Ergänzende Informationen**
- "Stammtexte" auf Seite B-166

## Farbzuordnung

*Stammdaten > Marktpartner > <F4> > Farbzuordnung*

*Abb. B-41 Farbzuordnung*

Dieser Dialog ist nur für Marktpartnertyp=Lieferant verfügbar. Hier hinterlegten Daten sind für den BMECat-Stammdaten-Import relevant. Dabei handelt es sich um eine Applikation zum Import von Artikel-Stammdaten von Lieferante. Beim Import einer neuen Lieferanten-Stammdaten-Datei wird anhand der korrespondierenden Tabelle lieffarzu überprüft, ob die Farben eines zu importierenden Artikels bereits im System als AWE-Farben angelegt sind oder nicht. Wenn erkannt wird, dass eine Lieferanten-Farbe noch nicht als AWE-Farbe angelegt ist, wird sie während des Imports angelegt.

Der Dialog liefert dann dem Benutzer die Übersicht aller angelegten Lieferanten-Farben.

Es kann auch vorkommen, dass für eine Bestellung bei einem Lieferanten eine Farbe benötigt wird, die noch nicht angelegt ist, weil nach dem letzten Lieferanten-Stammdaten-Import vom Lieferanten noch neue Farben zur Verfügung gestellt wurden. In diesem Fall kann über den Dialog die neue Lieferanten-Farbe manuell angelegt werden, um die Bestellung zu erfassen.

### Erläuterung der Felder

**Nr**
Farbnummer. Die Farben werden im Menüpunkt Farben (Stammdaten > Schlüssel > Produkte > Varianten > Farben) hinterlegt.
> Technische Info: <F9>, DB-Feld: lieffarbzu.farbnr

**AWE-Farbe**
AWE Farbbezeichnung. Nach der Farbnummerauswahl wird die entsprechenden Bezeichnung in diesem Feld angezeigt.
> Technische Info: <F9>, DB-Feld: lieffarbzu.farbnr

**Nr**
Farbnummer des Lieferanten.
> Technische Info: <F9>, DB-Feld: lieffarbzu.lifarbnr
**Lieferantenfarbe**
Farbbezeichnung des Lieferanten
> Technische Info: <F9>, DB-Feld: lieffarbzu.lifarbbez

## Bonuszuordnung

*Stammdaten > Marktpartner > <F4> > Bonuszuordnung*

*Abb. B-42 Bonuszuordnung*

In diesem Dialog können Sie einem Marktpartner einen Bonus zuordnen.

### Erläuterung der Felder

**Rang**
Angabe zur Priorität. Mit diesem Feld wird die Zuordnung in der Auftragserfassung zu den einzelnen Auftragsposition gesteuert. Die niedrigste Rangnummer mit den meisten übereinstimmenden Stellen in der Warengruppe wird hier herangezogen.
> Technische Info: Numerisches Feld, DB-Feld: bonuszu.rang

**WagrpCode**
Über dieses Feld können Sie den Bonus einer bestimmten Warengruppe oder einem Warengruppen-Bereich zuordnen.
> Technische Info: <F9>, DB-Feld: bonuszu.wagrp

**Bemerkung**
Hier kann eine Bemerkung hinterlegt werden, z. B. warum ein Bonus vergeben wurde.
> Technische Info: Alphanumerisches Feld, DB-Feld: bonuszu.txt

**Bonus**
Auswahl des gewünschten Bonus. Die entsprechenden Schlüssel werden über das Menü Bonus (Schlüssel > Marktpartner > Bonus) vergeben.
> Technische Info: <F9>, DB-Feld: bonuszu.bonusnr

## Artikelzuordnung

*Stammdaten > Marktpartner > <F4> > Artikelzuordnung*

*Abb. B-43 Artikelzuordnung*

In diesem Dialog können Sie einem Marktpartner mehrere Artikel mit spezifischen Angaben zuordnen. Die Artikel werden über `<SELO>` (`<F9>`) angezeigt und über ihre Artikelnummer eingetragen.

### Erläuterung der Felder im Register Übersicht

**Artikel**
Auswahl der Artikelnummer.
> Technische Info: <F9>, DB-Feld: artkuzu.artnr

**Bezeichnung**
Artikelbezeichnung.

**Artikeltyp**
Artikeltyp des ausgewählten Artikels.

**Ext.Artikel**
Artikelnummer des Marktpartners. Über diese Nummer kann die Auftragsposition direkt erfasst werden.
> Technische Info: Alphanumerisches Feld, DB-Feld: artkuzu.kuartnr

**Externe Artikelbezeichnung**
Artikelbezeichnung des Marktpartners.
> Technische Info: Alphanumerisches Feld, DB-Feld: artkuzu.kuartbez

**Preis**
Kundenartikelpreis. Je nach Preistyp wird dieser dann im Auftrag berechnet.
> Technische Info: Numerisches Feld, DB-Feld: artkuzu.preis

**Preistyp**
Preistyp:
- **WE/Stück:** Währungseinheit je Stück.
- **WE/ME:** Währungseinheit je Mengeneinheit
> Technische Info: Toggle-Feld, DB-Feld: artkuzu.ptyp

### Erläuterung der Felder im Register Details

**Wunschlieferant**
In diesem Feld können Sie den Wunschlieferanten des Marktpartners für Zukaufsartikel wählen.
> Technische Info: <F9>, DB-Feld: artkuzu.liwunsch

**Zusatzbezeichnung**
In diese Felder können Sie die marktpartnerspezifische Zusatzbezeichnung für den Artikel eingeben. Ihnen stehen hierfür drei Felder zur Verfügung. Das Feld betreten Sie mit `<Enter>`.
Die hier eingegebene Bezeichnung übersteuert für diesen Kunden die Artikelbezeichnung in der Vorgangsverwaltung.
> Technische Info: Alphanumerische Felder, DB-Felder: artkuzu.zusatz1, artkuzu.zusatz2, artkuzu.zusatz3

**EAN-Code**
In diesem Feld können Sie den marktpartnerspezifischen EAN-Code für diesen Artikel hinterlegen. Dieser wird auf den kundenseitigen Papieren ausgedruckt. Der EAN-Code kann für die Umsetzung von externen Artikeln in A+W Enterprise-Artikel innerhalb der automatischen Auftragsübernahme genutzt werden.
> Technische Info: Numerisches Feld, DB-Feld: artkuzu.eancode

**Rahmentextnummer**
In diesem Feld können Sie eine marktpartnerspezifische Rahmentextnummer für einen ISO-Artikel eingeben. Die Textformel wird im Menü Textverwaltung > Textgenerierung > Textformel hinterlegt.
Diese Formel wird in der Vorgangserfassung bei der Textgenerierung ausgewertet und auf den Rahmen gedruckt.
> Technische Info: Numerisches Feld, DB-Feld: artkuzu.rahmtxtnr

**Maß 1-20**
In diesen Feldern können Sie marktpartnerspezifische Artikelbemaßungen hinterlegen. Diese übersteuern dann die Werte aus den Parametern, die bei der Artikel-Vermaßung für diesen Artikel eingegeben wurden.

> **Es findet keinerlei Plausibilitätsprüfung statt!**
> Die Eingaben, die Sie hier machen, müssen sinnvoll sein.

> Technische Info: numerische Felder, DB-Felder: artkuzu.gv1 – artkuzu.gv20

## Marktpartnertexte

*Stammdaten > Marktpartner > <F4> > Texte / Druck > Marktpartnertexte*

*Abb. B-44 Marktpartnertexte*

In diesem Dialog ordnen Sie Marktpartnertexte für den Ausdruck auf den Formularen zu.

Mit `<F3>` öffnen Sie einen Dialog, in dem Sie die Stammtexte hinterlegen können.

> **Formulare**
> Mit `<F5>` legen Sie fest, auf welchen Formulararten (Auftragsbestätigung, Rechnung, etc.) diese Datei in der hier angegebenen Reihenfolge gedruckt wird.

### Erläuterung der Felder

**Datei**
Auswahl oder Eingabe der Textdatei, in der die Texte gespeichert werden.
> Technische Info: <F9>, DB-Feld: kltxtzu.dateiname

**Nr.**
Über dieses Feld steuern Sie die Reihenfolge, in der die Marktpartnertexte gedruckt werden.
> Technische Info: <F5>, DB-Feld: kltxtzu.Ifdnr

**Druckposition**
Auswahl der Druckposition:
- **Kopftext:** Die Datei wird im Formularkopf gedruckt.
- **Fußtext:** Die Datei wird im Formularfuß gedruckt.
> Technische Info: Toggle-Feld, DB-Feld: kltxtzu.ludrupos

**Ergänzende Informationen**
- "Stammtexte" auf Seite B-166

## Stammtexte

*Stammdaten > Marktpartner > <F4> > Texte / Druck > Marktpartnertexte > <F3>*

*Abb. B-45 Stammtexte*

In diesem Dialog werden Textblöcke neu erfasst und gleichzeitig in mehreren Sprachen für den Ausdruck der Formulare verwaltet. Damit ist es beispielsweise möglich, Weihnachtsgrüße, allgemeine Kundenhinweise oder Werbeaktionen textuell zu hinterlegen, um sie auf den kundenseitigen Papieren auszugeben.

### Erläuterung der Felder

**Datei**
Name der Textdatei, in der die Texte gespeichert werden.
> Technische Info: Alphanumerisches Feld, DB-Feld: xtxtnr.datei

**Sprache**
Auswahl der Sprache. Es stehen nur die Sprachen zur Auswahl, die im Systemstammdaten hinterlegt sind (Stammdaten > Schlüssel > System > Sprachen)
> Technische Info: <F9>, DB-Feld: xtxtnr.sprkz

**Text**
Eingabe des entsprechenden Textes. Mehrzeilige Eingaben sind möglich. Eingabe in einer Zeile ist maximale 160 Zeichen möglich. Die einzelne Zeilen werden mithilfe der Sequenznummer unterschieden.
> Technische Info: Alphanumerisches Feld, DB-Feld: stammtxt.stammtxt, stammtxt.seqnr

**Ergänzende Informationen**
- "Marktpartnertexte" auf Seite B-165

## Marktpartner-Artikeltexte

*Stammdaten > Marktpartner > <F4> > Texte / Druck > MP-Artikeltexte*

*Abb. B-46 Artikeltexte*

Dieser Dialog dient der Hinterlegung marktpartnerspezifischer Artikeltexte in verschiedenen Sprachen. Diese Texte können in Abhängigkeit des Kundensprachkennzeichens auf den Formularen ausgegeben werden.

### Erläuterung der Felder

**Artikel**
Auswahl der entsprechenden Artikelnummer. Im Feld dahinter erscheint die Artikelbezeichnung.
> Technische Info: <F9>, DB-Feld: artxtzu.artnr

**Datei**
Name der Textdatei, in der die Texte gespeichert werden. Mit `<F3>` wechseln Sie in den Dialog Stammdaten, in dem neue Texte hinterlegt werden können.
> Technische Info: Alphanumerisches Feld, DB-Feld: artxtzu.datei

## Formulare

*Stammdaten > Marktpartner > <F4> > Texte / Druck > Formulare*

*Abb. B-47 Formulare*

In diesem Dialog besteht die Möglichkeit, einen kundenindividueller Report für die bestehende Formularart zu hinterlegen.

### Erläuterung der Felder

**Formular**
Wählen Sie die gewünschte Formularart (Angebot, Rechnung, etc.) aus. Die Bezeichnung wird im Feld Bezeichnung angezeigt.
> Technische Info: <F9>, DB-Feld: kundruckanz.formart

**Exemplare**
bestimmt die kundenspezifische standardmäßige Ausgabenanzahl des Formulars.
> Technische Info: Numerisches Feld, DB-Feld: kundruckanz.anzahl

**Komm**
Mit diesem Feld steuern Sie, ob Kommissionstexte ausgegeben werden sollen.
- Kommissionstexte werden gedruckt.
- Kommissionstexte werden nicht gedruckt.
> Technische Info: Toggle-Feld, DB-Feld: kundruckanz.kommdrkz

**Reportname**
Abweichender, kundenspezifische Reportname.
> Technische Info: Alphanumerisches Feld, DB-Feld: kundruckanz.repname

## Dokumentenarten

*Stammdaten > Marktpartner > <F4> > Texte / Druck > Dokumentenarten*

*Abb. B-48 Dokumentenarten*

In diesem Dialog können Sie verschiedene Dokumentenarten und die Art der Ausgabe hinterlegen. Der Dialog wird an folgender Stelle ausführlich erläutert:
- "Dokumentenarten" auf Seite B-245

## Vorgangs-Recherche

*Stammdaten > Marktpartner > <F4> > Vorgangsrecherche*

*Abb. B-49 Vorgangsrecherche*

Die Benutzung der Vorgangs-Recherche wurde bereits ausführlich in den Kapiteln Verkauf und Einkauf behandelt, und kann dort nachgelesen werden!

## Marktpartner-Info

*Stammdaten > Marktpartner > <F4> > Marktpartner-Info*

*Abb. B-50 Marktpartner-Info*

Unter diesem Menüpunkt werden verschiedene statistische Informationen über den Marktpartner geführt:
- Beträge offene Posten bei einer FIBU-Anbindung
- Beträge nicht beglichener Rechnungen (offene Posten)
- Beträge noch nicht berechneter Aufträge
- Datum, Nummer, Haus und Betrag für den letzten Auftrag, das letzte Angebot und die letzte Rechnung
- Summe des aufgelaufenen Umsatz im aktuellen Jahr.

### Erläuterung der Felder

**Kunde**
Auswahl der Kundennummer. Der Kundennamen wird nach der Nummerauswahl im Klartext angezeigt.
> Technische Info: <F9>, DB-Feld: kuplus.kunr

> **Marktpartner-Info**
> Die Felder in diesem Dialog dienen der Information und sind nicht änderbar. Die Beträge werden aus der Datenbanktabelle kuplus entnommen. Die restliche Felder werden aktuell aus dem Tagesgeschäft ermittelt und angezeigt.

## Replikationsdaten

*Stammdaten > Marktpartner > <F4> > Replikationsdaten*

*Abb. B-51 Replikationsdaten*

Je nach Konfiguration können Sie in diesem Dialog eine Limitverteilung für die einzelnen Niederlassungen vornehmen.

### Erläuterung der Felder

**ges. Limit**
Anzeige des Firmenlimits. Der Wert kommt aus dem Feld Firmenlimit (Stammdaten > Marktpartner > Register Limits).
> Technische Info: Anzeigefeld

**ges. AKV-Limit**
Anzeige des AKV-Limits. Der Wert kommt aus dem Feld AKV-Llimit (Stammdaten > Marktpartner > Register Limits).
> Technische Info: Anzeigefeld

**Haus**
Auswahl des Mandanten, für den die Limitdaten gelten sollen.
> Technische Info: <F9>, DB-Feld: limits.hausnr

**Limit**
Firmenlimit für den entsprechenden Mandanten. Wenn Sie das Feld verlassen, wird Ihnen im Feld dahinter der Prozentsatz angezeigt, den dieser Wert im Verhältnis zum gesamt Limit darstellt.
> Technische Info: <F9>, DB-Feld: limits.limit

**AKV-Limit**
AKV-Firmenlimit für den entsprechenden Mandanten. Wenn Sie das Feld verlassen, wird Ihnen im Feld dahinter der Prozentsatz angezeigt, den dieser Wert im Verhältnis zum gesamten AKV-Limit darstellt.
> Technische Info: <F9>, DB-Feld: limits.akvlimit

**Route**
Auswahl der Route. Im Feld dahinter wird Ihnen die Routenbezeichnung angezeigt. Die Routen und ihre Bezeichnungen werden unter Stammdaten > Schlüssel > System > Versand > Routen > Routen hinterlegt.
> Technische Info: <F9>, DB-Feld: limits.routenr

**Def. Haus**
Default-Haus für den Mandaten. Mit `<F5>` können Sie das aktuelle Haus als Default-Haus für alle Einträge wählen.
> Technische Info: <F9>, DB-Feld: limits.defhausnr

> **Gesamtwerte**
> Es können weder das gesamte Limit noch das gesamte AKV-Limit überschritten werden. Bei einer Überschreitung erfolgt eine entsprechende Meldung.

> **Unterer Dialogbereich**
> Am unteren Dialogbereich werden Ihnen die aufsummierten Werte sowohl für die Beträge als auch für die Prozentwerte angezeigt.

## DFÜ-Konfiguration

*Stammdaten > Marktpartner > <F4> > DFÜ-Konfiguration*

*Abb. B-52 DFÜ Konfiguration*

In diesem Dialog konfigurieren Sie die Steuerung der DFÜ.

Für weitere Informationen kontaktieren Sie bitte einen Mitarbeiter der A+W Software GmbH

### Erläuterung der Felder

**Partnertyp**
Auswahl des Partnertyps.
> Technische Info: <F9>, DB-Feld: mpdfuectrl.kuliflag

**Marktpartner**
Auswahl der Marktpartnernummer. Nach der Nummerauswahl wird der Kundenname im Klartext dargestellt.
> Technische Info: <F9>, DB-Feld: mpdfuectrl.mpnr

**Typ der DFÜ**
Auswahl der DFÜ-Art. Im Feld dahinter wird Ihnen die Bezeichnung angezeigt. Typ der DFÜ entscheidet über die Art und Weise der Datenübertragung und soll somit sehr gewissenhaft bestimmt werden. Die Auswahl können Sie bereits im Dialogkopf treffen. In diesem Fall können neue Konfigurationseinträge auch nur für diesen Typ der DFÜ erfolgen.
> Technische Info: <F9>, DB-Feld: mpdfuectrl.dfuetyp

**Steuerungstyp**
Steuerungstyp der DFÜ. Im Feld dahinter wird Ihnen die Bezeichnung angezeigt.
> Technische Info: <F9>, DB-Feld: mpdfuectrl.id

**Wert**
Steuerungswert.
- [x] Der DFÜ-Typ ist aktiv.
- [ ] Der DFÜ-Typ ist nicht aktiv.
> Technische Info: <F9>, DB-Feld: mpdfuectrl.value

## Hausspezifische Angaben

*Stammdaten > Marktpartner > <F4> > Hausspezifische Angaben*

*Abb. B-53 Hausspezifische Angaben*

Die hausspezifischen Angaben werden für das Mehr-Mandantensystem (Multi-Site) verwendet. Hier können Sie den unterschiedlichen Häusern einzelne Vertreter und Konditionsdebitoren zuordnen.

### Erläuterung der Felder

**Haus**
Auswahl der Hausnummer.
> Technische Info: <F9>, DB-Feld: mdzu.hnr

**Name**
Der Hausbenennung wird im Klartext automatisch angezeigt, wenn Sie das Feld Haus verlassen.

**Vertr. (Erlös)**
Auswahl des erlösmäßigen Vertreters. Für den hier eingetragenen Mitarbeiter werden dann die jeweiligen Provisionssätze gebucht und stehen zur Abrechnung bereit.
> Technische Info: <F9>, DB-Feld: mpmdzu.lager

**Name**
Der Name des erlösmäßigen Vertreters wird im Klartext automatisch angezeigt, wenn Sie das Feld Vertr. (Erlös) verlassen.

**Konditions-Debitor**
Auswahl der Kundennummer, deren Konditionen für die erfassten Vorgänge gelten soll.
> Technische Info: <F9>, DB-Feld: mpmdzu.konddebnr

**Name**
Der Kundenname wird im Klartext automatisch angezeigt, wenn Sie das Feld Konditionsdebitor verlassen.
> Technische Info: <F9>, DB-Feld: mp.name

**MwSt**
Auswahl einer Mehrwertsteuer. Wenn die Mandanten in verschiedenen Mwst-Bereiche befinden, kann hier für einen Marktpartner die abweichende Mwst festgelegt werden.
> Technische Info: <F9>, DB-Feld: mpmdzu.mwst

**MwSt (%)**
Nach der MwSt-Auswahl wird hier die Bezeichnung im Klartext dargestellt.
> Technische Info: <F9>, Anzeige-Feld

# Mitarbeiter

*Stammdaten > Mitarbeiter*

Im Mitarbeiterstamm werden alle identifizierenden Angaben (wie z B. Personalnummer, Name, Zeichen, etc.) für die Mitarbeiter, Systemdienste und Berechtigungsgruppen festgelegt.

Darüber hinaus werden alle EDV-Rechte und Einschränkungen, die den Mitarbeiter oder eine Berechtigungsgruppe betreffen, hinterlegt. So kann sichergestellt werden, dass die Mitarbeiter nur Zugang zu bestimmten Bereichen und entsprechende Berechtigungen in A+W Enterprise bekommen.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Mitarbeiter / Berechtigungsgruppen" auf Seite B-177
- "Mitarbeiter - Rechte" auf Seite B-182

## Mitarbeiter / Berechtigungsgruppen

*Stammdaten > Mitarbeiter*

*Abb. B-54 Mitarbeiter*

In diesem Dialog werden alle Angaben zu Mitarbeitern, Mitarbeitergruppen und System-Dienste hinterlegt.

### Erläuterung der Felder im Bereich Personendaten

**Pers.-Nr.**
Auswahl der Personalnummer. Bei der Neuaufnahme geben Sie die gewünschte Nummer ein.
> Technische Info: <F9>, DB-Feld: mitarb.manr

**Typ**
Dieses Feld spezifiziert die Art des Stammdatensatzes. Folgende Werte sind möglich:
- **Mitarbeiter:** Jede Personalnummer kann nur einmal vergeben werden. Mit der `<F6>`-Taste haben Sie die Möglichkeit, die nächsten freie Nummer durch das System zu vergeben.
- **Systemdienst:** Als Systemdienst sollte ein Mitarbeitersatz mit Personalnummer -1 angelegt werden. Die Existenz dieses Satzes ist notwendig, da sich alle A+W Enterprise-Hintergrundprozesse (z. B. Hintergrund-Auftragsbearbeitung, etc.) mit Mitarbeiternummer -1 melden.
- **Berechtigungsgruppe:** Eine Berechtigungsgruppe wird mit Programmzugangsrechten für einen bestimmten Personalbereich angelegt. Mitarbeitern des Aufgabengebietes wird daraufhin im Feld Berechtigungsgruppe die vergebene Gruppennummer zugeordnet. Damit entfällt die Vergabe der einzelnen gruppenspezifischen Modulzugangsberechtigungen für jeden einzelnen Mitarbeiter.
> Technische Info: Toggle-Feld, DB-Feld: mitarb.matyp

**Name**
Nachname des Mitarbeiters. Mit `<F5>` öffnen Sie den Dialog Anmerkungstexte, in dem Sie die Informationen zu dem Mitarbeiter hinterlegen können. Mit `<F3>` öffnen Sie den Dialog für die Übersicht über Mitarbeiterrechte.
> Technische Info: alphabetisches Feld, DB-Feld: mitarb.maname

> **Mitarbeiter- und Abteilungs-Anmerkungen**
> Mitarbeiter- und Abteilungs-Anmerkungen mit Priorität **hoch** und Ort **überall** können direkt beim Starten des A+W Enterprise-Hauptmenü oder beim Start des Moduls Versand angezeigt werden. So können wichtige mitarbeiterbezogene Informationen beim Start präsentiert werden. Ihr System muss entsprechend konfiguriert werden.

**Vorname**
Vorname des Mitarbeiters.
> Technische Info: alphabetisches Feld, DB-Feld: mitarb.mavname

**Geschl.**
Toggle-Feld. Geschlecht des Mitarbeiters.
- weiblich
- männlich
> Technische Info: Toggle-Feld, DB-Feld: mitarb.sex

**Anrede**
Auswahl der Anrede. Die entsprechenden Schlüssel werden über das Menü Anreden (Stammdaten > Schlüssel > Marktpartner) vergeben.
> Technische Info: <F9>, DB-Feld: mitarb.anrede

**Geb.-Dat.**
Geburtsdatum des Mitarbeiters.
> Technische Info: Numerisches Feld, DB-Feld: mitarb.gebdat

**Zeichen**
Schriftkürzel des Mitarbeiters.
> Technische Info: Alphanumerisches Feld, DB-Feld: mitarb.zeichen

### Erläuterung der Felder im Bereich Letzte Änderung

**Name**
In diesem Feld wird Ihnen der Mitarbeiter angezeigt, der den Stammdatensatz zuletzt geändert hat.

**Datum**
In diesem Feld wird Ihnen das Datum angezeigt, an dem der Stammdatensatz zuletzt geändert wurde.

### Erläuterung der Felder im Bereich Anmeldeinformationen

**Login**
A+W Enterprise-Loginname, der zusammen mit dem Passwort zum Programmstart berechtigt. In der Nutzung von A+W Enterprise - Webanwendung sowie auch A+W iQuote wird hier eingetragener Name ebenfalls zur Anmeldung verwendet.
> Technische Info: Alphanumerisches Feld, DB-Feld: mitarb.loginname

**Passwort**
Passwort, das zusammen mit dem A+W Enterprise-Loginname zum Programmstart berechtigt. Das Passwort kann nur vom Administrator eingetragen bzw. geändert werden. Für die Nutzung der A+W Enterprise - Standard-Anwendung wird das Passwort über die Unix bzw. Linux-Administrator vergeben. Das Passwort aus diesem Feld berechtigt zur Anmeldung in der A+W Enterprise - Webanwendung bzw. A+W iQuote.

### Erläuterung der Felder im Bereich Einschränkungen

**Shell**
Shellberechtigung. Soll auch die Betriebssystemebene zugänglich sein, so aktivieren Sie bitte diese Checkbox.
> Technische Info: Toggle-Feld, DB-Feld: mitarb.shjn

**Abteilungseinschränkung**
Ist diese Checkbox aktiv, werden diverse Auswertungen (z. B. Liste der unberechneten Aufträge, Produktionsfreigabe, etc.) auf die Vorgänge der dem Mitarbeiter zugeordneten Abteilung eingeschränkt.
> Technische Info: Toggle-Feld, DB-Feld: mitarb.abtview

**Mandanteneinschränkung**
Ist diese Checkbox aktiv, werden diverse Auswertungen (z. B. Liste der unberechneten Aufträge, Produktionsfreigabe, etc.) auf die Vorgänge des Mandanten eingeschränkt.
> Technische Info: Toggle-Feld, DB-Feld: mitarb.hausview

### Erläuterung der Felder im Bereich Mitarbeiter-/Kontaktdaten

**Durchwahl**
Interne Telefondurchwahl.
> Technische Info: Numerisches Feld, DB-Feld: mitarb.durchw

**Fax**
Nummer des Faxgerätes.
> Technische Info: Numerisches Feld, DB-Feld: mitarb.faxnr

**E-Mail**
E-Mail-Adresse des Mitarbeiters.
> Technische Info: Alphanumerisches Feld, DB-Feld: mitarb.email

**Mandant**
Werks- bzw. Niederlassungsnummer (Hauptmandant). Mit `<Umschalt>` + `<F5>` öffnen Sie den Dialog für die Hauszuordnung. Dort können Sie dann weitere Häuser dem Mitarbeiter zuordnen.
> Technische Info: Alphanumerisches Feld, DB-Feld: mitarb.hnr

**Position**
Auswahl der Position des Mitarbeiters.
> Technische Info: <F9>, DB-Feld: mitarb.pos

**Funktion**
Auswahl, ob der Mitarbeiter als Geschäftsführer oder Vertreter tätig ist. So können z. B. nur Personen, die als Vertreter gekennzeichnet sind, als solche im Kundenstamm einem Kunden zugeordnet werden.
> Technische Info: <F9>, DB-Feld: mitarb.funktion

**Mail zu**
Auswahl der Mitarbeiter-Nummer für die Weiterleitung einer E-Mail.
> Technische Info: <F9>, DB-Feld: mitarb.vertretung

**Aktivieren**
Über diese Checkbox aktivieren Sie die E-Mail Weiterleitung.
> Technische Info: Toggle-Feld, DB-Feld: mitarb.vertr_aktiv

**Abteilung**
Nummer der Abteilung. Aus statistischen Programmzugriffsgründen sollte jeder Mitarbeiter einer Abteilung zugeordnet werden. Im Feld dahinter wird dann die Abteilung angezeigt. Die entsprechenden Abteilungen werden über das gleichnamige Menü vergeben.
> Technische Info: <F9>, DB-Feld: mitarb.abtnr

**Kunde**
Hier können Sie dem Mitarbeiter einen Kunden zuordnen.
> Technische Info: <F9>, DB-Feld: mitarb.manrkunr

**Externer Mitarbeiter**
Aktivieren Sie die Checkbox, wenn es sich bei dem Mitarbeiter um einen externen Mitarbeiter (mit eingeschränkten Rechten) handelt.
> Technische Info: Toggle-Feld, DB-Feld: mitarb.externflag

**SQL-Berechtigungsgruppe**
Auswahl der Berechtigungsgruppe.
> Technische Info: <F9>, DB-Feld: mitarb.logingrp

### Erläuterung der Felder im Bereich Rechtegruppen

**Gruppe**
Auswahl der Gruppennummer. Im Feld dahinter wird die Bezeichnung angezeigt. Damit entfällt die Vergabe der einzelnen gruppenspezifischen Modulzugangsberechtigungen für jeden einzelnen Mitarbeiter.
> Technische Info: <F9>, DB-Feld: bengrpzu.grp

**Haus**
Auswahl der zugeordneten Hausnummer.
> Technische Info: <F9>, DB-Feld: bengrpzu.hausnr

### Erläuterung der Felder im Bereich Rechte

**EDV-Modul**
Auswahl des EDV-Moduls, in dem der Mitarbeiter seine EDV-Rechte ausüben kann. * steht für alle Programm-Module. Im weiteren Feld wird die Modulbezeichnung im Klartext dargestellt. Mit `<F9>` können Sie nach bestimmten Modul suchen. Für die Übersicht über alle Modulen und deren Bedeutung wenden Sie sich an A+W Software GmbH - Mitarbeiter.
> Technische Info: <F9>, DB-Feld: login.modul

**Terminal**
Auswahl des Terminals bzw der Terminalgruppe, an dem der Mitarbeiter für das jeweilige Modul zugelassen ist. * steht für alle Terminals.
> Technische Info: <F9>, DB-Feld: login.ort

**Rechte**
Auswahl der Mitarbeiterrechte:
- **-:** Keine Rechte.
- **r:** Leserecht
- **w:** Schreibrecht
> Technische Info: Toggle-Feld, DB-Feld: login.rwx

**Haus**
Auswahl der zugeordneten Hausnummer, in der diese Einschränkung gilt (für Multi-Site-Systeme). Die hausindividuelle Einschränkungen können nur bei lokalen Rechten vorgenommen werden. Für weitere Informationen wenden Sie sich an A+W Software GmbH - Mitarbeiter.
> Technische Info: <F9>, DB-Feld: login.hausnr

## Mitarbeiter - Rechte

*Stammdaten > Mitarbeiter > Rechte (Übersicht) <F3>*

*Abb. B-55 Mitarbeiter, Rechte*

In diesem Dialog geben Sie die Mitarbeiternummer und die Hausnummer ein, zu dem Sie die Rechte sehen möchten.

### Erläuterung der Felder

**Mitarbeiter**
Eingabe der Mitarbeiternummer.
> Technische Info: Numerisches Feld

**Haus**
Eingabe der Hausnummer.
> Technische Info: Numerisches Feld

Wenn Sie den Dialog mit [OK] verlassen, werden Ihnen im nächsten Dialog die gewünschten Informationen angezeigt:

*Abb. B-56 Mitarbeiter, Rechte*

### Erläuterung der Felder

**Modul**
Anzeige der Modulnummer. Ein * kennzeichnet alle Module.
> Technische Info: Anzeige-Feld

**Recht**
Anzeige des Rechtes:
- **-:** Keine Rechte.
- **r:** Leserecht
- **w:** Schreibrecht
> Technische Info: Anzeige-Feld

**User/Gruppe**
Hier sehen Sie, ob es sich um ein User-Recht oder ein Gruppen-Recht handelt:
- **U:** User-Recht
- **G:** Gruppen-Recht
> Technische Info: Anzeige-Feld

**Drucken**
Über diese Schaltfläche können Sie sich die Übersicht der Mitarbeiterrechten ausdrucken.

# Abteilungen

*Stammdaten > Abteilungen > Abteilungen*
*Stammdaten > Abteilungen > Einzelne Bezeichnung*
*Stammdaten > Abteilungen > Alle Bezeichnung*

*Abb. B-57 Abteilungen*

In diesem Dialog werden alle die identifizierenden Angaben (wie z. B. Bezeichnung, Kürzel usw.) für die Abteilungen im Unternehmen festgelegt.

> **Mehrsprachige Bezeichnungen**
> Seit QR2209 können Sie in A+W Enterprise auch für Abteilungen mehrsprachige Bezeichnungen hinterlegen.

Mit `<F5>` öffnen Sie den Dialog Anmerkungstexte, in dem Sie die Informationen zu der Abteilung hinterlegen können.

> **Mitarbeiter- und Abteilungs-Anmerkungen**
> Mitarbeiter- und Abteilungs-Anmerkungen mit Priorität **hoch** und Ort **überall** können direkt beim Starten des A+W Enterprise-Hauptmenü oder beim Start des Moduls Versand angezeigt werden. So können wichtige mitarbeiterbezogene Informationen beim Start präsentiert werden. Ihr System muss entsprechend konfiguriert werden.

## Erläuterung der Felder

**Abteilung**
Auswahl der Abteilung.
> Technische Info: <F9>, DB-Feld: abteilung.abtnr

**Kürzel**
Stellt eine Abkürzung der Bezeichnung dar.
> Technische Info: Alphanumerisches Feld, DB-Feld: abteilung.abtid

**Bezeichnung**
Abteilungsbezeichnung. Die Bezeichnung kann überschrieben werden.
> Technische Info: Alphanumerisches Feld, DB-Feld: abteilung.bez

**Kostenstelle**
Auswahl der Kostenstelle. Der Eintrag kann zu statistischen Zwecken genutzt werden. Die entsprechenden Schlüssel werden über das Menü Kostenstelle (Stammdaten > Kostenstamm) vergeben.
> Technische Info: <F9>, DB-Feld: abteilung.kostenst

**Meldungsempfänger**
Auswahl des Meldungsempfängers. Der System-Meldungsempfänger der Abteilung ist die Person oder die Personengruppe, die Meldungen anderer Mitarbeiter dieser Abteilung entgegennimmt.
> Technische Info: <F9>, DB-Feld: abteilung.manr

**Formulargruppe**
Ein Eintrag der Formulargruppe, die diese Abteilung benutzt, wird beim Formulardruck berücksichtigt. In der Regel wird pro Abteilung eine Formulargruppe hinterlegt.
> Technische Info: Numerisches Feld, DB-Feld: abteilung.formgrp

**Fax**
Existiert ein eigener Faxanschluss, kann diese Nummer hier hinterlegt werden.
> Technische Info: Numerisches Feld, abteilung.faxnr

**Letzte Änderung**
Hier wird der Mitarbeiter angezeigt, der die Daten zuletzt geändert hat sowie das entsprechende Datum.

**Spr**
Sprachkennzeichen.
> Technische Info: <F9>, DB-Feld: xsprbez.sprkz

# Marktpartnerschlüssel

*Stammdaten > Schlüssel > Marktpartner*

In diesem Bereich werden Merkmale zur Beschreibung der Marktpartner (Kunden, Lieferanten, etc.) angelegt. Sie stehen dann bei der Erfassung der Marktpartner zur Verfügung. Die einzelnen Merkmale werden nachfolgend erläutert.

Sie haben Zugriff auf folgende Bereiche:

| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| a a/b | Anreden | -> "Anreden-Bezeichnungen" auf Seite B-188 |
| b | Bonus | -> "Bonus" auf Seite B-189 |
| ca | Gruppen | -> "Gruppen" auf Seite B-191 |
| c b/c | Gruppenbezeichnungen | -> "Gruppenbezeichnungen" auf Seite B-192 |
| d a/b | Branchen | -> "Branchenbezeichnungen" auf Seite B-193 |
| e | Etikettentexte | -> "Etikettentexte" auf Seite B-194 |
| fa | Kalender | -> "Kalender" auf Seite B-195 |
| fb | Spez. Kalender | -> "Spezielle Kalender" auf Seite B-197 |
| fc | Kundenkalender | -> "Kundenkalender" auf Seite B-199 |
| fd | Mandantenkalender | -> "Mandantenkalender" auf Seite B-201 |
| g | FIBU-Mandanten | -> "FIBU-Mandanten" auf Seite B-203 |
| ha | Länder | -> "Länder" auf Seite B-204 |
| h b/c | Länderbezeichnungen | -> "Länder" auf Seite B-204 |
| i a/b | Wirtschaftsräume | -> "Wirtschaftsraumbezeichnungen" auf Seite B-206 |
| j a/b | Region/Bundesländer | -> "Regionen / Bundesländerbezeichnungen" auf Seite B-207 |
| ka | Qualitätsskala | -> "Allgemeine Qualitätsskala" auf Seite B-208 |
| kb | Qual.-Skala Termine | -> "Termin-Qualitätsskala" auf Seite B-210 |
| kc | Qual.-Skala Preise | -> "Preise-Qualitätsskala" auf Seite B-212 |
| kd | Qual.-Skala Mengen | -> "Mengen-Qualitätsskala" auf Seite B-214 |
| ka | Qual.-Skala Spezial | -> "Spezial-Qualitätsskala" auf Seite B-216 |
| ia | Reklamationsgründe | -> "Reklamationsgründe" auf Seite B-218 |
| ib | Reklamationsorte | -> "Reklamationsorte" auf Seite B-220 |
| I c | Reklamationstypen | -> "Reklamationstypen" auf Seite B-222 |
| ma | Rabattmethoden | -> "Rabattmethoden" auf Seite B-224 |
| ma | Rabatte | -> "Rabatte" auf Seite B-228 |
| | | -> "Rabatte - Details" auf Seite B-230 |
| n | Hausspezifische Angaben | -> "Hausspezifische Marktpartner-Angaben" auf Seite B-235 |

> **Mehrsprachigkeit**
> Alle sprachabhängigen Schlüsseldaten werden in der Tabelle xsprbez gespeichert. Für den jeweiligen Dialog, z. B. Marktpartner > Anreden, wird dann zur Laufzeit eine View gebaut, die die Daten für die Anreden beinhaltet. Auf diese View kann man auch auf der Datenbankebene zugreifen. Daher haben wir in den Dialogen, die das betrifft, die Information über die View mit angegeben. In einigen Fällen existieren auch sprachunabhängige Daten. Diese werden über xx*-View geführt.

## Anreden-Bezeichnungen

*Stammdaten > Schlüssel > Marktpartner > Anreden > Einzelne Bezeichnungen*
*Stammdaten > Schlüssel > Marktpartner > Anreden > Alle Bezeichnungen*

*Abb. B-58 Anreden*

Diese beiden Dialoge enthalten die Anredeformen, die bei der Erfassung von Marktpartnern vorkommen können, in den jeweiligen Sprachen.

### Erläuterung der Felder

**Nummer/Nr**
Schlüssel-Nummer. Zum Anlegen einer neuen Anrede geben Sie die nächste freie Nummer ein.
> Technische Info: <F9>, DB-Feld: xsprbez.id
> View: xanrede.anrkz

**Spr**
Sprachkennzeichen.
> Technische Info: <F9>, DB-Feld: xsprbez.sprkz

**Bezeichnung**
Bezeichnung der Anrede, z. B. Firma.
> Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez1
> View: xanrede.anrkz

## Bonus

*Stammdaten > Schlüssel > Marktpartner > Bonus > Bonus*
*Stammdaten > Schlüssel > Marktpartner > Bonus > Einzelne Bezeichnung*
*Stammdaten > Schlüssel > Marktpartner > Bonus > Alle Bezeichnung*

*Abb. B-59 Bonus*

In diesem Dialog verfassen Sie die Regeln für die Bonität. Die Zuweisung eines Bonusverfahrens kann im Marktpartnerstamm oder während der Auftragserfassung erfolgen.

> **Mehrsprachige Bezeichnungen**
> Seit QR2209 können Sie in A+W Enterprise auch für Bonus mehrsprachige Bezeichnungen hinterlegen.

### Erläuterung der Felder

**Bonus/Nr**
Auswahl eines Verfahrens. Über die Eingabe einer neuen Nummer wird ein neues Verfahren angelegt.
> Technische Info: <F9>, DB-Feld: xbonus.bonusnr

**Bezeichnung**
Textuelle Erläuterung des Verfahrens.
> Technische Info: Alphanumerisches Feld, DB-Feld: xbonus.bonbez

**Art**
Auswahl der Kriterien, nach denen der Bonus gewährt werden soll. Erstes Feld:
- **WE:** Der Bonus wird nach dem Auftragsvolumen in der Währungseinheit gewährt.
- **QM:** Der Bonus wird nach der abgenommenen Menge in Quadratmetern gewährt.
> Technische Info: <F9>, DB-Feld: xbonus.bonart

Zweites Feld:
- **WE/qm:** Hier steuern Sie, ob sich der Bonus nach der Währungseinheit pro qm errechnet.
- **Max %-Satz:** Hier steuern Sie, ob es sich bei dem Bonus um einen maximalen Prozentwert handelt.
> Technische Info: <F9>, DB-Feld: xbonus.bontyp
Im Feld dahinter geben Sie den entsprechenden Berechnungswert ein.
> Technische Info: Numerisches Feld, DB-Feld: xbonus.satz

**Abrechnungszeitraum**
Hier wird die maximale Höhe des gewährten Bonus als Information festgehalten, z. B. 3 bedeutet, alle 3 Monate.
> Technische Info: Numerisches Feld, DB-Feld: xbonus.zeitraum

**im Monat**
Hier legen Sie fest, wann genau die Prüfung erfolgen soll. In dem gewünschten Monat tragen Sie ein j ein. In den Feldern, die mit einem n gekennzeichnet sind, erfolgt keine Berechnung.
> Technische Info: Toggle-Feld, DB-Feld: xbonus.zp1-12

**Bonusstaffel**
Im Anschluss an den allgemeinen Bereich folgt die Bonusstaffel. Die Spalte Bonus zeigt die Zuweisung zum Bonusschlüssel an. Für die Staffelung stehen mehrere Zeilen zur Verfügung, in den beschrieben wird, ab welchem Umsatz bzw. welcher Abnahmemenge welcher %-Satz gewährt wird.

**Spr**
Sprachkennzeichen.
> Technische Info: <F9>, DB-Feld: xsprbez.sprkz

## Gruppen

*Stammdaten > Schlüssel > Marktpartner > Gruppen > Gruppen*

*Abb. B-60 Gruppen*

Dieser Dialog zeigt die Marktpartner-Gruppen in der Mandantensprache. Die Gruppen können zu informativen Zwecken in Klassen eingeteilt werden. Die Klasse hat jedoch keine Auswirkung.

Das Löschen einzelner Gruppen ist nur in diesem Dialog möglich.
> Technische Info: Tabelle xxgrp

**Ergänzende Informationen**
- "Gruppenbezeichnungen" auf Seite B-192

## Gruppenbezeichnungen

*Stammdaten > Schlüssel > Marktpartner > Gruppen > Einzelne Bezeichnungen*
*Stammdaten > Schlüssel > Marktpartner > Gruppen > Alle Bezeichnungen*

*Abb. B-61 Gruppen*

Diese beiden Dialoge enthalten die Marktpartner-Gruppen, die bei der Erfassung von Marktpartnern vorkommen können, in den jeweiligen Sprachen.

### Erläuterung der Felder

**Gruppe**
Schlüssel-Nummer. Zum Anlegen einer neuen Gruppe geben Sie die nächste freie Nummer ein.
> Technische Info: <F9>, DB-Feld: xsprbez.id
> View: xgrp.grpnr

**Spr**
Sprachkennzeichen.
> Technische Info: <F9>, DB-Feld: xsprbez.sprkz

**Bezeichnung**
Bezeichnung der Gruppe, z. B. ISO-Fertigung.
> Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez1
> View: xgrp.atxt

## Branchenbezeichnungen

*Stammdaten > Schlüssel > Marktpartner > Branchen > Einzelne Bezeichnungen*
*Stammdaten > Schlüssel > Marktpartner > Branchen > Alle Bezeichnungen*

*Abb. B-62 Branchen*

Dieser Dialog enthält die Branchen, die bei der Erfassung von Marktpartnern vorkommen können, in den jeweiligen Sprachen. Über diese Branchen können alle speziellen Konditionen gepflegt werden.

### Erläuterung der Felder

**Nummer/Nr**
Schlüssel-Nummer. Zum Anlegen einer neuen Branche geben Sie die nächste freie Nummer ein.
> Technische Info: <F9>, DB-Feld: xsprbez.id
> View: xbranche.branchenr

**Spr**
Sprachkennzeichen.
> Technische Info: <F9>, DB-Feld: xsprbez.sprkz

**Bezeichnung**
Bezeichnung der Branche, z. B. ISO-Hersteller.
> Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez1
> View: xbranche.branche

## Etikettentexte

*Stammdaten > Schlüssel > Marktpartner > Etikettentexte > Etikettentexte*

*Abb. B-63 Etikettentexte*

In diesem Dialog hinterlegen Sie kundenspezifische Etikettentexte.
Der Eintrag im Feld Produktname erscheint als kundenspezifische Zusatzinformation auf den Scheibenetiketten. Über das frei wählbare Kürzel wird der Langtext referenziert.

### Erläuterung der Felder

**Nummer**
Zum Anlegen einer neuen Etikettentextnummer wählen Sie die nächst freie Nummer.
> Technische Info: Numerisches Feld, DB-Feld: xetikett.txtnr

**Produktname**
In diesem Feld ordnen Sie den Kunden bzw. das Objekt zu.
> Technische Info: Alphanumerisches Feld, DB-Feld: xetikett.etitxt1

**Kürzel**
Über das Kürzel wird der Langtext referenziert.
> Technische Info: Numerisches Feld, DB-Feld: xetikett.etitxt2

**Text**
Dieser Text erscheint als kundenspezifische Zusatzinformation auf den Scheibenetiketten.
> Technische Info: Alphanumerisches Feld, DB-Feld: xetikett.etitxt3

## Kalender

*Stammdaten > Schlüssel > Marktpartner > Kalender*
*System-Menü (<Strg> + <F4>) > Infodienste > Kalender > Kalender*

*Abb. B-64 Kalender (Tagesansicht)*

In diesem Dialog pflegen Sie Ihren Betriebskalender.
Wenn Sie mit dem Mehr-Mandantensystem (Multi-Site) arbeiten, handelt es sich dabei um den Kalender des Hauptmandanten. Abweichende Mandantenkalender pflegen Sie unter
- "Mandantenkalender" auf Seite B-201
Es stehen Ihnen zwei unterschiedliche Ansichten (`<F2>`) zur Verfügung:
- Tagesansicht
- Monatsansicht

### Erläuterung der Felder

**Datum**
Hier wird Ihnen jedes einzelne Datum angezeigt.

**Tag**
Hier wird Ihnen jeder einzelne Tag angezeigt.

**KW**
Hier wird Ihnen die Kalenderwoche angezeigt.

**H**
Auswahl, ob es sich bei dem Tag um einen Handelstag handelt.
> Technische Info: Toggle-Feld, DB-Feld: alkal.htag

**P**
Auswahl, ob es sich bei dem Tag um einen Produktionstag handelt.
> Technische Info: Toggle-Feld, DB-Feld: alkal.ptag

**H-MD**
Hier sehen Sie, ob es sich bei diesem Tag um einen mandantenspezifischen Handelstag handelt. Der Eintrag hier übersteuert den Eintrag im Feld H. Die mandantenspezifischen Handelstage werden in System > Schlüssel > Marktpartner > Kalender > Mandantenkalender gepflegt und können hier nicht geändert werden.

**P-MD**
Hier sehen Sie, ob es sich bei diesem Tag um einen mandantenspezifischen Produktionstag handelt. Der Eintrag hier übersteuert den Eintrag im Feld P. Die mandantenspezifischen Produktionstage werden in System > Schlüssel > Marktpartner > Kalender > Mandantenkalender gepflegt und können hier nicht geändert werden.

**Bemerkung**
In diesem Feld können Sie eine entsprechende Bemerkung hinterlegen.
> Technische Info: Alphanumerisches Feld, DB-Feld: alkal.bem

> **Arbeiten mit A+W Production**
> Sollten Sie mit A+W Production arbeiten, kann das System so konfiguriert werden, dass dieser Kalender auch in der Produktion ausgewertet wird. Diese Konfiguration erfolgt in A+W Production.

## Spezielle Kalender

*Stammdaten > Schlüssel > Marktpartner > Kalender > Spez. Kalender > Spez. Kalender*
*Stammdaten > Schlüssel > Marktpartner > Kalender > Spez. Kalender > Einzelne Bezeichnungen*
*Stammdaten > Schlüssel > Marktpartner > Kalender > Spez. Kalender > Alle Bezeichnungen*
*System-Menü (<Strg> + <F4>) > Infodienste > Kalender > Spez. Kalender*
*System-Menü (<Strg> + <F4>) > Infodienste > Kalender > Spez. Kalender > Einzelne Bezeichnungen*
*System-Menü (<Strg> + <F4>) > Infodienste > Kalender > Spez. Kalender > Alle Bezeichnungen*

*Abb. B-65 Spez. Kalender*

In diesem Kalender können Sie z. B. Daten für Ereignisse hinterlegen.

### Erläuterung der Felder

**Kalender**
Auswahl der Kalendernummer.
> Technische Info: <F9>, DB-Feld: almpkal.kalnr

**Datum**
Hier geben Sie das Datum ein.
> Technische Info: Numerisches Feld, DB-Feld: almpkal.datum

**Tag**
Wenn Sie das Feld Datum verlassen, wird der Tag automatisch eingeblendet.

**KW**
Wenn Sie das Feld Datum verlassen, wird die Kalenderwoche automatisch eingeblendet.

**BHT**
Hier sehen Sie, ob es sich um einen Betriebshandelstag handelt oder nicht.

**H**
Über dieses Feld können Sie Tage, an denen normalerweise nicht gearbeitet wird (z. B. Sonntage) als Handelstage definieren.
> Technische Info: Toggle-Feld, DB-Feld: almpkal.htag

**Bemerkung**
In diesem Feld können Sie eine entsprechende Bemerkung hinterlegen.
> Technische Info: Alphanumerisches Feld, DB-Feld: almpkal.bem

**Kalender/Nr**
Schlüssel-Nummer. Zum Anlegen eines neuen Kalenders geben Sie die nächste freie Nummer ein.
> Technische Info: Numerisches Feld, DB-Feld: xsprbez.id
> View: xkalender.kalnr

**Spr**
Sprachkennzeichen.
> Technische Info: <F9>, DB-Feld: xsprbez.sprkz

**Bezeichnung**
Bezeichnung des Kalenders, z. B. Lieferanten.
> Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez1
> View: xkalender.atxt

## Kundenkalender

*Stammdaten > Schlüssel > Marktpartner > Kalender > Kundenkalender*
*System-Menü (<Strg> + <F4>) > Infodienste > Kalender > Kundenkalender*

*Abb. B-66 Kundenkalender*

Für Marktpartner vom Typ Kunde und Sonstige können im Kundenkalender eigene Daten hinterlegt werden. D. h. es können Marktpartner-spezifisch Handels-, Produktions- und Feiertage hinterlegt werden.

### Erläuterung der Felder

**Partnertyp**
Auswahl des Partnertyps.
> Technische Info: <F9>, DB-Feld: almpkal.kuliflag

**Marktpartner**
Auswahl der Marktpartnernummer.
> Technische Info: <F9>, DB-Feld: almpkal.mpnr

**Datum**
Hier geben Sie das Datum ein.
> Technische Info: Numerisches Feld, DB-Feld: almpkal.datum

**Tag**
Wenn Sie das Feld Datum verlassen, wird der Tag automatisch eingeblendet.

**KW**
Wenn Sie das Feld Datum verlassen, wird die Kalenderwoche automatisch eingeblendet.

**BHT**
Hier sehen Sie, ob es sich um einen Betriebshandelstag handelt oder nicht.

**H**
Über dieses Feld können Sie Tage, an denen normalerweise nicht gearbeitet wird (z. B. Sonntage) als Handelstage definieren.
> Technische Info: Toggle-Feld, DB-Feld: almpkal.htag

**Bemerkung**
In diesem Feld können Sie eine entsprechende Bemerkung hinterlegen.
> Technische Info: Alphanumerisches Feld, DB-Feld: almpkal.bem
