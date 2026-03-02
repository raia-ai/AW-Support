# 02\_general

**Category:** Support Cantor / General | **Tickets:** 6

***

## \[AW-236436]

**Subject:** Zeitwirtschaft

**Status:** Unknown | **Category:** Support Cantor | **Last Action:** 25.07.2025 16:36

<details>

<summary>Full conversation</summary>

```
From: Stefan Rixecker
To: Dirk Horn | Date: 25.07.2025 16:36
Type: State changed | 
RE: [AW-236436] Zeitwirtschaft (26)
DH
```

</details>

***

## \[AW-235622]

**Subject:** Ermittlung der versandfertigen Einheiten

**Status:** Unknown | **Category:** Support Cantor | **Last Action:** 25.07.2025 14:08

<details>

<summary>Full conversation</summary>

```
From: Michael Roppert
To: | Date: 25.07.2025 14:08
Type: State changed | 
RE: [AW-235622] Ermittlung der versandfertigen Einheiten (6)
The calculation of the elements that are ready for dispatch is not connected to the terminal status as such. The calculation is based on the current production status in the barcode table, no matter from where this status was booked.
The calculation works on three layers: Delivery notes, order commissions that do not have delivery notes and orders  without delivery notes.
The overall quantity of ready elements for these is evaluated from the barcode table by counting all element barcodes (Element barcode = Barcode with fieldno 0) that have dispatch ready status. These are the status between the delivery start status specified by the Entry [LIEFERSCHEIN], ProdStatusLieferschein and the end status which is the status Shipped.
The total count of  found elements is distributed to the connected Delivery notes, order commissions and orders.
```

</details>

***

## \[AW-238050]

**Subject:** PW request at sending PO out of Cantor

**Status:** Unknown | **Category:** Support Cantor | **Last Action:** 24.07.2025 18:21

<details>

<summary>Full conversation</summary>

```
From: Marcus Büst
To: Dirk Horn | Date: 24.07.2025 18:21
Type: State changed | 
RE: [AW-238050] PW request at sending PO out of Cantor (3)
Hallo Dirk, 

mich hat Sachin vom NA Team wegen eines Problems mit dem Printspooler in Cantor angesprochen. 
Kannst du dir das Ticket einmal anschauen, ob du hier unterstützen kannst? Wie habt Ihr das Problem bei den deutschen Kunden gelöst?
Viele Grüße,
Marcus
```

</details>

***

## \[AW-236702]

**Subject:** Kumulierte Bestände - Fakturierung Konsi-Lager

**Status:** Unknown | **Category:** Support Cantor | **Last Action:** 24.07.2025 09:53

RE: WG: \[AW-236702] Kumulierte Bestände - Fakturierung Konsi-Lager (15) Hallo Frau Pferd, endschuldigen Sie bitte die Verzögerung. Bei der Verwendung der Systemaktion 76 - Pseudobestellungen für Konsilager wurde der Parameter CUMULATE nicht korrekt ausgewertet. Dies wurde nun behoben. Die aktuellen dll's stehen auf dem FTP-Server. V\_7\_8\_Unicode\_Build\_2023\_1\_0\_85\_Date\_24\_07\_2025\_\_09\_51\_19.zip Mit freundlichen Grüßen | Best regards Sabine Weidmann ###EOM## Phone: +49 641 96620 393 Mobile: +49 64...

<details>

<summary>Full conversation</summary>

```
From: Sabine Weidmann (support.cantor.de@a-w.com)
To: Sabrina.Pferdt@weru.de | Date: 24.07.2025 09:53
Type: Answer | 
RE: WG: [AW-236702] Kumulierte Bestände - Fakturierung Konsi-Lager (15)
Hallo Frau Pferd,
endschuldigen Sie bitte die Verzögerung.
Bei der Verwendung der Systemaktion 76 - Pseudobestellungen für Konsilager wurde der Parameter CUMULATE nicht korrekt ausgewertet. Dies wurde nun behoben.
Die aktuellen dll's stehen auf dem FTP-Server.
V_7_8_Unicode_Build_2023_1_0_85_Date_24_07_2025__09_51_19.zip
 
Mit freundlichen Grüßen | Best regards
Sabine Weidmann
###EOM##

Phone:  +49 641 96620 393
Mobile:  +49 6404 2051 362
A+W Software GmbH
Siemensstraße 3
35463 Fernwald
Germany

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie …
```

</details>

***

## \[AW-229697]

**Subject:** USWG - PMC Glass interface adjustment

**Status:** Unknown | **Category:** Support Cantor | **Last Action:** 23.07.2025 14:03

<details>

<summary>Full conversation</summary>

```
From: Damian Mizerny
To: Darius Porumb | Date: 23.07.2025 14:03
Type: State changed | 
USWG - PMC Glass interface adjustment (34)
Hello Darius,
 
Everything is described in dev-req.
 
In the adjustment we have included:
- dates in NH and NE records - right now we should get floor dates from a job if the job is created - previously it was just a dates from purchase order
- correct path of the interface file for each site, e.g. folder 102 for site 102, folder 140 for site 140 - previously all PMC interface files went to main folder without splitting
 
You need to prepared order and JOB. PMC interface file can be created for any purchase order for glass like other purchase order interfaces. You must check what dates you will get in NE, NH records in the file.
 
We have 2 options which must be tested:
- interface file for glass order created before the JOB was created
- interface file for glass order created after the JOB was created
```

</details>

***

## \[AW-235440]

**Subject:** Reportdefinition Rechnung (1000)

**Status:** Unknown | **Category:** Support Cantor | **Last Action:** 11.07.2025 14:48

RE: \[AW-235440] Reportdefinition Rechnung (1000) (17) Hallo Herr Fischer, da der Druck über die Report-Definitionen jetzt über ein Tabellenfeld erfolgt, gibt es Beschränkungen in der Anzahl der Zeichen. Bei der Bezeichnung sind das 60 Zeichen. Genau hier wird Ihr Text abgeschnitten. Im alten Druck gab es diese Begrenzung nicht, da keine Tabellenfeld hinter der Ausgabe lag und so Text während des Druckvorgangs zusammengesetzt wurde. Folgender Lösungsvorschlag zur Ausgabe der Montagartikel: Sie e...

<details>

<summary>Full conversation</summary>

```
From: Sabine Weidmann (support.cantor.de@a-w.com)
To: mfischer@tmp-fenster.de | Date: 11.07.2025 14:48
Type: Answer | 
RE: [AW-235440] Reportdefinition Rechnung (1000) (17)
Hallo Herr Fischer,
da der Druck über die Report-Definitionen jetzt über ein Tabellenfeld erfolgt, gibt es Beschränkungen in der Anzahl der Zeichen. Bei der Bezeichnung sind das  60 Zeichen. Genau hier wird Ihr Text abgeschnitten. Im alten Druck gab es diese Begrenzung nicht, da keine Tabellenfeld hinter der Ausgabe lag und so Text während des Druckvorgangs zusammengesetzt wurde.
Folgender Lösungsvorschlag zur Ausgabe der Montagartikel:
Sie erfassen eine neue Eigenschaft z.B. 1030 in der Klasse 730 und geben diese für den Druck auf den gewünschten Papieren über die Anzeigensteuerung frei. Die ES30 unterdrücken Sie auf diesen Papieren, ebenfalls über die Anzeigensteuerung. Die neue Eigenschaft belegen Sie mit dem Inhalt der ES30.

Die Ausgabe z.B. auf der Rechnung sieht dann wie folgt aus.

Mit freundlichen Grüßen | Best regards
Sabine Weidmann
###EOM##

Phone:  +49 641 96620 393
Mobile:  +49 6404 2051 362
A+W Software GmbH
Siemensstraße 3
35463 Fernwald
Germany

www…
```

</details>

***
