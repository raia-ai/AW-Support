# Support Cantor

This section contains **359 tickets** in the **Support Cantor** category.

[← Back to Index](README.md)

## Sub-categories

- [General (6)](#general)
- [Support Cantor - 2nd Level (2)](#support-cantor---2nd-level)
- [Support Fernwald - Cantor (99)](#support-fernwald---cantor)
- [Support Poland - Cantor (227)](#support-poland---cantor)
- [Support US - Cantor (25)](#support-us---cantor)

---

## General

### [AW-236436] — Zeitwirtschaft

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-236436]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor |
| **Last Action** | 25.07.2025 16:36 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Stefan Rixecker
To: Dirk Horn | Date: 25.07.2025 16:36
Type: State changed | 
RE: [AW-236436] Zeitwirtschaft (26)
DH
```

</details>

---

### [AW-235622] — Ermittlung der versandfertigen Einheiten

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-235622]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor |
| **Last Action** | 25.07.2025 14:08 |

<details>
<summary>View Full Conversation Thread</summary>

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

---

### [AW-238050] — PW request at sending PO out of Cantor

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-238050]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor |
| **Last Action** | 24.07.2025 18:21 |

<details>
<summary>View Full Conversation Thread</summary>

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

---

### [AW-236702] — Kumulierte Bestände - Fakturierung Konsi-Lager

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-236702]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor |
| **Last Action** | 24.07.2025 09:53 |

**Description:**

> RE: WG: [AW-236702] Kumulierte Bestände - Fakturierung Konsi-Lager (15) Hallo Frau Pferd, endschuldigen Sie bitte die Verzögerung. Bei der Verwendung der Systemaktion 76 - Pseudobestellungen für Konsilager wurde der Parameter CUMULATE nicht korrekt ausgewertet. Dies wurde nun behoben. Die aktuellen dll's stehen auf dem FTP-Server. V_7_8_Unicode_Build_2023_1_0_85_Date_24_07_2025__09_51_19.zip Mit freundlichen Grüßen | Best regards Sabine Weidmann ###EOM## Phone:  +49 641 96620 393 Mobile:  +49 64...

<details>
<summary>View Full Conversation Thread</summary>

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

---

### [AW-229697] — USWG - PMC Glass interface adjustment

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-229697]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor |
| **Last Action** | 23.07.2025 14:03 |

<details>
<summary>View Full Conversation Thread</summary>

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

---

### [AW-235440] — Reportdefinition Rechnung (1000)

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-235440]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor |
| **Last Action** | 11.07.2025 14:48 |

**Description:**

> RE: [AW-235440] Reportdefinition Rechnung (1000) (17) Hallo Herr Fischer, da der Druck über die Report-Definitionen jetzt über ein Tabellenfeld erfolgt, gibt es Beschränkungen in der Anzahl der Zeichen. Bei der Bezeichnung sind das  60 Zeichen. Genau hier wird Ihr Text abgeschnitten. Im alten Druck gab es diese Begrenzung nicht, da keine Tabellenfeld hinter der Ausgabe lag und so Text während des Druckvorgangs zusammengesetzt wurde. Folgender Lösungsvorschlag zur Ausgabe der Montagartikel: Sie e...

<details>
<summary>View Full Conversation Thread</summary>

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

---

## Support Cantor - 2nd Level

### [AW-237367] — Shape Error 441 with Extended Half Round - Rounding Errors

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-237367]` |
| **Status** | 🔵 In Progress |
| **Category** | Support Cantor / Support Cantor - 2nd Level |
| **Last Action** | 23.07.2025 18:00 |

**Description:**

> RE: [AW-237367] Shape Error 441 with Extended Half Round - Rounding Errors (25) Hi Darius, We are currently using version 7.9: I've exported two Cantor orders for you. One is the aforementioned 571296, and the other is the most recent problem order 573939. I've attached them along with their problem xmls. I've exported the Cantor orders via Transfer -> Export Orders/Quotations. Let me know if that is the correct method, or if you'd like me to export the orders in another way. In regards to how t...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Ethan Chau (EthanC@valuewds.com)
To: support.cantor.us@a-w.com | Date: 23.07.2025 18:00
Type: Request | 
RE: [AW-237367] Shape Error 441 with Extended Half Round - Rounding Errors (25)
Hi Darius,

We are currently using version 7.9:

I've exported two Cantor orders for you. One is the aforementioned 571296, and the other is the most recent problem order 573939. I've attached them along with their problem xmls.

I've exported the Cantor orders via Transfer -> Export Orders/Quotations. Let me know if that is the correct method, or if you'd like me to export the orders in another way.

In regards to how the xml is generated, we take the glass purchase order related to a manufacturing job, and create a Collective Purchase Order. Then, we go to External Interfaces -> A=W Glass Order XML to create the xml. Let me know if you'd like me to try another way.

We appreciate you forwarding this ticket to the R&D department. Please feel free to let me know if you or your team have any further questions for us.

Thank you and have a good rest of your week!

-Ethan

From: Support Cantor US …
```

</details>

---

### [AW-230928] — xRechnung Validation Error

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-230928]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Cantor - 2nd Level |
| **Last Action** | 23.07.2025 11:34 |

**Description:**

> RE: [EXTERN] AW: AW: [AW-230928] Datenbank Collation (66) Hallo Herr Esswein, das Update-Package für die 7.8 liegt auf dem FTP server. V_7_8_Unicode_Build_2023_1_0_85_Date_23_07_2025__11_27_29.zip Mit freundlichen Grüßen | Best regards Stefan Rixecker ###EOM## Phone:  +49 641 96620 393 A+W Software GmbH Siemensstraße 3 35463 Fernwald Germany www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan Amtsgericht Gießen/Gießen Local Cou...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Stefan Rixecker (support.cantor.de@a-w.com)
To: Philipp.Esswein@heka.de | Date: 23.07.2025 11:34
Type: Answer | 
RE: [EXTERN] AW: AW: [AW-230928] Datenbank Collation (66)
Hallo Herr Esswein,
das Update-Package für die 7.8 liegt auf dem FTP server.
V_7_8_Unicode_Build_2023_1_0_85_Date_23_07_2025__11_27_29.zip
Mit freundlichen Grüßen | Best regards
Stefan Rixecker
###EOM##

Phone:  +49 641 96620 393
 
A+W Software GmbH
Siemensstraße 3
35463 Fernwald
Germany

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus in Ihr System gelangen, haften wir nicht f…
```

</details>

---

## Support Fernwald - Cantor

### [AW-237463] — Workshop Mandantentrennung ACTUAL - nachträgliche Frage

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-237463]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 25.07.2025 16:38 |

**Description:**

> AW: [AW-237463] Workshop Mandantentrennung ACTUAL - nachträgliche Frage (30) Hallo Herr Tuider, Anlage eines weiteren Mandanten sowie Anlage von Produktionslinie(n) für Kosmos sollten problemlos möglich sein. Setzen der im Anhang genannten Konfigurationen („prodconfs“) sollte man, wie Sie beschrieben haben, zunächst ausklammern. Ich werde von 22.08. bis 12.09. im Urlaub sein. Eventuelle Abstimmungstermine können wir entweder direkt im Anschluss an Ihren Urlaub (KW34) oder dann erst ab KW 38 plan...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Wolfgang Schmid (Wolfgang.Schmid@a-w.com)
To: Harald.Tuider@actual.at, support.cantor.de@a-w.com | Date: 25.07.2025 16:38
Type: Request | 
AW: [AW-237463] Workshop Mandantentrennung ACTUAL - nachträgliche Frage (30)
Hallo Herr Tuider,
Anlage eines weiteren Mandanten sowie Anlage von Produktionslinie(n) für Kosmos sollten problemlos möglich sein.
 
Setzen der im Anhang genannten Konfigurationen („prodconfs“) sollte man, wie Sie beschrieben haben, zunächst ausklammern.
 
Ich werde von 22.08. bis 12.09. im Urlaub sein. Eventuelle Abstimmungstermine können wir entweder direkt im Anschluss an Ihren Urlaub (KW34) oder dann erst ab KW 38 planen.
 
Mit freundlichen Grüßen | Best regards
 
Wolfgang Schmid
Senior Consultant
A+W Cantor
 

 
Mobile:+49 160 7191258
Email: wolfgang.schmid@a-w.com
 
A+W Software GmbH
Siemensstraße 3
35463 Fernwald
Germany
 
www.a-w.com

 

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963

This e-mail is for the intended recipient only and may contain confidential and/or legally protected information. If you have received it by mistake pl…
```

</details>

---

### [AW-236819] — GROßER FEHLER Drucksteuerung

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-236819]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 25.07.2025 15:53 |

**Description:**

> FW: RE: [AW-236819] GROßER FEHLER Drucksteuerung (6) Hallo Herr Reuter, leider habe ich hier bisher keine Rückmeldung erhalten. Wurde der Tigger umgesetzt , so dass es nähere Informationen gibt, wann Daten verschwinden? Mit freundlichen Grüßen | Best regards Sabine Weidmann ###EOM## Phone:  +49 641 96620 393 Mobile:  +49 6404 2051 362 A+W Software GmbH Siemensstraße 3 35463 Fernwald Germany www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson,...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Sabine Weidmann (support.cantor.de@a-w.com)
To: M.Reuter@rekord.de | Date: 25.07.2025 15:53
Type: Answer | 
FW: RE: [AW-236819] GROßER FEHLER Drucksteuerung (6)
Hallo Herr Reuter,
leider habe ich hier bisher keine Rückmeldung erhalten.
Wurde der Tigger umgesetzt , so dass es nähere Informationen gibt, wann Daten verschwinden?
 
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
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotz…
```

</details>

---

### [AW-238187] — CIM: Musternummer am Bildschirmarbeitsplatz

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-238187]` |
| **Status** | 🟡 New |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 25.07.2025 15:48 |

**Description:**

> CIM: Musternummer am Bildschirmarbeitsplatz (2) Hallo, bitte nochmal Unterstützung bei der optimierten Übergabe Mit freundlichen Grüßen Arne Windscheid EDV/IT Bornemann GmbH & Co. KG Mergenthalerstraße 39 48268 Greven Mobil:      01511 2736842 E-Mail:     arne.windscheid@bornemann-rollladen.de<mailto:arne.windscheid@bornemann-rollladen.de> Internet:  http://www.bornemann-rollladen.de<http://www.bornemann-rollladen.de/> Kommanditgesellschaft Amtsgericht Steinfurt HRA 4807 Geschäftsführer: Christi...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Arne Windscheid (arne.windscheid@bornemann-rollladen.de)
To: support.cantor.de@a-w.com | Date: 25.07.2025 15:48
Type: Request | 
CIM: Musternummer am Bildschirmarbeitsplatz (2)
Hallo,

bitte nochmal Unterstützung bei der optimierten Übergabe

Mit freundlichen Grüßen

Arne Windscheid
EDV/IT

Bornemann GmbH & Co. KG
Mergenthalerstraße 39
48268 Greven

Mobil:      01511 2736842
E-Mail:     arne.windscheid@bornemann-rollladen.de<mailto:arne.windscheid@bornemann-rollladen.de>
Internet:  http://www.bornemann-rollladen.de<http://www.bornemann-rollladen.de/>

Kommanditgesellschaft Amtsgericht Steinfurt HRA 4807
Geschäftsführer: Christian Baur
Pers. haftende Gesellschafterin: Bornemann Verwaltungs GmbH,
Sitz Greven, Amtsgericht Steinfurt, HRB 6603
USt-Id Nr.: DE 207189570 · Steuer-Nr. 327/5768/3058

Informationen dazu, wie wir Ihre personenbezogenen Daten verar-
beiten und Ihre Rechte finden Sie in unserer Datenschutzerklärung:
www.bornemann-rollladen.de/informationspflicht<http://www.bornemann-rollladen.de/informationspflicht>
```

</details>

---

### [AW-238164] — Change settings for order totals

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-238164]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 25.07.2025 15:48 |

**Description:**

> RE: [AW-238164] Change settings for order totals (8) Hello Jorrit, as I have already written, this area is not configurable. If you would like to have more lines here, that would be a new request. Mit freundlichen Grüßen | Best regards Sabine Weidmann ###EOM## Phone:  +49 641 96620 393 Mobile:  +49 6404 2051 362 A+W Software GmbH Siemensstraße 3 35463 Fernwald Germany www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan Amtsgeri...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Sabine Weidmann (support.cantor.de@a-w.com)
To: jbakker@ploegkozijnen.nl | Date: 25.07.2025 15:48
Type: Answer | 
RE: [AW-238164] Change settings for order totals (8)
Hello Jorrit,
as I have already written, this area is not configurable.
If you would like to have more lines here, that would be a new request.
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
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus in Ihr Syste…
```

</details>

---

### [AW-238157] — Wareneingang Glas über CIM buchen

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-238157]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 25.07.2025 15:29 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Stefan Rixecker
To: Dirk Horn | Date: 25.07.2025 15:29
Type: State changed | 
RE: [AW-238157] Wareneingang Glas über CIM buchen (3)
DH
```

</details>

---

### [AW-238176] — OpenTrans, Bestätigung und Lieferschein importieren

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-238176]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 25.07.2025 15:02 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Sabine Weidmann
To: Sabine Weidmann | Date: 25.07.2025 15:02
Type: State changed | 
RE: [AW-238176] OpenTrans, Bestätigung und Lieferschein importieren (3)
SWE
```

</details>

---

### [AW-235774] — Reportdefinition 1000 - Druckdaten

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-235774]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 25.07.2025 14:30 |

**Description:**

> AW: [AW-235774] Reportdefinition 1000 - Druckdaten (33) Hallo Herr Fischer, ich habe versucht ein Beispiel zu erstellen, bei dem ich negative Beträge bekommen. Leider ist es mir nicht gelungen. Was muss ich tun oder können Sie mir eine Beispiel zur Verfügung, damit ich das im Report abbilden kann. Mit freundlichen Grüßen | Best regards Sabine Weidmann ###EOM## Phone:  +49 641 96620 393 Mobile:  +49 6404 2051 362 A+W Software GmbH Siemensstraße 3 35463 Fernwald Germany www.a-w.com Geschäftsführer...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Sabine Weidmann (support.cantor.de@a-w.com)
To: mfischer@tmp-fenster.de | Date: 25.07.2025 14:30
Type: Answer | 
AW: [AW-235774] Reportdefinition 1000 - Druckdaten (33)
Hallo Herr Fischer,
ich habe versucht ein Beispiel zu erstellen, bei dem ich negative Beträge bekommen. Leider ist es mir nicht gelungen.
Was muss ich tun oder können Sie mir eine Beispiel zur Verfügung, damit ich das im Report abbilden kann. 
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
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwe…
```

</details>

---

### [AW-234729] — verschiedene Kalkulationsarten MT Version

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-234729]` |
| **Status** | 🔵 In Progress |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 25.07.2025 13:07 |

**Description:**

> AW: [AW-234729] verschiedene Kalkulationsarten MT Version (11) Sehr geehrte Frau  Heyd, das ist denke nicht das was ich meine. Andere / weiterführende Informationen. Der Kunde x hat eine Händlerversion (Standalone) aus diesem sendet er mir nachfolgende Info aus dem Kalkulationsdialog: In der MT-Version vom Kunden, in der er ab Montag arbeiten möchte, fehlt ihm die Spalte manR und wenn man in der Spalte % der Unterordnung Handelsspanne einen Wert eingibt, wird dieser beim Wechsle wieder auf den U...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Stephan Kalbitz (S.Kalbitz@dth-tiemann.de)
To: support.cantor.de@a-w.com | Date: 25.07.2025 13:07
Type: Request | 
AW: [AW-234729] verschiedene Kalkulationsarten MT Version (11)
Sehr geehrte Frau  Heyd,

das ist denke nicht das was ich meine.

Andere / weiterführende Informationen.

Der Kunde x hat eine Händlerversion (Standalone) aus diesem sendet er mir nachfolgende Info aus dem Kalkulationsdialog:

In der MT-Version vom Kunden, in der er ab Montag arbeiten möchte, fehlt ihm die Spalte manR und wenn man in der Spalte % der Unterordnung Handelsspanne einen Wert eingibt, wird dieser beim Wechsle wieder auf den Ursprungswert eingetragen.

Damit ich nun dies erreichen kann, welche Option muss ich ziehen, oder einstellen sodass der Kunde wieder so arbeiten kann wie in seiner bisherigen Händler (Standalone)-Version?

Gibt es für diese ggf. noch ein prod / handconf Eintrag den ich umstellen muss? Wenn ja welche Auswirkungen im System hat diese Umstellung dann noch außer die Eintragung in der Kalkulationsmaske?

Mit freundlichen Grüßen aus Hille

Stephan Kalbitz
IT Appl…
```

</details>

---

### [AW-223307] — BE Update Routine 7.7 - 7.9 mit Umstieg auf SQL Server 2019

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-223307]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 25.07.2025 12:28 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Kerstin Heyd
To: Kerstin Heyd | Date: 25.07.2025 12:28
Type: State changed | 
RE: [AW-223307] BE Update Routine 7.7 - 7.9 mit Umstieg auf SQL Server 2019 (40)
Test Startup Aktion 9 mit und ohne Parameter 3 - Reports werden nicht aktualisiert
```

</details>

---

### [AW-238118] — Warten auf Zweitwerk

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-238118]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 25.07.2025 12:04 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Sascha Hermann
To: Dirk Horn | Date: 25.07.2025 12:04
Type: State changed | 
RE: [AW-238118] Warten auf Zweitwerk (3)
DH
```

</details>

---

### [AW-237996] — unklare Preise in Rabatte Kalulation

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-237996]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 25.07.2025 11:57 |

**Description:**

> RE: Antwort: RE: Antwort: RE: Antwort: RE: Antwort: RE: [AW-237996] unklare Preise in Rabatte Kalulation (14) Hallo Herr Otto, gibt es ein konkretes Beispiel, wo ein Preis bei' unabhängig' nicht ermittelt wird? Im Preisberechnungstrace sieht man in der Regel, das alle Varianten geprüft werden. Da Sie die bidirektionale Preisberechnung offensichtlich nicht kannten und daher nicht bewusst nutzten, warum schalten Sie diese nicht aus? Dann müssen keine Preise nachgepflegt werden. CODE: 149 ENTRY: =0...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Sabine Weidmann (support.cantor.de@a-w.com)
To: p.otto@pax.de | Date: 25.07.2025 11:57
Type: Answer | 
RE: Antwort: RE: Antwort: RE: Antwort: RE: Antwort: RE: [AW-237996] unklare Preise in Rabatte Kalulation (14)
Hallo Herr Otto,
gibt es ein konkretes Beispiel, wo ein Preis bei' unabhängig' nicht ermittelt wird?
Im Preisberechnungstrace sieht man in der Regel, das alle Varianten geprüft werden.
Da Sie die bidirektionale Preisberechnung offensichtlich nicht kannten und daher nicht bewusst nutzten, warum schalten Sie diese nicht aus? Dann müssen keine Preise nachgepflegt werden.

CODE: 149 
ENTRY: =0/1
DESCRIPTION: Aktiviert die Bidirektionale Preisberechnung in der Auftrags- und Bestellauftragserfassung. 
Gilt für Technik-Artikel, die auch in der Mawi erfasst sind (Lagerteile). 
Wird im Hauptbereich (VK - Technik, EK - Mawi) kein Preis gefunden, wird jeweils der Preis aus dem anderen Bereich gesucht. 
 
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

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs,…
```

</details>

---

### [AW-237803] — Cantor Wiki Suche funktioniert nicht

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-237803]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 25.07.2025 11:53 |

**Description:**

> RE: [AW-237803] Website Suche ohne Funktion (5) Hallo Herr Scholz, die Suche im Cantor Wiki sollte jetzt wieder funktionieren. Mit freundlichen Grüßen | Best regards Kerstin Heyd ###EOM## Phone:  +49 641 96620 393 Mobile:  +49 641 96620-363 A+W Software GmbH Siemensstraße 3 35463 Fernwald Germany www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan Amtsgericht Gießen/Gießen Local Court: HRB 7963 Diese E-Mail ist ausschließlich f...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Kerstin Heyd (support.cantor.de@a-w.com)
To: c.scholz@pax.de | Date: 25.07.2025 11:53
Type: Answer | 
RE: [AW-237803] Website Suche ohne Funktion (5)
Hallo Herr Scholz,
die Suche im Cantor Wiki sollte jetzt wieder funktionieren.
Mit freundlichen Grüßen | Best regards
Kerstin Heyd
###EOM##

Phone:  +49 641 96620 393
Mobile:  +49 641 96620-363
A+W Software GmbH
Siemensstraße 3
35463 Fernwald
Germany

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus in Ihr System gelangen, haften wir nicht für die evtl. entstandenen Schäden.

T…
```

</details>

---

### [AW-229431] — Cantor Wiki Suche funktioniert nicht

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-229431]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 25.07.2025 11:52 |

**Description:**

> RE: [AW-229431] Cantor Wiki Suche funktioniert nicht (6) Hallo Herr Bonniksen, die Suche im Cantor Wiki sollte jetzt wieder funktionieren. Könnten Sie es bitte einmal testen. Mit freundlichen Grüßen | Best regards Kerstin Heyd ###EOM## Phone:  +49 641 96620 393 A+W Software GmbH Siemensstraße 3 35463 Fernwald Germany www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan Amtsgericht Gießen/Gießen Local Court: HRB 7963 Diese E-Mail...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Kerstin Heyd (support.cantor.de@a-w.com)
To: p.bonniksen@dth-tiemann.de | Date: 25.07.2025 11:52
Type: Answer | 
RE: [AW-229431] Cantor Wiki Suche funktioniert nicht (6)
Hallo Herr Bonniksen,
die Suche im Cantor Wiki sollte jetzt wieder funktionieren. Könnten Sie es bitte einmal testen.
Mit freundlichen Grüßen | Best regards
Kerstin Heyd
###EOM##

Phone:  +49 641 96620 393
 
A+W Software GmbH
Siemensstraße 3
35463 Fernwald
Germany

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus in Ihr System gelangen, haften wir nicht für die evtl. entstandenen…
```

</details>

---

### [AW-228036] — Cantor WIKI Suche funktioniert nicht

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-228036]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 25.07.2025 11:49 |

**Description:**

> AW: [AW-228036] Cantor WIKI suchen (15) Hallo Herr Sönksen, der Entwickler hat eine weitere Anpassung vorgenommen. Jetzt sollte die Suche funktionieren (bei mir jedenfalls klappt es). Könnten Sie es bitte auch noch einmal testen. Vielen Dank Mit freundlichen Grüßen | Best regards Kerstin Heyd ###EOM## Phone:  +49 641 96620 393 A+W Software GmbH Siemensstraße 3 35463 Fernwald Germany www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Kerstin Heyd (support.cantor.de@a-w.com)
To: thorben.soenksen@aldra.de | Date: 25.07.2025 11:49
Type: Answer | 
AW: [AW-228036] Cantor WIKI suchen (15)
Hallo Herr Sönksen,
der Entwickler hat eine weitere Anpassung vorgenommen. Jetzt sollte die Suche funktionieren (bei mir jedenfalls klappt es).
Könnten Sie es bitte auch noch einmal testen.
Vielen Dank
Mit freundlichen Grüßen | Best regards
Kerstin Heyd
###EOM##

Phone:  +49 641 96620 393
 
A+W Software GmbH
Siemensstraße 3
35463 Fernwald
Germany

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail …
```

</details>

---

### [AW-237419] — ODBC-Fehlermeldung beim Start der MultiTrade-Testumgebung (Windows-Authentifizierung)

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-237419]` |
| **Status** | 🔵 In Progress |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 25.07.2025 11:19 |

**Description:**

> AW: [AW-237419] ODBC-Fehlermeldung beim Start der MultiTrade-Testumgebung (Windows-Authentifizierung) (7) Hallo Frau Heyd, ja, aber warum? Datenbank und CANTOR-INI sind 1:1 gleich!  Der Start der Anwendung als Supervisor funktioniert. Der Start über die rdp als Standard-User nicht. Mit freundlichen Grüßen Frank Grewe Staatl. geprüfter Techniker Holzverarbeitung u. Betriebstechnik IT-Abteilung ERP-Systemadministrator Tel.: +49 (2762) 9866-120 Fenster Türen Fassaden Hoffmann GmbH & Co. KG Fax: +49...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Frank Grewe (F.Grewe@fenster-hoffmann.de)
To: support.cantor.de@a-w.com | Date: 25.07.2025 11:19
Type: Request | 
AW: [AW-237419] ODBC-Fehlermeldung beim Start der MultiTrade-Testumgebung (Windows-Authentifizierung) (7)
Hallo Frau Heyd,

ja, aber warum?

Datenbank und CANTOR-INI sind 1:1 gleich!  Der Start der Anwendung als Supervisor funktioniert. Der Start über die rdp als Standard-User nicht.

Mit freundlichen Grüßen

Frank Grewe

Staatl. geprüfter Techniker Holzverarbeitung u. Betriebstechnik

IT-Abteilung
ERP-Systemadministrator

Tel.:

+49 (2762) 9866-120

Fenster Türen Fassaden
Hoffmann GmbH & Co. KG

Fax:

+49 (2762) 9866-2005

Mobil:

E-Mail:

f.grewe@fenster-hoffmann.de<mailto:f.grewe@fenster-hoffmann.de>

Nicolaus-Otto-Str. 8, 57462 Olpe

Web:

https://www.fenster-hoffmann.de

<https://www.instagram.com/fensterhoffmann/>

<https://de-de.facebook.com/fenster.hoffmann/>

Geschäftsführer: Jens Hoffmann, Andreas Hoffmann
Fenster Türen Fassaden HOFFMANN GmbH & Co. KG, Amtsgericht Siegen HRA 7514
Komple…
```

</details>

---

### [AW-227390] — Re: [JT#2025041510000613] CANTOR - Spooler AppCrash | Schlange 100 - Technische Analyse

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-227390]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 25.07.2025 11:17 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Markus Bechthold
To: Stefan Rixecker | Date: 25.07.2025 11:17
Type: State changed | 
RE: [AW-227390] Re: [JT#2025041510000613] CANTOR - Spooler AppCrash | Schlange 100 - Technische Analyse (48)
analysis/clarification/test with SK + SR
```

</details>

---

### [AW-237989] — Fehler beim Schreiben ins Belegarchiv

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-237989]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 25.07.2025 10:40 |

**Description:**

> AW: [AW-237989] Fehler beim Schreiben ins Belegarchiv (8) Hallo Frau Saathoff, das hat bei mir funktioniert. Könnten Sie bitte folgendes Trace aktivieren und mir die CaTraceU.txt zukommen wenn der Fehler wieder aufgetreten ist. Vielen Dank Mit freundlichen Grüßen | Best regards Sascha Hermann ###EOM## Phone:  +49 641 96620 393 Mobile:  +49 6404 2051 361 A+W Software GmbH Siemensstraße 3 35463 Fernwald Germany www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Ti...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Sascha Hermann (support.cantor.de@a-w.com)
To: ssaathoff@pollmann-renken.de | Date: 25.07.2025 10:40
Type: Answer | 
AW: [AW-237989] Fehler beim Schreiben ins Belegarchiv (8)
Hallo Frau Saathoff,
das hat bei mir funktioniert.
Könnten Sie bitte folgendes Trace aktivieren und mir die CaTraceU.txt zukommen wenn der Fehler wieder aufgetreten ist.

Vielen Dank
 
Mit freundlichen Grüßen | Best regards
Sascha Hermann
###EOM##

Phone:  +49 641 96620 393
Mobile:  +49 6404 2051 361
A+W Software GmbH
Siemensstraße 3
35463 Fernwald
Germany

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung di…
```

</details>

---

### [AW-233812] — Lagerlänge < Zuschnittslänge Artikel in Zubehörsäge

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-233812]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 25.07.2025 10:31 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Sascha Hermann
To: Dirk Horn | Date: 25.07.2025 10:31
Type: State changed | 
RE: [AW-233812] Lagerlänge < Zuschnittslänge Artikel in Zubehörsäge (31)
Für mich hört sich das an wie ein Logikfehler. Wie kann man dann etwas zuschneiden was länger als die Lagerlänge ist?
Man müsste das Profil in zwei Stücke aufteilen können (Lagerlänge und Restlänge).
```

</details>

---

### [AW-216857] — Planvorgänge werden zurückgesetzt

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-216857]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 25.07.2025 10:09 |

**Description:**

> FW: [AW-216857] Planvorgänge werden zurückgesetzt (32) Hallo Frau Hauf, ja passt. mit freundlichen Grüßen. Stefan Rixecker Angesetzt für Mi 30.07.  von 13-14 Uhr Mit Frau Hauf / Fa. Schock ________________________________________________________________________________ Microsoft Teams Benötigen Sie Hilfe? Jetzt an der Besprechung teilnehmen Besprechungs-ID: 352 417 785 738 1 Kennung: T2Zu6dg6 Für Organisatoren: Besprechungsoptionen ________________________________________________________________...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Stefan Rixecker (support.cantor.de@a-w.com)
To: marina.hauf@schock-fensterwerk.de | Date: 25.07.2025 10:09
Type: Answer | 
FW: [AW-216857] Planvorgänge werden zurückgesetzt (32)
Hallo Frau Hauf, ja passt.
mit freundlichen Grüßen. Stefan Rixecker
 Angesetzt für Mi 30.07.  von 13-14 Uhr
Mit Frau Hauf / Fa. Schock
________________________________________________________________________________

Microsoft Teams Benötigen Sie Hilfe?

Jetzt an der Besprechung teilnehmen

Besprechungs-ID: 352 417 785 738 1

Kennung: T2Zu6dg6

Für Organisatoren: Besprechungsoptionen

________________________________________________________________________________

 

Mit freundlichen Grüßen | Best regards
Stefan Rixecker
###EOM##
​
Phone:  +49 641 96620 393
Mobile:  +4964196620-0
A+W Software GmbH
Siemensstraße 3
35463 Fernwald
Germany

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. So…
```

</details>

---

### [AW-236992] — Auftragsnummer bei Versandetikett teilweise falsch

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-236992]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 25.07.2025 10:07 |

**Description:**

> Automatische Antwort: [EXT] AW: [EXT] RE: [AW-236992] Auftragsnummer bei Versandetikett teilweise falsch (9) ﻿ Sehr geehrte Damen und Herren, ich bin ich derzeit leider nicht im Büro. Ihre Emails werden nicht weitergeleitet. Mein Posteingang wird nach meiner Rückkehr am 28.07.2025 wieder bearbeitet. Freundliche Grüße Michael Kohlbacher Mit freundlichen Grüßen / With best regards Michael Kohlbacher Stammdaten Gaulhofer Industrie-Holding GmbH T: +433125282211145 Am Gewerbegrund 2 | 8124 Übelbach M...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Michael Kohlbacher (michael.kohlbacher@gaulhofer.com)
To: support.cantor.de@a-w.com | Date: 25.07.2025 10:07
Type: Request | 
Automatische Antwort: [EXT] AW: [EXT] RE: [AW-236992] Auftragsnummer bei Versandetikett teilweise falsch (9)
﻿

Sehr geehrte Damen und Herren,

ich bin ich derzeit leider nicht im Büro. Ihre Emails werden nicht weitergeleitet. Mein Posteingang wird nach meiner Rückkehr am 28.07.2025 wieder bearbeitet.

Freundliche Grüße

Michael Kohlbacher

                
Mit freundlichen Grüßen / With best regards

Michael Kohlbacher
Stammdaten

               Gaulhofer Industrie-Holding GmbH
T: +433125282211145
               Am Gewerbegrund 2 | 8124 Übelbach
M: +436649638730
E: Michael.Kohlbacher@gaulhofer.com
        <https://www.facebook.com/Gaulhofer.Fenster>     <https://www.instagram.com/gaulhofer.fenster>   <https://www.pinterest.at/gaulhoferfenster>     <https://www.linked…
```

</details>

---

### [AW-237979] — Darstellung CIM AP

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-237979]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 25.07.2025 09:46 |

**Description:**

> AW: [AW-237979] Darstellung CIM AP (7) wie geschrieben, können Sie die Systematik auch auf die letzten zwei Stellen ausweiten, dann ist die Chance hierfür sehr gering. Eine andere Alternative als die bedingte Formatierung der Farben gibt es hier leider nicht. Mit freundlichen Grüßen | Best regards Stefan Rixecker ###EOM## Phone:  +49 641 96620 393 Mobile:  +4964196620-0 A+W Software GmbH Siemensstraße 3 35463 Fernwald Germany www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia S...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Stefan Rixecker (support.cantor.de@a-w.com)
To: arne.windscheid@bornemann-rollladen.de | Date: 25.07.2025 09:46
Type: Answer | 
AW: [AW-237979] Darstellung CIM AP (7)
wie geschrieben, können Sie die Systematik auch auf die letzten zwei Stellen ausweiten, dann ist die Chance hierfür sehr gering.
Eine andere Alternative als die bedingte Formatierung der Farben gibt es hier leider nicht.
Mit freundlichen Grüßen | Best regards
Stefan Rixecker
###EOM##

Phone:  +49 641 96620 393
Mobile:  +4964196620-0
A+W Software GmbH
Siemensstraße 3
35463 Fernwald
Germany

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogram…
```

</details>

---

### [AW-238092] — Cim Linker Titel Text

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-238092]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 25.07.2025 08:40 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Sascha Hermann
To: Angelique Jäckel | Date: 25.07.2025 08:40
Type: State changed | 
RE: [AW-238092] Cim Linker Titel Text (3)
AJ
```

</details>

---

### [AW-230943] — FWD: "Problem", "Fehler" -  Cantor - Filter - offener Pool [Ticket#8014661]

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-230943]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 25.07.2025 08:26 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Sascha Hermann
To: Angelique Jäckel | Date: 25.07.2025 08:26
Type: State changed | 
RE: [AW-230943] FWD: "Problem", "Fehler" -  Cantor - Filter - offener Pool [Ticket#8014661] (17)
AJ
```

</details>

---

### [AW-237154] — Systemmeldung "Verarbeitung SER Archivierung" beim Rechnungsdruck – Bitte um Klärung und Lösungsansatz

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-237154]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 25.07.2025 08:23 |

**Description:**

> AW: [AW-237154] Systemmeldung "Verarbeitung SER Archivierung" beim Rechnungsdruck – Bitte um Klärung und Lösungsansatz (15) Hallo Frank, mir fehlt noch zwei Antworten? Ist die Datei tatsächlich nicht da und existieren alle betroffenen Pfade. Kannst Du bitte folgendes Trace aktivieren: Ich hab´s nochmal ausprobiert, hier läuft es: Mit freundlichen Grüßen | Best regards Sascha Hermann ###EOM## Phone:  +49 641 96620 393 Mobile:  +49 6404 2051 361 A+W Software GmbH Siemensstraße 3 35463 Fernwald Ger...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Sascha Hermann (support.cantor.de@a-w.com)
To: F.Grewe@fenster-hoffmann.de | Date: 25.07.2025 08:23
Type: Answer | 
AW: [AW-237154] Systemmeldung "Verarbeitung SER Archivierung" beim Rechnungsdruck – Bitte um Klärung und Lösungsansatz (15)
Hallo Frank,
mir fehlt noch zwei Antworten?
Ist die Datei tatsächlich nicht da und existieren alle betroffenen Pfade.
Kannst Du bitte folgendes Trace aktivieren:

Ich hab´s nochmal ausprobiert, hier läuft es:

Mit freundlichen Grüßen | Best regards
Sascha Hermann
###EOM##

Phone:  +49 641 96620 393
Mobile:  +49 6404 2051 361
A+W Software GmbH
Siemensstraße 3
35463 Fernwald
Germany

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme.…
```

</details>

---

### [AW-238084] — Feld „Statusinfo“ (Pflichtfeld) automatisch füllen

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-238084]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 25.07.2025 08:10 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Sascha Hermann
To: Sascha Hermann | Date: 25.07.2025 08:10
Type: State changed | 
RE: [AW-238084] Feld „Statusinfo“ (Pflichtfeld) automatisch füllen (3)
Warten auf Rückmeldung
```

</details>

---

### [AW-238081] — Systemmeldungen "Details zum Fehler siehe Bereich 'OP_TR'"

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-238081]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 25.07.2025 07:46 |

**Description:**

> RE: [AW-238081] Systemmeldungen "Details zum Fehler siehe Bereich 'OP_TR'" (4) Guten Morgen Frank, Details findest du ebenfalls in der Historie im Abschnitt OP_TR. Gleiche Uhrzeit, wie dieser Fehler. Bei openTrans werden die Fehler leider in 2 unterschiedliche Bereich der Systemhistorie geschrieben. Mit freundlichen Grüßen | Best regards Sabine Weidmann ###EOM## Phone:  +49 641 96620 393 Mobile:  +49 6404 2051 362 A+W Software GmbH Siemensstraße 3 35463 Fernwald Germany www.a-w.com Geschäftsführ...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Sabine Weidmann (support.cantor.de@a-w.com)
To: F.Grewe@fenster-hoffmann.de | Date: 25.07.2025 07:46
Type: Answer | 
RE: [AW-238081] Systemmeldungen "Details zum Fehler siehe Bereich 'OP_TR'" (4)
Guten Morgen Frank,
Details findest du ebenfalls in der Historie im Abschnitt OP_TR. Gleiche Uhrzeit, wie dieser Fehler.
Bei openTrans werden die Fehler leider in 2 unterschiedliche Bereich der Systemhistorie geschrieben.
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
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzp…
```

</details>

---

### [AW-238048] — ProductCamp 22.08.2025

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-238048]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 24.07.2025 17:34 |

**Description:**

> RE: [AW-238048] ProductCamp 22.08.2025 (2) Hallo Herr Kilic, es geht um den angesprochenen Vortrag. Wären Sie so nett und könnten mir Ihren aktuellen WebShopContentGen Ordner, mit den aufbereiteten Grafiken für iQuote auf den FTP laden? Recht herzlichen Dank! Mit freundlichen Grüßen | Best regards Stefan Rixecker ###EOM## Phone:  +49 641 96620 393 Mobile:  +4964196620-0 A+W Software GmbH Siemensstraße 3 35463 Fernwald Germany www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia S...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Stefan Rixecker (support.cantor.de@a-w.com)
To: yunus.kilic@schlotterer.at | Date: 24.07.2025 17:34
Type: Answer | 
RE: [AW-238048] ProductCamp 22.08.2025 (2)
Hallo Herr Kilic,
es geht um den angesprochenen Vortrag. Wären Sie so nett und könnten mir Ihren aktuellen WebShopContentGen Ordner, mit den aufbereiteten Grafiken für iQuote auf den FTP laden? 

Recht herzlichen Dank!
Mit freundlichen Grüßen | Best regards
Stefan Rixecker
###EOM##

Phone:  +49 641 96620 393
Mobile:  +4964196620-0
A+W Software GmbH
Siemensstraße 3
35463 Fernwald
Germany

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogram…
```

</details>

---

### [AW-237430] — Fehlermeldung - Übertragung an Mandant nicht möglich

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-237430]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 24.07.2025 16:26 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Kerstin Heyd
To: Kerstin Heyd | Date: 24.07.2025 16:26
Type: State changed | 
RE: [AW-237430] Fehlermeldung - Übertragung an Mandant nicht möglich (4)
Recherche
```

</details>

---

### [AW-235359] — Prüfen ob Produkttyp des Zubehörartikels gültig für Produkttyp des Elements ist

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-235359]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 24.07.2025 15:58 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Sascha Hermann
To: Angelique Jäckel | Date: 24.07.2025 15:58
Type: State changed | 
RE: [AW-235359] Prüfen ob Produkttyp des Zubehörartikels gültig für Produkttyp des Elements ist (7)
AJ
```

</details>

---

### [AW-237772] — [EXTERN] Teilrechnung wird nicht auf Schlussrechnung berücksichtigt

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-237772]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 24.07.2025 15:50 |

**Description:**

> RE: [AW-237772] [EXTERN] Teilrechnung wird nicht auf Schlussrechnung berücksichtigt (4) Hallo Frau Hauf, in genannten Beispiel handelt es sich nicht um eine Abschlagsrechnung (Typ AR), sondern um eine Teilrechnung (Typ N). Diese ist storniert, korrekt, gilt aber nicht als Abschlagsrechnung und wird daher auch nicht im Feld DR_ABSCHLAGBRUTTO ausgegeben. Sondern nur in der Zusammenfassung aller Rechnungen unter dem Summenblock. Ich würde hier leider wieder das konkrete Beispiel benötigen. Ich habe...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Sabine Weidmann (support.cantor.de@a-w.com)
To: Marina.Hauf@schock-fensterwerk.de | Date: 24.07.2025 15:50
Type: Answer | 
RE: [AW-237772] [EXTERN] Teilrechnung wird nicht auf Schlussrechnung berücksichtigt (4)
Hallo Frau Hauf,
in genannten Beispiel handelt es sich nicht um eine Abschlagsrechnung (Typ AR), sondern um eine Teilrechnung (Typ N). Diese ist storniert, korrekt, gilt aber nicht als Abschlagsrechnung und wird daher auch nicht im Feld DR_ABSCHLAGBRUTTO ausgegeben. Sondern nur in der Zusammenfassung aller Rechnungen unter dem Summenblock. 
Ich würde hier leider wieder das konkrete Beispiel benötigen.

Ich habe Ihnen die Doku zu den Rechnungen angehängt. Hier wurde versucht alle Konfigurationen und deren Auswirklungen zu beschreiben. Wenn Sie mal in die Doku reinschauen, sehen Sie, dass es sehr viele Konfigurationen gibt, die leider bei jedem unserer Kunden in  unterschiedlichen Kombination gesetzt sind, was einen Test nach eine Anpassung, in allen Kombinationen fast unmöglich macht. 
 
Mit freundlichen Grüßen | Best regards
Sabine Weidmann
###EOM##

Phone:  +49 641 96620 393
Mobile:  +49 6404 2051 362
A+W Software GmbH
Siemensstraße 3
35463 Fernwald
Germany

www.a-w…
```

</details>

---

### [AW-237946] — Meldung HTML-Tags bei Texten - Update auf 7.8

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-237946]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 24.07.2025 15:31 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Sascha Hermann
To: Stefan Rixecker | Date: 24.07.2025 15:31
Type: State changed | 
RE: [AW-237946] Meldung HTML-Tags bei Texten - Update auf 7.8 (8)
SR
```

</details>

---

### [AW-237833] — Fehlende Adressen

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-237833]` |
| **Status** | 🔵 In Progress |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 24.07.2025 14:49 |

**Description:**

> Antwort: RE: Antwort: RE: [AW-237833] Fehlende Adressen (7) Hallo, Strasser Michael hat anscheinend schon den gleichen Fehler bei Ihnen eingemeldet. Daher gehe ich davon aus, dass es nicht nur SAM Aufträge betrifft sondern auch andere Auftragstypen. Der Fehler ist Heute schon wieder mehrmals aufgetreten. Auftrag wird angelegt und nach dem einfügen den Debitorennummer kommt die Fehlermeldung. Schöne Grüße Florian Auer Key User Service Telefon: +43.7763.2241.1711 | Mobil: +43.664.8288419 E-Mail: f...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Florian Auer (florian.auer@josko.at)
To: support.cantor.de@a-w.com | Date: 24.07.2025 14:49
Type: Request | 
Antwort: RE: Antwort: RE: [AW-237833] Fehlende Adressen (7)
Hallo,

Strasser Michael hat anscheinend schon den gleichen Fehler bei Ihnen
eingemeldet.
Daher gehe ich davon aus, dass es nicht nur SAM Aufträge betrifft sondern
auch andere Auftragstypen.

Der Fehler ist Heute schon wieder mehrmals aufgetreten.
Auftrag wird angelegt und nach dem einfügen den Debitorennummer kommt die
Fehlermeldung.

Schöne Grüße

Florian Auer
Key User Service

Telefon: +43.7763.2241.1711 | Mobil: +43.664.8288419
E-Mail: florian.auer@josko.at

Josko Fenster und Türen GmbH
Josko-Straße 1 | A - 4770 Andorf

---------------------------------------------------------------------------------

Wir sind von 28.07. bis 08.08. (KW 31/32) im Betriebsurlaub.
Ab Montag dem 11.08. sind wir gerne wieder für Sie da.
---------------------------------------------------------------------------------

Firmenbuchnummer: 111546p | Firmenbuchgericht: Landesgericht Ried im
Innkreis | Firmensitz: Josko-Straße 1 | A - 4794 Kopfing | UID: ATU 239 15
4…
```

</details>

---

### [AW-237858] — WG: Druck Rechnung

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-237858]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 24.07.2025 12:09 |

**Description:**

> AW: [EXT] RE: [AW-237858] WG: Druck Rechnung (6) Hallo Frau Rogic, die Information wird im Kunden hinterlegt. Tabelle KUNDEN - Feld ANZAUSDRUCK Hier sind die Anzahl für alle Druck in einem Feld! z.B. für diesen Kunden ist der Inhalt von ANZAUSDRUCK=1113 Mit freundlichen Grüßen | Best regards Sabine Weidmann ###EOM## Phone:  +49 641 96620 393 Mobile:  +49 6404 2051 362 A+W Software GmbH Siemensstraße 3 35463 Fernwald Germany www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Sch...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Sabine Weidmann (support.cantor.de@a-w.com)
To: milica.rogic@gaulhofer.com | Date: 24.07.2025 12:09
Type: Answer | 
AW: [EXT] RE: [AW-237858] WG: Druck Rechnung (6)
Hallo Frau Rogic,
die Information wird im Kunden hinterlegt.
Tabelle KUNDEN - Feld ANZAUSDRUCK
Hier sind die Anzahl für alle Druck in einem Feld!
z.B. für diesen Kunden ist der Inhalt von ANZAUSDRUCK=1113

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
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sol…
```

</details>

---

### [AW-237981] — X-Rechnung und ZugPferd Rechnung aus Cantor fehlt Leistungsdatum

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-237981]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 24.07.2025 12:02 |

**Description:**

> RE: [AW-237981] X-Rechnung und ZugPferd Rechnung aus Cantor fehlt Leistungsdatum (4) Hallo Mario, das sind die Knoten BT-73 und BT-74. Diese können über einen Artikel (unter Auftragsinformationen) und die Umsetzungstabelle XRECHNUNG_ORDERINFO gefüllt werden. Format des Datum muss 20250720 sein. Über diesen Weg können alle noch fehlenden Knoten definiert werden. Doku findest du im Cantor-Wiki unter: A+W Cantor - Schnittstellen - XRechnung - Auftragsbezogene Informationen in der xRechnung Mit freu...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Sabine Weidmann (support.cantor.de@a-w.com)
To: m.markgraf@schmidt-boke.de | Date: 24.07.2025 12:02
Type: Answer | 
RE: [AW-237981] X-Rechnung und ZugPferd Rechnung aus Cantor fehlt Leistungsdatum (4)
Hallo Mario,
das sind die Knoten BT-73 und BT-74. Diese können über einen Artikel (unter Auftragsinformationen) und die Umsetzungstabelle XRECHNUNG_ORDERINFO gefüllt werden. Format des Datum muss 20250720 sein. Über diesen Weg können alle noch fehlenden Knoten definiert werden.

Doku findest du im Cantor-Wiki unter: A+W Cantor - Schnittstellen - XRechnung - Auftragsbezogene Informationen in der xRechnung
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
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in…
```

</details>

---

### [AW-237914] — GENIUS - Preisberechnung bei globalen Positionen

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-237914]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 24.07.2025 10:56 |

**Description:**

> RE: [AW-237914] GENIUS - Preisberechnung bei globalen Positionen (4) Hallo Herr Grasmäher, der PRODCONF hat keinen Einfluss auf die Preisberechnung. Die Ausprägung 3 bedeutet, dass globale Positionen sowohl für Aufträge, wie auch Bestellungen angelegt werden können. Bei Genius gibt es bei Einstellung 1 nur globale Positionen für Aufträge. Haben Sie die Preisberechnung mal getraced? Falls der Artikel auf der Rechnung fehlt, kann dies an der Prozeßsteuerung  liegen, hier muß 'Fakturierung' angehak...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Sabine Weidmann (support.cantor.de@a-w.com)
To: m.grasmaeher@grasmaeher-it.de | Date: 24.07.2025 10:56
Type: Answer | 
RE: [AW-237914] GENIUS - Preisberechnung bei globalen Positionen (4)
Hallo Herr Grasmäher,
der PRODCONF hat keinen Einfluss auf die Preisberechnung.
Die Ausprägung 3 bedeutet, dass globale Positionen sowohl für Aufträge, wie auch Bestellungen angelegt werden können. Bei Genius gibt es bei Einstellung 1 nur globale Positionen für Aufträge.
Haben Sie die Preisberechnung mal getraced?
Falls der Artikel auf der Rechnung fehlt, kann dies an der Prozeßsteuerung  liegen, hier muß 'Fakturierung' angehakt sein.
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
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein…
```

</details>

---

### [AW-234795] — Cantor CaMain trotz Umstellung der Anzeigesprache weiterhin auf Deutsch

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-234795]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 24.07.2025 10:54 |

**Description:**

> FW: RE: WG: [AW-234795] Cantor CaMain trotz Umstellung der Anzeigesprache weiterhin auf Deutsch (41) Hallo Herr Nestaval, mir ist noch etwas eingefallen: In neueren Versionen der Multitrade ist es möglich, in den Mandanten eine Anzeigesprache einzustellen. Vielleicht haben Sie das gemeint. Es gibt im Mandantendialog eine Checkbox für die Anzeigesprache: Damit sollte sowohl die Programmsprache umgestellt, als auch die Übersetzungen der Produkte angezeigt werden. Das ist dann ganz spezifisch nur f...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Kerstin Heyd (support.cantor.de@a-w.com)
To: horst.nestaval@schlotterer.at | Date: 24.07.2025 10:54
Type: Answer | 
FW: RE: WG: [AW-234795] Cantor CaMain trotz Umstellung der Anzeigesprache weiterhin auf Deutsch (41)
Hallo Herr Nestaval,
mir ist noch etwas eingefallen: In neueren Versionen der Multitrade ist es möglich, in den Mandanten eine Anzeigesprache einzustellen. Vielleicht haben Sie das gemeint.
Es gibt im Mandantendialog eine Checkbox für die Anzeigesprache:

Damit sollte sowohl die Programmsprache umgestellt, als auch die Übersetzungen der Produkte angezeigt werden.
Das ist dann ganz spezifisch nur für diesen Mandanten.
Wobei die bei den Mitarbeitern auch noch übersteuert werden kann:

 

 
Mit freundlichen Grüßen | Best regards
Kerstin Heyd
###EOM##

Phone:  +49 641 96620 393
Mobile:  +49 641 96620-363
A+W Software GmbH
Siemensstraße 3
35463 Fernwald
Germany

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalt…
```

</details>

---

### [AW-237742] — Falscher Eintrag innerhalb der Veka_Print-Tabelle

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-237742]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 24.07.2025 10:13 |

**Description:**

> RE: [AW-237742] Falscher Eintrag innerhalb der Veka_Print-Tabelle (4) Hallo Herr Wagner, wo definieren Sie die Tabelle? Könnte sie eine Screenshot aus den Report-Definitionen senden, der diese Tabelle zeigt? Im angehängten Report kann ich Sie ebenfalls nicht finden. Mit freundlichen Grüßen | Best regards Sabine Weidmann ###EOM## Phone:  +49 641 96620 393 Mobile:  +49 6404 2051 362 A+W Software GmbH Siemensstraße 3 35463 Fernwald Germany www.a-w.com Geschäftsführer/Managing Directors: Eric Herrma...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Sabine Weidmann (support.cantor.de@a-w.com)
To: twa@fenster-mueller.de | Date: 24.07.2025 10:13
Type: Answer | 
RE: [AW-237742] Falscher Eintrag innerhalb der Veka_Print-Tabelle (4)
Hallo Herr Wagner,
wo definieren Sie die Tabelle? Könnte sie eine Screenshot aus den Report-Definitionen senden, der diese Tabelle zeigt?
Im angehängten Report kann ich Sie ebenfalls nicht finden. 
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
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Z…
```

</details>

---

### [AW-237710] — Sperre von Planservice Einheit

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-237710]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 24.07.2025 10:05 |

**Description:**

> AW: [EXTERN] RE: [AW-237710] Sperre von Planservice Einheit (6) Hallo Herr Dörfler, die Bearbeitung einer Aktivität steuert nicht automatisch die Bearbeitung der Plantafel. Es ist bspw. durchaus möglich, dass Sie eine Aktivität bearbeiten und hier z.B. den Status von "Anfrage" auf "Zusage" ändern, aber anschließend noch die geplante Aktivität auf der Plantafel in der Länge kürzen/verlängern möchten/müssen. In der Praxis könnte dies bspw. der Fall sein wenn Sie einen Servicetermin vereinbaren möc...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Angelique Jäckel (support.cantor.de@a-w.com)
To: tim.doerfler@gugelfuss.de | Date: 24.07.2025 10:05
Type: Answer | 
AW: [EXTERN] RE: [AW-237710] Sperre von Planservice Einheit (6)
Hallo Herr Dörfler,
die Bearbeitung einer Aktivität steuert nicht automatisch die Bearbeitung der Plantafel.
Es ist bspw. durchaus möglich, dass Sie eine Aktivität bearbeiten und hier z.B. den Status von "Anfrage" auf "Zusage" ändern,
aber anschließend noch die geplante Aktivität auf der Plantafel in der Länge kürzen/verlängern möchten/müssen.
In der Praxis könnte dies bspw. der Fall sein wenn Sie einen Servicetermin vereinbaren möchten,
der Kunde sagt den vorgeschlagenen Termin zu und Sie bearbeiten den Aktivitätsstatus auf "Zusage".
Im Gespräch mit dem Kunden stellt sich dann aber bspw. raus, dass der Termin nicht wie ursprünglich geplant in 1 Stunde zu schaffen ist sondern aus Gründen doch eher 1,5 Stunden dauern wird. Also müssen Sie die Aktivität in der Plantafel anpassen und verlängern. Wenn es nun aber bspw. so wäre, dass die Plantafel nicht gesperrt werden würde, könnte z.B. ein Kollege ihre Aktivität verschieben oder einen Anschlusstermin für diese Serviceeinheit eintra…
```

</details>

---

### [AW-237708] — Drutex Händlerroutine - Serverinstallation - Domäne?

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-237708]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 24.07.2025 09:24 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Kerstin Heyd
To: Kerstin Heyd | Date: 24.07.2025 09:24
Type: State changed | 
RE: [AW-237708] Drutex Händlerroutine - Serverinstallation - Domäne? (5)
Telefonat mit Herrn Hecht
```

</details>

---

### [AW-237883] — Auftragststatus  größter gemeinsamer Nenner ?

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-237883]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 24.07.2025 08:27 |

**Description:**

> RE: [AW-237883] Auftragststatus  größter gemeinsamer Nenner ? (4) Hallo Marian, nein, daran hat sich eigentlich nichts geändert. Um herauszufinden was da passiert müsste man das ganze jetzt mal tiefer analysieren. Mit freundlichen Grüßen | Best regards Sascha Hermann ###EOM## Phone:  +49 641 96620 393 Mobile:  +49 6404 2051 361 A+W Software GmbH Siemensstraße 3 35463 Fernwald Germany www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler ...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Sascha Hermann (support.cantor.de@a-w.com)
To: Marian.Wilm@be-bauelemente.com | Date: 24.07.2025 08:27
Type: Answer | 
RE: [AW-237883] Auftragststatus  größter gemeinsamer Nenner ? (4)
Hallo Marian,
nein, daran hat sich eigentlich nichts geändert.
Um herauszufinden was da passiert müsste man das ganze jetzt mal tiefer analysieren.
Mit freundlichen Grüßen | Best regards
Sascha Hermann
###EOM##

Phone:  +49 641 96620 393
Mobile:  +49 6404 2051 361
A+W Software GmbH
Siemensstraße 3
35463 Fernwald
Germany

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus in Ihr Sy…
```

</details>

---

### [AW-237265] — Fehler Objekt ID

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-237265]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 24.07.2025 08:07 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Sascha Hermann
To: Sascha Hermann | Date: 24.07.2025 08:07
Type: State changed | 
RE: [AW-237265] Fehler Objekt ID (8)
Warten auf Rückmeldung
```

</details>

---

### [AW-233220] — Fehlende Bearbeitungen in Verbindung mit Mindestabstand

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-233220]` |
| **Status** | 🔵 In Progress |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 24.07.2025 07:23 |

**Description:**

> AW: [AW-233220] Fehlende Bearbeitungen in Verbindung mit Mindestabstand (8) Guten Morgen Herr Horn, vielen Dank für die Unterstützung. Aufgrund Urlaub und anderer Aufgaben komme ich leider erst heute wieder zu diesem Problem. Konfliktbehandlung zeigt keine Probleme. Ich würde einen DUMP bereitstellen lassen, geht aber leider erst Mitte August. Vorab folgende Frage zum Verständnis: Betrifft die Festlegung eines Mindestabstands die davor liegende Bearbeitung oder die danach folgende Bearbeitung? M...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Marco Fischer (mfischer@tmp-fenster.de)
To: support.cantor.de@a-w.com | Date: 24.07.2025 07:23
Type: Request | 
AW: [AW-233220] Fehlende Bearbeitungen in Verbindung mit Mindestabstand (8)
Guten Morgen Herr Horn,
vielen Dank für die Unterstützung.
Aufgrund Urlaub und anderer Aufgaben komme ich leider erst heute wieder zu diesem Problem.

Konfliktbehandlung zeigt keine Probleme.

Ich würde einen DUMP bereitstellen lassen, geht aber leider erst Mitte August.

Vorab folgende Frage zum Verständnis:
Betrifft die Festlegung eines Mindestabstands die davor liegende Bearbeitung oder die danach folgende Bearbeitung?

Mit freundlichem Gruß

Marco Fischer
Mitarbeiter EDV
Datenschutzbeauftragter

Telefon:        03685 4067-17
Fax:    03685 4067-29
E-Mail: mfischer@tmp-fenster.de
Web:    www.tmp-fenster.de<http://www.tmp-fenster.de>

Social: [https://www.tmp-fenster.de/fileadmin/bilder/social-ico/grey_linkedin.png] <https://www.linkedin.com/company/tmp-fenster-t%C3%BCren-gmbh/>  [https://www.tmp-fenster.de/fileadmin/bilder/social-ico/grey_insta.png] <https://www.instagram.com/tmp_fenster>  [https://www.tmp-fenster.de/fileadmin/bilder/social-ico/grey_youtube.png…
```

</details>

---

### [AW-235537] — Keine Meldung TA - kein Getriebe

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-235537]` |
| **Status** | 🔵 In Progress |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 23.07.2025 13:06 |

**Description:**

> AW: [AW-235537] Support-Ticket / Keine Meldung TA - kein Getriebe (10) Hallo, wann ist hier mit eine Antwort zu rechnen? VG Mit freundlichen Grüßen MARTIN RAßLOFF Leiter Informationstechnologie <http://www.fenster-mueller.de> Müller+Co GmbH | Merzhausener Straße 4 - 6 | 61389 Schmitten-Brombach Tel: 06084 42-45 | Fax: 06084 4255-45 www.fenster-mueller.de HRB Königstein 108077 - Geschäftsführer: Bernd Müller, Fabian Müller-Albrecht ________________________________ Diese E-Mail ist ausschließlich ...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Martin Raßloff (martin.rassloff@fenster-mueller.de)
To: support.cantor.de@a-w.com | Date: 23.07.2025 13:06
Type: Request | 
AW: [AW-235537] Support-Ticket / Keine Meldung TA - kein Getriebe (10)
Hallo,

wann ist hier mit eine Antwort zu rechnen?

VG

Mit freundlichen Grüßen
MARTIN RAßLOFF
Leiter Informationstechnologie

<http://www.fenster-mueller.de>

Müller+Co GmbH | Merzhausener Straße 4 - 6 | 61389 Schmitten-Brombach
Tel: 06084 42-45 | Fax: 06084 4255-45
www.fenster-mueller.de

HRB Königstein 108077 - Geschäftsführer: Bernd Müller, Fabian Müller-Albrecht
________________________________
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus in Ihr System gelangen, haften wir nicht für die evtl. entstande…
```

</details>

---

### [AW-236858] — CaImport in MT - CARLSAUE

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-236858]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 23.07.2025 12:49 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Kerstin Heyd
To: Kerstin Heyd | Date: 23.07.2025 12:49
Type: State changed | 
RE: [AW-236858] CaImport in MT - CARLSAUE (10)
Test CaExport - CaImport mit korrigierten DBs
ACHTUNG: Probleme beim Import, weil in der MT auf die CaExpK und -D Trigger gesetzt waren.
```

</details>

---

### [AW-236559] — Unterstützung Update auf Version 7.8 und Händler-Update

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-236559]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 23.07.2025 10:29 |

**Description:**

> FW: RE: [AW-236559] Unterstützung Update auf Version 7.8 und Händler-Update (14) Betreff: FW: RE: [AW-236559] Unterstützung Update auf Version 7.8 und Händler-Update Gesendet: 17.07.2025 10:43 Von: Kerstin Heyd (support.cantor.de@a-w.com) An: u.boelker@carls-aue.de Hallo Herr Bölker, hier wie abgesprochen die Informationen zur Korrektur der Multitrade Datenbank. 1. Tabellenstruktur Hier gibt es kleinere Fehler bezüglich Indices und Datentypen. Außerdem sind noch alle Produzententabellen enthalte...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Kerstin Heyd (support.cantor.de@a-w.com)
To: kerstin.heyd@a-w.com | Date: 23.07.2025 10:29
Type: Answer | 
FW: RE: [AW-236559] Unterstützung Update auf Version 7.8 und Händler-Update (14)
 
Betreff: FW: RE: [AW-236559] Unterstützung Update auf Version 7.8 und Händler-Update
Gesendet: 17.07.2025 10:43
Von: Kerstin Heyd (support.cantor.de@a-w.com)
An: u.boelker@carls-aue.de
Hallo Herr Bölker,
hier wie abgesprochen die Informationen zur Korrektur der Multitrade Datenbank.
1. Tabellenstruktur
Hier gibt es kleinere Fehler bezüglich Indices und Datentypen. Außerdem sind noch alle Produzententabellen enthalten.
In dem angehängten Korrekturskript: CarlsaueMT_DBStruktur_mitDrop_ohneROMA.sql habe ich die Löschbefehle der Roma-Tabellen schon entfernt. Bitte sehen Sie sich die übrigen Tabellen, die gelöscht werden sollen, noch einmal an; möglicherweise wurden ja absichtlich Zusatztabellen für die MT angelegt, die dann nicht gelöscht werden sollen.
Passen Sie vor dem Ausführen des Skripts bitte auch noch den Datenbanknamen an.

2. Mehrsprachigkeit
Um die Mehrsprachigkeit zurückzunehmen gehen Sie bitte wie folgt vor:
 • Löschen Sie im Cantor unter Stammdaten - Mar…
```

</details>

---

### [AW-235334] — Grafiken bei AB´s teilweise schwarz

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-235334]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 22.07.2025 14:11 |

**Description:**

> FW: RE: Antwort: Re: [JT#2025070210000669] [AW-235334] Grafiken bei AB´s teilweise schwarz (15) Hallo Herr Stadler, hierzu habe ich noch keine Rückmeldung erhalten. Könnten Sie mir bitte den Auftrag und die Grafiken zukommen lassen. Vielen Dank Mit freundlichen Grüßen | Best regards Sascha Hermann ###EOM## Phone:  +49 641 96620 393 Mobile:  +49 6404 2051 361 A+W Software GmbH Siemensstraße 3 35463 Fernwald Germany www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Denn...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Sascha Hermann (support.cantor.de@a-w.com)
To: Alois.Stadler@josko.at | Date: 22.07.2025 14:11
Type: Answer | 
FW: RE: Antwort: Re: [JT#2025070210000669] [AW-235334] Grafiken bei AB´s teilweise schwarz (15)
Hallo Herr Stadler,
hierzu habe ich noch keine Rückmeldung erhalten. Könnten Sie mir bitte den Auftrag und die Grafiken zukommen lassen.
Vielen Dank
 
Mit freundlichen Grüßen | Best regards
Sascha Hermann
###EOM##

Phone:  +49 641 96620 393
Mobile:  +49 6404 2051 361
A+W Software GmbH
Siemensstraße 3
35463 Fernwald
Germany

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus in Ih…
```

</details>

---

### [AW-236373] — dringend Fehlermeldung "nicht genügend Arbeitsspeicher" - Crystal Resport Windows Forms Viewer (PROD)

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-236373]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 22.07.2025 14:08 |

**Description:**

> FW: RE: Antwort: RE: Antwort: [AW-236373] dringend Fehlermeldung "nicht genügend Arbeitsspeicher" - Crystal Resport Windows Forms Viewer (PROD) (18) Hallo Herr Hintermeier, konnten Sie den Bericht verkleinern und damit drucken? Mit freundlichen Grüßen | Best regards Sascha Hermann ###EOM## Phone:  +49 641 96620 393 Mobile:  +49 6404 2051 361 A+W Software GmbH Siemensstraße 3 35463 Fernwald Germany www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Th...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Sascha Hermann (support.cantor.de@a-w.com)
To: Florian.Hintermaier@josko.at | Date: 22.07.2025 14:08
Type: Answer | 
FW: RE: Antwort: RE: Antwort: [AW-236373] dringend Fehlermeldung "nicht genügend Arbeitsspeicher" - Crystal Resport Windows Forms Viewer (PROD) (18)
Hallo Herr Hintermeier,
konnten Sie den Bericht verkleinern und damit drucken?
 
Mit freundlichen Grüßen | Best regards
Sascha Hermann
###EOM##

Phone:  +49 641 96620 393
Mobile:  +49 6404 2051 361
A+W Software GmbH
Siemensstraße 3
35463 Fernwald
Germany

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus in Ihr System gelangen, haften wir nicht für die evtl. entstandenen Schäden.…
```

</details>

---

### [AW-236365] — Kundenwünsche bzgl. Rechnungsformat XRechnung bzw. ZUGFeRD

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-236365]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 22.07.2025 12:16 |

**Description:**

> AW: [AW-236365] Kundenwünsche bzgl. Rechnungsformat XRechnung bzw. ZUGFeRD (26) Hallo Herr Kilic, zu 1) da wir nicht alle Knoten standardmäßig füllen, kann über den Artikel und die Umsetzungstabelle alle von uns bisher nicht angesprochenen Knoten gefüllt werden. zu 2) die Schnittstelle wird von uns so befüllt, das sie den Anforderung in Deutschland genügt. Erweiterungen sind über die unter 1) beschrieben Möglichkeiten möglich. Dazu gehört auch BT-1, BT-2 oder BT-10. Die Daten können über die Eig...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Sabine Weidmann (support.cantor.de@a-w.com)
To: yunus.kilic@schlotterer.at | Date: 22.07.2025 12:16
Type: Answer | 
AW: [AW-236365] Kundenwünsche bzgl. Rechnungsformat XRechnung bzw. ZUGFeRD (26)
Hallo Herr Kilic,
zu 1) da wir nicht alle Knoten standardmäßig füllen, kann über den Artikel und die Umsetzungstabelle alle von uns bisher nicht angesprochenen Knoten gefüllt werden. 
zu 2) die Schnittstelle wird von uns so befüllt, das sie den Anforderung in Deutschland genügt. Erweiterungen sind über die unter 1) beschrieben Möglichkeiten möglich. Dazu gehört auch BT-1, BT-2 oder BT-10. Die Daten können über die Eigenschaft des Artikels gefüllt werden.

Die Beschreibung im Cantor-WIKI umfasst die von Cantor angesprochenen Informationen. Wenn weitere gewünscht sind, benötige ich eine neues Ticket mit konkreten Beispielen. Welche Information fehlt wo, die gesetzlich vorgeschrieben ist. Vielleicht sollten Sie hier konkrete Anforderungen Ihrer Kunden abwarten. Bisher sind zwar noch fehlende Informationen aufgetaucht. Diese konnte aber alle über die Artikelkasse gefüllt werden.
 
Mit freundlichen Grüßen | Best regards
Sabine Weidmann
###EOM##

Phone:  +49 641 96620 393
Mobile…
```

</details>

---

### [AW-237472] — CaImport - Fehlermeldungen

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-237472]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 22.07.2025 09:53 |

**Description:**

> RE: [AW-237472] CaImport - Fehlermeldungen (4) Hallo Herr Bieker, die Meldung besagt, dass die Netzwerkverbindung unterbrochen wurde. Mir ist zwar nicht bekannt, dass dies mit der Größe der Import-Datei zu tun haben könnte, dennoch würde ich Ihnen empfehlen, den Import von Zubehör auszukoppeln und separat durchzuführen. Diese Vorgehensweise hat in der Vergangenheit vielen Kunden geholfen, die große Datenmengen importiert haben. Mit freundlichen Grüßen | Best regards Kerstin Heyd ###EOM## Phone: ...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Kerstin Heyd (support.cantor.de@a-w.com)
To: K.Bieker@fenster-hoffmann.de | Date: 22.07.2025 09:53
Type: Answer | 
RE: [AW-237472] CaImport - Fehlermeldungen (4)
Hallo Herr Bieker,
die Meldung besagt, dass die Netzwerkverbindung unterbrochen wurde.
Mir ist zwar nicht bekannt, dass dies mit der Größe der Import-Datei zu tun haben könnte, dennoch würde ich Ihnen empfehlen, den Import von Zubehör auszukoppeln und separat durchzuführen. Diese Vorgehensweise hat in der Vergangenheit vielen Kunden geholfen, die große Datenmengen importiert haben.
Mit freundlichen Grüßen | Best regards
Kerstin Heyd
###EOM##

Phone:  +49 641 96620 393
Mobile:  +49 641 96620-363
A+W Software GmbH
Siemensstraße 3
35463 Fernwald
Germany

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und d…
```

</details>

---

### [AW-237447] — Bogenbestellung

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-237447]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 22.07.2025 09:32 |

**Description:**

> AW: [AW-237447] Bogenbestellung (6) Hallo Frau Heinsohn, in der Klasse 99 kann man nur alle Beschlagsfelder oder keines auswerten. Das gleiche gilt für die Profile. Über den Vorbelegungssatz kann man auch nur alle Profile oder nur die gebogenen bestellen. Es gibt keine Möglichkeit den Flügel gesondert zu behandeln. Ich kann das gerne an unsere Projektierung weiterleiten, ob es eine Lösung im Cantor gibt oder ob das eine Neuanforderung wäre. Mit freundlichen Grüßen | Best regards Sabine Weidmann ...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Sabine Weidmann (support.cantor.de@a-w.com)
To: k.heinsohn@staderglas.de | Date: 22.07.2025 09:32
Type: Answer | 
AW: [AW-237447] Bogenbestellung (6)
Hallo Frau Heinsohn,
in der Klasse 99 kann man nur alle Beschlagsfelder oder keines auswerten. Das gleiche gilt für die Profile.
Über den Vorbelegungssatz kann man auch nur alle Profile oder nur die gebogenen bestellen. Es gibt keine Möglichkeit den Flügel gesondert zu behandeln. Ich kann das gerne an unsere Projektierung weiterleiten, ob es eine Lösung im Cantor gibt oder ob das eine Neuanforderung wäre.

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
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns …
```

</details>

---

### [AW-235768] — Händlersoftware 7.7 - CR lässt sich nicht aktualisieren

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-235768]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 22.07.2025 09:26 |

**Description:**

> FW: AW: CR Problem - und Problem beim Installieren der Prereq.7.7 [AW-235768] (19) Mit freundlichen Grüßen | Best regards Kerstin Heyd ###EOM## ​ Phone:  +49 641 96620 393 Mobile:  +49 641 96620-363 A+W Software GmbH Siemensstraße 3 35463 Fernwald Germany www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan Amtsgericht Gießen/Gießen Local Court: HRB 7963 Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertra...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Kerstin Heyd (support.cantor.de@a-w.com)
To: kerstin.heyd@a-w.com | Date: 22.07.2025 09:26
Type: Answer | 
FW: AW: CR Problem - und Problem beim Installieren der Prereq.7.7 [AW-235768] (19)
 
Mit freundlichen Grüßen | Best regards
Kerstin Heyd
###EOM##
​
Phone:  +49 641 96620 393
Mobile:  +49 641 96620-363
A+W Software GmbH
Siemensstraße 3
35463 Fernwald
Germany

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus in Ihr System gelangen, haften wir nicht für die evtl. entstandenen Schäden.

This e-mail is for the intended recipient only and may contain confidential an…
```

</details>

---

### [AW-237386] — CIM - Barcode wird bei Fertigmeldung nicht in Tabelle BDE geschrieben

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-237386]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 22.07.2025 08:21 |

**Description:**

> RE: [AW-237386] CIM - Barcode wird bei Fertigmeldung nicht in Tabelle BDE geschrieben (6) Hallo Herr Zießow, das lässt sich im nachhinein leider nicht mehr herausfinden. Wie oft passiert das? Lässt sich das nachvollziehen? Wenn ja, dann bitte mal ein DB-Trace und nachsehen ob da irgend etwas ungewöhnlich erscheint. Mit einer Kopie des Auftrages aus Ihrem Beispiel hatte ich die Buchungen in der Tabelle: B    - STATM 2848       08:15:12.17 |- INSERT INTO GAYKO_PRODU..CPB_BDE ([ZEITPUNKT],[MAID],[A...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Sascha Hermann (support.cantor.de@a-w.com)
To: Ziessow.Tim@gayko.de | Date: 22.07.2025 08:21
Type: Answer | 
RE: [AW-237386] CIM - Barcode wird bei Fertigmeldung nicht in Tabelle BDE geschrieben (6)
Hallo Herr Zießow,
das lässt sich im nachhinein leider nicht mehr herausfinden. 
Wie oft passiert das? Lässt sich das nachvollziehen? Wenn ja, dann bitte mal ein DB-Trace und nachsehen ob da irgend etwas ungewöhnlich erscheint.
Mit einer Kopie des Auftrages aus Ihrem Beispiel hatte ich die Buchungen in der Tabelle:

B    - STATM 2848       08:15:12.17 |- INSERT INTO GAYKO_PRODU..CPB_BDE ([ZEITPUNKT],[MAID],[APID],[BUID],[BGID],[TEILID],[VORGABEZEIT],[ELEMENTBARCODE],[INFO],[AUFNR],[PPOSNR],[STUECKNR],[TEILIDGLOBAL]) VALUES (?,?,?,?,?,?,?,?,?,?,?,?,?)
DB    - PARAM 2848       08:15:12.17 |- Parameter T [ZEITPUNKT]=[22.07.2025 08:15:12]
DB    - PARAM 2848       08:15:12.17 |- Parameter N [MAID]=[9999.000000]
DB    - PARAM 2848       08:15:12.18 |- Parameter N [APID]=[131200.000000]
DB    - PARAM 2848       08:15:12.18 |- Parameter S [BUID]=[3]
DB    - PARAM 2848       08:15:12.18 |- Parameter N [BGID]=[0.000000]
DB    - PARAM 2848       08:15:12.19 |- Parameter N [TEILID]=[53…
```

</details>

---

### [AW-237459] — Preiskorrektur Listenpreis/Festpreis

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-237459]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 21.07.2025 14:30 |

**Description:**

> RE: [AW-237459] Preiskorrektur Listenpreis/Festpreis (4) Hallo Frau Spiegel, [PREISOPTIONEN] PreisgruppeFest=FALSE DESCRIPTION: True:  bei Festpreisen wird die Preisgruppe #FEST verwendet False: bei Festpreisen wird die Preisgruppe des Einheitspreises (bzw. Zubehör als Position) verwendet Wenn der Eintrag aus FALSE steht, dann wird die Preisgruppe der Einheit bzw. des Zubehörs als Position verwendet, nicht die vordefinierte Preisgruppe #FEST. Bitte prüfen Sie für Ihre Beispiele, ob das Einstelle...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Sabine Weidmann (support.cantor.de@a-w.com)
To: Natalie.Spiegel@heinzmann.eu | Date: 21.07.2025 14:30
Type: Answer | 
RE: [AW-237459] Preiskorrektur Listenpreis/Festpreis (4)
Hallo Frau Spiegel,
[PREISOPTIONEN] 
PreisgruppeFest=FALSE

DESCRIPTION:
True:  bei Festpreisen wird die Preisgruppe #FEST verwendet
False: bei Festpreisen wird die Preisgruppe des Einheitspreises (bzw. Zubehör als Position) verwendet
Wenn der Eintrag aus FALSE steht, dann wird die Preisgruppe der Einheit bzw. des Zubehörs als Position verwendet, nicht die vordefinierte Preisgruppe #FEST.

Bitte prüfen Sie für Ihre Beispiele, ob das Einstellen des cantor.ini auf FLASE die gewünschte Buchung auslöst.
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
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informa…
```

</details>

---

### [AW-237440] — Open-Trans ROMA-Lieferscheine

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-237440]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 21.07.2025 13:54 |

**Description:**

> AW: [AW-237440] Open-Trans Fehler ROMA (9) Hallo Herr Kuhnert, ich gehe hier davon aus, das es sich um Zukaufteilbestellungen handelt. D.h. ich benötige den zugehörigen Auftrag, dann ich die Bestellung hier per TA erzeugen. Mit freundlichen Grüßen | Best regards Sabine Weidmann ###EOM## Phone:  +49 641 96620 393 Mobile:  +49 6404 2051 362 A+W Software GmbH Siemensstraße 3 35463 Fernwald Germany www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thomp...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Sabine Weidmann (support.cantor.de@a-w.com)
To: bkuhnert@albohn.de | Date: 21.07.2025 13:54
Type: Answer | 
AW: [AW-237440] Open-Trans Fehler ROMA (9)
Hallo Herr Kuhnert,
ich gehe hier davon aus, das es sich um Zukaufteilbestellungen handelt.
D.h. ich benötige den zugehörigen Auftrag, dann ich die Bestellung hier per TA erzeugen.
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
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E…
```

</details>

---

### [AW-231022] — Systemschlange 22: Aufträge archivieren

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-231022]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 21.07.2025 09:00 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Wolfgang Schmid
To: Wolfgang Schmid | Date: 21.07.2025 09:00
Type: State changed | 
RE: [AW-231022] Systemschlange 22: Aufträge archivieren (21)
warten
```

</details>

---

### [AW-230419] — Multitrade: Mgl., Briefpapier zu berücksichtigen - ZUGFeRD

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-230419]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 21.07.2025 08:43 |

**Description:**

> Automatische Antwort: RE: [AW-230419] Multitrade: Mgl., Briefpapier zu berücksichtigen - ZUGFeRD (18) Vielen Dank für Ihre Nachricht. Ich befinde mich zurzeit außer Haus und bin bis zum 25. Juli 2025 (einschl.) nicht für Sie erreichbar. Ihre Nachricht wird nicht automatisch weitergeleitet. Vielen Dank für Ihr Verständnis! Mit freundlichen Grüßen Christian Rausch ERP-Systembetreuung inkl. Händlerversion GAYKO Fenster-Türenwerk GmbH Dortmunder Straße 6 · D-57234 Wilnsdorf Tel.: +49 (2739) 873-196 ...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Christian Holger Rausch (rausch.christian@gayko.de)
To: support.cantor.de@a-w.com | Date: 21.07.2025 08:43
Type: Request | 
Automatische Antwort: RE: [AW-230419] Multitrade: Mgl., Briefpapier zu berücksichtigen - ZUGFeRD (18)
Vielen Dank für Ihre Nachricht.

Ich befinde mich zurzeit außer Haus und bin bis zum 25. Juli 2025 (einschl.) nicht für Sie erreichbar.

Ihre Nachricht wird nicht automatisch weitergeleitet.

Vielen Dank für Ihr Verständnis!

Mit freundlichen Grüßen

Christian Rausch
ERP-Systembetreuung inkl. Händlerversion

GAYKO Fenster-Türenwerk GmbH
Dortmunder Straße 6 · D-57234 Wilnsdorf
Tel.: +49 (2739) 873-196
E-Mail: rausch.christian@gayko.de<mailto:rausch.christian@gayko.de> · Website: www.gayko.de<http://www.gayko.de>

Geschäftsführer: Klaus Gayko, Kathrin Gayko
Amtsgericht Siegen, HRB 3295 · Handwerksrolle Arnsberg
USt-IdNr.: DE 126578454

Unsere Hinweise zum Umgang mit personenbezogenen Daten finden Sie hier<https://www.gayko.de/datenschutz>.
```

</details>

---

### [AW-235978] — Fwd: Performanceprobleme RomaConnect bei Gaulhofer

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-235978]` |
| **Status** | 🔵 In Progress |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 21.07.2025 08:29 |

**Description:**

> AW: [EXT] FW: AW: [AW-235978] Support-Ticket / Fwd: Performanceprobleme RomaConnect bei Gaulhofer (19) Guten Tag, wir werden in der KW 35 (sofern die Test’s alle i.O sind)  auf die 7.9 Version updaten. Mit freundlichen Grüßen / With best regards Günter Grabmeir Innovation & Technologie M: +43 (0) 664 9638685 Von: Support Pohlheim Cantor <support.cantor.de@a-w.com> Gesendet: Freitag, 18. Juli 2025 14:47 An: Günter Grabmeir <guenter.grabmeir@gaulhofer.com> Cc: m.grasmaeher@grasmaeher-it.de Betreff...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Günter Grabmeir (guenter.grabmeir@gaulhofer.com)
To: support.cantor.de@a-w.com | Date: 21.07.2025 08:29
Type: Request | 
AW: [EXT] FW: AW: [AW-235978] Support-Ticket / Fwd: Performanceprobleme RomaConnect bei Gaulhofer (19)
Guten Tag,

wir werden in der KW 35 (sofern die Test’s alle i.O sind)  auf die 7.9 Version updaten.

Mit freundlichen Grüßen / With best regards

Günter Grabmeir
Innovation & Technologie
 

M: +43 (0) 664 9638685

Von: Support Pohlheim Cantor <support.cantor.de@a-w.com>
Gesendet: Freitag, 18. Juli 2025 14:47
An: Günter Grabmeir <guenter.grabmeir@gaulhofer.com>
Cc: m.grasmaeher@grasmaeher-it.de
Betreff: [EXT] FW: AW: [AW-235978] Support-Ticket / Fwd: Performanceprobleme RomaConnect bei Gaulhofer

Hallo Herr Grabmeir,

in Absprache mit Herrn Grassmäher kontaktiere ich Sie zum Thema der Performance Probleme mit RomaConnect in der 7.7.

Die Probleme (verursacht durch eine Lochbreitenänderung) sind ab der 7.8 gelöst. Kann der Umstieg auf eine höre Version eine Lösung sein? Die 7.7 ist ab Ende des Jahres aus der Wartung.

Können wir zu diesem Thema heute bis 16 Uhr oder am Montag ab 8:30 Uhr telefonieren?

Schönes Wochenende

…
```

</details>

---

### [AW-237295] — Bei der Terminierung wird in der Bestellung im Reorg C25 Projekt wird das Wunschdatum nicht gefüllt

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-237295]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 18.07.2025 14:21 |

**Description:**

> RE: [AW-237295] Bei der Terminierung wird in der Bestellung im Reorg C25 Projekt wird das Wunschdatum nicht gefüllt (4) Hallo Herr Bonniksen, es fehlen sämtlichen Daten in der Auftragsgruppierung. Es gibt weder Linien, daher auch keine Zuordnung, noch sonstige Einträge. Daher kann keine Wunschtermin bestimmt werden. Wenn die Stammdaten hier ergänzt wurden, sollte auch das Wunschdatum der Bestellung gefüllt werden. Bis dahin kann der Workaround mit dem manuellen Füllen eines Wunschdatum erfolgt u...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Sabine Weidmann (support.cantor.de@a-w.com)
To: P.Bonniksen@dth-tiemann.de | Date: 18.07.2025 14:21
Type: Answer | 
RE: [AW-237295] Bei der Terminierung wird in der Bestellung im Reorg C25 Projekt wird das Wunschdatum nicht gefüllt (4)
Hallo Herr Bonniksen,
es fehlen sämtlichen Daten in der Auftragsgruppierung. Es gibt weder Linien, daher auch keine Zuordnung, noch sonstige Einträge.
Daher kann keine Wunschtermin bestimmt werden.
Wenn die Stammdaten hier ergänzt wurden, sollte auch das Wunschdatum der Bestellung gefüllt werden.
Bis dahin kann der Workaround mit dem manuellen Füllen eines Wunschdatum erfolgt und so die Bestellung gedruckt werden.
 
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
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie s…
```

</details>

---

### [AW-237283] — Filter Bestellübersicht

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-237283]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 18.07.2025 12:11 |

**Description:**

> AW: [AW-237283] AW: Filter Bestellübersicht (9) Hallo Herr Schaufler, leider steht die Info in der Bestellübersicht nicht zur Verfügung. Hier würde ein SQL Statement über das SQL-Tool vielleicht weiterhelfen. Unsere Projektierung kann Sie da sicher unterstürzen. Auch wie man diesen "Zustand" in Zukunft vielleicht verhindern kann. Mit freundlichen Grüßen | Best regards Sabine Weidmann ###EOM## Phone:  +49 641 96620 393 Mobile:  +49 6404 2051 362 A+W Software GmbH Siemensstraße 3 35463 Fernwald Ge...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Sabine Weidmann (support.cantor.de@a-w.com)
To: MSchaufler@albohn.de | Date: 18.07.2025 12:11
Type: Answer | 
AW: [AW-237283] AW: Filter Bestellübersicht (9)
Hallo Herr Schaufler,
leider steht die Info in der Bestellübersicht nicht zur Verfügung.
Hier würde ein SQL Statement über das SQL-Tool vielleicht weiterhelfen.
Unsere Projektierung kann Sie da sicher unterstürzen. Auch wie man diesen "Zustand" in Zukunft vielleicht verhindern kann.
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
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist …
```

</details>

---

### [AW-216429] — Positionsgrafiken als Binärcode

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-216429]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 18.07.2025 11:57 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Sabine Weidmann
To: Sabine Weidmann | Date: 18.07.2025 11:57
Type: State changed | 
RE: [AW-216429] Positionsgrafiken als Binärcode (53)
warten auf Rückmeldung
```

</details>

---

### [AW-237188] — Positionsübersicht Spalte Stückpreis inkl. Montage

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-237188]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 18.07.2025 11:32 |

**Description:**

> RE: [AW-237188] Positionsübersicht Spalte Stückpreis inkl. Montage (4) Hallo Herr Panholzer, die gewünschte Spalte ist nicht verfügbar und gab es in älteren Versionen auch nicht. Sollte diese Spalte für sie/ihren Partner notwendig sein, müsste eine Neuentwicklung erfolgen. Lassen Sie mich gerne wissen wenn Sie hierfür einen DR benötigen. Mit freundlichen Grüßen | Best regards Angelique Jäckel ###EOM## Phone:  +49 641 96620 393 Mobile:  +4964196620-0 A+W Software GmbH Siemensstraße 3 35463 Fernwa...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Angelique Jäckel (support.cantor.de@a-w.com)
To: thomas.panholzer@actual.at | Date: 18.07.2025 11:32
Type: Answer | 
RE: [AW-237188] Positionsübersicht Spalte Stückpreis inkl. Montage (4)
Hallo Herr Panholzer,
die gewünschte Spalte ist nicht verfügbar und gab es in älteren Versionen auch nicht.
Sollte diese Spalte für sie/ihren Partner notwendig sein, müsste eine Neuentwicklung erfolgen.
Lassen Sie mich gerne wissen wenn Sie hierfür einen DR benötigen.
Mit freundlichen Grüßen | Best regards
Angelique Jäckel
###EOM##

Phone:  +49 641 96620 393
Mobile:  +4964196620-0
A+W Software GmbH
Siemensstraße 3
35463 Fernwald
Germany

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. S…
```

</details>

---

### [AW-235226] — Auftragsimport via XML bleibt hängen

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-235226]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 18.07.2025 08:11 |

**Description:**

> AW: AW: [AW-235226] Auftragsimport via XML bleibt hängen (19) Hallo Yunus, in diesem Bereich gab es bereits ein ziemlich gutes Trace und Fehlerprotokollierung. Das relevante Tracing befindet sich im Abschnitt "XML" und die Fehlereinträge in der Tabelle "ERRORLOG" für "Bereich" = 'S_MAN'. Wir haben das Trace jetzt noch erweitert, es wäre interessant, die Fehlereinträge/Trace-Datei zu sehen, wenn das gemeldete Fehlverhalten des Programms auftritt. Programmstand dafür liegt auf dem ftp-Server Mit f...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Sascha Hermann (support.cantor.de@a-w.com)
To: yunus.kilic@schlotterer.at | Date: 18.07.2025 08:11
Type: Answer | 
AW: AW: [AW-235226] Auftragsimport via XML bleibt hängen (19)
Hallo Yunus,
in diesem Bereich gab es bereits ein ziemlich gutes Trace und Fehlerprotokollierung.
Das relevante Tracing befindet sich im Abschnitt "XML" und die Fehlereinträge in der Tabelle "ERRORLOG" für "Bereich" = 'S_MAN'.
Wir haben das Trace jetzt noch erweitert, es wäre interessant, die Fehlereinträge/Trace-Datei zu sehen, wenn das gemeldete Fehlverhalten des Programms auftritt.
Programmstand dafür liegt auf dem ftp-Server
 
Mit freundlichen Grüßen | Best regards
Sascha Hermann
###EOM##

Phone:  +49 641 96620 393
Mobile:  +49 6404 2051 361
A+W Software GmbH
Siemensstraße 3
35463 Fernwald
Germany

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bi…
```

</details>

---

### [AW-237214] — Glasgewicht auf AB drucken

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-237214]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 17.07.2025 15:51 |

**Description:**

> RE: [AW-237214] Glasgewicht auf AB drucken (4) Hallo Frau urban, derzeit gibt es im Positionsbereich keine Möglichkeit das Glasgewicht auszugeben. Wir können nur die Felder drucken, die in den Report-Definitionen zur Verfügung stehen. Mit freundlichen Grüßen | Best regards Sabine Weidmann ###EOM## Phone:  +49 641 96620 393 Mobile:  +49 6404 2051 362 A+W Software GmbH Siemensstraße 3 35463 Fernwald Germany www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs,...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Sabine Weidmann (support.cantor.de@a-w.com)
To: iurban@tmp-fenster.de | Date: 17.07.2025 15:51
Type: Answer | 
RE: [AW-237214] Glasgewicht auf AB drucken (4)
Hallo Frau urban,
derzeit gibt es im Positionsbereich keine Möglichkeit das Glasgewicht auszugeben. 
Wir können nur die Felder drucken, die in den Report-Definitionen zur Verfügung stehen.
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
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung …
```

</details>

---

### [AW-235340] — Störung LogiKal-Schnittstelle nach Aktualisierung der CANTOR-dlls (dll von Version 7.9.19 auf 7.9.20)

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-235340]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 17.07.2025 13:19 |

**Description:**

> FW: AW: [AW-235340] Störung LogiKal-Schnittstelle nach Aktualisierung der CANTOR-dlls (dll von Version 7.9.19 auf 7.9.20) (10) Hallo Herr Grewe, Stand meiner Recherche. Auch andere Kunden haben keine Auftragsreports, die eine feldweise Gruppierung bei Logikal Positionen ermöglichen. Der Grund ist klar, für reine Zubehörpositionen gibt es keinen Eintrag in der Tabelle  FELDTAB, die Feldnummer ist daher im Printschema nicht gefüllt. Die Feldnummer dient aber als Gruppierungsmerkmal im Unterbericht...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Stefan Rixecker (support.cantor.de@a-w.com)
To: F.Grewe@fenster-hoffmann.de | Date: 17.07.2025 13:19
Type: Answer | 
FW: AW: [AW-235340] Störung LogiKal-Schnittstelle nach Aktualisierung der CANTOR-dlls (dll von Version 7.9.19 auf 7.9.20) (10)
Hallo Herr Grewe,
Stand meiner Recherche. Auch andere Kunden haben keine Auftragsreports, die eine feldweise Gruppierung bei Logikal Positionen ermöglichen.
 
Der Grund ist klar, für reine Zubehörpositionen gibt es keinen Eintrag in der Tabelle  FELDTAB, die Feldnummer ist daher im Printschema nicht gefüllt.

Die Feldnummer dient aber als Gruppierungsmerkmal im Unterbericht für das Zubehör.
den einzigen Ansatzpunkt den ich auf Cantor Seite sehe ist die ES1102 im Orgadata -Glasartikel.
Leider kommen aus der Feld FieldNo der Schnittstelle nicht ganz eindeutige Werte zurück. Können Sie sich die Doppelungen in der ES1102 erklären?

 
Ebenso stehen die Werte nur innerhalb eines Memo-Feldes in der DB.
Man könnte in CR versuchen in einem eigenen Formelfeld den ES-Wert zu extrahieren, um diesen dann als Gruppierungsmerkmal zu verwenden.
Alles in allem viel Aufwand. Geben die Logikal-Report etwas her?
 
P.s: Mit vertretbarem Aufwand kann ich nur Ansätze zu einer möglichen Reporto…
```

</details>

---

### [AW-230510] — Fehlerhafter Import Order Response

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-230510]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 17.07.2025 10:50 |

**Description:**

> AW: [AW-230510] Fehlerhafter Import Order Response (18) Hallo Michael, wenn es Abweichungen gibt, kann man die im Lieferantenbestätigungsmodus über die rechte Maustaste je Position sehen. Das Kontextmenü heißt: Auf Origianlwert zurücksetzten Das Zurücksetzen passiert nur, wenn man den Wert anhakt. Wenn man den Dialog nur öffnet, sieht man die Unterschiede zur Menge, Einheit, Preis, Datum, ... Mit freundlichen Grüßen | Best regards Sabine Weidmann ###EOM## Phone:  +49 641 96620 393 Mobile:  +49 6...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Sabine Weidmann (support.cantor.de@a-w.com)
To: michael.hanska@katzbeck.at | Date: 17.07.2025 10:50
Type: Answer | 
AW: [AW-230510] Fehlerhafter Import Order Response (18)
Hallo Michael,
wenn es Abweichungen gibt, kann man die im Lieferantenbestätigungsmodus über die rechte Maustaste je Position sehen.
Das Kontextmenü heißt: Auf Origianlwert zurücksetzten 
Das Zurücksetzen passiert nur, wenn man den Wert anhakt. Wenn man den Dialog nur öffnet, sieht man die Unterschiede zur Menge, Einheit, Preis, Datum, ...
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
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte K…
```

</details>

---

### [AW-236739] — Datev Schnittstelle bei der Händlerversion (21793)

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-236739]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 17.07.2025 10:08 |

**Description:**

> AW: [AW-236739] Datev Schnittstelle bei der Händlerversion (21793) (10) Hallo Frau Beeken, wird unterstützen derzeit die Versionen 2.21, 4.3 und 5.1 von Datev. Das diese auch Bildformate unterstützen ist mir nicht bekannt. In der Regel sind FIBU Schnittstellen immer kundenindividuell. Wenn der Händler eine Anbindung möchte, muss das von unserer Projektierung geprüft und dann ein Dev. Request ausgearbeitet werden. Ich habe die Mail an Herrn Kunz in CC gesendet. Mit freundlichen Grüßen | Best rega...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Sabine Weidmann (support.cantor.de@a-w.com)
To: christa.beeken@siems-fenster.de | Date: 17.07.2025 10:08
Type: Answer | 
AW: [AW-236739] Datev Schnittstelle bei der Händlerversion (21793) (10)
Hallo Frau Beeken,
wird unterstützen derzeit die Versionen 2.21, 4.3 und 5.1 von Datev.
Das diese auch Bildformate unterstützen ist mir nicht bekannt.
In der Regel sind FIBU Schnittstellen immer kundenindividuell. Wenn der Händler eine Anbindung möchte, muss das von unserer Projektierung geprüft und dann ein Dev. Request ausgearbeitet werden. Ich habe die Mail an Herrn Kunz in CC gesendet.
 
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
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung …
```

</details>

---

### [AW-235335] — XRechnung / Gutschrift

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-235335]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 17.07.2025 09:29 |

**Description:**

> Automatische Antwort: AW: [AW-235335] XRechnung / Gutschrift (18) ﻿ Sehr geehrte Damen und Herren, ich befinde mich bis einschließlich dem 27.07.2025 nicht im Hause. Ihre E-Mail wird nicht weitergeleitet und von mir ab dem 28.07.2025 bearbeitet. In dringenden Fällen wenden Sie sich bitte an Herrn Teich (fteich@feba.de) Mit freundlichen Grüßen aus Burbach i.A. Kai Themanns - IT-Leitung - ________________________________ FeBa Fensterbau GmbH | Carl-Benz-Straße 23 | 57299 Burbach Tel.: 02736 497 57...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Kai Themanns (KThemanns@feba.de)
To: support.cantor.de@a-w.com | Date: 17.07.2025 09:29
Type: Request | 
Automatische Antwort: AW: [AW-235335] XRechnung / Gutschrift (18)
﻿
Sehr geehrte Damen und Herren,

ich befinde mich bis einschließlich dem 27.07.2025 nicht im Hause.
Ihre E-Mail wird nicht weitergeleitet und von mir ab dem 28.07.2025 bearbeitet.
In dringenden Fällen wenden Sie sich bitte an Herrn Teich (fteich@feba.de)

Mit freundlichen Grüßen aus Burbach
i.A. Kai Themanns
- IT-Leitung -
________________________________

FeBa Fensterbau GmbH | Carl-Benz-Straße 23 | 57299 Burbach
Tel.: 02736 497 579
E-Mail: KThemanns@feba.de<mailto:KThemanns@feba.de> | www.feba.de<http://www.feba.de/>

Geschäftsführer: Simon Menk, Norman Menk
Handelsregister: Amtsgericht Siegen - HRB 1964
```

</details>

---

### [AW-236129] — Performance

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-236129]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 17.07.2025 08:04 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Sascha Hermann
To: Sascha Hermann | Date: 17.07.2025 08:04
Type: State changed | 
RE: [AW-236129] Performance (15)
Waiting for Performance in Auftragsmaske bei vielen Positionen [AW-232961]
```

</details>

---

### [AW-219104] — Windows Server 2025

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-219104]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 16.07.2025 12:18 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Sascha Hermann
To: Kerstin Heyd | Date: 16.07.2025 12:18
Type: State changed | 
RE: [AW-219104] Windows Server 2025 (23)
ich hab keine Liste. Das WebView ist ja an vielen Stellen im Einsatz, z.B. die Desktopseite, bei den Aufgaben, in der Positionsliste unter der Grafik, ...
```

</details>

---

### [AW-223308] — BE Installationsroutine 7.9

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-223308]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 16.07.2025 11:20 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Kerstin Heyd
To: Kerstin Heyd | Date: 16.07.2025 11:20
Type: State changed | 
RE: [AW-223308] BE Installationsroutine 7.9 (27)
Routine auf \\cansrv\CANTOR_SETUP\Cantor Installationen abgelegt.
```

</details>

---

### [AW-236447] — Updateserver 2024 für Drutex

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-236447]` |
| **Status** | 🔵 In Progress |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 16.07.2025 08:56 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Kerstin Heyd
To: Dirk Horn | Date: 16.07.2025 08:56
Type: State changed | 
RE: [AW-236447] Updateserver 2024 für Drutex (13)
```

</details>

---

### [AW-236821] — negativ Bestände häufen sich per Scanner

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-236821]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 15.07.2025 11:47 |

**Description:**

> AW: [AW-236821] negativ Bestände häufen sich per Scanner (9) Hallo Frau Pferdt, das wäre super. Vielleicht gibt es ja doch eine Gemeinsamkeit, um es einzugrenzen und dann vielleicht auch nachvollziehbar zu bekommen. Wen Sie ein paar Daten gesammelt haben, können Sie mir dann den dump zukommen lassen? Vielen Dank. Mit freundlichen Grüßen | Best regards Sabine Weidmann ###EOM## Phone:  +49 641 96620 393 Mobile:  +49 6404 2051 362 A+W Software GmbH Siemensstraße 3 35463 Fernwald Germany www.a-w.com...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Sabine Weidmann (support.cantor.de@a-w.com)
To: Sabrina.Pferdt@weru.de | Date: 15.07.2025 11:47
Type: Answer | 
AW: [AW-236821] negativ Bestände häufen sich per Scanner (9)
Hallo Frau Pferdt,
das wäre super. Vielleicht gibt es ja doch eine Gemeinsamkeit, um es einzugrenzen und dann vielleicht auch nachvollziehbar zu bekommen. Wen Sie ein paar Daten gesammelt haben, können Sie mir dann den dump zukommen lassen? Vielen Dank.
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
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständl…
```

</details>

---

### [AW-236518] — Tastaturkürzel zur Navigation in der Schnellerfassung (TOP-Attribute)

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-236518]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 14.07.2025 12:36 |

**Description:**

> AW: [AW-236518] Tastaturkürzel zur Navigation in der Schnellerfassung (TOP-Attribute) (6) Hallo Frau Groß, hierfür ist keine Tastenbelegung konfiguriert, innerhalb der Auftragserfassung sollte dies standartmäßig funktionieren. In welcher Version arbeiten Sie zum testen und welche DLL's verwenden Sie? Mit freundlichen Grüßen | Best regards Angelique Jäckel ###EOM## Phone:  +49 641 96620 393 Mobile:  +4964196620-0 A+W Software GmbH Siemensstraße 3 35463 Fernwald Germany www.a-w.com Geschäftsführer...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Angelique Jäckel (support.cantor.de@a-w.com)
To: K.Gross@dth-tiemann.de | Date: 14.07.2025 12:36
Type: Answer | 
AW: [AW-236518] Tastaturkürzel zur Navigation in der Schnellerfassung (TOP-Attribute) (6)
Hallo Frau Groß,
hierfür ist keine Tastenbelegung konfiguriert, innerhalb der Auftragserfassung sollte dies standartmäßig funktionieren.
In welcher Version arbeiten Sie zum testen und welche DLL's verwenden Sie?

Mit freundlichen Grüßen | Best regards
Angelique Jäckel
###EOM##

Phone:  +49 641 96620 393
Mobile:  +4964196620-0
A+W Software GmbH
Siemensstraße 3
35463 Fernwald
Germany

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. S…
```

</details>

---

### [AW-236413] — Pos 3 aus Angebot kopieren / danach falsche Sprossenteilung

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-236413]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 14.07.2025 10:32 |

**Description:**

> RE: [AW-236413] Pos 3 aus Angebot kopieren / danach falsche Sprossenteilung (4) Hallo Herr Corrigeux, bei mir im Test wird die Sprossenteilung korrekt aus Position 3 übernommen. Welche DLL's verwenden Sie? Ich habe Ihnen einmal die aktuellsten DLL's auf dem FTP-Server abgelegt, bitte testen Sie damit einmal ob der Fehler weiterhin bei Ihnen auftritt und geben mir eine Rückmeldung. Mit freundlichen Grüßen | Best regards Angelique Jäckel ###EOM## Phone:  +49 641 96620 393 Mobile:  +4964196620-0 A+...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Angelique Jäckel (support.cantor.de@a-w.com)
To: Jannik.Corrigeux@aldra.de | Date: 14.07.2025 10:32
Type: Answer | 
RE: [AW-236413] Pos 3 aus Angebot kopieren / danach falsche Sprossenteilung (4)
Hallo Herr Corrigeux,
bei mir im Test wird die Sprossenteilung korrekt aus Position 3 übernommen.
Welche DLL's verwenden Sie?
Ich habe Ihnen einmal die aktuellsten DLL's auf dem FTP-Server abgelegt, bitte testen Sie damit einmal ob der Fehler weiterhin bei Ihnen auftritt und geben mir eine Rückmeldung.
Mit freundlichen Grüßen | Best regards
Angelique Jäckel
###EOM##

Phone:  +49 641 96620 393
Mobile:  +4964196620-0
A+W Software GmbH
Siemensstraße 3
35463 Fernwald
Germany

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe d…
```

</details>

---

### [AW-219248] — 7.9 - Neuer Texteditor und HTML-Tags (Crystal Reports)

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-219248]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 10.07.2025 11:29 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Stefan Rixecker
To: Stefan Rixecker | Date: 10.07.2025 11:29
Type: State changed | 
RE: [AW-219248] 7.9 - Neuer Texteditor und HTML-Tags (Crystal Reports) (65)
Tests für Leerzeilen für vor und nach einem Textbaustein.
Leerzeile wie von DRO beschrieben, jetzt: Damit funktionieren auch mehrere Leerzeilen vor und nachgestellt.
<p><font size="4">&nbsp;</font>
<p><font size="4">&nbsp;</font>
Wird eine Leerzeile aber wieder gelöscht, verliert er alle &nbsp; und die Dartstellung funktioniert wieder nicht.
<p><font size="4"></font>
<p><font size="4"></font>
Am besten verleifen die Tests mit immer eine SPACETASTE (" ") pro Zeile.
<p><font size="4"> </font>
<p><font size="4"> </font>
Markierung immer mit Cursor an den Anfang des Paragraphs der erhalten bleiben soll und dann mit SHIFT + ARROWUP den ganzen vorangehenden Paragraph löschen, dann kommt es nicht zu ungewollten Leerzeilen.
Meldung?

Force Update?
```

</details>

---

### [AW-235547] — dopellte Sprachid´s

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-235547]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 10.07.2025 10:17 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Stefan Rixecker
To: Stefan Rixecker | Date: 10.07.2025 10:17
Type: State changed | 
RE: [AW-235547] dopellte Sprachid´s (8)
Telefonat Herr Kirmse / Herr Scholz
Sie schicken einen neuen MT Dump, mit ohne doppelte SprachIDs und melden sich. Ebenso LOG Dateien.
Problembeschreibung:
1. nach erfolgreicher Reorganisation der Mehrsprachigkeit (AV + MT) weisen beide Systeme keine doppelten SprachIDs mehr auf
2. der Import (gesplittet in 2 Export-Files) läuft einmal fehlerfrei durch
3. Prüfung mit SQL Tool ergibt wieder doppelte SprachIDs durch Import
4. Wird der Import danach wieder durchgeführt läuft dieser jetzt wieder auf PK Fehler.
 
--> Dem Kunden die Anweisung mitgegeben, bitte noch einmal zu testen ob der Import beim dritten mal fehlerfrei durchläuft. (inkonsistente Datensätze)
```

</details>

---

### [AW-221001] — Cantor Programm Abstürze wegen Webview

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-221001]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 09.07.2025 16:11 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Oliver Hainz
To: Sascha Hermann | Date: 09.07.2025 16:11
Type: State changed | 
RE: [AW-221001] Cantor Programm Abstürze wegen Webview (90)
Internal meeting - CaDatBas Memory handling.
```

</details>

---

### [AW-236226] — Bitte an Herrn Horn weiterleiten

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-236226]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 09.07.2025 13:01 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Sascha Hermann
To: Dirk Horn | Date: 09.07.2025 13:01
Type: State changed | 
RE: [AW-236226] Bitte an Herrn Horn weiterleiten (3)
DH
```

</details>

---

### [AW-218866] — Error when transferring jobs to CIM

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-218866]` |
| **Status** | 🔵 In Progress |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 09.07.2025 10:30 |

**Description:**

> [AW-218866] Error when transferring jobs to CIM (17) Auch hier nochmals die Rückfrage zum Stand des Tickets. Das Thema ist täglich relevant in der Fertigung. Mit freundlichen Grüßen Kai Bieker IT-Abteilung Prozessmanager Tel.: +49 (2762) 9866-124 Fenster Türen Fassaden Hoffmann GmbH & Co. KG Fax: +49 (2762) 9866-2013 Mobil: E-Mail: K.Bieker@fenster-hoffmann.de<mailto:K.Bieker@fenster-hoffmann.de> Nicolaus-Otto-Str. 8, 57462 Olpe Web: https://www.fenster-hoffmann.de <https://www.instagram.com/fen...

<details>
<summary>View Full Conversation Thread</summary>

```
From: IPE Industrial Projects & Engineering GmbH & Co.KG (K.Bieker@fenster-hoffmann.de)
To: support.cantor.de@a-w.com | Date: 09.07.2025 10:30
Type: Request | 
[AW-218866] Error when transferring jobs to CIM (17)
Auch hier nochmals die Rückfrage zum Stand des Tickets. Das Thema ist täglich relevant in der Fertigung.

Mit freundlichen Grüßen

Kai Bieker

IT-Abteilung
Prozessmanager

Tel.:

+49 (2762) 9866-124

Fenster Türen Fassaden
Hoffmann GmbH & Co. KG

Fax:

+49 (2762) 9866-2013

Mobil:

E-Mail:

K.Bieker@fenster-hoffmann.de<mailto:K.Bieker@fenster-hoffmann.de>

Nicolaus-Otto-Str. 8, 57462 Olpe

Web:

https://www.fenster-hoffmann.de

<https://www.instagram.com/fensterhoffmann/>

<https://de-de.facebook.com/fenster.hoffmann/>

Geschäftsführer: Jens Hoffmann, Andreas Hoffmann
Fenster Türen Fassaden HOFFMANN GmbH & Co. KG, Amtsgericht Siegen HRA 7514
Komplementär: HOFFMANN Geschäftsführungs-GmbH, Amtsgericht Siegen HRB 7218
Steuer-Nr. 338/5862/4986
```

</details>

---

### [AW-234169] — [Ticket#PaX-10223050] Escaping von Sonderzeichen in Auftragstexten (PP-online)

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-234169]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 09.07.2025 07:30 |

**Description:**

> RE: Antwort: RE: Fw: [AW-234169] [Ticket#PaX-10223050] Escaping von Sonderzeichen in Auftragstexten (PP-online) (34) Hallo Herr Kerst, der Bug mit dem fehlerhaften Escaping des "<" Zeichens sollte behoben sein. Meine Tests verliefen erfolgreich. Bitte testen Sie Ihrerseits. Danke. Die neuesten DLL finden Sie auf dem Updateserver V_7_9_Unicode_Build_2024_1_0_22_Date_09_07_2025__07_29_02.zip Mit freundlichen Grüßen | Best regards Stefan Rixecker ###EOM## Phone:  +49 641 96620 393 Mobile:  +4964196...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Stefan Rixecker (support.cantor.de@a-w.com)
To: M.Kerst@pax.de | Date: 09.07.2025 07:30
Type: Answer | 
RE: Antwort: RE: Fw: [AW-234169] [Ticket#PaX-10223050] Escaping von Sonderzeichen in Auftragstexten (PP-online) (34)
Hallo Herr Kerst,
der Bug mit dem fehlerhaften Escaping des "<" Zeichens sollte behoben sein.
Meine Tests verliefen erfolgreich. Bitte testen Sie Ihrerseits. Danke.
Die neuesten DLL finden Sie auf dem Updateserver
V_7_9_Unicode_Build_2024_1_0_22_Date_09_07_2025__07_29_02.zip
Mit freundlichen Grüßen | Best regards
Stefan Rixecker
###EOM##

Phone:  +49 641 96620 393
Mobile:  +4964196620-0
A+W Software GmbH
Siemensstraße 3
35463 Fernwald
Germany

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gesta…
```

</details>

---

### [AW-236014] — AW: Cantor Audit 2024

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-236014]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 08.07.2025 10:10 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Nicole Dießel
To: Dirk Horn | Date: 08.07.2025 10:10
Type: State changed | 
RE: [AW-236014] AW: Cantor Audit 2024 (6)
-----Ursprünglicher Termin-----
Von: Martin Raßloff <martin.rassloff@fenster-mueller.de>
Gesendet: Dienstag, 8. Juli 2025 13:44
An: Dießel, Nicole
Betreff: Zugesagt: A+W Cantor Audit bei Müller+Co
Zeit: Donnerstag, 31. Juli 2025 09:00-10:00 (UTC+01:00) Amsterdam, Berlin, Bern, Rom, Stockholm, Wien.
Ort: Microsoft Teams-Besprechung
Mit freundlichen Grüßen
MARTIN RAßLOFF
Leiter Informationstechnologie

-----Ursprünglicher Termin-----
Von: Dießel, Nicole
Gesendet: Dienstag, 8. Juli 2025 10:10
An: Martin Raßloff; Horn, Dirk
Betreff: A+W Cantor Audit bei Müller+Co
Zeit: Donnerstag, 31. Juli 2025 09:00-10:00 (UTC+01:00) Amsterdam, Berlin, Bern, Rom, Stockholm, Wien.
Ort: Microsoft Teams-Besprechung
Hallo zusammen,
ich lade mal für 1 Stunde ein, auch wenn es voraussichtlich schneller geht.
Viele Grüße
Nicole
________________________________________________________________________________
Microsoft Teams Benötigen Sie Hilfe?
Jetzt an der Besprechung teilnehmen
Besp…
```

</details>

---

### [AW-233287] — Glasbestellung Menge>1 Opentrans, GlasbarcodeMode

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-233287]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 08.07.2025 08:11 |

**Description:**

> Automatische Antwort: [AW-233287] Glasbestellung Menge>1 Opentrans, GlasbarcodeMode (17) ﻿ Dies ist eine automatische Antwort. Ich bin bis einschließlich 25.07.2025 nicht im Haus. Ihre Mail wird nicht weitergeleitet, in dringenden Fällen wenden Sie sich bitte an unsere Zentrale (06561/9555-0). Mit freundlichen Grüßen i.A. Patrick Eberhard Leitung IT RITTER Fenster & Türen GmbH +49 6561 9555-711<tel:+49%206561%209555-711> +49 6561 9555-701<tel:+49%206561%209555-711> p.eberhard@ritter-fenster.de<m...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patrick Eberhard (p.eberhard@ritter-fenster.de)
To: support.cantor.de@a-w.com | Date: 08.07.2025 08:11
Type: Request | 
Automatische Antwort: [AW-233287] Glasbestellung Menge>1 Opentrans, GlasbarcodeMode (17)
﻿
Dies ist eine automatische Antwort.

Ich bin bis einschließlich 25.07.2025 nicht im Haus. Ihre Mail wird nicht weitergeleitet, in dringenden Fällen wenden Sie sich bitte an unsere Zentrale (06561/9555-0).

Mit freundlichen Grüßen

i.A. Patrick Eberhard
Leitung IT
RITTER Fenster & Türen GmbH

+49 6561 9555-711<tel:+49%206561%209555-711>

+49 6561 9555-701<tel:+49%206561%209555-711>

p.eberhard@ritter-fenster.de<mailto:p.eberhard@ritter-fenster.de>

https://www.ritter-fenster.de

Kopernikusstraße 3, 54634 Bitburg

Geschäftsführung
Werner Hardt
Stephan Graf

Gesellschaftssitz: Bitburg
HRB Wittlich 31816
USt.Id.-Nr.: DE 164 660 876
Steuer-Nr.: 10/657/0551/8

Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie d…
```

</details>

---

### [AW-230309] — Textgröße im CIM Formular ändert sich bei umgestellter Skalierung nicht

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-230309]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 07.07.2025 15:06 |

**Description:**

> RE: WG: [AW-230309] Textgröße im CIM Formular ändert sich bei umgestellter Skalierung nicht (26) Hallo Herr Nestaval, das ist wahrscheinlich im Meeting-Excel von letzter Woche untergegangen. Hier müssen wir die Basis für die Grid-Konfiguration ändern. Damit sind wir bei einer kommenden Programmversion und gehen von einem M-Paket aus. Könnten Sie mal testen, ob man die Windows-Skalierung verwenden kann. Mit freundlichen Grüßen | Best regards Sascha Hermann ###EOM## Phone:  +49 641 96620 393 Mobil...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Sascha Hermann (support.cantor.de@a-w.com)
To: horst.nestaval@schlotterer.at | Date: 07.07.2025 15:06
Type: Answer | 
RE: WG: [AW-230309] Textgröße im CIM Formular ändert sich bei umgestellter Skalierung nicht (26)
Hallo Herr Nestaval,
das ist wahrscheinlich im Meeting-Excel von letzter Woche untergegangen.
Hier müssen wir die Basis für die Grid-Konfiguration ändern. Damit sind wir bei einer kommenden Programmversion und gehen von einem M-Paket aus. Könnten Sie mal testen, ob man die Windows-Skalierung verwenden kann.
Mit freundlichen Grüßen | Best regards
Sascha Hermann
###EOM##

Phone:  +49 641 96620 393
Mobile:  +49 6404 2051 361
A+W Software GmbH
Siemensstraße 3
35463 Fernwald
Germany

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weite…
```

</details>

---

### [AW-235833] — BORNEMANN_MULTITRADE  DB einspielen

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-235833]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 07.07.2025 10:18 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Sascha Hermann
To: Wolfgang Schmid | Date: 07.07.2025 10:18
Type: State changed | 
RE: [AW-235833] BORNEMANN_MULTITRADE  DB einspielen (6)
DB importiert.
```

</details>

---

### [AW-230213] — SQL Server 2025

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-230213]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 04.07.2025 15:46 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Kerstin Heyd
To: Kerstin Heyd | Date: 04.07.2025 15:46
Type: State changed | 
RE: [AW-230213] SQL Server 2025 (9)
SQL Server zum Download bei Microsoft nicht verfügbar
ICT Ticket erstellt Ticket ID [AW-235835].
```

</details>

---

### [AW-217573] — Unterbindung von unerwünschten Anpassungen in Übersichten

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-217573]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 04.07.2025 10:23 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Stefan Rixecker
To: Stefan Rixecker | Date: 04.07.2025 10:23
Type: State changed | 
RE: [AW-217573] Unterbindung von unerwünschten Anpassungen in Übersichten (13)
Wiedervorlage, nach dem Urlaub von Herrn Grewe in KW29
```

</details>

---

### [AW-233289] — Schnittstelle Putzmaschine

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-233289]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 02.07.2025 12:00 |

**Description:**

> Automatische Antwort: [AW-233289] Schnittstelle Putzmaschine (16) Sehr geehrter Absender, ich bin ab dem 14.07.2025 wieder zu erreichen. Ihre Mail wird nicht weitergeleitet. Wenden Sie sich in dringenden Fällen bitte an unsere Zentrale 04141-491-0 Mit freundlichen Grüßen Ralf Lüdtke --------------------------------------------------------------------- Stader Glas GmbH & Co KG Am Schwingedeich 54 - 21680 Stade Tel.: 04141 491 - 110 Fax: 04141 491 - 200 EMail: R.Luedtke@StaderGlas.de<mailto:o@Stad...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Ralf Lüdtke (r.luedtke@staderglas.de)
To: support.cantor.de@a-w.com | Date: 02.07.2025 12:00
Type: Request | 
Automatische Antwort: [AW-233289] Schnittstelle Putzmaschine (16)
Sehr geehrter Absender,
ich bin ab dem 14.07.2025 wieder zu erreichen.
Ihre Mail wird nicht weitergeleitet.
Wenden Sie sich in dringenden Fällen bitte an unsere Zentrale
04141-491-0

Mit freundlichen Grüßen

Ralf Lüdtke

---------------------------------------------------------------------
Stader Glas GmbH & Co KG
Am Schwingedeich 54 - 21680 Stade
Tel.: 04141 491 - 110
Fax: 04141 491 - 200
EMail: R.Luedtke@StaderGlas.de<mailto:o@StaderGlas.de>
www.StaderGlas.de<http://www.staderglas.de/>
-------------------------------------------------------------------------------------
Amtsgericht Tostedt HRA 100075
Persönlich haftende Gesellschafterin:
Stader Glas Verwaltungs GmbH - 21680 Stade
Amtsgericht Tostedt HRB 100069
GmbH Geschäftsführer: Hans-Hermann Lemke, Dipl. -Kfm. Frank Schürmann,
--------------------------------------------------------------------

Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte…
```

</details>

---

### [AW-233459] — Migration von Oracle nach MSSQL / Problem bei BAZ-Einstellungen

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-233459]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 02.07.2025 08:17 |

**Description:**

> RE: [AW-233459] Migration von Oracle nach MSSQL / Problem bei BAZ-Einstellungen (5) Hallo Herr Seibold, konnten sie den Dump bereitstellen? Mit freundlichen Grüßen | Best regards Dirk Horn ###EOM## Phone:  +49 641 96620 393 Mobile:  +49 6404 2051 360 A+W Software GmbH Siemensstraße 3 35463 Fernwald Germany www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan Amtsgericht Gießen/Gießen Local Court: HRB 7963 Diese E-Mail ist aussch...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Dirk Horn (support.cantor.de@a-w.com)
To: rafael.seibold@weru.de | Date: 02.07.2025 08:17
Type: Answer | 
RE: [AW-233459] Migration von Oracle nach MSSQL / Problem bei BAZ-Einstellungen (5)
Hallo Herr Seibold,
konnten sie den Dump bereitstellen?
Mit freundlichen Grüßen | Best regards
Dirk Horn
###EOM##

Phone:  +49 641 96620 393
Mobile:  +49 6404 2051 360
A+W Software GmbH
Siemensstraße 3
35463 Fernwald
Germany

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus in Ihr System gelangen, haften wir nicht für die evtl. entstandenen Schäden.

This e-mail is for the inte…
```

</details>

---

### [AW-232805] — Cantor Audit 2024 - Terminvorschlag

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-232805]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 01.07.2025 10:00 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Dirk Horn
To: Axe_API | Date: 01.07.2025 10:00
Type: State changed | 
RE: [AW-232805] Cantor Audit 2024 - Terminvorschlag (5)
Termin auf 18.9. verschoben.
```

</details>

---

### [AW-234136] — Eingabmass

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-234136]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 30.06.2025 10:45 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Dirk Horn
To: Dirk Horn | Date: 30.06.2025 10:45
Type: State changed | 
RE: [AW-234136] Eingabmass (13)
Warten ob weitere Fälle auftreten.
```

</details>

---

### [AW-234215] — Aldra - Eindeutiger Key bei mehrehren RA-Profile auf einer Seite (STUERTZ2_07_ALDRA - Maschine 150)

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-234215]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 30.06.2025 10:02 |

**Description:**

> RE: [AW-234215] Aldra - Eindeutiger Key bei mehrehren RA-Profile auf einer Seite (STUERTZ2_07_ALDRA - Maschine 150) (10) Hallo Thorben. die Programmänderung für oben genannten Vorgang steht auf dem FTP-Server zum Download bereit. Wir haben die Spezifikationen des Maschinenherstellers analysiert: 1) Feld E - es kann nicht den Wert E101 oder E102 für Rahmen haben. Gemäß der Spezifikation muss es immer E100 sein. 2) Feld U - es gibt einen Kommentar: "Bei Sonderkonstruktionen für Flügel-/Rahmenteile...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Dirk Horn (support.cantor.de@a-w.com)
To: thorben.soenksen@aldra.de | Date: 30.06.2025 10:02
Type: Answer | 
RE: [AW-234215] Aldra - Eindeutiger Key bei mehrehren RA-Profile auf einer Seite (STUERTZ2_07_ALDRA - Maschine 150) (10)
Hallo Thorben.
die Programmänderung für oben genannten Vorgang steht auf dem FTP-Server zum Download bereit.
Wir haben die Spezifikationen des Maschinenherstellers analysiert:
1) Feld E - es kann nicht den Wert E101 oder E102 für Rahmen haben. Gemäß der Spezifikation muss es immer E100 sein.
2) Feld U - es gibt einen Kommentar: "Bei Sonderkonstruktionen für Flügel-/Rahmenteile, aufsteigende Nummern im Uhrzeigersinn vom oberen Profil aus". Das bedeutet, dass die Ausrichtung die Nummer sein kann.
3) Das Feld U ist ein Teil des Schlüssels.
Basierend auf der Spezifikation haben wir beschlossen, das Feld E so zu belassen wie es ist und das Feld U zu ändern. Für spezielle Fälle, in denen zwei Profile auf derselben Seite des Rahmens sind, wird der Wert des Feldes U der Profilindex sein.
Diese Änderung wurde nur für Rahmenprofile eingeführt und löst das Problem der nicht eindeutigen Schlüssel.
Gruß Dirk
Mit freundlichen Grüßen | Best regards
Dirk Horn
###EOM##

Phone:  +49 641 9…
```

</details>

---

### [AW-222571] — Ansprechpartner - Kaufmännische Abwicklung (x-Rechnung)

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-222571]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 27.06.2025 09:52 |

**Description:**

> AW: AW: AW: AW: [AW-222571] Ansprechpartner - Kaufmännische Abwicklung (x-Rechnung) (47) Hallo Herr Kell, bitte füllen sie den angehängten Dev. Request im Punkt 1 möglichst ausführlich aus. Mit freundlichen Grüßen | Best regards Sabine Weidmann ###EOM## Phone:  +49 641 96620 393 Mobile:  +49 6404 2051 362 A+W Software GmbH Siemensstraße 3 35463 Fernwald Germany www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan Amtsgericht Gie...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Sabine Weidmann (support.cantor.de@a-w.com)
To: martin.kell@unilux.de | Date: 27.06.2025 09:52
Type: Answer | 
AW: AW: AW: AW: [AW-222571] Ansprechpartner - Kaufmännische Abwicklung (x-Rechnung) (47)
Hallo Herr Kell,
bitte füllen sie den angehängten Dev. Request im Punkt 1 möglichst ausführlich aus.
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
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus in Ihr System gelangen, haften wir nicht für die evtl. e…
```

</details>

---

### [AW-217532] — Genius - Profilfarben im Druck

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-217532]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 24.06.2025 08:47 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Stefan Rixecker
To: Stefan Rixecker | Date: 24.06.2025 08:47
Type: State changed | 
RE: [AW-217532] Genius - Profilfarben im Druck (20)
Telefonat mit Herrn Grassmäher und die Sachlage erklärt. Er bespricht es mit Genius, ob Sie sie einen Dev.Request wollen. Alternativ stellt er die Texturen wieder ab. #
Warten auf Rückmeldung durch Herrn Grassmäher
```

</details>

---

### [AW-230605] — Problem with login into customer portal - GevelNed

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-230605]` |
| **Status** | 🔵 In Progress |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 04.06.2025 14:05 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Dirk Horn
To: Axe_API | Date: 04.06.2025 14:05
Type: State changed | 
RE: [AW-230605] Problem with login into customer portal - GevelNed (7)
```

</details>

---

### [AW-224562] — Cantor Wiki Suche funktioniert nicht

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-224562]` |
| **Status** | 🔵 In Progress |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 28.05.2025 12:53 |

**Description:**

> AW: [AW-224562] Support-Ticket / Cantor Wiki Suche (13) Hallo, vor über zwei Montage hatte ich gemeldet, dass die Such-Funktion im Cantor Wiki nicht funktioniert. Leider funktioniert die Suche immer noch nicht: Mit freundlichen Grüßen aus Burbach i.A. Kai Themanns - IT-Leitung - ________________________________ [FeBa_Briefbogen_Kopf] FeBa Fensterbau GmbH | Carl-Benz-Straße 23 | 57299 Burbach Tel.: 02736 497 579 E-Mail: KThemanns@feba.de<mailto:KThemanns@feba.de> | www.feba.de<http://www.feba.de/...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Kai Themanns (KThemanns@feba.de)
To: support.cantor.de@a-w.com | Date: 28.05.2025 12:53
Type: Request | 
AW: [AW-224562] Support-Ticket / Cantor Wiki Suche (13)
Hallo,

vor über zwei Montage hatte ich gemeldet, dass die Such-Funktion im Cantor Wiki nicht funktioniert.
Leider funktioniert die Suche immer noch nicht:

Mit freundlichen Grüßen aus Burbach
i.A. Kai Themanns
- IT-Leitung -
________________________________

[FeBa_Briefbogen_Kopf]

FeBa Fensterbau GmbH | Carl-Benz-Straße 23 | 57299 Burbach
Tel.: 02736 497 579
E-Mail: KThemanns@feba.de<mailto:KThemanns@feba.de> | www.feba.de<http://www.feba.de/>

Geschäftsführer: Simon Menk, Norman Menk
Handelsregister: Amtsgericht Siegen - HRB 1964

Von: Support Pohlheim Cantor <support.cantor.de@a-w.com>
Gesendet: Freitag, 21. März 2025 13:01
An: Themanns, Kai - FeBa Fensterbau GmbH <KThemanns@feba.de>
Cc: Emailsammler <Emailsammler@feba.de>
Betreff: [AW-224562] Support-Ticket / Cantor Wiki Suche

Sehr geehrte Damen und Herren,

Vielen Dank, dass Sie sich an das A+W-Support-Team gewandt haben.

Ihre Anfrage ist in unserem Ticket-S…
```

</details>

---

### [AW-223310] — Schweiker Installationsroutine 7.9

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-223310]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 27.05.2025 15:19 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Kerstin Heyd
To: Kerstin Heyd | Date: 27.05.2025 15:19
Type: State changed | 
RE: [AW-223310] Schweiker Installationsroutine 7.9 (11)
```

</details>

---

### [AW-223309] — Schweiker Update Routine 7.7 - 7.9

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-223309]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 27.05.2025 12:52 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Angelique Jäckel
To: Kerstin Heyd | Date: 27.05.2025 12:52
Type: State changed | 
RE: [AW-223309] Schweiker Update Routine 7.7 - 7.9 (15)
KHE
```

</details>

---

### [AW-229403] — Kunden Portal

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-229403]` |
| **Status** | 🔵 In Progress |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 22.05.2025 08:47 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Dirk Horn
To: Axe_API | Date: 22.05.2025 08:47
Type: State changed | 
RE: [AW-229403] Kunden Portal (8)
```

</details>

---

### [AW-229163] — Zugangsdaten zu Altbestand Dokumente

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-229163]` |
| **Status** | 🔵 In Progress |
| **Category** | Support Cantor / Support Fernwald - Cantor |
| **Last Action** | 22.05.2025 08:40 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Dirk Horn
To: Axe_API | Date: 22.05.2025 08:40
Type: State changed | 
RE: [AW-229163] Zugangsdaten zu Altbestand Dokumente (11)
```

</details>

---

## Support Poland - Cantor

### [AW-233349] — CaExport/Import - Inconsistent product class master data

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-233349]` |
| **Status** | 🔵 In Progress |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 25.07.2025 16:07 |

**Description:**

> RE: [Email extern]Re: [Email extern]CaExport/Import - Inconsistent product class master data [AW-233349] (24) Hello, 2025_07_25_CAN_QFORT_MTE.bak On ftp Best regards Ionut Botoaga IT Department Casa Noastra SRL 207450 Pielesti, Calea Bucuresti, 113 Tel.: 0728.286099 <http://www.casanoastra.ro/> www.casanoastra.ro From: Support Cantor Poland <support.cantor.pl@a-w.com> Sent: Monday, July 21, 2025 11:52 AM To: ionut.botoaga@casanoastra.ro; horia.epure@casanoastra.ro Cc: luiza.dobos@casanoastra.ro ...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Ionut Botoaga (ionut.botoaga@casanoastra.ro)
To: support.cantor.pl@a-w.com | Date: 25.07.2025 16:07
Type: Request | 
RE: [Email extern]Re: [Email extern]CaExport/Import - Inconsistent product class master data [AW-233349] (24)
Hello,

2025_07_25_CAN_QFORT_MTE.bak

On ftp

Best regards

Ionut Botoaga
IT Department
Casa Noastra SRL

207450 Pielesti, Calea Bucuresti, 113
Tel.: 0728.286099
<http://www.casanoastra.ro/> www.casanoastra.ro

From: Support Cantor Poland <support.cantor.pl@a-w.com>
Sent: Monday, July 21, 2025 11:52 AM
To: ionut.botoaga@casanoastra.ro; horia.epure@casanoastra.ro
Cc: luiza.dobos@casanoastra.ro
Subject: [Email extern]Re: [Email extern]CaExport/Import - Inconsistent product class master data [AW-233349]

EMAIL EXTERN: Acest email este din exteriorul organizației. Vă rugăm să examinați cu atenție sursa și conținutul acestuia. Nu deschideți atașamente sau link-uri suspecte. În cazul în care aveți îndoieli cu privire la autenticitatea acestuia, raportați situația departamentului IT.

Hi,

I analyzed the logs, but unfortunately, everything seems to be fine from this side - I did not find a reason why the data is not refresh…
```

</details>

---

### [AW-235247] — RE: [Email extern]RE: Order confirmation in Iquote

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-235247]` |
| **Status** | 🔵 In Progress |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 25.07.2025 16:02 |

**Description:**

> RE: [Email extern]RE: [Email extern]FW: RE: [Email extern]RE: [Email extern]RE: [Email extern]FW: RE: [Email extern]RE: [AW-235247] RE: [Email extern]RE: Order confirmation in Iquote (18) Hello, It looks ok from what we teste until new. Best regards Ionut Botoaga IT Department Casa Noastra SRL 207450 Pielesti, Calea Bucuresti, 113 Tel.: 0728.286099 <http://www.casanoastra.ro/> www.casanoastra.ro From: Support Cantor Poland <support.cantor.pl@a-w.com> Sent: Thursday, July 24, 2025 3:03 PM To: ion...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Ionut Botoaga (ionut.botoaga@casanoastra.ro)
To: support.cantor.pl@a-w.com | Date: 25.07.2025 16:02
Type: Request | 
RE: [Email extern]RE: [Email extern]FW: RE: [Email extern]RE: [Email extern]RE: [Email extern]FW: RE: [Email extern]RE: [AW-235247] RE: [Email extern]RE: Order confirmation in Iquote (18)
Hello,

It looks ok from what we teste until new.

Best regards

Ionut Botoaga
IT Department
Casa Noastra SRL

207450 Pielesti, Calea Bucuresti, 113
Tel.: 0728.286099
<http://www.casanoastra.ro/> www.casanoastra.ro

From: Support Cantor Poland <support.cantor.pl@a-w.com>
Sent: Thursday, July 24, 2025 3:03 PM
To: ionut.botoaga@casanoastra.ro
Subject: [Email extern]RE: [Email extern]FW: RE: [Email extern]RE: [Email extern]RE: [Email extern]FW: RE: [Email extern]RE: [AW-235247] RE: [Email extern]RE: Order confirmation in Iquote

EMAIL EXTERN: Acest email este din exteriorul organizației. Vă rugăm să examinați cu atenție sursa și conținutul acestuia. Nu deschideți atașamente sau link-uri suspecte. În cazul în care aveți îndoieli cu privire la autenticitatea acestuia, raportați situația departamentului IT.

Please try again - I fixed the problem.

The Reason was that someone changed data for connection (in prodconf 25):

S…
```

</details>

---

### [AW-237976] — DOMEL - zaślepki do odwodnien

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-237976]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 25.07.2025 15:48 |

**Description:**

> RE: [AW-237976] DOMEL - zaślepki do odwodnien (5) Cześć Darek, Ten warunek, który widzisz rozróżnia typy zleceń. Akurat wprowadziłeś zlecenie testowe "T", a on do niego nie dorzuci zaślepek, tylko do zleceń "N" i "P". Nie wiem czy jest w ogóle to Wam do czegoś potrzebne? Chyba możemy to wywalić, no chyba, że po coś to było zrobione. W tym warunku, który jest wykorzystany sprawdzamy AUSSENUNTEN=1 czyli zaślepki powstaną tylko dla kwater na samym dole. W tym przykładzie 4-kwaterowego okna z FIXami...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Damian Mizerny (support.cantor.pl@a-w.com)
To: dariusz.zabielski@domel.pl | Date: 25.07.2025 15:48
Type: Answer | 
RE: [AW-237976] DOMEL - zaślepki do odwodnien (5)
Cześć Darek,
Ten warunek, który widzisz rozróżnia typy zleceń. Akurat wprowadziłeś zlecenie testowe "T", a on do niego nie dorzuci zaślepek, tylko do zleceń "N" i "P". Nie wiem czy jest w ogóle to Wam do czegoś potrzebne? Chyba możemy to wywalić, no chyba, że po coś to było zrobione.
W tym warunku, który jest wykorzystany sprawdzamy AUSSENUNTEN=1 czyli zaślepki powstaną tylko dla kwater na samym dole. W tym przykładzie 4-kwaterowego okna z FIXami, zaślepki generują się tylko dla dolnych dwóch kwater.
 
Kolejna sprawa to ilość. Macie formułę, która zlicza ile ma być tych zaślepek w specyfikacji do 2810. Dla kwatery poniżej szerokości 200mm będzie to 1 zaślepka. Dla kwatery powyżej 200mm szerokości będą 2 zaślepki, 3 będą powyżej 1100, a 4 powyżej 2110.

Z tego co widzę to na obróbkach macie właściwie możliwe 1, 2 lub 3 odwodnienia i są one robione na każdej kwaterze w dolnym profilu ramy/słupka.

Ilość odwodnień na obróbkach sprawdzacie za pomocą poniższej funkcji, czyli dla ko…
```

</details>

---

### [AW-238175] — Problem odnośnie AW-237332

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-238175]` |
| **Status** | 🟡 New |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 25.07.2025 14:42 |

**Description:**

> Problem odnośnie AW-237332 (1) Cześć Mimo, że poprawka którą otrzymaliśmy od was nie działa to zgłoszenie AW-237332 zostało zamknięte (oznaczone jako dostarczone). Proszę o kontynuację tematu i naprawę błędu.

<details>
<summary>View Full Conversation Thread</summary>

```
From: Piotr Płotek (pplotek@drutex.com.pl)
To: support.cantor.pl@a-w.com | Date: 25.07.2025 14:42
Type: Request | 
Problem odnośnie AW-237332 (1)
Cześć

Mimo, że poprawka którą otrzymaliśmy od was nie działa to zgłoszenie
AW-237332 zostało zamknięte (oznaczone jako dostarczone). Proszę o
kontynuację tematu i naprawę błędu.
```

</details>

---

### [AW-237837] — Ceny - błąd w różnicy ZAK/SPD

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-237837]` |
| **Status** | 🔵 In Progress |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 25.07.2025 14:20 |

**Description:**

> Re: [AW-237837] Ceny - błąd w różnicy ZAK/SPD (3) Hej, my nic nie zmienialiśmy. Być może Marcin coś robił na sesji z Michałem Hawro, ponieważ oni zajmują się cennikami, ale tego dowiemy się w poniedziałek, dzisiaj Marcin jest na urlopie. Pozdrawiam Jacek Kreft Inżynier ds. oprogramowania <https://www.drutex.eu/> *PL:* + 48 59 822 91 01 | *Fax:* + 48 59 822 91 03 DRUTEX S.A. Lęborska 31 | Bytów 77-100 | Polska NIP 8‌42 1‌6 2‌2 7‌20 www.drutex.eu <https://www.drutex.eu/> <https://www.facebook.com/...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Jacek Kreft (jkreft@drutex.com.pl)
To: support.cantor.pl@a-w.com | Date: 25.07.2025 14:20
Type: Request | 
Re: [AW-237837] Ceny - błąd w różnicy ZAK/SPD (3)
Hej,

my nic nie zmienialiśmy. Być może Marcin coś robił na sesji z Michałem
Hawro, ponieważ oni zajmują się cennikami, ale tego dowiemy się w
poniedziałek, dzisiaj Marcin jest na urlopie.

Pozdrawiam

Jacek Kreft

Inżynier ds. oprogramowania

<https://www.drutex.eu/>

*PL:* + 48 59 822 91 01 | *Fax:* + 48 59 822 91 03

DRUTEX S.A.

Lęborska 31 | Bytów 77-100 | Polska
NIP 8‌42 1‌6 2‌2 7‌20
www.drutex.eu <https://www.drutex.eu/>

<https://www.facebook.com/DrutexSA/>
<http://www.instagram.com/drutex_com/>

<https://www.drutex.pl/pl/produkty/d-gate.html>

DRUTEX S.A. z siedzibą w Bytowie zarejestrowany został w Krajowym
Rejestrze Sądowym pod nr 0000140428 prowadzonym przez Sąd Rejonowy VIII
Wydział Gospodarczy Krajowego Rejestru Sądowego w Gdańsku. BDO
0‌00001469. Kapitał zakładowy, opłacony DRUTEX S.A. wynosi 21.690.000,00 zł

DRUTEX S.A. oświadcza, że posiada status dużego przedsiębiorcy w
rozumieniu Ustawy z dnia 8 marca 2013 r. o przeciwdział…
```

</details>

---

### [AW-237781] — [ZEWNĘTRZNE] Dealer - błąd podczas wysyłania zamówienia

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-237781]` |
| **Status** | 🔵 In Progress |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 25.07.2025 14:10 |

**Description:**

> Re: [AW-237781] [ZEWNĘTRZNE] Dealer - błąd podczas wysyłania zamówienia (3) Hej, temat do zamknięcia. Pozdrawiam Jacek Kreft Inżynier ds. oprogramowania <https://www.drutex.eu/> *PL:* + 48 59 822 91 01 | *Fax:* + 48 59 822 91 03 DRUTEX S.A. Lęborska 31 | Bytów 77-100 | Polska NIP 8‌42 1‌6 2‌2 7‌20 www.drutex.eu <https://www.drutex.eu/> <https://www.facebook.com/DrutexSA/> <http://www.instagram.com/drutex_com/> <https://www.drutex.pl/pl/produkty/d-gate.html> DRUTEX S.A. z siedzibą w Bytowie zarej...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Jacek Kreft (jkreft@drutex.com.pl)
To: support.cantor.pl@a-w.com | Date: 25.07.2025 14:10
Type: Request | 
Re: [AW-237781] [ZEWNĘTRZNE] Dealer - błąd podczas wysyłania zamówienia (3)
Hej,

temat do zamknięcia.

Pozdrawiam

Jacek Kreft

Inżynier ds. oprogramowania

<https://www.drutex.eu/>

*PL:* + 48 59 822 91 01 | *Fax:* + 48 59 822 91 03

DRUTEX S.A.

Lęborska 31 | Bytów 77-100 | Polska
NIP 8‌42 1‌6 2‌2 7‌20
www.drutex.eu <https://www.drutex.eu/>

<https://www.facebook.com/DrutexSA/>
<http://www.instagram.com/drutex_com/>

<https://www.drutex.pl/pl/produkty/d-gate.html>

DRUTEX S.A. z siedzibą w Bytowie zarejestrowany został w Krajowym
Rejestrze Sądowym pod nr 0000140428 prowadzonym przez Sąd Rejonowy VIII
Wydział Gospodarczy Krajowego Rejestru Sądowego w Gdańsku. BDO
0‌00001469. Kapitał zakładowy, opłacony DRUTEX S.A. wynosi 21.690.000,00 zł

DRUTEX S.A. oświadcza, że posiada status dużego przedsiębiorcy w
rozumieniu Ustawy z dnia 8 marca 2013 r. o przeciwdziałaniu nadmiernym
opóźnieniom w transakcjach handlowych (Dz. U. z 2013 r., poz. 403 ze zm.).

Administratorem danych osobowych przetwarzanych w związku z prowadzoną…
```

</details>

---

### [AW-234614] — Problem with HTML in widget translations

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-234614]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 25.07.2025 13:21 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Stefan Rixecker
To: | Date: 25.07.2025 13:21
Type: State changed | 
RE: [AW-234614] Problem with HTML in widget translations (5)
LL
```

</details>

---

### [AW-238142] — Jak usunąć cenę ustawioną recznie?

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-238142]` |
| **Status** | 🟡 New |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 25.07.2025 13:06 |

**Description:**

> Jak usunąć cenę ustawioną recznie? (1) Cześć Jak usunąć taką cenę?  Jeśli wejdziemy do kalkulacji kosztów i zapiszemy cenę z kosztów niebieskim przyciskiem to potem nie da się w żaden sposób obliczyć standardowo. Usuń ceny nie działa, oblicz ceny nie działa - jak ktoś przypadkiem zrobi o mona całą ofertę wyrzucić. Pozdrawiam, Marek Gwozdz IT Manager Dział IT mobile: 663 442 325 email: m.gwozdz@budvar.pl tel.: +48 43 824 31 32 wew. 262 <https://www.budvar.pl/> <https://www.budvarcentrum.pl/typ-pr...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Marek Gwozdz (m.gwozdz@budvar.pl)
To: support.cantor.pl@a-w.com | Date: 25.07.2025 13:06
Type: Request | 
Jak usunąć cenę ustawioną recznie? (1)
Cześć

Jak usunąć taką cenę?  Jeśli wejdziemy do kalkulacji kosztów i zapiszemy cenę z kosztów niebieskim przyciskiem to potem nie da się w żaden sposób obliczyć standardowo.
Usuń ceny nie działa, oblicz ceny nie działa - jak ktoś przypadkiem zrobi o mona całą ofertę wyrzucić.

       Pozdrawiam,

Marek Gwozdz
IT Manager
Dział IT

mobile: 663 442 325
email: m.gwozdz@budvar.pl
tel.: +48 43 824 31 32 wew. 262

<https://www.budvar.pl/>

<https://www.budvarcentrum.pl/typ-produktu/drzwi-wejsciowe-aluminiowe/>

<https://www.budvarcentrum.pl>

<https://www.budvarcentrum.pl/>

<https://www.budvarcentrum.pl/>

<https://www.budvarcentrum.pl/><https://www.budvarcentrum.pl/>

<https://www.budvarcentrum.pl/><https://www.budvarcentrum.pl/produkt/okna-pvc/t-passive-perfekt/><https://katalog.grupamtp.pl/pl?oid=1588647&ec=T132301&ec=T992301><https://www.budvarcentrum.pl/typ-produktu/ok…
```

</details>

---

### [AW-237059] — orders locked by SPOOLER

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-237059]` |
| **Status** | 🔵 In Progress |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 25.07.2025 11:27 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Oskar Bielejewski
To: | Date: 25.07.2025 11:27
Type: State changed | 
RE: [AW-237059] orders locked by SPOOLER (5)
```

</details>

---

### [AW-238112] — Filtr wyszukiwania pochodzenia ofert/zleceń

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-238112]` |
| **Status** | 🟡 New |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 25.07.2025 10:42 |

**Description:**

> Filtr wyszukiwania pochodzenia ofert/zleceń (1) Witam, U nas na stanowiskach tworzymy dla jednego klienta kilka ofert (wersje). Klient wybiera jedną z nich. Wtedy z tej wybranej oferty robimy kopie i podnosi się nowy rekord jako zlecenie. W tym zleceniu w kolumnie Ref pojawia się numer z której to oferty przyszło. Ok. To jest super, ale na liście ofert nie mogę znaleźć znacznika, czy ta Oferta została przekształcona do Zlecenia. Filtr jak powyżej super rozróżnia rekordy, jako "skąd i co przyszło...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Ireneusz Iwańca (iiwanca@drutex.com.pl)
To: support.cantor.pl@a-w.com | Date: 25.07.2025 10:42
Type: Request | 
Filtr wyszukiwania pochodzenia ofert/zleceń (1)
Witam,

U nas na stanowiskach tworzymy dla jednego klienta kilka ofert (wersje).
Klient wybiera jedną z nich. Wtedy z tej wybranej oferty robimy kopie i
podnosi się nowy rekord jako zlecenie. W tym zleceniu w kolumnie Ref
pojawia się numer z której to oferty przyszło. Ok. To jest super, ale na
liście ofert nie mogę znaleźć znacznika, czy ta Oferta została
przekształcona do Zlecenia.

Filtr jak powyżej super rozróżnia rekordy, jako "skąd i co przyszło" ale
nie ma chyba tej funkcjonalności o którą pytam.
Czy jest możliwość takiego filtrowania, aby Oferty przekształcone do
Zlecenia miały taki znacznik?

Pozdrawiam

Ireneusz Iwańca

Specjalista ds. IT

<https://www.drutex.eu/>

*PL:* + 48 59 822 91 01 | *Fax:* + 48 59 822 91 03

DRUTEX S.A.

Lęborska 31 | Bytów 77-100 | Polska
NIP 8‌42 1‌6 2‌2 7‌20
www.drutex.eu <https://www.drutex.eu/>

<https://www.facebook.com/DrutexSA/>
<http://www.instagram.com/drutex_com/>

<https://www.drutex.pl/pl/produkt…
```

</details>

---

### [AW-236926] — Wielokolorowy próg

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-236926]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 25.07.2025 10:37 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Damian Mizerny
To: Damian Mizerny | Date: 25.07.2025 10:37
Type: State changed | 
Wielokolorowy próg (6)
Ten drugi ticket, ten sam problem.
```

</details>

---

### [AW-238108] — Wymiarowanie skrzydeł

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-238108]` |
| **Status** | 🟡 New |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 25.07.2025 10:26 |

**Description:**

> Wymiarowanie skrzydeł (1) Cześć, Czy jest opcja, aby zablokować w programie podział skrzydeł z wartościami dziesiętnymi? Pozdrawiam, Marta Kosecka Technolog ds. Systemów Wycen Dział IT mobile: 697 400 481 email: m.kosecka@budvar.pl tel.: +48 43 824 31 32 wew. 262 <https://www.budvar.pl/> <https://www.budvarcentrum.pl/typ-produktu/drzwi-wejsciowe-aluminiowe/> <https://www.budvarcentrum.pl> <https://www.budvarcentrum.pl/> <https://www.budvarcentrum.pl/> <https://www.budvarcentrum.pl/><https://www....

<details>
<summary>View Full Conversation Thread</summary>

```
From: Marta Kosecka (m.kosecka@budvar.pl)
To: support.cantor.pl@a-w.com | Date: 25.07.2025 10:26
Type: Request | 
Wymiarowanie skrzydeł (1)
Cześć,
Czy jest opcja, aby zablokować w programie podział skrzydeł z wartościami dziesiętnymi?

  Pozdrawiam,
Marta Kosecka
Technolog ds. Systemów Wycen
Dział IT

mobile: 697 400 481
email: m.kosecka@budvar.pl
tel.: +48 43 824 31 32 wew. 262

<https://www.budvar.pl/>

<https://www.budvarcentrum.pl/typ-produktu/drzwi-wejsciowe-aluminiowe/>

<https://www.budvarcentrum.pl>

<https://www.budvarcentrum.pl/>

<https://www.budvarcentrum.pl/>

<https://www.budvarcentrum.pl/><https://www.budvarcentrum.pl/>

<https://www.budvarcentrum.pl/><https://www.budvarcentrum.pl/produkt/okna-pvc/t-passive-perfekt/><https://katalog.grupamtp.pl/pl?oid=1588647&ec=T132301&ec=T992301><https://www.budvarcentrum.pl/typ-produktu/okna-aluminiowe/>

Administratorem danych osobowych jest BUDVAR Sp. z o.o. z siedzibą w Warszawie, Przetwarzamy dane osobowe w …
```

</details>

---

### [AW-237134] — Kopia bazy przesłana na ftp.

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-237134]` |
| **Status** | 🔵 In Progress |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 25.07.2025 10:10 |

**Description:**

> RE: [AW-237134] Kopia bazy przesłana na ftp. (6) Anulowaliśmy już zlecenie, więc będzie problem z kopią do analizy. Pozdrawiam Jakub Alachamowicz From: Support Cantor Poland <support.cantor.pl@a-w.com> Sent: Thursday, July 24, 2025 12:08 PM To: jakub.alachamowicz@domel.pl Subject: RE: [AW-237134] Kopia bazy przesłana na ftp. Dzień dobry. Zwracam się do Państwa z prośbą o ponowne wgranie backupu bazy danych w celu podjęcia analizy przypadku. Serdecznie pozdrawiam Oskar Bielejewski ###EOM## Phone:...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Jakub Alachamowicz (jakub.alachamowicz@domel.pl)
To: support.cantor.pl@a-w.com | Date: 25.07.2025 10:10
Type: Request | 
RE: [AW-237134] Kopia bazy przesłana na ftp. (6)
Anulowaliśmy już zlecenie, więc będzie problem z kopią do analizy.

Pozdrawiam

Jakub Alachamowicz

From: Support Cantor Poland <support.cantor.pl@a-w.com>
Sent: Thursday, July 24, 2025 12:08 PM
To: jakub.alachamowicz@domel.pl
Subject: RE: [AW-237134] Kopia bazy przesłana na ftp.

Dzień dobry.

Zwracam się do Państwa z prośbą o ponowne wgranie backupu bazy danych w celu podjęcia analizy przypadku.

Serdecznie pozdrawiam

Oskar Bielejewski
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com <mailto:support.pl@a-w.com>

A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

<http://www.a-w.com/> www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963

 _____  

Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder re…
```

</details>

---

### [AW-234565] — VPI - adjustment of SFMC#2

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-234565]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 25.07.2025 09:11 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Sascha Hermann
To: Damian Mizerny | Date: 25.07.2025 09:11
Type: State changed | 
RE: [AW-234565] VPI - adjustment of SFMC#2 (8)
DM
```

</details>

---

### [AW-238097] — Błąd z cenami na wydruku marża

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-238097]` |
| **Status** | 🟡 New |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 25.07.2025 09:11 |

**Description:**

> Błąd z cenami na wydruku marża (1) Witam, Zauważyliśmy pewien błąd na Dealer, jak wycenimy coś połączonego na łącznik i policzymy marże to na ofercie przy pozycji wyświetla się cena zakupu zamiast ceny sprzedaży (z marżą). Proszę o naprawienie tego błędu. Pozdrawiam Ireneusz Iwańca Specjalista ds. IT <https://www.drutex.eu/> *PL:* + 48 59 822 91 01 | *Fax:* + 48 59 822 91 03 DRUTEX S.A. Lęborska 31 | Bytów 77-100 | Polska NIP 8‌42 1‌6 2‌2 7‌20 www.drutex.eu <https://www.drutex.eu/> <https://www....

<details>
<summary>View Full Conversation Thread</summary>

```
From: Ireneusz Iwańca (iiwanca@drutex.com.pl)
To: support.cantor.pl@a-w.com | Date: 25.07.2025 09:11
Type: Request | 
Błąd z cenami na wydruku marża (1)
Witam,

Zauważyliśmy pewien błąd na Dealer, jak wycenimy coś połączonego na
łącznik i policzymy marże to na ofercie przy pozycji wyświetla się cena
zakupu zamiast ceny sprzedaży (z marżą). Proszę o naprawienie tego błędu.

Pozdrawiam

Ireneusz Iwańca

Specjalista ds. IT

<https://www.drutex.eu/>

*PL:* + 48 59 822 91 01 | *Fax:* + 48 59 822 91 03

DRUTEX S.A.

Lęborska 31 | Bytów 77-100 | Polska
NIP 8‌42 1‌6 2‌2 7‌20
www.drutex.eu <https://www.drutex.eu/>

<https://www.facebook.com/DrutexSA/>
<http://www.instagram.com/drutex_com/>

<https://www.drutex.pl/pl/produkty/d-gate.html>

DRUTEX S.A. z siedzibą w Bytowie zarejestrowany został w Krajowym
Rejestrze Sądowym pod nr 0000140428 prowadzonym przez Sąd Rejonowy VIII
Wydział Gospodarczy Krajowego Rejestru Sądowego w Gdańsku. BDO
0‌00001469. Kapitał zakładowy, opłacony DRUTEX S.A. wynosi 21.690.000,00 zł

DRUTEX S.A. oświadcza, że posiada status dużego przedsiębiorcy w
rozumieniu Ustawy z dnia 8 …
```

</details>

---

### [AW-237284] — Best Practice Performance

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-237284]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 25.07.2025 09:01 |

**Description:**

> Automatyczna odpowiedź: [EXT] RE: [AW-237284] Best Practice Performance (4) Dzień dobry, W dniu 25.07.2025 przebywam na urlopie. Na wszytkie wiadomości odpowiem po powrocie. Waldemar Korbik KRISHOME Sp. z o.o., ul. Budowlana 1, Psary Małe, 62-300 Września, tel. +48 61 639 86 88, fax +48 436 76 48, e-mail: biuro@krishome.eu, NIP PL 7891787470, KRS 0000768528, Kapitał zakładowy 26 050 000 PLN [https://krishome.pl/stopka/promo.png]  <https://eu1.hubs.ly/H0dpQ270> Uwaga: ten e-mail jest przeznaczony...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Waldemar Korbik (w.korbik@krishome.eu)
To: support.cantor.pl@a-w.com | Date: 25.07.2025 09:01
Type: Request | 
Automatyczna odpowiedź: [EXT] RE: [AW-237284] Best Practice Performance (4)
Dzień dobry,
W dniu 25.07.2025 przebywam na urlopie.

Na wszytkie wiadomości odpowiem po powrocie.

Waldemar Korbik

KRISHOME Sp. z o.o., ul. Budowlana 1, Psary Małe, 62-300 Września, tel. +48 61 639 86 88, fax +48 436 76 48, e-mail: biuro@krishome.eu,
NIP PL 7891787470, KRS 0000768528, Kapitał zakładowy 26 050 000 PLN [https://krishome.pl/stopka/promo.png]  <https://eu1.hubs.ly/H0dpQ270> Uwaga: ten e-mail jest przeznaczony wyłącznie dla adresata, może zawierać informacje zastrzeżone i prawnie zastrzeżone. Jeżeli otrzymałeś/aś tę wiadomość e-mail przez pomyłkę, powiadom nadawcę i usuń tę wiadomość e-mail wraz ze wszystkimi załącznikami.
```

</details>

---

### [AW-236541] — Report 700 is missing some data in the database

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-236541]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 25.07.2025 08:32 |

**Description:**

> Re: [AW-236541] Re: Raport 700 brak danych w bazie print (18) Cześć, Zmiany wprowadzone na devie przeniosą się podczas migracji. Jedno małe sprostowanie odnośnie zmian w prodconf. Nie wprowadzajcie tych zmian w pliku ini tylko z poziomu bazy, dodatkowo należy zmienić również wartość na 1 dla handcof 1121. Serdecznie pozdrawiam Lukasz Lieske ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września ...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Lukasz Lieske (support.cantor.pl@a-w.com)
To: mmedwid@drutex.com.pl | Date: 25.07.2025 08:32
Type: Answer | 
Re: [AW-236541] Re: Raport 700 brak danych w bazie print (18)
Cześć,
Zmiany wprowadzone na devie przeniosą się podczas migracji.
Jedno małe sprostowanie odnośnie zmian w prodconf. Nie wprowadzajcie tych zmian w pliku ini tylko z poziomu bazy, dodatkowo należy zmienić również wartość na 1 dla handcof 1121.
Serdecznie pozdrawiam
Lukasz Lieske
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestatt…
```

</details>

---

### [AW-237971] — Rysunek rolety

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-237971]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 25.07.2025 08:15 |

**Description:**

> RE: [AW-237971] Rysunek rolety (4) Dzień dobry. Przypuszczalnie jest to możliwe. Prawdodpodobnie jest to temat na konsultacje, więc jeśli jest taka potrzeba, to proszę dać znać w odpowiedzi na tę wiadomość, a ja przekażę temat do działu PS. Serdecznie pozdrawiam Oskar Bielejewski ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric He...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Oskar Bielejewski (support.cantor.pl@a-w.com)
To: lukasz.urwanowicz@witraz.eu | Date: 25.07.2025 08:15
Type: Answer | 
RE: [AW-237971] Rysunek rolety (4)
Dzień dobry.
Przypuszczalnie jest to możliwe. Prawdodpodobnie jest to temat na konsultacje, więc jeśli jest taka potrzeba, to proszę dać znać w odpowiedzi na tę wiadomość, a ja przekażę temat do działu PS.
 
Serdecznie pozdrawiam
Oskar Bielejewski
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden …
```

</details>

---

### [AW-237939] — 361510 - kolory łączników Schuco

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-237939]` |
| **Status** | 🔵 In Progress |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 24.07.2025 11:16 |

**Description:**

> RE: [AW-237939] 361510 - kolory łączników Schuco (4) Pozdrawiam, Marta Kosecka Technolog ds. Systemów Wycen Dział IT mobile: 697 400 481 email: m.kosecka@budvar.pl tel.: +48 43 824 31 32 wew. 262 <https://www.budvar.pl/> <https://www.budvarcentrum.pl/typ-produktu/drzwi-wejsciowe-aluminiowe/> <https://www.budvarcentrum.pl> <https://www.budvarcentrum.pl/> <https://www.budvarcentrum.pl/> <https://www.budvarcentrum.pl/><https://www.budvarcentrum.pl/> <https://www.budvarcentrum.pl/><https://www.budva...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Marta Kosecka (m.kosecka@budvar.pl)
To: support.cantor.pl@a-w.com | Date: 24.07.2025 11:16
Type: Request | 
RE: [AW-237939] 361510 - kolory łączników Schuco (4)

  Pozdrawiam,
Marta Kosecka
Technolog ds. Systemów Wycen
Dział IT

mobile: 697 400 481
email: m.kosecka@budvar.pl
tel.: +48 43 824 31 32 wew. 262

<https://www.budvar.pl/>

<https://www.budvarcentrum.pl/typ-produktu/drzwi-wejsciowe-aluminiowe/>

<https://www.budvarcentrum.pl>

<https://www.budvarcentrum.pl/>

<https://www.budvarcentrum.pl/>

<https://www.budvarcentrum.pl/><https://www.budvarcentrum.pl/>

<https://www.budvarcentrum.pl/><https://www.budvarcentrum.pl/produkt/okna-pvc/t-passive-perfekt/><https://katalog.grupamtp.pl/pl?oid=1588647&ec=T132301&ec=T992301><https://www.budvarcentrum.pl/typ-produktu/okna-aluminiowe/>

Administratorem danych osobowych jest BUDVAR Sp. z o.o. z siedzibą w Warszawie, Przetwarzamy dane osobowe w celu kontaktu lub realizacji usługi. Kontakt w sprawach ochrony danych osobowych możliwy jest pod a…
```

</details>

---

### [AW-232998] — CANTOR 7.8 (DLL 2023.1.0.69) - wydruki potwierdzeń na MT generują wpisy na spooler

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-232998]` |
| **Status** | 🔵 In Progress |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 24.07.2025 11:16 |

**Description:**

> RE: [AW-232998] CANTOR 7.8 (DLL 2023.1.0.69) - wydruki potwierdzeń na MT generują wpisy na spooler (8) Cześć, Sprawdziłem temat i ten prodconf nie pomaga - sprawdziłem na wartości 0, 1, 2. Obecnie jesteśmy na 7.9, DLL 2024.1.0.20 ________________________________________ Paweł Stojek Kierownik Działu IT / Head of IT department M  +48 798 831 409 E   p.stojek@krispol.pl<mailto:p.stojek@krispol.pl> From: Support Cantor Poland <support.cantor.pl@a-w.com> Sent: Tuesday, July 15, 2025 11:03 AM To: Paw...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Paweł Stojek (P.Stojek@krispol.pl)
To: support.cantor.pl@a-w.com | Date: 24.07.2025 11:16
Type: Request | 
RE: [AW-232998] CANTOR 7.8 (DLL 2023.1.0.69) - wydruki potwierdzeń na MT generują wpisy na spooler (8)
Cześć,
Sprawdziłem temat i ten prodconf nie pomaga - sprawdziłem na wartości 0, 1, 2.

Obecnie jesteśmy na 7.9, DLL 2024.1.0.20

________________________________________

Paweł Stojek
Kierownik Działu IT / Head of IT department
M  +48 798 831 409
E   p.stojek@krispol.pl<mailto:p.stojek@krispol.pl>

From: Support Cantor Poland <support.cantor.pl@a-w.com>
Sent: Tuesday, July 15, 2025 11:03 AM
To: Paweł Stojek <P.Stojek@krispol.pl>
Subject: RE: [AW-232998] CANTOR 7.8 (DLL 2023.1.0.69) - wydruki potwierdzeń na MT generują wpisy na spooler

Musisz wpisać tylko ten który chcesz nadpisać

Serdecznie pozdrawiam

Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com<mailto:support.pl@a-w.com>

A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com<http://www.a-w.com/>

Geschäftsführer/Managing Directo…
```

</details>

---

### [AW-234897] — Class as accessory is not available for choosing for users in group 1013 (meanwhile working fine for supervisor)

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-234897]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 23.07.2025 17:05 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Stefan Rixecker
To: Radoslaw Jaruszewski | Date: 23.07.2025 17:05
Type: State changed | 
RE: [AW-234897]  Class as accessory is not available for choosing for users in group 1013 (meanwhile working fine for supervisor) (19)
The reason why product class 2005 is not visible for USER of site 1030, is because class 2005 is assigned to site 1060 in MT!

There is a doubling of product class 2005 between ERP and MT, because of NOT seperated number ranges for product classes.
It seems to be the matter of fact, that QFORT were testing with basic products for dealers for one site 1060.
Afterwards creating new product class 2005 in the AV system, exported it to Multitrade System, where it kept it's assignment to site 1060.

Checklist to solve this is
1. GoTo Site - Generate Site Article Classes (checkable in ARTKLMANDANT)
Delete assignments by unchecking box (program behaves a little bit strange but do not crash),
(if it's not possible to uncheck, there are products of this class in product master which have to be deleted first)
@Radek
together we solved this by deleting relevant dataset from table ARTKLMANDANT. Afterwards it worked in lookup-help of order.
 
2. To prevent this in future you have to se…
```

</details>

---

### [AW-237819] — Wydruk ofertowy

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-237819]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 23.07.2025 13:54 |

**Description:**

> RE: [AW-237819] Wydruk ofertowy (2) Dzień dobry. Nie jest to możliwe. Serdecznie pozdrawiam Oskar Bielejewski ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan Amtsgericht Gießen/Gießen Local Court: HRB 7963 Diese E-Mail ist ausschließlich für den Adressaten bestim...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Oskar Bielejewski (support.cantor.pl@a-w.com)
To: iiwanca@drutex.com.pl | Date: 23.07.2025 13:54
Type: Answer | 
RE: [AW-237819] Wydruk ofertowy (2)
Dzień dobry.
 
Nie jest to możliwe.
 
Serdecznie pozdrawiam
Oskar Bielejewski
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus in Ihr System gelangen, haften wir nicht für die evtl. entstandenen Schäden.

This e…
```

</details>

---

### [AW-237045] — Problem with short code for French Mullion

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-237045]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 23.07.2025 13:26 |

**Description:**

> FW: [AW-237045] Problem with short from French Mullion (7.9 vs 7.8) (15) Hello Billel, translation was corrected in today's dll build (available on FTP). Please let me know if it's fine for you. Serdecznie pozdrawiam Radoslaw Jaruszewski ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark T...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Radoslaw Jaruszewski (support.cantor.pl@a-w.com)
To: billel.benmakhlouf@oxxo.dz | Date: 23.07.2025 13:26
Type: Answer | 
FW: [AW-237045] Problem with short from French Mullion (7.9 vs 7.8) (15)
Hello Billel,
translation was corrected in today's dll build (available on FTP).
Please let me know if it's fine for you.
Serdecznie pozdrawiam
Radoslaw Jaruszewski
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus …
```

</details>

---

### [AW-237777] — [ZEWNĘTRZNE] Ilość materiału w rezerwacji JOB 4460

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-237777]` |
| **Status** | 🟡 New |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 23.07.2025 12:58 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Sascha Hermann
To: | Date: 23.07.2025 12:58
Type: State changed | 
RE: [AW-237777] [ZEWNĘTRZNE] Ilość materiału w rezerwacji JOB 4460 (3)
```

</details>

---

### [AW-232245] — Limit for items generated from price matrix (1000) on 64bit Cantor version

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-232245]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 23.07.2025 11:16 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Jessica Renno
To: Radoslaw Jaruszewski | Date: 23.07.2025 11:16
Type: State changed | 
RE: [AW-232245] Limit for items generated from price matrix (1000) on 64bit Cantor version (16)
just for clarification
in 32 bit version like 7.9.1: Removing the limit does not mean the functionality will work. the exact number depends on the master data and complexity of the unit
```

</details>

---

### [AW-237810] — Liczniki na CIM

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-237810]` |
| **Status** | 🟡 New |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 23.07.2025 11:11 |

**Description:**

> Liczniki na CIM (1) Cześć, Nie działają nam liczniki na CIM’ach. Cały czas pokazują 0. Jak je włączyć? Np. PVC – Okuwanie ramy - licznik chcielibyśmy dodać na CIM 20425 - Okuwanie ram. Z poważaniem / Mit freundlichen Grüssen / Best Regards Michał Sługocki Informatyk <https://empol.pl/> EMPOL S.A Źródła ul. Inwestycyjna 1 55-330 Miękinia Sąd Rejonowy dla Wrocławia - Fabrycznej IX Wydział Gospodarczy KRS 0000679349 NIP 894 17 64 662 REGON 930912244 Wysokość kapitału zakładowego 1 000 000,00 PLN. K...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Michał Sługocki (mslugocki@empol.pl)
To: support.cantor.pl@a-w.com | Date: 23.07.2025 11:11
Type: Request | 
Liczniki na CIM (1)
Cześć,

Nie działają nam liczniki na CIM’ach. Cały czas pokazują 0. Jak je włączyć?
Np. PVC – Okuwanie ramy - licznik chcielibyśmy dodać na CIM 20425 - Okuwanie
ram.

Z poważaniem / Mit freundlichen Grüssen / Best Regards
Michał Sługocki
Informatyk

<https://empol.pl/>

EMPOL S.A
Źródła ul. Inwestycyjna 1
55-330 Miękinia
Sąd Rejonowy dla Wrocławia - Fabrycznej IX Wydział Gospodarczy
KRS 0000679349 NIP 894 17 64 662 REGON 930912244
Wysokość kapitału zakładowego 1 000 000,00 PLN. Kapitał wpłacony w całości.

tel: +48 (71) 772 64 07
fax: +48 (71) 772 64 19
e-mail:  <mailto:mslugocki@empol.pl> mslugocki@empol.pl
<http://www.empol.pl/> www.empol.pl

<https://www.google.com/maps/place/Empol+Fabryka+Okien/@51.1611274,16.710358
1,18z/data=!4m12!1m6!3m5!1s0x470f96263633bd6f:0x45e73603f3c09332!2sEmpol+Fab
ryka+Okien!8m2!3d51.1611264!4d16.7110088!3m4!1s0x470f96263633bd6f:0x45e73603
f3c09332!8m2!3d51.1611264!4d16.7110088?hl=pl> Pokaż na ma…
```

</details>

---

### [AW-237648] — Wydruki ofert/zleceń - dodatkowe grafiki/raporty

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-237648]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 23.07.2025 10:54 |

**Description:**

> RE: [AW-237648] Wydruki ofert/zleceń - dodatkowe grafiki/raporty (2) Szczerze mówiąc nie spotkałem się z tym problemem, ale zgaduje, że wynika on z ograniczonej ilości pamięci która może być zaadresowana dla aplikacji 32bit (ok 2GB RAM). Ciężko mi powiedzieć coś więcej, przydałby cały zrzut błędu jaki pojawia sie w trakcie drukowania. Nie wiem czy zmiana rozszerzenia samej grafiki z jpg na bmp nie pomogłaby ograniczyć zużycia pamięci (aplikacja zapewne zużywa część RAM-U na konwersję, więc mając...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Radoslaw Jaruszewski (support.cantor.pl@a-w.com)
To: d.precht@pagen.pl | Date: 23.07.2025 10:54
Type: Answer | 
RE: [AW-237648] Wydruki ofert/zleceń - dodatkowe grafiki/raporty (2)
Szczerze mówiąc nie spotkałem się z tym problemem, ale zgaduje, że wynika on z ograniczonej ilości pamięci która może być zaadresowana dla aplikacji 32bit (ok 2GB RAM). Ciężko mi powiedzieć coś więcej, przydałby cały zrzut błędu jaki pojawia sie w trakcie drukowania.
Nie wiem czy zmiana rozszerzenia samej grafiki z jpg na bmp nie pomogłaby ograniczyć zużycia pamięci (aplikacja zapewne zużywa część RAM-U na konwersję, więc mając grafikę już w formacie BMP mogłoby się okazać, że uda się zmieścić w dostępnych zasobach).
Serdecznie pozdrawiam
Radoslaw Jaruszewski
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertra…
```

</details>

---

### [AW-237401] — Uprawnienie do kopiowanie klientów

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-237401]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 23.07.2025 09:36 |

**Description:**

> RE: [ZEWNĘTRZNE] RE: [AW-237401] Uprawnienie do kopiowanie klientów (4) Nie ma uprawnienia na samo kopiowanie. Serdecznie pozdrawiam Oskar Bielejewski ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan Amtsgericht Gießen/Gießen Local Court: HRB 7963 Diese E-Mail ist...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Oskar Bielejewski (support.cantor.pl@a-w.com)
To: m.gwozdz@budvar.pl | Date: 23.07.2025 09:36
Type: Answer | 
RE: [ZEWNĘTRZNE] RE: [AW-237401] Uprawnienie do kopiowanie klientów (4)
Nie ma uprawnienia na samo kopiowanie.
 
Serdecznie pozdrawiam
Oskar Bielejewski
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus in Ihr System gelangen, haften wir nicht für die evtl. entstandenen Schäden.

This …
```

</details>

---

### [AW-236657] — Reinforcement Generation Issue in Interface Files (7.9 version)

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-236657]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 23.07.2025 09:25 |

**Description:**

> RE: TR: RE: RE: RE: [AW-236657] Reinforcement Generation Issue in Interface Files (7.9 version) (45) Hello, we received bugfix from R&D - the logic in this interface was changed, because of "switching cart" issue, so please enable optimization "per cart" - you will get result like below: Also problem where reinforcement where not assigned to profile but section in xml was not empty was fixed. All bugfixes are included into the newwest dll build - available on ftp server. Please test it and let m...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Radoslaw Jaruszewski (support.cantor.pl@a-w.com)
To: djameleddine.achacha@oxxo.dz | Date: 23.07.2025 09:25
Type: Answer | 
RE: TR: RE: RE: RE: [AW-236657] Reinforcement Generation Issue in Interface Files (7.9 version) (45)
Hello,
we received bugfix from R&D - the logic in this interface was changed, because of "switching cart" issue, so please enable optimization "per cart" - you will get result like below:
Also problem where reinforcement where not assigned to profile but section in xml was not empty was fixed.

All bugfixes are included into the newwest dll build - available on ftp server.
Please test it and let me know if it's work fine for you.

PS. I was unable to reproduce the issue when the additional reinforcement file (xxxxx-RF.xml) was generated. Please verify whether any configuration changes have been made on the machine center — perhaps a new profile type has been added:
Serdecznie pozdrawiam
Radoslaw Jaruszewski
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tieg…
```

</details>

---

### [AW-237700] — Reinforcement Generation Issue - wrong data in xml file while no reinforcement assigned to profile

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-237700]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 23.07.2025 08:44 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Stefan Rixecker
To: | Date: 23.07.2025 08:44
Type: State changed | 
RE: [AW-237700] Reinforcement Generation Issue - wrong data in xml file while no reinforcement assigned to profile (4)
Back to Support PL
```

</details>

---

### [AW-237706] — błąd w poz a w lustrzanym odbiciu już nie

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-237706]` |
| **Status** | 🟡 New |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 22.07.2025 16:05 |

**Description:**

> błąd w poz a w lustrzanym odbiciu już nie (1) Cześć jest błąd w poz 8 w ofercie  w EPR-ie 250044450 Poz 10 jest lustrzanym odbicie i nie ma błędu -- Logo Wikęd *Robert* *Krampikowski* Specjalista ds. IT tel. (+48) 601-194-538 <tel:(+48) 601-194-538> | (58) 738-66-80 <tel:(58) 738-66-80> robert.krampikowski@wiked.pl *WIKĘD Sp. z o.o.* ul. Wielki Las 19, 84-242 Luzino www.wiked.pl <https://wiked.pl>

<details>
<summary>View Full Conversation Thread</summary>

```
From: Robert Krampikowski (robert.krampikowski@wiked.pl)
To: support.cantor.pl@a-w.com | Date: 22.07.2025 16:05
Type: Request | 
błąd w poz a w lustrzanym odbiciu już nie (1)
Cześć jest błąd w poz 8 w ofercie  w EPR-ie 250044450

Poz 10 jest lustrzanym odbicie i nie ma błędu

--
Logo Wikęd *Robert* *Krampikowski*
Specjalista ds. IT
tel. (+48) 601-194-538 <tel:(+48) 601-194-538> | (58) 738-66-80
<tel:(58) 738-66-80>
robert.krampikowski@wiked.pl *WIKĘD Sp. z o.o.*
ul. Wielki Las 19, 84-242 Luzino
www.wiked.pl <https://wiked.pl>
```

</details>

---

### [AW-237316] — PAGEN - Błędne dane do wydruku.

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-237316]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 22.07.2025 15:49 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Dawid Cegła
To: | Date: 22.07.2025 15:49
Type: State changed | 
RE: [AW-237316] PAGEN - Błędne dane do wydruku. (2)
Rozmawiałem z Dominikiem i to zaczeło się dziać od jakiegoś czasu, wygląda na buga.
```

</details>

---

### [AW-215627] — Incorrect cycle execution of system queue

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-215627]` |
| **Status** | 🔵 In Progress |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 22.07.2025 15:23 |

**Description:**

> RE: RE: RE: [AW-215627] CANTOR 7.8 (DLL 2023.1.0.45) -> Kolejka systemowa nie sprawdza ustawionej godziny (34) Proszę bardzo, oczywiście usunąłem rozszerzenie ________________________________________ Paweł Stojek Kierownik Działu IT / Head of IT department M  +48 798 831 409 E   p.stojek@krispol.pl<mailto:p.stojek@krispol.pl> From: Support Cantor Poland <support.cantor.pl@a-w.com> Sent: Tuesday, July 22, 2025 1:25 PM To: Paweł Stojek <P.Stojek@krispol.pl> Subject: RE: RE: RE: [AW-215627] CANTOR ...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Paweł Stojek (P.Stojek@krispol.pl)
To: support.cantor.pl@a-w.com | Date: 22.07.2025 15:23
Type: Request | 
RE: RE: RE: [AW-215627] CANTOR 7.8 (DLL 2023.1.0.45) -> Kolejka systemowa nie sprawdza ustawionej godziny (34)
Proszę bardzo, oczywiście usunąłem rozszerzenie

________________________________________

Paweł Stojek
Kierownik Działu IT / Head of IT department
M  +48 798 831 409
E   p.stojek@krispol.pl<mailto:p.stojek@krispol.pl>

From: Support Cantor Poland <support.cantor.pl@a-w.com>
Sent: Tuesday, July 22, 2025 1:25 PM
To: Paweł Stojek <P.Stojek@krispol.pl>
Subject: RE: RE: RE: [AW-215627] CANTOR 7.8 (DLL 2023.1.0.45) -> Kolejka systemowa nie sprawdza ustawionej godziny

Wyślij proszę ten plik .cmd

Serdecznie pozdrawiam

Oskar Bielejewski
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com<mailto:support.pl@a-w.com>

A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com<http://www.a-w.com/>

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gie…
```

</details>

---

### [AW-237670] — Tłumaczenia się nie przenoszą między instancjami

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-237670]` |
| **Status** | 🟡 New |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 22.07.2025 14:35 |

**Description:**

> Tłumaczenia się nie przenoszą między instancjami (1) Hej, mamy taki problem, że na instancji DEV mamy więcej tłumaczeń niż na PrePROD i PROD. Tak powinno być? DEV: PrePROD: PROD: Pozdrawiam Jacek Kreft Inżynier ds. oprogramowania <https://www.drutex.eu/> *PL:* + 48 59 822 91 01 | *Fax:* + 48 59 822 91 03 DRUTEX S.A. Lęborska 31 | Bytów 77-100 | Polska NIP 8‌42 1‌6 2‌2 7‌20 www.drutex.eu <https://www.drutex.eu/> <https://www.facebook.com/DrutexSA/> <http://www.instagram.com/drutex_com/> <https://...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Jacek Kreft (jkreft@drutex.com.pl)
To: support.cantor.pl@a-w.com | Date: 22.07.2025 14:35
Type: Request | 
Tłumaczenia się nie przenoszą między instancjami (1)
Hej,

mamy taki problem, że na instancji DEV mamy więcej tłumaczeń niż na
PrePROD i PROD. Tak powinno być?

DEV:

PrePROD:

PROD:

Pozdrawiam

Jacek Kreft

Inżynier ds. oprogramowania

<https://www.drutex.eu/>

*PL:* + 48 59 822 91 01 | *Fax:* + 48 59 822 91 03

DRUTEX S.A.

Lęborska 31 | Bytów 77-100 | Polska
NIP 8‌42 1‌6 2‌2 7‌20
www.drutex.eu <https://www.drutex.eu/>

<https://www.facebook.com/DrutexSA/>
<http://www.instagram.com/drutex_com/>

<https://www.drutex.pl/pl/produkty/d-gate.html>

DRUTEX S.A. z siedzibą w Bytowie zarejestrowany został w Krajowym
Rejestrze Sądowym pod nr 0000140428 prowadzonym przez Sąd Rejonowy VIII
Wydział Gospodarczy Krajowego Rejestru Sądowego w Gdańsku. BDO
0‌00001469. Kapitał zakładowy, opłacony DRUTEX S.A. wynosi 21.690.000,00 zł

DRUTEX S.A. oświadcza, że posiada status dużego przedsiębiorcy w
rozumieniu Ustawy z dnia 8 marca 2013 r. o przeciwdziałaniu nadmiernym
opóźnieniom w transakcjach handlowych…
```

</details>

---

### [AW-237393] — [PILNE] Błędy w tłumaczeniach / zduplikowane wpisy w tłumaczeniach

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-237393]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 22.07.2025 14:16 |

**Description:**

> RE: [AW-237393] [PILNE] Błędy w tłumaczeniach / zduplikowane wpisy w tłumaczeniach (11) Co do tłumaczeń, to na ERP nie będą widoczne, tłumaczenia są przeznaczone dla klientów/dilerów - dlatego w ERP tylko na wydrukach będą widoczne tłumaczenia. Dopiero po imporcie danych do MT będzie tam można zobaczyć czy teksty są tłumaczone. Na chwilę obecną, proponuję wrócić do Backupu, który w tabalach SPRSTAMM i SPRTEXTE będzie miał poprawnie wpisane tłumaczenia, czyli niemieckie słowa dla wierszy które od...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Radoslaw Jaruszewski (support.cantor.pl@a-w.com)
To: d.precht@pagen.pl | Date: 22.07.2025 14:16
Type: Answer | 
RE: [AW-237393] [PILNE] Błędy w tłumaczeniach / zduplikowane wpisy w tłumaczeniach (11)
Co do tłumaczeń, to na ERP nie będą widoczne, tłumaczenia są przeznaczone dla klientów/dilerów - dlatego w ERP tylko na wydrukach będą widoczne tłumaczenia.
Dopiero po imporcie danych do MT będzie tam można zobaczyć czy teksty są tłumaczone.
Na chwilę obecną, proponuję wrócić do Backupu, który w tabalach SPRSTAMM i SPRTEXTE będzie miał poprawnie wpisane tłumaczenia, czyli niemieckie słowa dla wierszy które odpowiadają za niemiecki itd (taka forma weryfikacji będzie wystarczająca dla importu tłumaczeń przez CSV):

Serdecznie pozdrawiam
Radoslaw Jaruszewski
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertraul…
```

</details>

---

### [AW-237462] — Właściwość o naruszeniu gwarancji

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-237462]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 22.07.2025 13:12 |

**Description:**

> Re: [AW-237462] Właściwość o naruszeniu gwarancji (4) To już temat na konsultacje. Daj znać, czy podać temat dalej. Serdecznie pozdrawiam Oskar Bielejewski ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan Amtsgericht Gießen/Gießen Local Court: HRB 7963 Diese E-Mai...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Oskar Bielejewski (support.cantor.pl@a-w.com)
To: iiwanca@drutex.com.pl | Date: 22.07.2025 13:12
Type: Answer | 
Re: [AW-237462] Właściwość o naruszeniu gwarancji (4)
To już temat na konsultacje. Daj znać, czy podać temat dalej.
 
Serdecznie pozdrawiam
Oskar Bielejewski
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus in Ihr System gelangen, haften wir nicht für die evtl. entstan…
```

</details>

---

### [AW-237603] — iq-iis błąd

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-237603]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 22.07.2025 10:57 |

**Description:**

> Automatyczna odpowiedź: [AW-237603] iq-iis błąd (3) Dzień dobry, dziękuję za wiadomość. Obecnie przebywam na urlopie i wrócę do pracy  2025-07-28. W pilnych sprawach proszę o kontakt z działem IT pod adresem it@wiked.pl W sprawach dotyczących klientów proszę pisać na adres: login@wiked.pl Kontakt telefoniczny z działem IT pod telefonem: 601 194 538 Pozdrawiam: [https://outlook.office365.com/mail/options/accounts-category/automaticReply] Szymon Kaczykowski Kierownik działu IT szymon.kaczykowski<m...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Szymon Kaczykowski (szymon.kaczykowski@wiked.pl)
To: support.cantor.pl@a-w.com | Date: 22.07.2025 10:57
Type: Request | 
Automatyczna odpowiedź: [AW-237603] iq-iis błąd (3)
Dzień dobry,

dziękuję za wiadomość. Obecnie przebywam na urlopie i wrócę do pracy  2025-07-28.

W pilnych sprawach proszę o kontakt z działem IT pod adresem it@wiked.pl

W sprawach dotyczących klientów proszę pisać na adres: login@wiked.pl

Kontakt telefoniczny z działem IT pod telefonem: 601 194 538

Pozdrawiam:

[https://outlook.office365.com/mail/options/accounts-category/automaticReply]
Szymon Kaczykowski
Kierownik działu IT
szymon.kaczykowski<mailto:szymon.kaczykowski@wiked.pl>@wiked.pl<mailto:szymon.kaczykowski@wiked.pl>  |  tel. 602 497 702                     |  tel. (58) 738-66-80 wewn.   199
WIKĘD Sp. z o.o.
ul. Wielki Las 19, 84-242 Luzino
www.wiked.pl  |  tel. (58) 678 01 77  |  tel. 601-194-538  |  fax. (58) 738 66 61
```

</details>

---

### [AW-237331] — Dealer - nowa funkcja (błąd przy wyborze bram)

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-237331]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 22.07.2025 10:17 |

**Description:**

> Re: [AW-237331] Dealer - nowa funkcja (błąd przy wyborze bram) (8) Raczej coś takiego: CSELECT_S("TOP 1 P8" wyświetli pierwszy rezultat wg pola p8. Zależy co miał dokładnie robić tamten skrypt. TOP-a nie daje się na końcu w tym sqlu. Serdecznie pozdrawiam Oskar Bielejewski ###EOM## Phone:  +48 61 438 47 44 Mobile: Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt,...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Oskar Bielejewski (support.cantor.pl@a-w.com)
To: jkreft@drutex.com.pl | Date: 22.07.2025 10:17
Type: Answer | 
Re: [AW-237331] Dealer - nowa funkcja (błąd przy wyborze bram) (8)
Raczej coś takiego: CSELECT_S("TOP 1 P8" wyświetli pierwszy rezultat wg pola p8. Zależy co miał dokładnie robić tamten skrypt.
TOP-a nie daje się na końcu w tym sqlu.
 
Serdecznie pozdrawiam
Oskar Bielejewski
###EOM##

Phone:  +48 61 438 47 44
Mobile:  
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung di…
```

</details>

---

### [AW-237332] — Znikające opcje szyby.

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-237332]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 22.07.2025 10:09 |

**Description:**

> Re: [AW-237332] Znikające opcje szyby. (4) Cześć Załadowaliśmy najnowsze .dll. Problem nadal występuje. W dniu 21.07.2025 o 14:02, Support Cantor Poland pisze: > > Cześć. > > Zweryfikowałem -  na najnowszych DLL-kach działa już poprawnie. > Właśnie je wysłałem. > > Proszę sprawdzić po swojej stronie. > > Serdecznie pozdrawiam > > Oskar Bielejewski > ###EOM## > > > > Phone: +48 61 438 47 44 > Mobile: > Email: _*MailScanner has detected a possible fraud attempt from > "a-w.com" claiming to be* sup...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Piotr Płotek (pplotek@drutex.com.pl)
To: support.cantor.pl@a-w.com | Date: 22.07.2025 10:09
Type: Request | 
Re: [AW-237332] Znikające opcje szyby. (4)
Cześć

Załadowaliśmy najnowsze .dll.

Problem nadal występuje.

W dniu 21.07.2025 o 14:02, Support Cantor Poland pisze:
>
> Cześć.
>
> Zweryfikowałem -  na najnowszych DLL-kach działa już poprawnie.
> Właśnie je wysłałem.
>
> Proszę sprawdzić po swojej stronie.
>
> Serdecznie pozdrawiam
>
> Oskar Bielejewski
> ###EOM##
>
>
>
> Phone: +48 61 438 47 44
> Mobile:
> Email: _*MailScanner has detected a possible fraud attempt from
> "a-w.com" claiming to be* support.cantor.pl@a-w.com
> <mailto:support.pl@a-w.com>_
>
> A+W Software Polska Sp. z o. o.
> ul. Sikorskiego 44
> 62-300 Września
> Polska
>
>
>
> *www.a-w.com* <http://www.a-w.com/>
>
>
> Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt,
> Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
> Amtsgericht Gießen/Gießen Local Court: HRB 7963
>
> ------------------------------------------------------------------------
>
> Diese E-Mail ist ausschließlich für den Adressaten bestimmt…
```

</details>

---

### [AW-231521] — Wariant szyby - błąd

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-231521]` |
| **Status** | 🔵 In Progress |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 22.07.2025 08:49 |

**Description:**

> Re: FW: RE: [AW-231521] Re: Wariant szyby - błąd (20) Cześć,. poniżej restrykcje (dla ułatwienia wklejam warunek ze screena) dla festa 2000x2000 restrykcje nr 24,25,44,45 24: NOT(IloscSzyb=2 AND PowierzchniaProst>fn_SzybyOgrPowDlBoku(IloscSzyb,0,fn_getScheibVarFeldN(SCHEIBE_1,180),ABSTANDH_STAERKE_1,SCHEIBE_TYP_1=8,"MAX_POW")AND FINDINSTR(PROFILSATZ,"MB78",1)=0 AND FINDINSTR(PROFILSATZ,"MB60",1)=0 AND FINDINSTR(ARTNRFUELLUNG,"NAR",1)=0) 25: NOT(IloscSzyb=2 AND PowierzchniaProst>fn_SzybyOgrPowDlB...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Dawid Dawid (dakmiecik@drutex.com.pl)
To: support.cantor.pl@a-w.com | Date: 22.07.2025 08:49
Type: Request | 
Re: FW: RE: [AW-231521] Re: Wariant szyby - błąd (20)
Cześć,.

poniżej restrykcje (dla ułatwienia wklejam warunek ze screena) dla festa
2000x2000 restrykcje nr 24,25,44,45

24:

NOT(IloscSzyb=2 AND
PowierzchniaProst>fn_SzybyOgrPowDlBoku(IloscSzyb,0,fn_getScheibVarFeldN(SCHEIBE_1,180),ABSTANDH_STAERKE_1,SCHEIBE_TYP_1=8,"MAX_POW")AND
FINDINSTR(PROFILSATZ,"MB78",1)=0 AND FINDINSTR(PROFILSATZ,"MB60",1)=0
AND FINDINSTR(ARTNRFUELLUNG,"NAR",1)=0)

25:

NOT(IloscSzyb=2 AND
PowierzchniaProst>fn_SzybyOgrPowDlBoku(IloscSzyb,0,fn_getScheibVarFeldN(SCHEIBE_2,180),ABSTANDH_STAERKE_1,SCHEIBE_TYP_2=8,"MAX_POW")AND
FINDINSTR(PROFILSATZ,"MB78",1)=0 AND FINDINSTR(PROFILSATZ,"MB60",1)=0
AND FINDINSTR(ARTNRFUELLUNG,"NAR",1)=0)

44:

NOT(IloscSzyb=2 AND
MinDlugBoku>fn_SzybyOgrPowDlBoku(IloscSzyb,0,fn_getScheibVarFeldN(SCHEIBE_1,180),ABSTANDH_STAERKE_1,SCHEIBE_TYP_1=8,"MAX_KR_BOK")
AND FINDINSTR(PROFILSATZ,"MB78",1)=0 AND
FINDINSTR(PROFILSATZ,"MB60",1)=0 AND FINDINSTR(ARTNRFUELLUNG,"NAR",1)=0)

45:

NOT(IloscSzyb=2 AND
M…
```

</details>

---

### [AW-231727] — Duplicated SPRACHID

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-231727]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 21.07.2025 14:04 |

**Description:**

> FW: RE: [AW-231727] FW: Problem z eksportem Master Daty - zdublowane SPRACHID w tabeli PREISGRUPPED (9) Ten temat również naprawiony w najnowszych DLL-kach Serdecznie pozdrawiam Oskar Bielejewski ###EOM## Phone:  +48 61 438 47 44 Mobile: Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan Amtsgericht Gießen/Gießen Local Co...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Oskar Bielejewski (support.cantor.pl@a-w.com)
To: G.Babicz@krispol.pl | Date: 21.07.2025 14:04
Type: Answer | 
FW: RE: [AW-231727] FW: Problem z eksportem Master Daty - zdublowane SPRACHID w tabeli PREISGRUPPED (9)
Ten temat również naprawiony w najnowszych DLL-kach
Serdecznie pozdrawiam
Oskar Bielejewski
###EOM##

Phone:  +48 61 438 47 44
Mobile:  
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus in Ihr System gelangen, haften wir nicht für die evtl. entstandenen Schäden.

This e-m…
```

</details>

---

### [AW-236939] — Błędny status zlecenia

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-236939]` |
| **Status** | 🟡 New |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 21.07.2025 12:39 |

**Description:**

> PD: Błędny status zlecenia (2) Cześć, Ponawiam poniższego maila. Z poważaniem / Mit freundlichen Grüssen / Best Regards Michał Sługocki Informatyk <https://empol.pl/> EMPOL S.A Źródła ul. Inwestycyjna 1 55-330 Miękinia Sąd Rejonowy dla Wrocławia - Fabrycznej IX Wydział Gospodarczy KRS 0000679349 NIP 894 17 64 662 REGON 930912244 Wysokość kapitału zakładowego 1 000 000,00 PLN. Kapitał wpłacony w całości. tel: +48 (71) 772 64 07 fax: +48 (71) 772 64 19 e-mail:  <mailto:mslugocki@empol.pl> mslugock...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Michał Sługocki (mslugocki@empol.pl)
To: support.cantor.pl@a-w.com | Date: 21.07.2025 12:39
Type: Request | 
PD: Błędny status zlecenia (2)
Cześć,

Ponawiam poniższego maila.

Z poważaniem / Mit freundlichen Grüssen / Best Regards
Michał Sługocki
Informatyk

<https://empol.pl/>

EMPOL S.A
Źródła ul. Inwestycyjna 1
55-330 Miękinia
Sąd Rejonowy dla Wrocławia - Fabrycznej IX Wydział Gospodarczy
KRS 0000679349 NIP 894 17 64 662 REGON 930912244
Wysokość kapitału zakładowego 1 000 000,00 PLN. Kapitał wpłacony w całości.

tel: +48 (71) 772 64 07
fax: +48 (71) 772 64 19
e-mail:  <mailto:mslugocki@empol.pl> mslugocki@empol.pl
<http://www.empol.pl/> www.empol.pl

<https://www.google.com/maps/place/Empol+Fabryka+Okien/@51.1611274,16.710358
1,18z/data=!4m12!1m6!3m5!1s0x470f96263633bd6f:0x45e73603f3c09332!2sEmpol+Fab
ryka+Okien!8m2!3d51.1611264!4d16.7110088!3m4!1s0x470f96263633bd6f:0x45e73603
f3c09332!8m2!3d51.1611264!4d16.7110088?hl=pl> Pokaż na mapie

Znajdź nas:

<https://www.facebook.com/Empol.Okna>
<https://www.linkedin.com/company/empol-fabryka-okien/?viewAsMember=true>
<…
```

</details>

---

### [AW-237318] — A+W Cantor CIM - Terminal Designer (DLL 2023.1.0 - 69)

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-237318]` |
| **Status** | 🟡 New |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 18.07.2025 12:52 |

**Description:**

> A+W Cantor CIM - Terminal Designer (DLL 2023.1.0 - 69) (1) Dzień dobry, W CIM (Cloud Apps - Krispol) na stanowisku 15100 - Magazyn - Wydawanie materialow marketingowych mamy problem z grupowaniem poszczególnych pozycji ze zlecenia. Przykładowe zlecenie testowe - 898915, 6 pozycji z "Próbnik bram K2 R" z różnymi "Nr materiału do Spd.". Po wczytaniu danych na terminal CIM dla każdej pozycji pokazuje się ten sam "Indeks" co w 1 pozycji (poniżej): Warunek na "Indeks" wygląda następująco: Dopiero po ...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Łukasz Kempiak (L.Kempiak@krispol.pl)
To: support.cantor.pl@a-w.com | Date: 18.07.2025 12:52
Type: Request | 
A+W Cantor CIM - Terminal Designer (DLL 2023.1.0 - 69) (1)
Dzień dobry,

W CIM (Cloud Apps - Krispol) na stanowisku 15100 - Magazyn - Wydawanie materialow marketingowych mamy problem z grupowaniem poszczególnych pozycji ze zlecenia.

Przykładowe zlecenie testowe - 898915, 6 pozycji z "Próbnik bram K2 R" z różnymi "Nr materiału do Spd.".

Po wczytaniu danych na terminal CIM dla każdej pozycji pokazuje się ten sam "Indeks" co w 1 pozycji (poniżej):

Warunek na "Indeks" wygląda następująco:

Dopiero po "obejściu" stworzenia zmiennej etykiet w CANTOR:

I podpięciu jej w "Etykiety/listy cięć":

oraz skorygowanie funkcji w CIM na poniższą, zaczęło to działać prawidłowo:

Prośba o weryfikację tego przypadku ponieważ "Indeksy" powinny być rozdzielone również dla funkcji "Materialnummer+MaterialnummerGK"

________________________________…
```

</details>

---

### [AW-234894] — Informacja o ograniczeniach

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-234894]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 18.07.2025 12:50 |

**Description:**

> Re: [AW-234894] Informacja o ograniczeniach (4) Cześć. Na ERP nie umożliwiamy tłumaczeń restrykcji, dlatego tu zawsze wartość do bazy będzie lądowała w języku systemowym (polskim). Natomiast na dealerze restrykcje są tłumaczone, więc w AUFARTIK teksty są w języku klienta. Serdecznie pozdrawiam Oskar Bielejewski ###EOM## Phone:  +48 61 438 47 44 Mobile: Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing D...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Oskar Bielejewski (support.cantor.pl@a-w.com)
To: mmedwid@drutex.com.pl | Date: 18.07.2025 12:50
Type: Answer | 
Re: [AW-234894] Informacja o ograniczeniach (4)
Cześć.
Na ERP nie umożliwiamy tłumaczeń restrykcji, dlatego tu zawsze wartość do bazy będzie lądowała w języku systemowym (polskim).

Natomiast na dealerze restrykcje są tłumaczone, więc w AUFARTIK teksty są w języku klienta.

Serdecznie pozdrawiam
Oskar Bielejewski
###EOM##

Phone:  +48 61 438 47 44
Mobile:  
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich ve…
```

</details>

---

### [AW-237273] — Zmiana ewaluacji na zlecenie

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-237273]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 18.07.2025 10:19 |

**Description:**

> RE: [AW-237273] Zmiana ewaluacji na zlecenie (2) Cześć, Na standardowych profilach nie jesteśmy w stanie wybrać ewaluacji zlecenie, ponieważ profile mogą mieć dodatkowe korekty długości czy innych parametrów w technice profilowej, która wylicza się dopiero po analizie. Artykuły z ewaluacją "Zlecenie" nie będą w ogóle brały pod uwagę tych konfiguracji z techniki profilowej i mogłyby generować się niepoprawnie. Serdecznie pozdrawiam Damian Mizerny ###EOM## Phone:  +48 61 438 47 44 Mobile:  +48 512...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Damian Mizerny (support.cantor.pl@a-w.com)
To: MLIPINSKI@DRUTEX.COM.PL | Date: 18.07.2025 10:19
Type: Answer | 
RE: [AW-237273] Zmiana ewaluacji na zlecenie (2)
Cześć,
Na standardowych profilach nie jesteśmy w stanie wybrać ewaluacji zlecenie, ponieważ profile mogą mieć dodatkowe korekty długości czy innych parametrów w technice profilowej, która wylicza się dopiero po analizie.
Artykuły z ewaluacją "Zlecenie" nie będą w ogóle brały pod uwagę tych konfiguracji z techniki profilowej i mogłyby generować się niepoprawnie.
Serdecznie pozdrawiam
Damian Mizerny
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +48 512 172 718
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu …
```

</details>

---

### [AW-237187] — Dealer - błąd przy wybraniu FS505

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-237187]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 18.07.2025 09:13 |

**Description:**

> RE: [AW-237187] Dealer - błąd przy wybraniu FS505 (2) Cześć. Z trace'a, jak i komunikatu nie jestem w stanie wywnioskować skąd ten błąd. Prześlij proszę backup tej bazy. Serdecznie pozdrawiam Oskar Bielejewski ###EOM## Phone:  +48 61 438 47 44 Mobile: Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan Amtsgericht Gießen/G...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Oskar Bielejewski (support.cantor.pl@a-w.com)
To: jkreft@drutex.com.pl | Date: 18.07.2025 09:13
Type: Answer | 
RE: [AW-237187] Dealer - błąd przy wybraniu FS505 (2)
Cześć.
Z trace'a, jak i komunikatu nie jestem w stanie wywnioskować skąd ten błąd.
Prześlij proszę backup tej bazy.
 
Serdecznie pozdrawiam
Oskar Bielejewski
###EOM##

Phone:  +48 61 438 47 44
Mobile:  
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus in Ihr System gelan…
```

</details>

---

### [AW-232597] — DOMEL: DZIWNA CENA DRZWI Z PANELEM

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-232597]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 17.07.2025 14:28 |

**Description:**

> RE: [AW-232597] DOMEL: DZIWNA CENA DRZWI Z PANELEM (5) Cześć, Sprawdziłem temat. Ta tabela jest używana stricte do ograniczeń. Czyli rozrysowujesz sobie drzwi z panelem i po prostu sprawdzane są obecne wartości dla szerokości i wysokości i porównywane z tym, co masz w tabeli. Wyskoczy Ci restrykcja jeśli przekraczasz, jeśli się mieścisz jest ok. Z tej tabeli przekazujecie wartość do poniższych właściwości, a z nich tworzycie ograniczenia na klasie 1200 do paneli. Ceny nie muszą z tego korzystać ...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Damian Mizerny (support.cantor.pl@a-w.com)
To: dariusz.zabielski@domel.pl | Date: 17.07.2025 14:28
Type: Answer | 
RE: [AW-232597] DOMEL: DZIWNA CENA DRZWI Z PANELEM (5)
Cześć,
 
Sprawdziłem temat.
Ta tabela jest używana stricte do ograniczeń. Czyli rozrysowujesz sobie drzwi z panelem i po prostu sprawdzane są obecne wartości dla szerokości i wysokości i porównywane z tym, co masz w tabeli. Wyskoczy Ci restrykcja jeśli przekraczasz, jeśli się mieścisz jest ok.
Z tej tabeli przekazujecie wartość do poniższych właściwości, a z nich tworzycie ograniczenia na klasie 1200 do paneli.
 

 

 
Ceny nie muszą z tego korzystać i mogą być skonfigurowane w zupełnym oderwaniu od tych ograniczeń, co tutaj ma miejsce.
W ograniczeniu sprawdzacie czy wysokość waszego panelu jest wyższa niż WysokoscMax2, no i tutaj żadne ograniczenie nie wyskoczy, bo dopuszczacie w tabeli wysokość do 2100, a panel ma 2078. Nie ma restrykcji.
 

 
W raporcie cenowym widać, że cena policzyła się ze schematu 50 i jest to dopłata 1.
 

 
Wywaliło Wam cenę 99999 pomnożoną przez współczynnik, bo tak macie ustawioną dopłatę w macierzy PCV_DOD do klasy 1200 i do modelu BL.
…
```

</details>

---

### [AW-236410] — Brak przekładni do profili CT70 RONDO

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-236410]` |
| **Status** | 🔵 In Progress |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 17.07.2025 13:34 |

**Description:**

> Re: [AW-236410] Brak przekładni do profili CT70 RONDO (4) Hej, Udało się coś ustalić w tym temacie? Z poważaniem / Mit freundlichen Grüssen / Best Regards *Kamil Miłkowski* Specjalista ds. baz danych <https://www.empol.pl> *EMPOL S.A* Źródła ul. Inwestycyjna 1 55-330 Miękinia Sąd Rejonowy dla Wrocławia - Fabrycznej IX Wydział Gospodarczy KRS 0000679349 NIP 894 17 64 662 REGON 930912244 Wysokość kapitału zakładowego 1 000 000,00 PLN. Kapitał wpłacony w całości. kom: +48 606 382 775 tel: +48 (71) ...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Empol Wdrożenie (wdrozenie@empol.pl)
To: support.cantor.pl@a-w.com | Date: 17.07.2025 13:34
Type: Request | 
Re: [AW-236410] Brak przekładni do profili CT70 RONDO (4)
Hej,

Udało się coś ustalić w tym temacie?

Z poważaniem / Mit freundlichen Grüssen / Best Regards
*Kamil Miłkowski*
Specjalista ds. baz danych

<https://www.empol.pl>

*EMPOL S.A*
Źródła ul. Inwestycyjna 1
55-330 Miękinia
Sąd Rejonowy dla Wrocławia - Fabrycznej IX Wydział Gospodarczy
KRS 0000679349 NIP 894 17 64 662 REGON 930912244
Wysokość kapitału zakładowego 1 000 000,00 PLN. Kapitał wpłacony w całości.

kom: +48 606 382 775
tel: +48 (71) 772 64 07
fax: +48 (71) 772 64 19
e-mail: kmilkowski@empol.pl
www.empol.pl <http://empol.pl>
Pokaż na mapie <http://empol.pl/index.php/pl/kontakt/mapa/zrodla>

Znajdź nas:
<https://www.facebook.com/Empol.Okna>
<https://www.linkedin.com/company/empol-fabryka-okien/?viewAsMember=true>
<https://www.youtube.com/channel/UCxbu7bdmIdRfiPtETbfTUrA>

W dniu 2025-07-10 o 13:26, Kamil Miłkowski pisze:
>
> Proszę bardzo, zlecenie testowe 2047259 na bazie testowej.
> Problem dotyczy obu skrzydeł rondo 18867, 18620, niezależni…
```

</details>

---

### [AW-236870] — Wysokość klamki na rysunku

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-236870]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 16.07.2025 16:00 |

**Description:**

> RE: [AW-236870] Wysokość klamki na rysunku (4) tak, jest możliwość odpalenia jej w wersji 64 bit Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan Amtsgericht Gießen/Gießen Local Court: HRB 7963 Diese E-Mail ist ausschließlich ...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: m.gwozdz@budvar.pl | Date: 16.07.2025 16:00
Type: Answer | 
RE: [AW-236870] Wysokość klamki na rysunku (4)
tak, jest możliwość odpalenia jej w wersji 64 bit
Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus in Ihr System gelangen, haften wir nicht für die evtl. entstandenen Schäden.
…
```

</details>

---

### [AW-224579] — During system language change, system removes translations from sprstamm/sprtexte

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-224579]` |
| **Status** | 🔵 In Progress |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 15.07.2025 11:59 |

**Description:**

> Re: [AW-224579] Re: [AW-231828] Fwd: Cantor - problem z językiem po imporcie masterdata (32) Hej, w nawiązaniu do dzisiejszej rozmowy podsyłam .bak bazy od klienta oraz screen z jego interfejsu po update. Link do chmury z .bak: https://cloud.drutex.pl/s/igwy732FHbEPoOa Hasło: dj%T3ct&5JYm$8boA*e7Gc%E4gbT Pozdrawiam Jacek Kreft Inżynier ds. oprogramowania <https://www.drutex.eu/> *PL:* + 48 59 822 91 01 | *Fax:* + 48 59 822 91 03 DRUTEX S.A. Lęborska 31 | Bytów 77-100 | Polska NIP 8‌42 1‌6 2‌2 7‌...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Jacek Kreft (jkreft@drutex.com.pl)
To: support.cantor.pl@a-w.com, Radoslaw.Jaruszewski@a-w.com | Date: 15.07.2025 11:59
Type: Request | 
Re: [AW-224579] Re: [AW-231828] Fwd: Cantor - problem z językiem po imporcie masterdata (32)
Hej,

w nawiązaniu do dzisiejszej rozmowy podsyłam .bak bazy od klienta oraz
screen z jego interfejsu po update.

Link do chmury z .bak: https://cloud.drutex.pl/s/igwy732FHbEPoOa
Hasło: dj%T3ct&5JYm$8boA*e7Gc%E4gbT

Pozdrawiam

Jacek Kreft

Inżynier ds. oprogramowania

<https://www.drutex.eu/>

*PL:* + 48 59 822 91 01 | *Fax:* + 48 59 822 91 03

DRUTEX S.A.

Lęborska 31 | Bytów 77-100 | Polska
NIP 8‌42 1‌6 2‌2 7‌20
www.drutex.eu <https://www.drutex.eu/>

<https://www.facebook.com/DrutexSA/>
<http://www.instagram.com/drutex_com/>

<https://www.drutex.pl/pl/produkty/d-gate.html>

DRUTEX S.A. z siedzibą w Bytowie zarejestrowany został w Krajowym
Rejestrze Sądowym pod nr 0000140428 prowadzonym przez Sąd Rejonowy VIII
Wydział Gospodarczy Krajowego Rejestru Sądowego w Gdańsku. BDO
0‌00001469. Kapitał zakładowy, opłacony DRUTEX S.A. wynosi 21.690.000,00 zł

DRUTEX S.A. oświadcza, że posiada status dużego przedsiębiorcy w
rozumieniu Ustawy z dnia 8 m…
```

</details>

---

### [AW-236715] — Ograniczenie uprawnień Cantor Dealer

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-236715]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 15.07.2025 10:25 |

**Description:**

> Re: [AW-236715] Ograniczenie uprawnień Cantor Dealer (7) Cześć, wcześniej wysłana przeze mnie wiadomość była błędna, okazało się że mamy taką możliwość. Są dwie opcje, można wyłączyć zmianę naroży za pomocą PRODCONF 854=0 (zmiana powinna dotyczyć tylko dilera,nie ERP-a): lub można zablokować możliwość zmiany użytkownikowi za pomocą uprawnienia 345: Jeśli chcielibyście ograć to zmianą Prodconf-a, to warto przetestować zanim wdrożycie u klienta - sprawdziłem po swojej stronie i wygląda, że automat...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Radoslaw Jaruszewski (support.cantor.pl@a-w.com)
To: iiwanca@drutex.com.pl | Date: 15.07.2025 10:25
Type: Answer | 
Re: [AW-236715] Ograniczenie uprawnień Cantor Dealer (7)
Cześć,
wcześniej wysłana przeze mnie wiadomość była błędna, okazało się że mamy taką możliwość.
Są dwie opcje, można wyłączyć zmianę naroży za pomocą PRODCONF 854=0 (zmiana powinna dotyczyć tylko dilera,nie ERP-a):

lub można zablokować możliwość zmiany użytkownikowi za pomocą uprawnienia 345:

Jeśli chcielibyście ograć to zmianą Prodconf-a, to warto przetestować zanim wdrożycie u klienta - sprawdziłem po swojej stronie i wygląda, że automatyczne zmiany połączeń działają prawidłowo ale nie jestem w stanie zapewnić, że w każdym przypadku tak będzie dlatego istotne jest przeprowadzenie również testów po Waszej stronie.
Serdecznie pozdrawiam
Radoslaw Jaruszewski
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gieße…
```

</details>

---

### [AW-236452] — CANTOR 7.8 iQuote - konfiguracja użytkownika

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-236452]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 15.07.2025 09:41 |

**Description:**

> RE: [AW-236452] CANTOR 7.8 iQuote - konfiguracja użytkownika (6) Hej, sorry jednak 709 musi być nadane. Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan Amtsgericht Gießen/Gießen Local Court: HRB 7963 Diese E-Mail ist ausschli...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: P.Stojek@krispol.pl | Date: 15.07.2025 09:41
Type: Answer | 
RE: [AW-236452] CANTOR 7.8 iQuote - konfiguracja użytkownika (6)
Hej, sorry jednak 709 musi być nadane.
 

Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus in Ihr System gelangen, haften wir nicht für die evtl. entstandenen Schäden.

This …
```

</details>

---

### [AW-236636] — Scan problem on CIM terminal after update to 7.9

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-236636]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 14.07.2025 14:17 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Radoslaw Jaruszewski
To: | Date: 14.07.2025 14:17
Type: State changed | 
RE: [AW-236636] Scan problem on CIM terminal after update to 7.9 (10)
```

</details>

---

### [AW-236687] — Urgent: Blocking Issues After Installing Version 7.9

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-236687]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 14.07.2025 11:43 |

**Description:**

> Automatische Antwort: [AW-236687] Urgent: Blocking Issues After Installing Version 7.9 (3) Dear Ladies and Gentlemen, Thank you for your e-mail. I will be out of office until July 17th, 2025. I will reply to your e-mail asap. Mit freundlichen Grüßen / Best regards Alfred Cortisse COO EMEA / APAC Business Unit A+W Clarity ______________________________ A+W Software GmbH Am Pfahlgraben 4 - 10 D-35415 Pohlheim G e r m a n y e-mail: alfred.cortisse@a-w.com Tel.: +49 6404/2051-205 (direct) Mobile +49...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Alfred Cortisse (Alfred.Cortisse@a-w.com)
To: support.cantor.pl@a-w.com | Date: 14.07.2025 11:43
Type: Request | 
Automatische Antwort: [AW-236687] Urgent: Blocking Issues After Installing Version 7.9 (3)
Dear Ladies and Gentlemen,
 
Thank you for your e-mail. I will be out of office until July 17th, 2025.
I will reply to your e-mail asap.
 
Mit freundlichen Grüßen / Best regards
 
Alfred Cortisse
COO EMEA / APAC
Business Unit A+W Clarity
______________________________
A+W Software GmbH
Am Pfahlgraben 4 - 10
D-35415 Pohlheim
G e r m a n y
 
e-mail: alfred.cortisse@a-w.com
Tel.: +49 6404/2051-205 (direct)
Mobile +49 151 16228-823
Fax: +49 6404/2051-877
http://www.a-w.com
 
Geschäftsführer/Managing Directors: Peter Dixen (Vorsitzender), George Evers
Mark Thompson, Daniel Lee
Amtsgericht Gießen/Gießen Local Court: HRB 7963
 
 
This e-mail is for the intended recipient only and may contain confidential and/or legally protected information. If you have received it by mistake please contact us and delete it from your system. Copying as well as unauthorized relaying is strictly prohibited. Of course we use anti virus programs. Should a virus have reached your system…
```

</details>

---

### [AW-236240] — Na jekiej podstawie ustawia sie to pole w ofercie?

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-236240]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 11.07.2025 15:18 |

**Description:**

> RE: [AW-236240] Na jekiej podstawie ustawia sie to pole w ofercie? (4) Cześć, Nr schematu pochodzi z konfiguracji programu [KALKULATION] StandardSchemaEK Nr rekordu jest ustalany poprzez znalezienie pierwszego wpisu dla danego schematu w Zestawach kalkulacyjnych Można go nadpisać poprzez konfigurację programu [KALKULATION] StandardSatzEK Serdecznie pozdrawiam Radoslaw Jaruszewski ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Radoslaw Jaruszewski (support.cantor.pl@a-w.com)
To: m.gwozdz@budvar.pl | Date: 11.07.2025 15:18
Type: Answer | 
RE: [AW-236240] Na jekiej podstawie ustawia sie to pole w ofercie? (4)
Cześć,
Nr schematu pochodzi z konfiguracji programu [KALKULATION] StandardSchemaEK
Nr rekordu jest ustalany poprzez znalezienie pierwszego wpisu dla danego schematu w Zestawach kalkulacyjnych
Można go nadpisać poprzez konfigurację programu [KALKULATION] StandardSatzEK

Serdecznie pozdrawiam
Radoslaw Jaruszewski
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weiterga…
```

</details>

---

### [AW-236600] — PILNE! Zmienna z długością wrębu okuciowego ze słupkiem ruchomym. PILNE!

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-236600]` |
| **Status** | 🟡 New |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 11.07.2025 15:15 |

**Description:**

> PILNE! Zmienna z długością wrębu okuciowego ze słupkiem ruchomym. PILNE! (1) Cześć, Temat jest pilny. Muszę dodać artykuł do konstrukcji na podstawie długości wrębu danego skrzydła. W przypadku skrzydła biernego musi to być wrąb powiększony o słupek ruchomy. Nie ma większego znaczenia gdzie to dodam, czy do skrzydła, czy z Pola_s. Zmienne które podają szerokość wrębu nie uwzględniają powiększenia przez słupek ruchomy. Zmienna FFB przyjmuje wartość z słupkiem ruchomym dopiero w momencie analizy g...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Empol Wdrożenie (wdrozenie@empol.pl)
To: support.cantor.pl@a-w.com, Damian.Mizerny@a-w.com | Date: 11.07.2025 15:15
Type: Request | 
PILNE! Zmienna z długością wrębu okuciowego ze słupkiem ruchomym. PILNE! (1)
Cześć,

Temat jest pilny.

Muszę dodać artykuł do konstrukcji na podstawie długości wrębu danego
skrzydła.
W przypadku skrzydła biernego musi to być wrąb powiększony o słupek ruchomy.

Nie ma większego znaczenia gdzie to dodam, czy do skrzydła, czy z Pola_s.
Zmienne które podają szerokość wrębu nie uwzględniają powiększenia przez
słupek ruchomy.
Zmienna FFB przyjmuje wartość z słupkiem ruchomym dopiero w momencie
analizy garnituru okuć.

Analizowaliśmy temat z Damianem przy okazji innego tematu i poprosił
abym zgłosił to na support.
Naszym zdaniem zmienna FFB lub jakaś inna powinna zawierać poprawne
wartości wszędzie a nie tylko w garniturach okuć.

Nie wiem jak wam to zoobrazować, ale puszczając trace na dowolnej
konstrukcji z słupkiem ruchomym + analizę techniczną okuć.
Zmienne FFB "sprawdzane z Pole_s/profili" dla obu skrzydeł przyjmują
taką samą wartość, a zmienne puszczone z garniturów mają poprawne wartości.

W tym przypadku nie udało mi się wyszuk…
```

</details>

---

### [AW-236537] — Ograniczenie Tworzenia ofert

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-236537]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 11.07.2025 13:30 |

**Description:**

> RE: [AW-236537] Ograniczenie Tworzenia ofert (2) Cześć, Niestety nie - za tworzenie i edycje odpowiada jedno uprawnienie: Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan Amtsgericht Gießen/Gießen Local Court: HRB 7963 Diese E...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: m.gwozdz@budvar.pl | Date: 11.07.2025 13:30
Type: Answer | 
RE: [AW-236537] Ograniczenie Tworzenia ofert (2)
Cześć,
Niestety nie - za tworzenie i edycje odpowiada jedno uprawnienie:

Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus in Ihr System gelangen, haften wir nicht für die evtl…
```

</details>

---

### [AW-236448] — DRUTEX Installationsroutine 7.9

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-236448]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 11.07.2025 10:59 |

**Description:**

> Re: [AW-236448] DRUTEX Installationsroutine 7.9 (7) ok, tylko jedna uwaga, cantorlog zawsze uruchamiamy po nieudanej instalacji - dopiero wtedy może on zacząć gromadzić wszystkie dane. Czyli najpierw należy uruchomić instalację, gdy instalacja zakończy się błędem, to należy go potwierdzić i zakończyć pracę instalatora, a następnie można przejść do uruchomienia cantorlog. Serdecznie pozdrawiam Radoslaw Jaruszewski ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Radoslaw Jaruszewski (support.cantor.pl@a-w.com)
To: iiwanca@drutex.com.pl | Date: 11.07.2025 10:59
Type: Answer | 
Re: [AW-236448] DRUTEX Installationsroutine 7.9 (7)
ok, tylko jedna uwaga, cantorlog zawsze uruchamiamy po nieudanej instalacji - dopiero wtedy może on zacząć gromadzić wszystkie dane.
Czyli najpierw należy uruchomić instalację, gdy instalacja zakończy się błędem, to należy go potwierdzić i zakończyć pracę instalatora, a następnie można przejść do uruchomienia cantorlog.
Serdecznie pozdrawiam
Radoslaw Jaruszewski
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das…
```

</details>

---

### [AW-236063] — Cena na podstawie kosztów - błąd z walutą

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-236063]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 10.07.2025 15:52 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet
To: | Date: 10.07.2025 15:52
Type: State changed | 
RE: [AW-236063] Cena na podstawie kosztów - błąd z walutą (6)
```

</details>

---

### [AW-236421] — Błąd aktywacji Dealer 7.9

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-236421]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 10.07.2025 15:39 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet
To: | Date: 10.07.2025 15:39
Type: State changed | 
RE: [AW-236421] Błąd aktywacji Dealer 7.9 (9)
```

</details>

---

### [AW-235916] — wymagania dla programu Cantor

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-235916]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 10.07.2025 14:15 |

**Description:**

> RE: [AW-235916] wymagania dla programu Cantor (2) Cześć, poniżej odpowiedzi na moje pytania odnośnie wymagań sprzętowo-systemowych: • Specyfikacja oprogramowania: Jakie są minimalne wymagania dotyczące sprzętu i systemu operacyjnego? • Wydajność: Jakie są wymagania dotyczące wydajności (CPU, RAM, przestrzeń dyskowa)? • Wymagania sieciowe: Jaka prędkość i stabilność połączenia sieciowego są wymagane? Na trzy powyższe pytania odpowiedź znajduje się na zrzucie poniżej (+ uzupełnienie do tego): Na z...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Radoslaw Jaruszewski (support.cantor.pl@a-w.com)
To: mtelega@drutex.com.pl | Date: 10.07.2025 14:15
Type: Answer | 
RE: [AW-235916] wymagania dla programu Cantor (2)
Cześć,
poniżej odpowiedzi na moje pytania odnośnie wymagań sprzętowo-systemowych:
 • Specyfikacja oprogramowania: Jakie są minimalne wymagania dotyczące sprzętu i systemu operacyjnego?
 • Wydajność: Jakie są wymagania dotyczące wydajności (CPU, RAM, przestrzeń dyskowa)?
 • Wymagania sieciowe: Jaka prędkość i stabilność połączenia sieciowego są wymagane?
Na trzy powyższe pytania odpowiedź znajduje się na zrzucie poniżej (+ uzupełnienie do tego):

Na zrzucie widzimy wymagania dla ERP i CIM jednak można to wykorzystać także dla wersji dilerskiej, weźcie jednak pod uwagę że nie są to graniczne minimalne wymagania a takie które pozwolą pracownikowi wykonywać pracę w miarę przyzwoitych warunkach - np. da się uruchomić Cantora na systemie z 2GB RAM, ale praca nie będzie na pewno przyjemna na takim systemie. Co do połączenia internetowego to mówimy o łączu symetrycznym, co do stabilności to należy mieć na uwadze, że nagłe przerwanie połączenia sieciowego będzie skutkowało zamknięcie…
```

</details>

---

### [AW-219865] — DRUTEX Installationsroutine 7.9

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-219865]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 10.07.2025 13:40 |

**Description:**

> [AW-219865] DRUTEX Installationsroutine 7.9 (27) Witam, Mamy taki problem: W pliku log: MSI (c) (7C:D8) [14:58:24:606]: MainEngineThread is returning 1603 Prosimy o pomoc w rozwiązaniu problemu. W załączniku cały plik log. Wersja 7.9 ma taki sam problem jak 7.8. Pozdrawiam Ireneusz Iwańca Specjalista ds. IT <https://www.drutex.eu/> *PL:* + 48 59 822 91 01 | *Fax:* + 48 59 822 91 03 DRUTEX S.A. Lęborska 31 | Bytów 77-100 | Polska NIP 8‌42 1‌6 2‌2 7‌20 www.drutex.eu <https://www.drutex.eu/> <https...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Ireneusz Iwańca (iiwanca@drutex.com.pl)
To: support.cantor.pl@a-w.com | Date: 10.07.2025 13:40
Type: Request | 
[AW-219865] DRUTEX Installationsroutine 7.9 (27)
Witam,

Mamy taki problem:

W pliku log:
MSI (c) (7C:D8) [14:58:24:606]: MainEngineThread is returning 1603

Prosimy o pomoc w rozwiązaniu problemu. W załączniku cały plik log.

Wersja 7.9 ma taki sam problem jak 7.8.

Pozdrawiam

Ireneusz Iwańca

Specjalista ds. IT

<https://www.drutex.eu/>

*PL:* + 48 59 822 91 01 | *Fax:* + 48 59 822 91 03

DRUTEX S.A.

Lęborska 31 | Bytów 77-100 | Polska
NIP 8‌42 1‌6 2‌2 7‌20
www.drutex.eu <https://www.drutex.eu/>

<https://www.facebook.com/DrutexSA/>
<http://www.instagram.com/drutex_com/>

<https://www.drutex.pl/pl/produkty/d-gate.html>

DRUTEX S.A. z siedzibą w Bytowie zarejestrowany został w Krajowym
Rejestrze Sądowym pod nr 0000140428 prowadzonym przez Sąd Rejonowy VIII
Wydział Gospodarczy Krajowego Rejestru Sądowego w Gdańsku. BDO
0‌00001469. Kapitał zakładowy, opłacony DRUTEX S.A. wynosi 21.690.000,00 zł

DRUTEX S.A. oświadcza, że posiada status dużego przedsiębiorcy w
rozumieniu Ustawy z dnia 8 m…
```

</details>

---

### [AW-229996] — Fwd: Fwd: Fwd: Fwd: CANTOR | Błąd wizualizacji drzwi MB86 z panelem 2x zlicowanym

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-229996]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 10.07.2025 13:04 |

**Description:**

> Re: [AW-229996] Fwd: Fwd: Fwd: Fwd: CANTOR | Błąd wizualizacji drzwi MB86 z panelem 2x zlicowanym (9) Hej, Wartości które nas interesują: Przyjmują następujące wartości na: dealerze: W ERPie (tu należy wziąć poprawkę że nie mam tablic customowych z których brane są domyślne więc mogę mieć zakłamane dane) Po kolei 1220 jest identyczna na obu instancjach 1190 różni się pomiędzy ERPem i dealerem, ale jej wartość pochodzi z customa którego nie mam, więc może na mojej bazie ERP źle to wskazywać - mus...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: iiwanca@drutex.com.pl | Date: 10.07.2025 13:04
Type: Answer | 
Re: [AW-229996] Fwd: Fwd: Fwd: Fwd: CANTOR | Błąd wizualizacji drzwi MB86 z panelem 2x zlicowanym (9)
Hej,
Wartości które nas interesują:

Przyjmują następujące wartości na:
dealerze:

W ERPie (tu należy wziąć poprawkę że nie mam tablic customowych z których brane są domyślne więc mogę mieć zakłamane dane)

Po kolei
1220 jest identyczna na obu instancjach
1190 różni się pomiędzy ERPem i dealerem, ale jej wartość pochodzi z customa którego nie mam, więc może na mojej bazie ERP źle to wskazywać - musisz sprawdzić po swojej stronie jaką wartość ta właściwość przyjmuje na ERPie

165 również się różni:
po lewej ERP, po prawej dealer

Na dealerze zachodzi warunek #40, na ERPie dopiero #43 (Seq #)

NakładkaTypProd to również właściwość - 1050 - ona swoją wartość bierze również z tablicy customowej której nie mam więc to również może umnie na ERPie zakłamywać (na dealerze mam customy bo otrzymuje pełny backup bazy)

Problemem mogą tu być np różnice w wartościach w tabelach customowych, do zweryfikowania po waszej stronie wartości właściwości w aufartik dla zlecenia na ERPie…
```

</details>

---

### [AW-235621] — Brak wydruku do producenta szyb - wydruk szprosu

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-235621]` |
| **Status** | 🔵 In Progress |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 10.07.2025 12:31 |

**Description:**

> Re: [AW-235621] Brak wydruku do producenta szyb - wydruk szprosu (3) tak tylko że jak mają  szprosy zawsze im się domyślnie tworzą 2 pliki jeden z wymiarami drugi rysunkami (szkic szprosów) a w tym przypadku nie. dla szprosu 18,26 lub wiedeński  to działa  tylko przy samym duplexie nie Logo Wikęd *Robert* *Krampikowski* Specjalista ds. IT tel. (+48) 601-194-538 <tel:(+48) 601-194-538> | (58) 738-66-80 <tel:(58) 738-66-80> robert.krampikowski@wiked.pl *WIKĘD Sp. z o.o.* ul. Wielki Las 19, 84-242 ...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Robert Krampikowski (robert.krampikowski@wiked.pl)
To: support.cantor.pl@a-w.com | Date: 10.07.2025 12:31
Type: Request | 
Re: [AW-235621] Brak wydruku do producenta szyb - wydruk szprosu (3)
tak tylko że jak mają  szprosy zawsze im się domyślnie tworzą 2 pliki
jeden z wymiarami drugi rysunkami (szkic szprosów) a w tym przypadku nie.

dla szprosu 18,26 lub wiedeński  to działa  tylko przy samym duplexie nie

Logo Wikęd *Robert* *Krampikowski*
Specjalista ds. IT
tel. (+48) 601-194-538 <tel:(+48) 601-194-538> | (58) 738-66-80
<tel:(58) 738-66-80>
robert.krampikowski@wiked.pl *WIKĘD Sp. z o.o.*
ul. Wielki Las 19, 84-242 Luzino
www.wiked.pl <https://wiked.pl>

W dniu 2025-07-10 o 09:52, Support Cantor Poland pisze:
>
> Cześć,
> W domyślnym raporcie 25000 (wydruk zamówienia) nie wyświetlamy
> grafiki, ale system można wysterować w ten sposób aby generować
> specjalny załącznik zawierający wszelkie informacje o szprosach:
>
> Tak wygląda przykładowy plik:
>
> Serdecznie pozdrawiam
>
> Patryk Muszkiet
> ###EOM##
>
>
>
> Phone: +48 61 438 47 44
> Mobile: +4964196620-0
> Email: _support.cantor.pl@a-w.com <mailto:support.pl@a-w.com>_
>
> A+W …
```

</details>

---

### [AW-236068] — [urgent] Na ftp tworzą się zipy zamówieniami klientów

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-236068]` |
| **Status** | 🔵 In Progress |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 10.07.2025 09:08 |

**Description:**

> Re: [AW-236068] [urgent] Na ftp tworzą się zipy zamówieniami klientów (6) Cześć. Nie jesteśmy w stanie tego u nas odtworzyć. Błąd dalej występuje. Z tego co widzę nie jest to też reguła u jednego klienta. Jest jakaś losowość. Wielu rożnych  klientów. Na bazie AWSOA_DES_PROD zapytanie /SELECT TOP (1000) [Guid] ,[VersionId] ,[LockingToken] ,[SenderPartnerGuid] ,[DataPackageType] ,[Sequence] ,[Data] ,[Description] ,[EntryDate] FROM [AWSOA_DES_PROD].[dbo].[Core_BuPa_DataPackages] where Data like '%....

<details>
<summary>View Full Conversation Thread</summary>

```
From: Dawid Prądziński (dpradzinski@drutex.com.pl)
To: support.cantor.pl@a-w.com | Date: 10.07.2025 09:08
Type: Request | 
Re: [AW-236068] [urgent] Na ftp tworzą się zipy zamówieniami klientów (6)
Cześć.

Nie jesteśmy w stanie tego u nas odtworzyć.

Błąd dalej występuje.

Z tego co widzę nie jest to też reguła u jednego klienta. Jest jakaś
losowość. Wielu rożnych  klientów.

Na bazie AWSOA_DES_PROD zapytanie

/SELECT TOP (1000) [Guid]
      ,[VersionId]
      ,[LockingToken]
      ,[SenderPartnerGuid]
      ,[DataPackageType]
      ,[Sequence]
      ,[Data]
      ,[Description]
      ,[EntryDate]
  FROM [AWSOA_DES_PROD].[dbo].[Core_BuPa_DataPackages] where Data like
'%.zip%' and DataPackageType  = 2 order by EntryDate desc/

Wynik w załączniku.

Pozdrawiam.

W dniu 10.07.2025 o 08:18, Support Cantor Poland pisze:
>
> Hej,
>
> Temat nie odtwarza się na naszym środowisku, nawet po wskazaniu tej
> konkretniej wersji dllek z której korzystacie.
>
> Pytanie czy wy jesteście w stanie to wywołać na jednej ze swoich
> testowych instancji dealerskich?
>
> Serdecznie pozdrawiam
>
> Patryk Muszkiet
> ###EOM##
>
>
>
> Phone: +48 61…
```

</details>

---

### [AW-235551] — Domyślny dostawca - nieprawidłowe wyświetlanie

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-235551]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 09.07.2025 15:45 |

**Description:**

> RE: [AW-235551] Domyślny dostawca - nieprawidłowe wyświetlanie (2) Hej, Nie jest to kolumna cantorowa, tylko customowy widok. Systemowa kolumna zwraca prawidłowy numer Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan Amtsgeric...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: L.Kempiak@krispol.pl | Date: 09.07.2025 15:45
Type: Answer | 
RE: [AW-235551] Domyślny dostawca - nieprawidłowe wyświetlanie (2)
Hej,
Nie jest to kolumna cantorowa, tylko customowy widok.
Systemowa kolumna zwraca prawidłowy numer 

Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus in Ihr System gelangen,…
```

</details>

---

### [AW-234369] — Konfigurator Rodenberg

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-234369]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 09.07.2025 15:20 |

**Description:**

> RE: [AW-234369] Konfigurator Rodenberg (4) Hej, My jako A+W jedynie umożliwiamy integracje z interfejsem Rodenberg, nie odpowiadamy za jego rozwój. To pytanie należy skierować do supportu po ich stronie Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mar...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: wdrozenie@empol.pl | Date: 09.07.2025 15:20
Type: Answer | 
RE: [AW-234369] Konfigurator Rodenberg (4)
Hej,
My jako A+W jedynie umożliwiamy integracje z interfejsem Rodenberg, nie odpowiadamy za jego rozwój. To pytanie należy skierować do supportu po ich stronie 
Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung …
```

</details>

---

### [AW-231407] — Kolor prowadnic rolet / zakończeń prowadnic

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-231407]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 09.07.2025 14:53 |

**Description:**

> RE: [AW-231407] Brak odwzorowania koloru skrzynki rolety po zmianie (4) Hej Dawid, Udało mi się namierzyć gdzie jest problem - brakuje koloru systemowego A53, dlatego wyświelta się biały zamiast niego: Dodałem wpis na podstawie A23 Po dodaniu wpisu: Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: ...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: d.precht@pagen.pl | Date: 09.07.2025 14:53
Type: Answer | 
RE: [AW-231407] Brak odwzorowania koloru skrzynki rolety po zmianie (4)
Hej Dawid,
Udało mi się namierzyć gdzie jest problem - brakuje koloru systemowego A53, dlatego wyświelta się biały zamiast niego:
Dodałem wpis na podstawie A23

Po dodaniu wpisu:

Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. …
```

</details>

---

### [AW-231814] — Cantor is crashing

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-231814]` |
| **Status** | 🔵 In Progress |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 09.07.2025 14:33 |

**Description:**

> Re: [AW-231814] Błąd | Cantor wyłącza się (23) Hej, Wykonują się bezproblemowo. Pozdrawiam, Mateusz Medwid Mateusz Medwid Specjalista ds. IT <https://www.drutex.eu/> *PL:* + 48 59 822 91 01 | *Fax:* + 48 59 822 91 03 DRUTEX S.A. Lęborska 31 | Bytów 77-100 | Polska NIP 8‌42 1‌6 2‌2 7‌20 www.drutex.eu <https://www.drutex.eu/> <https://www.facebook.com/DrutexSA/> <http://www.instagram.com/drutex_com/> <https://www.drutex.pl/pl/produkty/d-gate.html> DRUTEX S.A. z siedzibą w Bytowie zarejestrowany zo...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Mateusz Medwid (mmedwid@drutex.com.pl)
To: support.cantor.pl@a-w.com | Date: 09.07.2025 14:33
Type: Request | 
Re: [AW-231814] Błąd | Cantor wyłącza się (23)
Hej,

Wykonują się bezproblemowo.

Pozdrawiam,

Mateusz Medwid

Mateusz Medwid

Specjalista ds. IT

<https://www.drutex.eu/>

*PL:* + 48 59 822 91 01 | *Fax:* + 48 59 822 91 03

DRUTEX S.A.

Lęborska 31 | Bytów 77-100 | Polska
NIP 8‌42 1‌6 2‌2 7‌20
www.drutex.eu <https://www.drutex.eu/>

<https://www.facebook.com/DrutexSA/>
<http://www.instagram.com/drutex_com/>

<https://www.drutex.pl/pl/produkty/d-gate.html>

DRUTEX S.A. z siedzibą w Bytowie zarejestrowany został w Krajowym
Rejestrze Sądowym pod nr 0000140428 prowadzonym przez Sąd Rejonowy VIII
Wydział Gospodarczy Krajowego Rejestru Sądowego w Gdańsku. BDO
0‌00001469. Kapitał zakładowy, opłacony DRUTEX S.A. wynosi 21.690.000,00 zł

DRUTEX S.A. oświadcza, że posiada status dużego przedsiębiorcy w
rozumieniu Ustawy z dnia 8 marca 2013 r. o przeciwdziałaniu nadmiernym
opóźnieniom w transakcjach handlowych (Dz. U. z 2013 r., poz. 403 ze zm.).

Administratorem danych osobowych przetwarzanych w …
```

</details>

---

### [AW-235772] — rozchody materiału - różnice

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-235772]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 09.07.2025 14:30 |

**Description:**

> RE: [AW-235772] rozchody materiału - różnice (5) Rozumiem, myślę że jeśli usuniemy księgowanie, które Pan wykonał, to powinno nam wystarczyć do odtworzenia problemu po naszej stronie. Serdecznie pozdrawiam Radoslaw Jaruszewski ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Ty...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Radoslaw Jaruszewski (support.cantor.pl@a-w.com)
To: magazyn@pagen.pl | Date: 09.07.2025 14:30
Type: Answer | 
RE: [AW-235772] rozchody materiału - różnice (5)
Rozumiem, myślę że jeśli usuniemy księgowanie, które Pan wykonał, to powinno nam wystarczyć do odtworzenia problemu po naszej stronie.
Serdecznie pozdrawiam
Radoslaw Jaruszewski
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem…
```

</details>

---

### [AW-235392] — Rozróżnienie narzutów wg kosztów

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-235392]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 09.07.2025 14:21 |

**Description:**

> RE: [AW-235392] Rozróżnienie narzutów wg kosztów (2) Cześć, Z tego co sprawdziłem nie da się tym sterować w ten sposób - narzuty są przypisane według rekordu użytego w kalkulacji kosztów: Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyl...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: m.gwozdz@budvar.pl | Date: 09.07.2025 14:21
Type: Answer | 
RE: [AW-235392] Rozróżnienie narzutów wg kosztów (2)
Cześć,
Z tego co sprawdziłem nie da się tym sterować w ten sposób - narzuty są przypisane według rekordu użytego w kalkulacji kosztów:

Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem e…
```

</details>

---

### [AW-236213] — Customers doesn't see the tickets which are assigned to channel R&D Cantor/R&D Cantor Machines

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-236213]` |
| **Status** | 🟡 New |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 09.07.2025 11:42 |

**Description:**

> [AW-236213] Customers doesn't see the tickets which are assigned to channel R&D Cantor/R&D Cantor Machines (2) Hello Leon, we have recently been receiving occasional reports from our customers that they are unable to see their tickets in the customer portal [AW-234591]: I suspect the issue might be related to the assigned channel 'R&D Cantor/R&D Cantor Machines'. Could you check if there's anything missing in the channel's master data? Serdecznie pozdrawiam Radoslaw Jaruszewski ###EOM## Phone:  ...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Support Cantor Poland (support.cantor.pl@a-w.com)
To: pf-support@a-w.com | Date: 09.07.2025 11:42
Type: Request | 
[AW-236213] Customers doesn't see the tickets which are assigned to channel R&D Cantor/R&D Cantor Machines (2)
 Hello Leon, we have recently been receiving occasional reports from our customers that they are unable to see their tickets in the customer portal [AW-234591]:

I suspect the issue might be related to the assigned channel 'R&D Cantor/R&D Cantor Machines'. Could you check if there's anything missing in the channel's master data?
Serdecznie pozdrawiam
Radoslaw Jaruszewski
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu lö…
```

</details>

---

### [AW-236010] — Dealer - wersja zamówienia wyższa niż baza danych

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-236010]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 09.07.2025 10:50 |

**Description:**

> RE: [AW-236010] Dealer - wersja zamówienia wyższa niż baza danych (4) Cześć, Zamówienie z załącznika ma wersje 277, a więc komunikat jest zasadny. Serdecznie pozdrawiam Lukasz Lieske ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan Amtsgericht Gießen/Gießen Local ...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Lukasz Lieske (support.cantor.pl@a-w.com)
To: jkreft@drutex.com.pl | Date: 09.07.2025 10:50
Type: Answer | 
RE: [AW-236010] Dealer - wersja zamówienia wyższa niż baza danych (4)
Cześć,
Zamówienie z załącznika ma wersje 277, a więc komunikat jest zasadny.

Serdecznie pozdrawiam
Lukasz Lieske
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus in Ihr System gelangen, haften wir nicht für die ev…
```

</details>

---

### [AW-230659] — Brak tłumaczenia

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-230659]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 08.07.2025 14:58 |

**Description:**

> Re: [AW-230659] Brak tłumaczenia (6) Hej, Bo w tablicy wyszukiwań wciąż powołujesz sie na tablicę customową i z jej kolumny opis wyświetlasz tekst Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan Amtsgericht Gießen/Gießen Loca...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: mmedwid@drutex.com.pl | Date: 08.07.2025 14:58
Type: Answer | 
Re: [AW-230659] Brak tłumaczenia (6)
Hej,
Bo w tablicy wyszukiwań wciąż powołujesz sie na tablicę customową i z jej kolumny opis wyświetlasz tekst

Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus in Ihr System ge…
```

</details>

---

### [AW-236034] — Refreshing All Properties After Position Changes

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-236034]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 08.07.2025 12:39 |

**Description:**

> RE: [AW-236034] Refreshing All Properties After Position Changes (2) Hello Billel, Thank you for your message. Unfortunately, it’s not possible to force the update of all properties automatically every time something changes in the position. However, you can use the top-attribute refresh option to trigger updates based on selected attributes. Please keep in mind that enabling all available options in this configuration can have a significant impact on Cantor’s performance — especially when enter...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Radoslaw Jaruszewski (support.cantor.pl@a-w.com)
To: billel.benmakhlouf@oxxo.dz | Date: 08.07.2025 12:39
Type: Answer | 
RE: [AW-236034] Refreshing All Properties After Position Changes (2)
Hello Billel,
Thank you for your message.
Unfortunately, it’s not possible to force the update of all properties automatically every time something changes in the position. However, you can use the top-attribute refresh option to trigger updates based on selected attributes.

Please keep in mind that enabling all available options in this configuration can have a significant impact on Cantor’s performance — especially when entering or modifying positions. We recommend using this feature with care and only for attributes that are truly critical for dependent calculations or validations.
Serdecznie pozdrawiam
Radoslaw Jaruszewski
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Di…
```

</details>

---

### [AW-235968] — Dealer - błąd przy wyborze trawersów

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-235968]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 08.07.2025 09:03 |

**Description:**

> Re: [AW-235968] Dealer - błąd przy wyborze trawersów (4) Hej, Być może, wniosek jest taki że na dealerze nie zadziała bo nie ma tam MWMAT i pozostałych tabel materiałowych Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan Amtsg...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: jkreft@drutex.com.pl | Date: 08.07.2025 09:03
Type: Answer | 
Re: [AW-235968] Dealer - błąd przy wyborze trawersów (4)
Hej,
Być może, wniosek jest taki że na dealerze nie zadziała bo nie ma tam MWMAT i pozostałych tabel materiałowych 
Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus in Ihr Syste…
```

</details>

---

### [AW-235331] — Numeracja zleceń

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-235331]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 07.07.2025 14:56 |

**Description:**

> Re: [AW-235331] Numeracja zleceń (4) Hej, Możesz to zmienić według własnego uznania – sprawdź również zakładkę „Number Pool” i usuń istniejącą wartość. Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan Amtsgericht Gießen/Gießen...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: jkreft@drutex.com.pl | Date: 07.07.2025 14:56
Type: Answer | 
Re: [AW-235331] Numeracja zleceń (4)
Hej,
Możesz to zmienić według własnego uznania – sprawdź również zakładkę „Number Pool” i usuń istniejącą wartość.

Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus in Ihr Syst…
```

</details>

---

### [AW-234305] — Znikająca grafika - bramy

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-234305]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 07.07.2025 14:39 |

**Description:**

> FW: Re: [AW-234305] Znikająca grafika - bramy (8) Hej, Możesz podrzucić mi paczkę z weekendu? Chodzi o dev -> prePROD Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan Amtsgericht Gießen/Gießen Local Court: HRB 7963 Diese E-Mai...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: jkreft@drutex.com.pl | Date: 07.07.2025 14:39
Type: Answer | 
FW: Re: [AW-234305] Znikająca grafika - bramy (8)
Hej,
Możesz podrzucić mi paczkę z weekendu?
Chodzi o dev -> prePROD
Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus in Ihr System gelangen, haften wir nicht für die evtl. ents…
```

</details>

---

### [AW-235790] — DES - brak dostępu do DES

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-235790]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 07.07.2025 10:07 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Radoslaw Jaruszewski
To: | Date: 07.07.2025 10:07
Type: State changed | 
RE: [AW-235790] DES - brak dostępu do DES (5)
Sesja z klientem - wykonany test na poświadczeniach dilera: połączenie nawiązane poprawnie (Jacek wpisał poswiadczenia na swojej wersji testowej dilera i wykonał prosty test z nadaniem guid dla dilera drugiego poziomu).
Sprawdzone logi IIS oraz ICE, w logach IIS widoczne błędy z kodem 500 w godzinach 8:00 do 9:55 (04.07.25), w ICE w tym samym czasie brak jakichkolwiek błedów, jednoczśnie pojawiają się błędy w późniejszym przedziale czasowym 10:10 do około 12:00 z wpisem o pustym parametrze w żądaniu.
Na tę chwilę należy zweryfikować czy problem nadal istnieje po stronie klienta - jeśli tak to, należałoby na serwerze DES uruchomić wireshark i sprawdzić czy żądania przychodzące i odpowiedzi są przetwarzane prawidłowo na poziomie sieciowym.
Wszystkie informacje przekazane Jackowi - da nam znać po wykonaniu testów z wiresharkiem.
```

</details>

---

### [AW-232641] — Zgłoszenie błędu

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-232641]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 07.07.2025 09:36 |

**Description:**

> RE: [AW-232641] Zgłoszenie błędu (2) Hej, Nowe dllki na FTPie: Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan Amtsgericht Gießen/Gießen Local Court: HRB 7963 Diese E-Mail ist ausschließlich für den Adressaten bestimmt und ka...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: lukasz.urwanowicz@witraz.eu | Date: 07.07.2025 09:36
Type: Answer | 
RE: [AW-232641] Zgłoszenie błędu (2)
Hej,
Nowe dllki na FTPie:

Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus in Ihr System gelangen, haften wir nicht für die evtl. entstandenen Schäden.

This e-mail is for t…
```

</details>

---

### [AW-235771] — bRAK ZAKŁADEK IQUOTE

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-235771]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 04.07.2025 14:23 |

**Description:**

> RE: [AW-235771] bRAK ZAKŁADEK IQUOTE (2) Cześć Przemek, czy w momencie zgłoszenia tego przez klienta - usługi nie były wykorzystane w 100% - w sensie nie było już wolnych commercial document-ów lub webconfiguratorów czy sprawdzaliście w momencie awarii ile osób było zalogowanych w danym momencie do IQuote? Serdecznie pozdrawiam Radoslaw Jaruszewski ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 W...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Radoslaw Jaruszewski (support.cantor.pl@a-w.com)
To: przemyslaw.barthelke@wiked.pl | Date: 04.07.2025 14:23
Type: Answer | 
RE: [AW-235771] bRAK ZAKŁADEK IQUOTE (2)
Cześć Przemek,
czy w momencie zgłoszenia tego przez klienta - usługi nie były wykorzystane w 100% - w sensie nie było już wolnych commercial document-ów lub webconfiguratorów czy sprawdzaliście w momencie awarii ile osób było zalogowanych w danym momencie do IQuote?
 
Serdecznie pozdrawiam
Radoslaw Jaruszewski
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe …
```

</details>

---

### [AW-233795] — Automatyczna zmiana połączeń

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-233795]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 04.07.2025 11:48 |

**Description:**

> Automatyczna odpowiedź: [AW-233795] Automatyczna zmiana połączeń (4) Witam, W dniach 20.06 - 04.07.2025 przebywam na urlopie. Zgłoszenia dotyczące technologii proszę wysyłać na Helpdesk. Na pozostałe odpowiem sukcesywnie po powrocie. Pozdrawiam Mariusz Marczak KRISHOME Sp. z o.o., ul. Budowlana 1, Psary Małe, 62-300 Września, tel. +48 61 639 86 88, fax +48 436 76 48, e-mail: biuro@krishome.eu, NIP PL 7891787470, KRS 0000768528, Kapitał zakładowy 26 050 000 PLN [https://krishome.pl/stopka/promo.p...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Mariusz Marczak (m.marczak@krishome.eu)
To: support.cantor.pl@a-w.com | Date: 04.07.2025 11:48
Type: Request | 
Automatyczna odpowiedź: [AW-233795] Automatyczna zmiana połączeń (4)
Witam,

W dniach 20.06 - 04.07.2025 przebywam na urlopie.
Zgłoszenia dotyczące technologii proszę wysyłać na Helpdesk.
Na pozostałe odpowiem sukcesywnie po powrocie.

Pozdrawiam
Mariusz Marczak

KRISHOME Sp. z o.o., ul. Budowlana 1, Psary Małe, 62-300 Września, tel. +48 61 639 86 88, fax +48 436 76 48, e-mail: biuro@krishome.eu,
NIP PL 7891787470, KRS 0000768528, Kapitał zakładowy 26 050 000 PLN [https://krishome.pl/stopka/promo.png]  <https://eu1.hubs.ly/H0dpQ270> Uwaga: ten e-mail jest przeznaczony wyłącznie dla adresata, może zawierać informacje zastrzeżone i prawnie zastrzeżone. Jeżeli otrzymałeś/aś tę wiadomość e-mail przez pomyłkę, powiadom nadawcę i usuń tę wiadomość e-mail wraz ze wszystkimi załącznikami.
```

</details>

---

### [AW-234120] — Problem podczas aktualizacji cim do wersji 7.9

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-234120]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 04.07.2025 09:47 |

**Description:**

> RE: [AW-234120] Problem podczas aktualizacji cim do wersji 7.9 (3) Dzień dobry, znaczna większość błędów odnosi się do duplikatów tzn wartości są już w bazie - te można potwierdzić. Do zweryfikowania jak fizycznie wyglądają te dwie tabele z poniższych błędów Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Di...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: M.Malyjasiak@krishome.eu | Date: 04.07.2025 09:47
Type: Answer | 
RE: [AW-234120] Problem podczas aktualizacji cim do wersji 7.9 (3)
Dzień dobry,
znaczna większość błędów odnosi się do duplikatów tzn wartości są już w bazie - te można potwierdzić.
Do zweryfikowania jak fizycznie wyglądają te dwie tabele z poniższych błędów 

Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schut…
```

</details>

---

### [AW-235540] — Cantor crashes whenever any action is performed on Order 5106648

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-235540]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 04.07.2025 08:27 |

**Description:**

> FW: RE: [AW-235540] Issue with Order 5106648 – System Block (10) Hello Billel, I received a response from R&D — the issue was caused by an incorrect product type ('P') in the AUFPOS table. We have updated it to the correct value ('E'), and everything is working properly now: The question here is: how it happend and how we can reproduce this issue? Serdecznie pozdrawiam Radoslaw Jaruszewski ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Pols...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Radoslaw Jaruszewski (support.cantor.pl@a-w.com)
To: billel.benmakhlouf@oxxo.dz | Date: 04.07.2025 08:27
Type: Answer | 
FW: RE: [AW-235540] Issue with Order 5106648 – System Block (10)
Hello Billel,
I received a response from R&D — the issue was caused by an incorrect product type ('P') in the AUFPOS table. We have updated it to the correct value ('E'), and everything is working properly now:

The question here is: how it happend and how we can reproduce this issue?
Serdecznie pozdrawiam
Radoslaw Jaruszewski
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unb…
```

</details>

---

### [AW-233256] — wiki

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-233256]` |
| **Status** | 🔵 In Progress |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 04.07.2025 05:51 |

**Description:**

> RE: [EXT] RE: [AW-233256] wiki (8) Brakuje podstawowych danych konfiguracyjnych np. takich jak typ lokalizacji Albo typów zleceń Nie ma podstawowych informacji, które raczej się nie zmieniają ☹ Waldemar Korbik From: Support Cantor Poland <support.cantor.pl@a-w.com> Sent: Thursday, July 3, 2025 2:31 PM To: Waldemar Korbik <w.korbik@krishome.eu> Subject: RE: [EXT] RE: [AW-233256] wiki Cześć Waldek, niestety ale jeśli jakiegoś dokumentu nie ma w Wiki to znaczy, że był na tyle nieaktualny, że został...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Waldemar Korbik (w.korbik@krishome.eu)
To: support.cantor.pl@a-w.com | Date: 04.07.2025 05:51
Type: Request | 
RE: [EXT] RE: [AW-233256] wiki (8)
Brakuje podstawowych danych konfiguracyjnych np. takich jak typ lokalizacji

Albo typów zleceń

Nie ma podstawowych informacji, które raczej się nie zmieniają ☹

Waldemar Korbik

From: Support Cantor Poland <support.cantor.pl@a-w.com>
Sent: Thursday, July 3, 2025 2:31 PM
To: Waldemar Korbik <w.korbik@krishome.eu>
Subject: RE: [EXT] RE: [AW-233256] wiki

Cześć Waldek,
niestety ale jeśli jakiegoś dokumentu nie ma w Wiki to znaczy, że był na tyle nieaktualny, że został wycofany.
Poniżej przesyłam dla pewności dokumenty jakie ja mam widoczne w wiki:

Serdecznie pozdrawiam

Radoslaw Jaruszewski
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com<mailto:support.pl@a-w.com>

A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com<http://www.…
```

</details>

---

### [AW-232129] — Rezerwacja materiału.

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-232129]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 03.07.2025 13:25 |

**Description:**

> RE: [AW-232129] Re: Rezerwacja materiału. (4) Hej, Jedyna szansa to odtworzyć bazę z backupa, wyzerować zlecenie i przekalkulować z trace na te opcje. Jeśli test na poligonie był wykonany w ten właśnie sposób i nie zwrócił tego samego wyniku to niestety nie dojdziemy co tam zaszło Serdecznie pozdrawiam Patryk Muszkiet ###EOM## ​ Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Ge...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: wdrozenie@empol.pl | Date: 03.07.2025 13:25
Type: Answer | 
RE: [AW-232129] Re: Rezerwacja materiału. (4)
Hej,
Jedyna szansa to odtworzyć bazę z backupa, wyzerować zlecenie i przekalkulować z trace na te opcje.

Jeśli test na poligonie był wykonany w ten właśnie sposób i nie zwrócił tego samego wyniku to niestety nie dojdziemy co tam zaszło
Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##
​
Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. …
```

</details>

---

### [AW-235635] — Problem z rozchodem materiałów

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-235635]` |
| **Status** | 🟡 New |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 03.07.2025 11:47 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet
To: | Date: 03.07.2025 11:47
Type: State changed | 
RE: [AW-235635] Problem z rozchodem materiałów (2)
```

</details>

---

### [AW-235511] — Db szyb

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-235511]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 03.07.2025 08:50 |

**Description:**

> RE: [AW-235511] Db szyb (3) Cze Michał, Informacje dotyczące szyby lecą do tabeli FELDFUEL a jej wartość RW znajduje się w kolumnie RWRWERT tak jak na poniższym zdjęciu: Serdecznie pozdrawiam Lukasz Lieske ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan Amtsgeric...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Lukasz Lieske (support.cantor.pl@a-w.com)
To: mslugocki@empol.pl | Date: 03.07.2025 08:50
Type: Answer | 
RE: [AW-235511] Db szyb (3)
Cze Michał,
 
Informacje dotyczące szyby lecą do tabeli FELDFUEL a jej wartość RW znajduje się w kolumnie RWRWERT tak jak na poniższym zdjęciu:

Serdecznie pozdrawiam
Lukasz Lieske
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail tr…
```

</details>

---

### [AW-235161] — Wyświetlenie właściwości klasy na wydruku ofert/zleceń

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-235161]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 02.07.2025 14:29 |

**Description:**

> RE: [AW-235161] Wyświetlenie właściwości klasy na wydruku ofert/zleceń (4) To najlepsze rozwiązanie odpalić trace podczas wydruku na bazę danych i szukać po wartości kluczowej '8000' Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: d.precht@pagen.pl | Date: 02.07.2025 14:29
Type: Answer | 
RE: [AW-235161] Wyświetlenie właściwości klasy na wydruku ofert/zleceń (4)
To najlepsze rozwiązanie odpalić trace podczas wydruku na bazę danych i szukać po wartości kluczowej '8000'

Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus in Ihr System gelan…
```

</details>

---

### [AW-235155] — Request for Documentation – Cart (Rack) Management Module in CANTOR

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-235155]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 02.07.2025 14:26 |

**Description:**

> RE: [AW-235155] Request for Documentation – Cart (Rack) Management Module in CANTOR (2) Hi Billel, Access to whole available documentation you can find on https://portal.a-w.com/us/member-login/ Your account was created in the past From what I have checked, we do not have a manual on the subject and I think the best source of knowledge in this case would be a meeting with a consultant. You can send me an agenda in response: what you want to achieve and what topics to cover and I will send it to ...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: billel.benmakhlouf@oxxo.dz | Date: 02.07.2025 14:26
Type: Answer | 
RE: [AW-235155] Request for Documentation – Cart (Rack) Management Module in CANTOR (2)
Hi Billel,
Access to whole available documentation you can find on https://portal.a-w.com/us/member-login/
Your account was created in the past 

From what I have checked, we do not have a manual on the subject and I think the best source of knowledge in this case would be a meeting with a consultant. You can send me an agenda in response: what you want to achieve and what topics to cover and I will send it to the Professional services channel
Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nic…
```

</details>

---

### [AW-235175] — W jaki sposób możemy czyścić bazę AWSOA ?

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-235175]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 02.07.2025 14:17 |

**Description:**

> RE: ODP: [AW-235175] W jaki sposób możemy czyścić bazę AWSOA ? (4) Hej, Faktycznie web_carts przoduje, usunięcie starszych ofert powinno zwolnić sporo miejsca i nie być aż tak bardzo inwazyjne (nawet jeśli ktoś będzie chciał wrócić do koszyka to można zlecenie skopiować i działać dalej na kopii) Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska w...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: szymon.kaczykowski@wiked.pl | Date: 02.07.2025 14:17
Type: Answer | 
RE: ODP: [AW-235175] W jaki sposób możemy czyścić bazę AWSOA ? (4)
Hej,
Faktycznie web_carts przoduje, usunięcie starszych ofert powinno zwolnić sporo miejsca i nie być aż tak bardzo inwazyjne (nawet jeśli ktoś będzie chciał wrócić do koszyka to można zlecenie skopiować i działać dalej na kopii) 
Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstver…
```

</details>

---

### [AW-235491] — Układ kolumn

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-235491]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 02.07.2025 12:28 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Lukasz Lieske
To: Lukasz Lieske | Date: 02.07.2025 12:28
Type: State changed | 
Układ kolumn (3)
Lukasz Lieske has taken the ticket
```

</details>

---

### [AW-235305] — Wyświetlanie szerokości prowadnic na rysunku

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-235305]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 02.07.2025 11:45 |

**Description:**

> Re: [AW-235305] Wyświetlanie szerokości prowadnic na rysunku (4) Hej za pomocą właściwości 144-146 możesz skalować obiekty rysunkowe Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan Amtsgericht Gießen/Gießen Local Court: HRB 7...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: dakmiecik@drutex.com.pl | Date: 02.07.2025 11:45
Type: Answer | 
Re: [AW-235305] Wyświetlanie szerokości prowadnic na rysunku (4)
Hej za pomocą właściwości 144-146 możesz skalować obiekty rysunkowe 

Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus in Ihr System gelangen, haften wir nicht für die evtl. ent…
```

</details>

---

### [AW-218582] — DUMP to analyse - random times while working with the program, the application is shutting down on its own

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-218582]` |
| **Status** | 🔵 In Progress |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 02.07.2025 07:16 |

**Description:**

> Re: FW: Re: [AW-218582] Niespodziewane zamykanie się aplikacji Cantor (59) Cześć. Dalej wywala program. Ciężko powiedzieć ale zdaje się jakby mniej było tych błędów. Z kilkunastu do powiedzmy 5. Możliwe że związane jest to z intensywnością pracy a nie samą zmianą parametru. Pozdrawiam. W dniu 27.06.2025 o 14:40, Support Cantor Poland pisze: > > Cześć Dawid, > czy mógłbym Cie prosić o przestawienie konfiguracji programu > "MemoryMode" na wartość 2 w sekcji DATENBANK: > > Ustawienie to zwalnia pam...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Dawid Prądziński (dpradzinski@drutex.com.pl)
To: support.cantor.pl@a-w.com | Date: 02.07.2025 07:16
Type: Request | 
Re: FW: Re: [AW-218582] Niespodziewane zamykanie się aplikacji Cantor (59)
Cześć.

Dalej wywala program. Ciężko powiedzieć ale zdaje się jakby mniej było
tych błędów. Z kilkunastu do powiedzmy 5.

Możliwe że związane jest to z intensywnością pracy a nie samą zmianą
parametru.

Pozdrawiam.

W dniu 27.06.2025 o 14:40, Support Cantor Poland pisze:
>
> Cześć Dawid,
> czy mógłbym Cie prosić o przestawienie konfiguracji programu
> "MemoryMode" na wartość 2 w sekcji DATENBANK:
>
> Ustawienie to zwalnia pamięć z głównego procesu, trzeba jednak wziąć
> pod uwagę, że może spaść prędkość działania aplikacji w razie
> problemów należy wrócić do poprzedniej konfiguracji.
> Wartość dla tego ustawienia należy wprowadzić w pliku ini:
>
> Po zmianie wymagany jest restart cantora u użytkownika który ma
> problem z samoczynnym zamykaniem aplikacji.
>
> Serdecznie pozdrawiam
>
> Radoslaw Jaruszewski
> ###EOM##
>
>
>
> Phone: +48 61 438 47 44
> Mobile: +4964196620-0
> Email: _*MailScanner has detected a possible fraud attempt from
> "a-…
```

</details>

---

### [AW-235066] — błąd grafiki podczas kopiowania oferty

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-235066]` |
| **Status** | 🔵 In Progress |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 30.06.2025 12:09 |

**Description:**

> Re: FW: RE: [AW-235066] błąd grafiki podczas kopiowania oferty (5) a zobacz  102110224 to są tez kopie oferty 102110127,102110128,102110161,102110226 Logo Wikęd *Robert* *Krampikowski* Specjalista ds. IT tel. (+48) 601-194-538 <tel:(+48) 601-194-538> | (58) 738-66-80 <tel:(58) 738-66-80> robert.krampikowski@wiked.pl *WIKĘD Sp. z o.o.* ul. Wielki Las 19, 84-242 Luzino www.wiked.pl <https://wiked.pl> W dniu 2025-06-30 o 09:52, Support Cantor Poland pisze: > > Hej, > > Wyeksportuj mi proszę wspomni...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Robert Krampikowski (robert.krampikowski@wiked.pl)
To: support.cantor.pl@a-w.com | Date: 30.06.2025 12:09
Type: Request | 
Re: FW: RE: [AW-235066] błąd grafiki podczas kopiowania oferty (5)
a zobacz  102110224

to są tez kopie oferty 102110127,102110128,102110161,102110226

Logo Wikęd *Robert* *Krampikowski*
Specjalista ds. IT
tel. (+48) 601-194-538 <tel:(+48) 601-194-538> | (58) 738-66-80
<tel:(58) 738-66-80>
robert.krampikowski@wiked.pl *WIKĘD Sp. z o.o.*
ul. Wielki Las 19, 84-242 Luzino
www.wiked.pl <https://wiked.pl>

W dniu 2025-06-30 o 09:52, Support Cantor Poland pisze:
>
> Hej,
>
> Wyeksportuj mi proszę wspomniane zamówienie 102110124
>
> Ja mam problem:
>
> Serdecznie pozdrawiam
>
> Patryk Muszkiet
> ###EOM##
>
>
>
> Phone: +48 61 438 47 44
> Mobile: +4964196620-0
> Email: _support.cantor.pl@a-w.com <mailto:support.pl@a-w.com>_
>
> A+W Software Polska Sp. z o. o.
> ul. Sikorskiego 44
> 62-300 Września
> Polska
>
>
>
> *www.a-w.com* <http://www.a-w.com/>
>
>
> Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt,
> Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
> Amtsgericht Gießen/Gießen Local Court: HRB 7…
```

</details>

---

### [AW-234126] — DEALER TEST - błąd przy imporcie

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-234126]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 30.06.2025 08:00 |

**Description:**

> RE: [AW-234126] DEALER TEST - błąd przy imporcie (11) Cześć, ok - będziemy w kontakcie Serdecznie pozdrawiam Radoslaw Jaruszewski ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan Amtsgericht Gießen/Gießen Local Court: HRB 7963 Diese E-Mail ist ausschließlich für d...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Radoslaw Jaruszewski (support.cantor.pl@a-w.com)
To: jkreft@drutex.com.pl | Date: 30.06.2025 08:00
Type: Answer | 
RE: [AW-234126] DEALER TEST - błąd przy imporcie (11)
Cześć,
ok - będziemy w kontakcie
Serdecznie pozdrawiam
Radoslaw Jaruszewski
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus in Ihr System gelangen, haften wir nicht für die evtl. entstandenen Schäden.

This e-mai…
```

</details>

---

### [AW-235063] — [urgent] Błąd pobierania update Cantor DEALER u klienta

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-235063]` |
| **Status** | 🔵 In Progress |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 30.06.2025 07:16 |

**Description:**

> Re: [AW-235063] [urgent] Błąd pobierania update Cantor DEALER u klienta (5) Cześć. Tu nie chodzi o opóźnienie, tylko o to że w ogóle się nie synchronizuje status dla tego klienta z bazą AWSOA. Klient nie był zablokowany w chwili zgłaszania taska, pisałem o tym na samym początku. Da się sprawdzić status sychronizacji? Czy był poprawny? Albo gdzie znajdę informacje w bazie AWSOA o statusie? Pozdrawiam. W dniu 27.06.2025 o 15:01, Support Cantor Poland pisze: > > Z tego co widzę to ten klient jest j...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Dawid Prądziński (dpradzinski@drutex.com.pl)
To: support.cantor.pl@a-w.com | Date: 30.06.2025 07:16
Type: Request | 
Re: [AW-235063] [urgent] Błąd pobierania update Cantor DEALER u klienta (5)
Cześć.

Tu nie chodzi o opóźnienie, tylko o to że w ogóle się nie synchronizuje
status dla tego klienta z bazą AWSOA.

Klient nie był zablokowany w chwili zgłaszania taska, pisałem o tym na
samym początku.

Da się sprawdzić status sychronizacji? Czy był poprawny? Albo gdzie
znajdę informacje w bazie AWSOA o statusie?

Pozdrawiam.

W dniu 27.06.2025 o 15:01, Support Cantor Poland pisze:
>
> Z tego co widzę to ten klient jest już aktywny:
>
> Sprawdź proszę jeszcze raz, sądzę, że powodem problemu jest opóźnienie
> z jakim usługa dodaje dane do bazy AWSOA (z informacja o statusie).
>
> Serdecznie pozdrawiam
>
> Radoslaw Jaruszewski
> ###EOM##
>
>
>
> Phone: +48 61 438 47 44
> Mobile: +4964196620-0
> Email: _*MailScanner has detected a possible fraud attempt from
> "a-w.com" claiming to be* support.cantor.pl@a-w.com
> <mailto:support.pl@a-w.com>_
>
> A+W Software Polska Sp. z o. o.
> ul. Sikorskiego 44
> 62-300 Września
> Polska
>
>
>
> *www…
```

</details>

---

### [AW-230058] — Moving with arrow keys through Top Packages and Top Attributes

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-230058]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 27.06.2025 14:09 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Nicola Pierre Wurbs
To: | Date: 27.06.2025 14:09
Type: State changed | 
RE: [AW-230058] Moving with arrow keys through Top Packages and Top Attributes (5)
We did a thorough analysis of the code and logic behind the navigation inside top attributes and it's meant to be done from top to bottom. If you use arrow down and are in the value column, it will stay in the same column and skip expandable rows. If you then use upward arrow you can select these and open/close them again with down.
It would be too great of an effort to make changes here and could lead to potential problems.
```

</details>

---

### [AW-219864] — DRUTEX Updateroutine 7.8-7.9

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-219864]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 26.06.2025 11:42 |

**Description:**

> RE: [AW-219864] DRUTEX Updateroutine 7.8-7.9 (47) Cześć, na FTP wrzuciłem paczkę z aktualizacją wersji dilerskiej 7.8 --->7.9 W paczce wykorzystane zostały dll-ki z 11.05.25 jeśli chcielibyście aby w trakcie aktualizacji podegrały się inne dll-ki to należy je umieścić w instalatorze w folderze: \Drutex_7.8-7.9\installdir\Cversion Przetestujcie proszę, jeśli pojawia się pytania to jesteśmy do dyspozycji. Serdecznie pozdrawiam Radoslaw Jaruszewski ###EOM## Phone:  +48 61 438 47 44 Mobile:  +496419...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Radoslaw Jaruszewski (support.cantor.pl@a-w.com)
To: jkreft@drutex.com.pl, mtelega@drutex.com.pl | Date: 26.06.2025 11:42
Type: Answer | 
RE: [AW-219864] DRUTEX Updateroutine 7.8-7.9 (47)
Cześć,
na FTP wrzuciłem paczkę z aktualizacją wersji dilerskiej 7.8 --->7.9

W paczce wykorzystane zostały dll-ki z 11.05.25 jeśli chcielibyście aby w trakcie aktualizacji podegrały się inne dll-ki to należy je umieścić w instalatorze w folderze: 
\Drutex_7.8-7.9\installdir\Cversion
Przetestujcie proszę, jeśli pojawia się pytania to jesteśmy do dyspozycji.
Serdecznie pozdrawiam
Radoslaw Jaruszewski
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung z…
```

</details>

---

### [AW-231641] — Błędy w menedżerze buforowania - kolejka 122 - Księgowanie statusów stojaków

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-231641]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 26.06.2025 10:56 |

**Description:**

> RE: [AW-231641] Błędy w menedżerze buforowania - kolejka 122 - Księgowanie statusów stojaków (13) Hej, Bazę mam - dzięki spojrzę na temat dziś lub jutro. Co do serwera FTP my nic nie blokujemy (jak widzisz z prywatnej sieci możesz się nawet dobić :P), również żaden inny klient nie miał podobnych problemów, więc raczej coś po waszej stronie blokuje Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: d.precht@pagen.pl | Date: 26.06.2025 10:56
Type: Answer | 
RE: [AW-231641] Błędy w menedżerze buforowania - kolejka 122 - Księgowanie statusów stojaków (13)
Hej,
Bazę mam - dzięki spojrzę na temat dziś lub jutro.
Co do serwera FTP my nic nie blokujemy (jak widzisz z prywatnej sieci możesz się nawet dobić :P), również żaden inny klient nie miał podobnych problemów, więc raczej coś po waszej stronie blokuje 
Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nic…
```

</details>

---

### [AW-234882] — Cena z narzutem w podpozycjach

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-234882]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 26.06.2025 10:46 |

**Description:**

> RE: [AW-234882] Cena z narzutem w podpozycjach (2) Cześć, Niestety nie ma możliwości aby to wysterować. Globalny rabat tyczy się pozycji, tak jak również wskazuje na to nazwa kolumny Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: mmedwid@drutex.com.pl | Date: 26.06.2025 10:46
Type: Answer | 
RE: [AW-234882] Cena z narzutem w podpozycjach (2)
Cześć,
Niestety nie ma możliwości aby to wysterować. Globalny rabat tyczy się pozycji, tak jak również wskazuje na to nazwa kolumny

Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein …
```

</details>

---

### [AW-234877] — Mapa bazy print

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-234877]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 26.06.2025 09:55 |

**Description:**

> RE: [AW-234877] Mapa bazy print (2) Hej, Struktura tej bazy jest dynamiczna - zależy co jest drukowane - od tego zależą nazwy kolumn np ..._600_102: jaki raport, który numer porządkowy itp. W związku z tym nie da się zrobić mapy tej bazy Jedynie informacjach o dostępnych kolumnach i ich nazwach jest dostępna w definicjach raportów: Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Si...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: mmedwid@drutex.com.pl | Date: 26.06.2025 09:55
Type: Answer | 
RE: [AW-234877] Mapa bazy print (2)
Hej,
Struktura tej bazy jest dynamiczna - zależy co jest drukowane - od tego zależą nazwy kolumn np ..._600_102: jaki raport, który numer porządkowy itp.
W związku z tym nie da się zrobić mapy tej bazy 
Jedynie informacjach o dostępnych kolumnach i ich nazwach jest dostępna w definicjach raportów:

Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sow…
```

</details>

---

### [AW-234530] — Pliki w instalatorze 7.9

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-234530]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 24.06.2025 15:15 |

**Description:**

> RE: [AW-234530] Pliki w instalatorze 7.9 (2) Hej, Potwierdzam, przyjąłem 🙂 Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan Amtsgericht Gießen/Gießen Local Court: HRB 7963 Diese E-Mail ist ausschließlich für den Adressaten bes...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: jkreft@drutex.com.pl | Date: 24.06.2025 15:15
Type: Answer | 
RE: [AW-234530] Pliki w instalatorze 7.9 (2)
Hej,
Potwierdzam, przyjąłem 🙂
Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus in Ihr System gelangen, haften wir nicht für die evtl. entstandenen Schäden.

This e-mail is fo…
```

</details>

---

### [AW-233168] — Przygotowanie paczki z wersją Cantor 7.9

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-233168]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 24.06.2025 13:14 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet
To: | Date: 24.06.2025 13:14
Type: State changed | 
RE: [AW-233168] Przygotowanie paczki z wersją Cantor 7.9 (14)
```

</details>

---

### [AW-234570] — dostęp do cenników

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-234570]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 24.06.2025 12:37 |

**Description:**

> RE: [AW-234570] dostęp do cenników (2) Cześć, Jest taka możliwość. Uprawnienia do odczytu i modyfikacji macierzy cen to 105 i 2002. Natomiast uprawnienia do odczytu i modyfikacji w tabelach kodów to 286 i 287. Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tie...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: mtelega@drutex.com.pl | Date: 24.06.2025 12:37
Type: Answer | 
RE: [AW-234570] dostęp do cenników (2)
Cześć,
Jest taka możliwość.
Uprawnienia do odczytu i modyfikacji macierzy cen to 105 i 2002.
   

Natomiast uprawnienia do odczytu i modyfikacji w tabelach kodów to 286 i 287.

Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. So…
```

</details>

---

### [AW-230519] — Zlecenie 2043895 nieprawidłowa ilość na CIM

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-230519]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 24.06.2025 10:17 |

**Description:**

> RE: [AW-230519] Zlecenie 2043895 nieprawidłowa ilość na CIM (3) Hej, Spojrzałem na przykład i wydaje mi się że 6 to prawidłowa liczba Baza CIM: 6 sztuk w tabeli CPB_TEILINFO Poprzez CPB_TEIL możemy sprawdzić barcody oraz LFDNR z aufartik barcody odnoszą się do poz1 ze wskazanego zlecenia: mamy odpowiednio 3 sztuki AUFARTIK widać tu również 3 sztuki Natomiast w zleceniu ilość na pozycji to 2, stąd ilość 6 =(2x(1+2)) Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  ...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: wdrozenie@empol.pl | Date: 24.06.2025 10:17
Type: Answer | 
RE: [AW-230519] Zlecenie 2043895 nieprawidłowa ilość na CIM (3)
Hej,
Spojrzałem na przykład i wydaje mi się że 6 to prawidłowa liczba
Baza CIM:
6 sztuk w tabeli CPB_TEILINFO

Poprzez CPB_TEIL możemy sprawdzić barcody oraz LFDNR z aufartik

barcody odnoszą się do poz1 ze wskazanego zlecenia: mamy odpowiednio 3 sztuki  

AUFARTIK widać tu również 3 sztuki 

Natomiast w zleceniu ilość na pozycji to 2, stąd ilość 6 =(2x(1+2))

Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbin…
```

</details>

---

### [AW-234427] — podział pól iQuote

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-234427]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 23.06.2025 15:16 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet
To: | Date: 23.06.2025 15:16
Type: State changed | 
RE: [AW-234427] podział pól iQuote (6)
```

</details>

---

### [AW-234140] — Błędy po wstawieniu / usunięciu przewiązki w top atrybutach

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-234140]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 23.06.2025 12:39 |

**Description:**

> RE: [AW-234140] Błędy po wstawieniu / usunięciu przewiązki w top atrybutach (2) Hej, Wrzuciłem na FTPa dzisiejsze dllki do testów - nie zauważyłem podobnego zachowania podczas korzystania z nich. Przetestuj na nich w miarę możliwości, jeśli będzie ok podrzucę podpisane cyfrowo Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäft...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: ksot@drutex.com.pl | Date: 23.06.2025 12:39
Type: Answer | 
RE: [AW-234140] Błędy po wstawieniu / usunięciu przewiązki w top atrybutach (2)
Hej,
Wrzuciłem na FTPa dzisiejsze dllki do testów - nie zauważyłem podobnego zachowania podczas korzystania z nich. Przetestuj na nich w miarę możliwości, jeśli będzie ok podrzucę podpisane cyfrowo 
Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Sc…
```

</details>

---

### [AW-234084] — IQuote- zmiany opisu przycisku

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-234084]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 23.06.2025 12:12 |

**Description:**

> RE: [AW-234084] IQuote- zmiany opisu przycisku (2) Hej, żeby przetłumaczyć lub zmienić nazwę - przejdź do lokalizacji: znajdziesz tam pliki dla wybranych języków w których możesz zmienić wyświetlany tekst w Iquote. Dla tego przycisku powinien być wpis WebPurchaseButtonOrder - zlecenie WebPurchaseButtonQuote - oferta Co ważne niektórych opisów nie jesteś w stanie zmienić, są tłumaczone z DLL'ki językowej! Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: G.Babicz@krispol.pl | Date: 23.06.2025 12:12
Type: Answer | 
RE: [AW-234084] IQuote- zmiany opisu przycisku (2)
Hej,
żeby przetłumaczyć lub zmienić nazwę - przejdź do lokalizacji:

znajdziesz tam pliki dla wybranych języków w których możesz zmienić wyświetlany tekst w Iquote.

Dla tego przycisku powinien być wpis 
WebPurchaseButtonOrder - zlecenie
WebPurchaseButtonQuote - oferta 
Co ważne niektórych opisów nie jesteś w stanie zmienić, są tłumaczone z DLL'ki językowej!
 
Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindun…
```

</details>

---

### [AW-234073] — Duplikacja wpisów do tłumaczeń

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-234073]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 23.06.2025 11:50 |

**Description:**

> RE: [AW-234073] Duplikacja wpisów do tłumaczeń (2) Hej, Możesz mi dostarczyć backup tej bazy? Po jakim procesie doszło do takiego efektu? Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan Amtsgericht Gießen/Gießen Local Court: ...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: mmedwid@drutex.com.pl | Date: 23.06.2025 11:50
Type: Answer | 
RE: [AW-234073] Duplikacja wpisów do tłumaczeń (2)
Hej,
Możesz mi dostarczyć backup tej bazy? Po jakim procesie doszło do takiego efektu?
Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus in Ihr System gelangen, haften wir nicht …
```

</details>

---

### [AW-234292] — Duplikaty podczas migracji na PrePROD

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-234292]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 23.06.2025 08:44 |

**Description:**

> RE: [AW-234292] Duplikaty podczas migracji na PrePROD (2) Hej, Super! Operacja zakończona sukcesem. W dalszej kolejności sprawdź czy materiały mają podpięte schematy cenowe (dane główne -> baza produktów -> dany materiał -> u dołu ekranu są podłączone schematy, chodzi zależności w ARTPRSCHEMA a ARTSTAMM - ARTIKELID). Jeśli jest ok można PRODa w podobny sposób skorygować PS te błędy również dostałem przy imporcie standardowej paczki master data, która w kolejności była zaraz po paczce korygującej...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: jkreft@drutex.com.pl | Date: 23.06.2025 08:44
Type: Answer | 
RE: [AW-234292] Duplikaty podczas migracji na PrePROD (2)
Hej,
Super! Operacja zakończona sukcesem. W dalszej kolejności sprawdź czy materiały mają podpięte schematy cenowe (dane główne -> baza produktów -> dany materiał -> u dołu ekranu są podłączone schematy, chodzi zależności w ARTPRSCHEMA a ARTSTAMM - ARTIKELID). Jeśli jest ok można PRODa w podobny sposób skorygować 
PS te błędy również dostałem przy imporcie standardowej paczki master data, która w kolejności była zaraz po paczce korygującej.
Dalsze już importy nie powodowały wystąpienia tych błędów
Można je zignorować, informują nas o tym że dane są już w bazie 
Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich …
```

</details>

---

### [AW-233808] — rysunek rolety

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-233808]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 20.06.2025 15:43 |

**Description:**

> [autoresponder] RE: [AW-233808] rysunek rolety (3) Dzień dobry, Do dnia 20 czerwca przebywam poza biurem. Na wszystkie wiadomości odpowiem zaraz po powrocie. Pozdrawiam Łukasz Urwanowicz

<details>
<summary>View Full Conversation Thread</summary>

```
From: Lukasz Urwanowicz (lukasz.urwanowicz@witraz.eu)
To: support.cantor.pl@a-w.com | Date: 20.06.2025 15:43
Type: Request | 
[autoresponder] RE: [AW-233808] rysunek rolety (3)
Dzień dobry,
Do dnia 20 czerwca przebywam poza biurem.
Na wszystkie wiadomości odpowiem zaraz po powrocie.

Pozdrawiam
Łukasz Urwanowicz
```

</details>

---

### [AW-233336] — Brak danych na wydruku

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-233336]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 20.06.2025 12:21 |

**Description:**

> Re: [AW-233336] Brak danych na wydruku (4) Hej, W tłumaczeniach jest ok, bywały przypadki że tam zamiast tekstu wpisanego we właściwości wydruku było pusto. Zweryfikuj raz jeszcze swój przykład, na moim środowisku działa bez problemów testowe zlecenie to zwykła jednostka F100 o wymiarach 1000x1000 Wydruk: Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Wrześni...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: mmedwid@drutex.com.pl | Date: 20.06.2025 12:21
Type: Answer | 
Re: [AW-233336] Brak danych na wydruku (4)
Hej,
W tłumaczeniach jest ok, bywały przypadki że tam zamiast tekstu wpisanego we właściwości wydruku było pusto.
Zweryfikuj raz jeszcze swój przykład, na moim środowisku działa bez problemów

testowe zlecenie to zwykła jednostka F100 o wymiarach 1000x1000

Wydruk:

Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe di…
```

</details>

---

### [AW-233617] — URGENT - błąd przy aktualizacji dealera

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-233617]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 20.06.2025 09:46 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet
To: | Date: 20.06.2025 09:46
Type: State changed | 
RE: [AW-233617] URGENT - błąd przy aktualizacji dealera (6)
```

</details>

---

### [AW-234142] — RE: Brak odwzorowania koloru skrzynki rolety po zmianie

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-234142]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 18.06.2025 15:45 |

**Description:**

> RE: [AW-234142] RE: Brak odwzorowania koloru skrzynki rolety po zmianie (2) Hej, Zgłoszenie czeka na analizę, w pierwotnym wątku odpiszemy gdy będą wnioski Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan Amtsgericht Gießen/Gi...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: d.precht@pagen.pl | Date: 18.06.2025 15:45
Type: Answer | 
RE: [AW-234142] RE: Brak odwzorowania koloru skrzynki rolety po zmianie (2)
Hej,
Zgłoszenie czeka na analizę, w pierwotnym wątku odpiszemy gdy będą wnioski 
Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus in Ihr System gelangen, haften wir nicht für di…
```

</details>

---

### [AW-234145] — RE: nowe kolory nie posiadają okleiny na widoku IFS_ORDER_ITEMS_BOM

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-234145]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 18.06.2025 15:44 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet
To: | Date: 18.06.2025 15:44
Type: State changed | 
RE: [AW-234145] RE: nowe kolory nie posiadają okleiny na widoku IFS_ORDER_ITEMS_BOM (2)
```

</details>

---

### [AW-233464] — Problem  zamówieniem na szyby

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-233464]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 18.06.2025 13:35 |

**Description:**

> RE: [AW-233464] Problem  zamówieniem na szyby (2) Hej, Tylko wymiary na rysunku nie są zgodne, te w xmlu są ok Tak to zamówienie wygląda u mnie na środowisku - wymiary na rysunku są poprawne Nie chce u Was na produkcji drukować tego zamówienia, macie może jakiś poligon? Być może to kwestia dllek albo konfiguracji Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: m.gwozdz@budvar.pl | Date: 18.06.2025 13:35
Type: Answer | 
RE: [AW-233464] Problem  zamówieniem na szyby (2)
Hej,
Tylko wymiary na rysunku nie są zgodne, te w xmlu są ok

Tak to zamówienie wygląda u mnie na środowisku - wymiary na rysunku są poprawne 

Nie chce u Was na produkcji drukować tego zamówienia, macie może jakiś poligon? Być może to kwestia dllek albo konfiguracji 
Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe di…
```

</details>

---

### [AW-233135] — Brak możliwości aktualizacji zlecenia

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-233135]` |
| **Status** | 🔵 In Progress |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 18.06.2025 13:34 |

**Description:**

> Re: [AW-233135] Brak możliwości aktualizacji zlecenia (5) Hej, a co jeśli w zeszłym tygodniu eksportowaliśmy 2 razy paczkę z PROD na klienta (PRODCONF się pewnie zinkrementował), a w weekend został nadpisany przez CaImport i ten PRODCONF się "cofnął"? Pozdrawiam Jacek Kreft Inżynier ds. oprogramowania <https://www.drutex.eu/> *PL:* + 48 59 822 91 01 | *Fax:* + 48 59 822 91 03 DRUTEX S.A. Lęborska 31 | Bytów 77-100 | Polska NIP 8‌42 1‌6 2‌2 7‌20 www.drutex.eu <https://www.drutex.eu/> <https://www...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Jacek Kreft (jkreft@drutex.com.pl)
To: support.cantor.pl@a-w.com | Date: 18.06.2025 13:34
Type: Request | 
Re: [AW-233135] Brak możliwości aktualizacji zlecenia (5)
Hej,

a co jeśli w zeszłym tygodniu eksportowaliśmy 2 razy paczkę z PROD na
klienta (PRODCONF się pewnie zinkrementował), a w weekend został
nadpisany przez CaImport i ten PRODCONF się "cofnął"?

Pozdrawiam

Jacek Kreft

Inżynier ds. oprogramowania

<https://www.drutex.eu/>

*PL:* + 48 59 822 91 01 | *Fax:* + 48 59 822 91 03

DRUTEX S.A.

Lęborska 31 | Bytów 77-100 | Polska
NIP 8‌42 1‌6 2‌2 7‌20
www.drutex.eu <https://www.drutex.eu/>

<https://www.facebook.com/DrutexSA/>
<http://www.instagram.com/drutex_com/>

<https://www.drutex.pl/pl/produkty/d-gate.html>

DRUTEX S.A. z siedzibą w Bytowie zarejestrowany został w Krajowym
Rejestrze Sądowym pod nr 0000140428 prowadzonym przez Sąd Rejonowy VIII
Wydział Gospodarczy Krajowego Rejestru Sądowego w Gdańsku. BDO
0‌00001469. Kapitał zakładowy, opłacony DRUTEX S.A. wynosi 21.690.000,00 zł

DRUTEX S.A. oświadcza, że posiada status dużego przedsiębiorcy w
rozumieniu Ustawy z dnia 8 marca 2013 r. o przeci…
```

</details>

---

### [AW-232735] — URGENT - błąd podczas aktywacji klienta

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-232735]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 18.06.2025 13:04 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet
To: | Date: 18.06.2025 13:04
Type: State changed | 
RE: [AW-232735] URGENT - błąd podczas aktywacji klienta (6)
```

</details>

---

### [AW-232763] — CANTOR 7.8 (DLL 2023.1.0.69) - Top pakiet dla klasy 1750

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-232763]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 18.06.2025 11:26 |

**Description:**

> RE: [AW-232763] CANTOR 7.8 (DLL 2023.1.0.69) - Top pakiet dla klasy 1750 (2) Hej, Pozycje globalne nie są dostępne w topatrybutach/toppakietach Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan Amtsgericht Gießen/Gießen Local C...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: P.Stojek@krispol.pl | Date: 18.06.2025 11:26
Type: Answer | 
RE: [AW-232763] CANTOR 7.8 (DLL 2023.1.0.69) - Top pakiet dla klasy 1750 (2)
Hej,
Pozycje globalne nie są dostępne w topatrybutach/toppakietach
Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus in Ihr System gelangen, haften wir nicht für die evtl. entsta…
```

</details>

---

### [AW-233031] — ARTIKELID in MWMAT not matching the ARTIKELID in ARTSTAMM for BEREICH = 9 after performing an import

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-233031]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 18.06.2025 11:13 |

**Description:**

> Re: FW: Re: [AW-233031] URGENT URGENT URGENT - błąd przy tablicach wyszukiwań (19) Hej, napierw musisz dla ARTSTAMM nadać numer np 26, a następnie po kolei możesz korygować od 9 do 25 Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: jkreft@drutex.com.pl | Date: 18.06.2025 11:13
Type: Answer | 
Re: FW: Re: [AW-233031] URGENT URGENT URGENT - błąd przy tablicach wyszukiwań (19)
Hej, napierw musisz dla ARTSTAMM nadać numer np 26, a następnie po kolei możesz korygować od 9 do 25 
Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus in Ihr System gelangen, haf…
```

</details>

---

### [AW-233841] — Re: URGENT - CANTOR DEALER - po wydruku raportu 700 zlecenie dostaje statu F

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-233841]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 17.06.2025 13:14 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet
To: | Date: 17.06.2025 13:14
Type: State changed | 
RE: [AW-233841] Re: URGENT - CANTOR DEALER - po wydruku raportu 700 zlecenie dostaje statu F (2)
Odpowiedź została udzielona w wątku głównym: [AW-233755]
```

</details>

---

### [AW-233261] — Błąd Cantor - Nieprawidłowy wpis w specyfikacji materiałowej

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-233261]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 17.06.2025 13:03 |

**Description:**

> Re: Fwd: [AW-233261] Błąd Cantor - Nieprawidłowy wpis w specyfikacji materiałowej (12) Hej, No to chyba namierzone - system producenta NIE_DLA_DEALERA jak nazwa wskazuje nie transferujecie go na dealera Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mar...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: iiwanca@drutex.com.pl | Date: 17.06.2025 13:03
Type: Answer | 
Re: Fwd: [AW-233261] Błąd Cantor - Nieprawidłowy wpis w specyfikacji materiałowej (12)
Hej,
No to chyba namierzone - system producenta NIE_DLA_DEALERA jak nazwa wskazuje nie transferujecie go na dealera 

Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus in Ihr Sy…
```

</details>

---

### [AW-233331] — JAk monitorowac dzialanie Iquote

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-233331]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 17.06.2025 13:01 |

**Description:**

> RE: [AW-233331] JAk monitorowac dzialanie Iquote (4) Cześć, Nie da się Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan Amtsgericht Gießen/Gießen Local Court: HRB 7963 Diese E-Mail ist ausschließlich für den Adressaten bestimm...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: G.Babicz@krispol.pl | Date: 17.06.2025 13:01
Type: Answer | 
RE: [AW-233331] JAk monitorowac dzialanie Iquote (4)
Cześć,
Nie da się 
Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus in Ihr System gelangen, haften wir nicht für die evtl. entstandenen Schäden.

This e-mail is for the intend…
```

</details>

---

### [AW-233323] — S200 - na rysunku brak skosu

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-233323]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 16.06.2025 13:42 |

**Description:**

> RE: [AW-233323] S200 - na rysunku brak skosu (2) Hej, Jak to ścięcie ma zostać wykonane, skoro w wartości B1 wpisujesz pełny rozmiar okna? Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan Amtsgericht Gießen/Gießen Local Court:...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: zgloszeniacantor@wiked.pl, robert.krampikowski@wiked.pl | Date: 16.06.2025 13:42
Type: Answer | 
RE: [AW-233323] S200 - na rysunku brak skosu (2)
Hej,
Jak to ścięcie ma zostać wykonane, skoro w wartości B1 wpisujesz pełny rozmiar okna?

Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus in Ihr System gelangen, haften wir n…
```

</details>

---

### [AW-233782] — RE: MM KRAGUJEVAC

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-233782]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 16.06.2025 13:16 |

**Description:**

> RE: [AW-233782] RE: MM KRAGUJEVAC (2) The email support.cantor.pl@a-w.com refers to Cantor's Polish support department. We are not the correct addressee of the message, so we cannot help you with the topic. Please direct only problems with the A+W Cantor application to us Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführ...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: Susanna@mab-export.si | Date: 16.06.2025 13:16
Type: Answer | 
RE: [AW-233782] RE: MM KRAGUJEVAC (2)
The email support.cantor.pl@a-w.com refers to Cantor's Polish support department. We are not the correct addressee of the message, so we cannot help you with the topic. 
Please direct only problems with the A+W Cantor application to us
Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selb…
```

</details>

---

### [AW-233755] — CANTOR DEALER - po wydruku raportu 700 zlecenie dostaje statu F

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-233755]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 16.06.2025 10:49 |

**Description:**

> RE: [AW-233755] CANTOR DEALER - po wydruku raportu 700 zlecenie dostaje statu F (3) Hej, Tego zgłoszenia nie będziemy przetwarzali w trybie urgent. Nie jest to błąd, raport 700 działa w ten sposób od zawsze, rozumiem że może Was to blokować/wprowadzać w błąd ze względu na status który zlecenie osiąga po wydrukowaniu tego raportu. Niestety ale z tego co zweryfikowałem nie mamy opcji aby sterować tym zachowaniem poprzez dostępne konfiguracje programu. Zaproponować mogę rozszerzenie programu (poprz...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: mtelega@drutex.com.pl | Date: 16.06.2025 10:49
Type: Answer | 
RE: [AW-233755] CANTOR DEALER - po wydruku raportu 700 zlecenie dostaje statu F (3)
Hej,
Tego zgłoszenia nie będziemy przetwarzali w trybie urgent.
Nie jest to błąd, raport 700 działa w ten sposób od zawsze, rozumiem że może Was to blokować/wprowadzać w błąd ze względu na status który zlecenie osiąga po wydrukowaniu tego raportu.
Niestety ale z tego co zweryfikowałem nie mamy opcji aby sterować tym zachowaniem poprzez dostępne konfiguracje programu.
Zaproponować mogę rozszerzenie programu (poprzez devRequest - dodatkowo płatne), które np doda nam ustawienie aby status nie zmieniał się na F po wydrukowaniu pliku zamówienie dealera, jest to tylko koncept, po spisaniu dokumentu, dział R&D przeanalizuje jest wykonalność oraz sens wdrożenia.
Z drugiej strony poprzez prodconf 372 =0 możemy wyłączyć dealerowi dostęp do tego wydruku, być może jest to dla Was rozwiązanie?

Czekam na info jaką decyzje podejmujecie w temacie 
Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Softw…
```

</details>

---

### [AW-225995] — For grilles - duplex white/white color information is not inserted into the database

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-225995]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 13.06.2025 15:07 |

**Description:**

> Re: Fwd: FW: RE: [AW-225995] Re: brak kolorów białych dla szprosów naklejanych (17) Hej, FARBCODEINNENBEZ oraz FARBCODEAUSSENBEZ odnoszą się do kodów kolorów Np w szprosach międzyszybowych 26mm/8mm Używacie tu kolorów systemowych, nie kodów kolorów więc te pola muszą być nullami Ale nie znaczy to że informacji której potrzebujecie nie ma w bazie - jest tylko w polu FARBEINNENBEZ, FARBEAUSSENBEZ Natomiast np Szpros naklejany 27mm obustronnie + 1 x duplex korzysta z kodów kolorów Więc dla niego or...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: iiwanca@drutex.com.pl | Date: 13.06.2025 15:07
Type: Answer | 
Re: Fwd: FW: RE: [AW-225995] Re: brak kolorów białych dla szprosów naklejanych (17)
Hej,
FARBCODEINNENBEZ oraz FARBCODEAUSSENBEZ odnoszą się do kodów kolorów
Np w szprosach międzyszybowych 26mm/8mm
Używacie tu kolorów systemowych, nie kodów kolorów więc te pola muszą być nullami 

Ale nie znaczy to że informacji której potrzebujecie nie ma w bazie - jest tylko w polu FARBEINNENBEZ, FARBEAUSSENBEZ

Natomiast np Szpros naklejany 27mm obustronnie + 1 x duplex korzysta z kodów kolorów

Więc dla niego oraz jego kolorów pola FARBCODEINNENBEZ oraz FARBCODEAUSSENBEZ są wypełnione 

Nie ma tu błędu w programie, wszystkie potrzebne informacje znajdują się w bazie print po ustawieniu opcji NIE
Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Co…
```

</details>

---

### [AW-233183] — PROD - brak przypisanych schematów w przeglądzie artykułów

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-233183]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 13.06.2025 13:03 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet
To: | Date: 13.06.2025 13:03
Type: State changed | 
RE: [AW-233183] PROD - brak przypisanych schematów w przeglądzie artykułów (8)
```

</details>

---

### [AW-224366] — Fwd: Znikające atrybuty

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-224366]` |
| **Status** | 🔵 In Progress |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 13.06.2025 13:02 |

**Description:**

> Re: [AW-224366] Fwd: Znikające atrybuty (8) Uprawnienia są nadawane od Folderu C:\ProgramData\Drutex W dniu 13.06.2025 o 12:52, Jacek Kreft pisze: > > Hej Paweł, > > już chyba to sprawdzaliśmy i nie działało, ale zobacz jeszcze raz i > odpowiedz w tym ticket na support. > > > Pozdrawiam > > Jacek Kreft > > Inżynier ds. oprogramowania > > <https://www.drutex.eu/> > > *PL:* + 48 59 822 91 01 | *Fax:* + 48 59 822 91 03 > > DRUTEX S.A. > > Lęborska 31 | Bytów 77-100 | Polska > NIP 8‌42 1‌6 2‌2 7‌20 ...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Paweł Suszko (psuszko@drutex.com.pl)
To: jkreft@drutex.com.pl | Date: 13.06.2025 13:02
Type: Request | 
Re: [AW-224366] Fwd: Znikające atrybuty (8)
Uprawnienia są nadawane od Folderu C:\ProgramData\Drutex

W dniu 13.06.2025 o 12:52, Jacek Kreft pisze:
>
> Hej Paweł,
>
> już chyba to sprawdzaliśmy i nie działało, ale zobacz jeszcze raz i
> odpowiedz w tym ticket na support.
>
>
> Pozdrawiam
>
> Jacek Kreft
>
> Inżynier ds. oprogramowania
>
> <https://www.drutex.eu/>
>
> *PL:* + 48 59 822 91 01 | *Fax:* + 48 59 822 91 03
>
> DRUTEX S.A.
>
> Lęborska 31 | Bytów 77-100 | Polska
> NIP 8‌42 1‌6 2‌2 7‌20
> www.drutex.eu <https://www.drutex.eu/>
>
> <https://www.facebook.com/DrutexSA/>
> <http://www.instagram.com/drutex_com/>
>
>
> <https://www.drutex.pl/pl/produkty/d-gate.html>
>
> DRUTEX S.A. z siedzibą w Bytowie zarejestrowany został w Krajowym
> Rejestrze Sądowym pod nr 0000140428 prowadzonym przez Sąd Rejonowy
> VIII Wydział Gospodarczy Krajowego Rejestru Sądowego w Gdańsku. BDO
> 0‌00001469. Kapitał zakładowy, opłacony DRUTEX S.A. wynosi
> 21.690.000,00 zł
>
> DRUTEX S.A. oświadcza, że …
```

</details>

---

### [AW-229504] — towary -łączniki

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-229504]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 10.06.2025 13:38 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Michal Hawro
To: | Date: 10.06.2025 13:38
Type: State changed | 
RE: [AW-229504] towary -łączniki (5)
Cześć, 
możecie to proszę zweryfikować, sprawdzaliśmy to z Dawidem i to jest jak dla nas Bug do zgłoszenia do R&D. Chyba że Wam uda się odnaleźć co jest błędnie ustawione.
W razie pytań śmiało
```

</details>

---

### [AW-232629] — aktualizacja zlecenia po migracji danych

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-232629]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 10.06.2025 12:11 |

**Description:**

> RE: [AW-232629] aktualizacja zlecenia po migracji danych (2) Hej, Jeśli jest takie zapotrzebowanie możemy przygotować devRequest, bo obecnie nie ma takiej funkcjonalności. Proszę o informację Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson,...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: mtelega@drutex.com.pl | Date: 10.06.2025 12:11
Type: Answer | 
RE: [AW-232629] aktualizacja zlecenia po migracji danych (2)
Hej,
Jeśli jest takie zapotrzebowanie możemy przygotować devRequest, bo obecnie nie ma takiej funkcjonalności. Proszę o informację 
Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Vi…
```

</details>

---

### [AW-232506] — Brak wartości na wydruku

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-232506]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 10.06.2025 11:43 |

**Description:**

> RE: [AW-232506] Brak wartości na wydruku (2) Hej, Warunki jakie muszą zostać spełnione aby korzystać ze zmiennej LOOKUP: Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan Amtsgericht Gießen/Gießen Local Court: HRB 7963 Diese E-...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: iiwanca@drutex.com.pl | Date: 10.06.2025 11:43
Type: Answer | 
RE: [AW-232506] Brak wartości na wydruku (2)
Hej,
Warunki jakie muszą zostać spełnione aby korzystać ze zmiennej LOOKUP:

Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus in Ihr System gelangen, haften wir nicht für die e…
```

</details>

---

### [AW-232476] — Delete edit-status button is not active

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-232476]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 09.06.2025 17:16 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Lukasz Lieske
To: | Date: 09.06.2025 17:16
Type: State changed | 
RE: [AW-232476] Delete edit-status button is not active (11)
Status update
```

</details>

---

### [AW-232276] — URGENT - po błędnym obliczaniu ceny można wysłać zamówienie przez DES

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-232276]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 09.06.2025 12:08 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet
To: | Date: 09.06.2025 12:08
Type: State changed | 
RE: [AW-232276] URGENT - po błędnym obliczaniu ceny można wysłać zamówienie przez DES (8)
Update from customer:
Zostawmy na chwilę ten temat. Przegadamy to wewnętrznie
```

</details>

---

### [AW-229482] — Missing Italian translations

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-229482]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 06.06.2025 15:15 |

**Description:**

> Re: [AW-229482] Cantor - niemieckie wpisy (9) Hej, Tłumaczenie jest już dostępne - dllki które w tygodniu wgraliście zawierają poprawkę Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan Amtsgericht Gießen/Gießen Local Court: HR...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: mmedwid@drutex.com.pl | Date: 06.06.2025 15:15
Type: Answer | 
Re: [AW-229482] Cantor - niemieckie wpisy (9)
Hej,
Tłumaczenie jest już dostępne - dllki które w tygodniu wgraliście zawierają poprawkę 
Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus in Ihr System gelangen, haften wir ni…
```

</details>

---

### [AW-232955] — iQuote OPASKA/PORTAL

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-232955]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 06.06.2025 14:42 |

**Description:**

> RE: [AW-232955] iQuote OPASKA/PORTAL (2) Hej, W tym miejscu deklarujemy które właściwości mają się tam wyświetlać Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan Amtsgericht Gießen/Gießen Local Court: HRB 7963 Diese E-Mail is...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: przemyslaw.barthelke@wiked.pl | Date: 06.06.2025 14:42
Type: Answer | 
RE: [AW-232955] iQuote OPASKA/PORTAL (2)
Hej,
W tym miejscu deklarujemy które właściwości mają się tam wyświetlać 

Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus in Ihr System gelangen, haften wir nicht für die evt…
```

</details>

---

### [AW-224636] — URGENT - Błędne ramki w zleceniach

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-224636]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 05.06.2025 14:41 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet
To: | Date: 05.06.2025 14:41
Type: State changed | 
RE: [AW-224636] URGENT - Błędne ramki w zleceniach (10)
Waiting for reproduction steps
```

</details>

---

### [AW-225928] — Dealer - brak białego koloru osłonek okuć

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-225928]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 05.06.2025 14:22 |

**Description:**

> Re: [AW-225928] Dealer - brak białego koloru osłonek okuć (19) Hej, Doraźnym rozwiązaniej jest dopisać typ produktu 10127 do koloru białego (na erp a następnie eksport do dealera) Tak jak wcześniej pisałem wygląda tak jakby typy produktów były skopane, bądź cokolwiek innego - za bardzo już tu wchodzimy w szczegóły. Temat mogę przesłać ewentualnie na konsulting aby sprawdzić to głębiej jeśli jest taka potrzeba Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +49641...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: jkreft@drutex.com.pl | Date: 05.06.2025 14:22
Type: Answer | 
Re: [AW-225928] Dealer - brak białego koloru osłonek okuć (19)
Hej,
Doraźnym rozwiązaniej jest dopisać typ produktu 10127 do koloru białego (na erp a następnie eksport do dealera)

Tak jak wcześniej pisałem wygląda tak jakby typy produktów były skopane, bądź cokolwiek innego - za bardzo już tu wchodzimy w szczegóły.
Temat mogę przesłać ewentualnie na konsulting aby sprawdzić to głębiej jeśli jest taka potrzeba
Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und d…
```

</details>

---

### [AW-232271] — Projekt iQuote 2.0 - widok "Dane główne" -> "Klienci

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-232271]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 05.06.2025 12:47 |

**Description:**

> RE: [AW-232271] Projekt iQuote 2.0 - widok "Dane główne" -> "Klienci (4) I tak i nie: z cantora nie możemy tym sterować bo nie jest to żadnym widgetem, tylko domyślnie dostarczonym przez nas menu, ale za pomocą stylu CSS można: każdy element to osobne id (niektóre mogą być wymagane więc zweryfikujcie przed ich ukryciem) Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: P.Stojek@krispol.pl | Date: 05.06.2025 12:47
Type: Answer | 
RE: [AW-232271] Projekt iQuote 2.0 - widok "Dane główne" -> "Klienci (4)
I tak i nie: z cantora nie możemy tym sterować bo nie jest to żadnym widgetem, tylko domyślnie dostarczonym przez nas menu, ale za pomocą stylu CSS można: każdy element to osobne id (niektóre mogą być wymagane więc zweryfikujcie przed ich ukryciem)

Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht g…
```

</details>

---

### [AW-232753] — URGENT URGENT URGENT program cantor dealer nie procesuje paczki aktualizacyjnej

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-232753]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 05.06.2025 11:30 |

**Description:**

> Re: [AW-232753] URGENT URGENT URGENT program cantor dealer nie procesuje paczki aktualizacyjnej (8) ok, to zgłoszenie które wskazałeś mamy oznaczone jako succesfully closed, jeśli jest inaczej w rzeczywistości prześlę je ponownie do R&D [AW-174261] Dodatkowo znalazłem taką inforację: master data wykonuje się jako pierwsze jeśli ma status 3 [Core_BuPa_DataPackageReceivers](wcześniej się nie wykonało i musi się ponownie pobrać) Nie wiem na ile chcecie się bawić w wycofywanie paczek w DES ale po Re...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: mjanik@drutex.com.pl | Date: 05.06.2025 11:30
Type: Answer | 
Re: [AW-232753] URGENT URGENT URGENT program cantor dealer nie procesuje paczki aktualizacyjnej (8)
ok, to zgłoszenie które wskazałeś mamy oznaczone jako succesfully closed, jeśli jest inaczej w rzeczywistości prześlę je ponownie do R&D [AW-174261]
Dodatkowo znalazłem taką inforację: master data wykonuje się jako pierwsze jeśli ma status 3 [Core_BuPa_DataPackageReceivers](wcześniej się nie wykonało i musi się ponownie pobrać) 
Nie wiem na ile chcecie się bawić w wycofywanie paczek w DES 
ale po ReceiverPartnerGuid idzie połapać tych którzy wykonali wadliwą wersję 

Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen en…
```

</details>

---

### [AW-225939] — CANTOR 7.8 (2023.1.0.62) - domyślne wartości parametrów w narzędziach SQL

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-225939]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 04.06.2025 16:04 |

**Description:**

> RE: [AW-225939] CANTOR 7.8 (2023.1.0.62) - domyślne wartości parametrów w narzędziach SQL (7) Nic mi nie wiadomo żebyśmy zmieniali, dzwoń na ten z mojej stopki 61 438 47 44 Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan Amts...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: P.Stojek@krispol.pl | Date: 04.06.2025 16:04
Type: Answer | 
RE: [AW-225939] CANTOR 7.8 (2023.1.0.62) - domyślne wartości parametrów w narzędziach SQL (7)
Nic mi nie wiadomo żebyśmy zmieniali, dzwoń na ten z mojej stopki
61 438 47 44
Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus in Ihr System gelangen, haften wir nicht für die …
```

</details>

---

### [AW-232634] — API

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-232634]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 04.06.2025 14:34 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet
To: | Date: 04.06.2025 14:34
Type: State changed | 
RE: [AW-232634] API (5)
```

</details>

---

### [AW-231812] — [Fwd: ##RE-69332## : Discounts from quotation are not transferred]

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-231812]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 04.06.2025 11:57 |

**Description:**

> RE: [AW-231812] [Fwd: ##RE-69332## : Discounts from quotation are not transferred] (2) Cześć, wydruki mogły zostać puszczeone w większym odstępie czasowym, to co widzimy to czas kiedy zostały wykonane na spoolerze (mogła być kolejka i czekały na swoją kolej), fakt że są tam prawie identyczne czasy nie jest niczym nadzwyczajnym, jest masa zamówień które drukują się w identycznym czasie Co do rabatów jeśli ktoś ma możliwość zmiany to nie jesteśmy w stanie upilnować co robi, może należy przejrzeć u...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: helpdesk@krispol.pl | Date: 04.06.2025 11:57
Type: Answer | 
RE: [AW-231812] [Fwd: ##RE-69332## : Discounts from quotation are not transferred] (2)
Cześć,
wydruki mogły zostać puszczeone w większym odstępie czasowym, to co widzimy to czas kiedy zostały wykonane na spoolerze (mogła być kolejka i czekały na swoją kolej), fakt że są tam prawie identyczne czasy nie jest niczym nadzwyczajnym, jest masa zamówień które drukują się w identycznym czasie 

Co do rabatów jeśli ktoś ma możliwość zmiany to nie jesteśmy w stanie upilnować co robi, może należy przejrzeć uprawnienia użytkowników
Systemowo jest UpdateOrderAfterCopy

Wartość 167 składa się z następujących bitów, które sumują się do tej liczby: 128 + 32 + 4 + 2 + 1. Każdy z tych bitów odpowiada konkretnemu znaczeniu:
 • 128: Should orders with incomplete status be saved

 • 32: The profile deductions are loaded anew from the master data

 • 4: Restrictions will be checked

 • 2: The exchange conditions of the associated profile record will be evaluated

 • 1: The accessories will be updated

Czyli macie wyłączone wszystkie opcje odświeżania cen, zatem jedynie …
```

</details>

---

### [AW-231851] — Jak zrobić żeby zdolności produkcyjne były zajmowane dopiero po uruchomieniu na produkcję

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-231851]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 04.06.2025 10:35 |

**Description:**

> RE: [AW-231851] Jak zrobić żeby zdolności produkcyjne były zajmowane dopiero po uruchomieniu na produkcję (2) Cześć, Takie jest założenie zdolności żeby wiedzieć przed produkcją czy będziemy mieli możliwości aby dane zamówienie wykonać, nie da się tego przestawić. Może warto przestawić tryby na zdolnościach aby takie duże zlecenia rozbijało np na 3 dni produkcyjne Dokument w załączniku: Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support....

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: m.gwozdz@budvar.pl | Date: 04.06.2025 10:35
Type: Answer | 
RE: [AW-231851] Jak zrobić żeby zdolności produkcyjne były zajmowane dopiero po uruchomieniu na produkcję (2)
Cześć,
Takie jest założenie zdolności żeby wiedzieć przed produkcją czy będziemy mieli możliwości aby dane zamówienie wykonać, nie da się tego przestawić.
Może warto przestawić tryby na zdolnościach aby takie duże zlecenia rozbijało np na 3 dni produkcyjne
Dokument w załączniku:
Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weit…
```

</details>

---

### [AW-231403] — Nie przechodzą zamówienia od klienta do Cantora

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-231403]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 04.06.2025 09:47 |

**Description:**

> Re: [AW-231403] Nie przechodzą zamówienia od klienta do Cantora (9) Zatem zlecenie przeszło i jest dostępne pod tym numerem: Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan Amtsgericht Gießen/Gießen Local Court: HRB 7963 Dies...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: jkreft@drutex.com.pl | Date: 04.06.2025 09:47
Type: Answer | 
Re: [AW-231403] Nie przechodzą zamówienia od klienta do Cantora (9)
Zatem zlecenie przeszło i jest dostępne pod tym numerem:

Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus in Ihr System gelangen, haften wir nicht für die evtl. entstandenen Sc…
```

</details>

---

### [AW-230542] — Akceptacja konfliktów

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-230542]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 03.06.2025 13:43 |

**Description:**

> Re: [AW-230542] Akceptacja konfliktów (7) Dobrze że się o to upomniałeś, jednak problem faktycznie wciąż istnieje. Możesz mnie na przyszłość dodawać w DW to będę widział (pmuszkiet@a-w.com), a sam problem ze znikającymi mailami jeszcze raz postaramy się przeprocesować Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/M...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: wdrozenie@empol.pl | Date: 03.06.2025 13:43
Type: Answer | 
Re: [AW-230542] Akceptacja konfliktów (7)
Dobrze że się o to upomniałeś, jednak problem faktycznie wciąż istnieje. Możesz mnie na przyszłość dodawać w DW to będę widział (pmuszkiet@a-w.com), a sam problem ze znikającymi mailami jeszcze raz postaramy się przeprocesować 
Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverstän…
```

</details>

---

### [AW-231653] — Uprawnienie

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-231653]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 02.06.2025 19:20 |

**Description:**

> RE: [AW-231653] Uprawnienie (3) Cześć, Kombinacja uprawnień 2056,2074 oraz 222 upoważnia do edycji statusu oraz zapisu zmian w osprzęcie. Daj mi znać jak działa to u ciebie. Serdecznie pozdrawiam Lukasz Lieske ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan Amtsg...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Lukasz Lieske (support.cantor.pl@a-w.com)
To: G.Babicz@krispol.pl | Date: 02.06.2025 19:20
Type: Answer | 
RE: [AW-231653] Uprawnienie (3)
Cześć,
 
Kombinacja uprawnień 2056,2074 oraz 222 upoważnia do edycji statusu oraz zapisu zmian w osprzęcie.
Daj mi znać jak działa to u ciebie.
 
Serdecznie pozdrawiam
Lukasz Lieske
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail …
```

</details>

---

### [AW-230843] — CANTOR 7.8 - iQuote oznaczenie zlecenia po akceptacji ograniczenia STOP

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-230843]` |
| **Status** | 🔵 In Progress |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 02.06.2025 12:53 |

**Description:**

> RE: [AW-230843] CANTOR 7.8 - iQuote oznaczenie zlecenia po akceptacji ograniczenia STOP (8) @Support Cantor Poland<mailto:support.cantor.pl@a-w.com> Czy udało się ustalić coś w kwestii tej konfiguracji ? Pozdrawiam / Best regards _________________________________________ Grzegorz Babicz Specjalista ds. Systemów ERP M  +48 515 036 816 E   g.babicz@krispol.pl<mailto:g.babicz@krispol.pl> From: Support Cantor Poland <support.cantor.pl@a-w.com> Sent: Tuesday, May 27, 2025 4:00 PM To: Paweł Stojek <P....

<details>
<summary>View Full Conversation Thread</summary>

```
From: Grzegorz Babicz (G.Babicz@krispol.pl)
To: support.cantor.pl@a-w.com, P.Stojek@krispol.pl | Date: 02.06.2025 12:53
Type: Request | 
RE: [AW-230843] CANTOR 7.8 - iQuote oznaczenie zlecenia po akceptacji ograniczenia STOP (8)
@Support Cantor Poland<mailto:support.cantor.pl@a-w.com> Czy udało się ustalić coś w kwestii tej konfiguracji ?

Pozdrawiam / Best regards
_________________________________________

Grzegorz Babicz
Specjalista ds. Systemów ERP

M  +48 515 036 816
E   g.babicz@krispol.pl<mailto:g.babicz@krispol.pl>

From: Support Cantor Poland <support.cantor.pl@a-w.com>
Sent: Tuesday, May 27, 2025 4:00 PM
To: Paweł Stojek <P.Stojek@krispol.pl>
Cc: Arek Raczak <a.raczak@krispol.de>; Grzegorz Babicz <G.Babicz@krispol.pl>; Piotr Matluch <P.Matluch@krispol.pl>
Subject: RE: [AW-230843] CANTOR 7.8 - iQuote oznaczenie zlecenia po akceptacji ograniczenia STOP

To akurat nie jest błąd, tak jak komunikat mówi

Zmiany z MT nie odświeżają się w iQuote, takie zlecenie nie powinno być możliwe już do wczytania (mogę poszukać konfiguracji która odblokowuje możliwość wczytania i pewnie z niej korzystacie)

Serdecznie pozdrawiam

Patryk Muszkiet
###EOM##
…
```

</details>

---

### [AW-230645] — Problem pozostającej właściwości po zmianie typu produktu

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-230645]` |
| **Status** | 🔵 In Progress |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 30.05.2025 14:44 |

**Description:**

> ODP: [AW-230645] Problem pozostającej właściwości po zmianie typu produktu (3) Ale w IQUOTE, klient pracuje tylko na top-atrybut. Więc coś jest nie tak Szymon Kaczykowski Kierownik działu IT szymon.kaczykowski<mailto:szymon.kaczykowski@wiked.pl>@wiked.pl<mailto:szymon.kaczykowski@wiked.pl>  |  tel. 602 497 702                     |  tel. (58) 738-66-80 wewn.   199 WIKĘD Sp. z o.o. ul. Wielki Las 19, 84-242 Luzino www.wiked.pl  |  tel. (58) 678 01 77  |  tel. 601-194-538  |  fax. (58) 738 66 61 _...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Szymon Kaczykowski (szymon.kaczykowski@wiked.pl)
To: support.cantor.pl@a-w.com | Date: 30.05.2025 14:44
Type: Request | 
ODP: [AW-230645] Problem pozostającej właściwości po zmianie typu produktu (3)
Ale w IQUOTE, klient pracuje tylko na top-atrybut.
Więc coś jest nie tak

Szymon Kaczykowski
Kierownik działu IT

szymon.kaczykowski<mailto:szymon.kaczykowski@wiked.pl>@wiked.pl<mailto:szymon.kaczykowski@wiked.pl>  |  tel. 602 497 702                     |  tel. (58) 738-66-80 wewn.   199

WIKĘD Sp. z o.o.
ul. Wielki Las 19, 84-242 Luzino
www.wiked.pl  |  tel. (58) 678 01 77  |  tel. 601-194-538  |  fax. (58) 738 66 61

________________________________
Od: Support Cantor Poland <support.cantor.pl@a-w.com>
Wysłane: piątek, 30 maja 2025 14:21
Do: Szymon Kaczykowski <szymon.kaczykowski@wiked.pl>
Temat: RE: [AW-230645] Problem pozostającej właściwości po zmianie typu produktu

Parametr CHANGE, działa tylko gdy ręcznie i bezpośrednio zmieniamy daną włąściwość, w tym wypadku nie zmieniamy jej bezpośrednio, tylko przez top-atrybut, dlatego to nie działa

Serdecznie pozdrawiam

Patryk Muszkiet
###EOM##

 …
```

</details>

---

### [AW-231127] — TR: Cutting angle inversion

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-231127]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 29.05.2025 14:42 |

**Description:**

> RE: [AW-231127] TR: Cutting angle inversion (4) Hi Zahir, According to the specifications of the schirmer machine, these results are correct PROFTAB of mentioned order: You can manually overwrite the results of AngleOnCut/AngleOffCut using properties 624, 625 as we mentioned in [AW-132563] Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: zahir.azi@oxxo.dz | Date: 29.05.2025 14:42
Type: Answer | 
RE: [AW-231127] TR: Cutting angle inversion (4)
Hi Zahir,
According to the specifications of the schirmer machine, these results are correct
PROFTAB of mentioned order:

You can manually overwrite the results of AngleOnCut/AngleOffCut using properties 624, 625 as we mentioned in [AW-132563]
Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gest…
```

</details>

---

### [AW-230649] — Issue whith status set in remake orders

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-230649]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 29.05.2025 11:51 |

**Description:**

> RE: [AW-230649] Issue whith status set in remake orders (2) Hi Zahir, Perform this action again with trace enabled on the options highlighted below, send the result to me. Thank you in advance Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: zahir.azi@oxxo.dz | Date: 29.05.2025 11:51
Type: Answer | 
RE: [AW-230649] Issue whith status set in remake orders (2)
Hi Zahir,
Perform this action again with trace enabled on the options highlighted below, send the result to me. Thank you in advance

Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein…
```

</details>

---

### [AW-231413] — Błąd przy imporcie zamówienia od klienta

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-231413]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 28.05.2025 13:09 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet
To: | Date: 28.05.2025 13:09
Type: State changed | 
RE: [AW-231413] Błąd przy imporcie zamówienia od klienta (6)
```

</details>

---

### [AW-228563] — HVBoben - incorrect value

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-228563]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 27.05.2025 16:04 |

**Description:**

> RE: RE: [AW-228563] Błędna wartość zmiennej na centrum obróbczym. (13) Cześć, Zmianę konfiguracji o której pisałem mamy już przetestowaną u innego klienta. Błąd w tej konfiguracji byl od samego początku, czyli również w 2014 Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schm...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: g.sieradzki@krishome.eu | Date: 27.05.2025 16:04
Type: Answer | 
RE: RE: [AW-228563] Błędna wartość zmiennej na centrum obróbczym. (13)
Cześć,
Zmianę konfiguracji o której pisałem mamy już przetestowaną u innego klienta. Błąd w tej konfiguracji byl od samego początku, czyli również w 2014 
Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser…
```

</details>

---

### [AW-230932] — brak wartości koloru dla PP

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-230932]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 27.05.2025 12:40 |

**Description:**

> RE: [AW-230932] brak wartości koloru dla PP (2) Cześć, A jaka jest wartość tej właściwości w aufartik dla zlecenia z przykładu 525088146? Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan Amtsgericht Gießen/Gießen Local Court: ...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: mtelega@drutex.com.pl | Date: 27.05.2025 12:40
Type: Answer | 
RE: [AW-230932] brak wartości koloru dla PP (2)
Cześć,
A jaka jest wartość tej właściwości w aufartik dla zlecenia z przykładu 525088146? 
Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus in Ihr System gelangen, haften wir ni…
```

</details>

---

### [AW-230910] — Pogrubienie na ofercie opisu z klasy 2801

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-230910]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 27.05.2025 12:38 |

**Description:**

> Re: [AW-230910] Pogrubienie na ofercie opisu z klasy 2801 (4) Nie ma innych miejsc aby z poziomu cantora tym zarządzać. Może z poziomu crystala da radę ale tu już nie jestem ekspertem Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: jkreft@drutex.com.pl | Date: 27.05.2025 12:38
Type: Answer | 
Re: [AW-230910] Pogrubienie na ofercie opisu z klasy 2801 (4)
Nie ma innych miejsc aby z poziomu cantora tym zarządzać. Może z poziomu crystala da radę ale tu już nie jestem ekspertem 
Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus in Ihr…
```

</details>

---

### [AW-230802] — [Fwd: ##RE-69224## : PSS/238712940 PL/HDF/3 POLA ip]

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-230802]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 27.05.2025 10:58 |

**Description:**

> RE: [AW-230802] [Fwd: ##RE-69224## : PSS/238712940 PL/HDF/3 POLA ip] (2) Cześć, Ofert wprowadzonych w iQuote nie można zmieniać z poziomu MT. Mówi o tym komunikat przy wejściu do zlecenia: Skoro zostało to już zrobione należy dalej procesować ofertę w MT: drukować, zamówić itp. W iQuote zmiany wprowadzone z MT nie będą widoczne Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikors...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: helpdesk@krispol.pl | Date: 27.05.2025 10:58
Type: Answer | 
RE: [AW-230802] [Fwd: ##RE-69224## : PSS/238712940 PL/HDF/3 POLA ip] (2)
Cześć,
Ofert wprowadzonych w iQuote nie można zmieniać z poziomu MT. Mówi o tym komunikat przy wejściu do zlecenia:

Skoro zostało to już zrobione należy dalej procesować ofertę w MT: drukować, zamówić itp. W iQuote zmiany wprowadzone z MT nie będą widoczne 
Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail …
```

</details>

---

### [AW-230917] — Ustawienie prodconf

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-230917]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 27.05.2025 09:05 |

**Description:**

> Re: [AW-230917] Ustawienie prodconf (8) wpisz dokładnie takie wartości jak na zrzucie - powinno zadziałać :) Serdecznie pozdrawiam Radoslaw Jaruszewski ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan Amtsgericht Gießen/Gießen Local Court: HRB 7963 Diese E-Mail is...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Radoslaw Jaruszewski (support.cantor.pl@a-w.com)
To: jkreft@drutex.com.pl | Date: 27.05.2025 09:05
Type: Answer | 
Re: [AW-230917] Ustawienie prodconf (8)
wpisz dokładnie takie wartości jak na zrzucie - powinno zadziałać :)
Serdecznie pozdrawiam
Radoslaw Jaruszewski
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus in Ihr System gelangen, haften wir nicht für die evtl. …
```

</details>

---

### [AW-221216] — 7.9 inheritance of values from the info status column for workflow statuses for which this column is unavailable

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-221216]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 26.05.2025 16:07 |

**Description:**

> RE: [AW-221216] 7.9 CANTOR VERSION (21) Hi, We already have customer who use 7.9, I see no objection to do the update if you have tested it earlier Best Regards Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan Amtsgericht Gießen/Gießen Local Court:...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: billel.benmakhlouf@oxxo.dz | Date: 26.05.2025 16:07
Type: Answer | 
RE: [AW-221216] 7.9 CANTOR VERSION (21)
Hi,
We already have customer who use 7.9, I see no objection to do the update if you have tested it earlier 
Best Regards
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus in Ihr System gelangen, haft…
```

</details>

---

### [AW-231231] — Linki do top atrybutow

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-231231]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 26.05.2025 14:49 |

**Description:**

> RE: [AW-231231] Linki do top atrybutow (2) Cześć, ~ oznacza link konfiguratora Czyli będzie esklep.krispol.pl/web.web/pl/Info/język_ze_zmiennej/Prowadzenia_przeymsl.pdf Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan Amtsgeri...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: G.Babicz@krispol.pl | Date: 26.05.2025 14:49
Type: Answer | 
RE: [AW-231231] Linki do top atrybutow (2)
Cześć,
~ oznacza link konfiguratora

Czyli będzie esklep.krispol.pl/web.web/pl/Info/język_ze_zmiennej/Prowadzenia_przeymsl.pdf
Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus…
```

</details>

---

### [AW-231379] — Problemy z wydrukami - PILNE

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-231379]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 26.05.2025 13:50 |

**Description:**

> Re: [AW-231379] Problemy z wydrukami - PILNE (4) No też mnie zaciekawiło od kiedy faktur zaczeliście używać. Jest to kwestia uprawnień np TEST-DYS Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan Amtsgericht Gießen/Gießen Loca...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: arkadiusz.guth@wiked.pl | Date: 26.05.2025 13:50
Type: Answer | 
Re: [AW-231379] Problemy z wydrukami - PILNE (4)
No też mnie zaciekawiło od kiedy faktur zaczeliście używać. Jest to kwestia uprawnień 

np TEST-DYS

Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus in Ihr System gelangen, h…
```

</details>

---

### [AW-229192] — Wartość zmiennej YFUAMIN

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-229192]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 26.05.2025 10:36 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Radoslaw Jaruszewski
To: | Date: 26.05.2025 10:36
Type: State changed | 
RE: [AW-229192] Wartość zmiennej YFUAMIN (6)
```

</details>

---

### [AW-229990] — Cantor Dealer - message not translated

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-229990]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 26.05.2025 09:51 |

**Description:**

> Re: FW: RE: [AW-229990] Fwd: Fwd: cantor - polskie teksty , uwagi (12) Hej, Nazwa zakresu w caexport jest taka sama jak nazwa nagłówka w bazie - sprawdź czy to się przenosi i ewentualnie dodaj ten zakres do eksportu Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Denn...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: jkreft@drutex.com.pl | Date: 26.05.2025 09:51
Type: Answer | 
Re: FW: RE: [AW-229990] Fwd: Fwd: cantor - polskie teksty , uwagi (12)
Hej,
Nazwa zakresu w caexport jest taka sama jak nazwa nagłówka w bazie - sprawdź czy to się przenosi i ewentualnie dodaj ten zakres do eksportu 

Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail…
```

</details>

---

### [AW-230281] — Report 700 is treated as Production documents in print settings

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-230281]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 26.05.2025 08:56 |

**Description:**

> Re: [AW-230281] wydruk 700 nie wyświetla wszystkich informacji (2) Hej, Raport do testu w załączniku Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan Amtsgericht Gießen/Gießen Local Court: HRB 7963 Diese E-Mail ist ausschließl...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: mtelega@drutex.com.pl | Date: 26.05.2025 08:56
Type: Answer | 
Re: [AW-230281] wydruk 700 nie wyświetla wszystkich informacji (2)
Hej,
Raport do testu w załączniku
Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus in Ihr System gelangen, haften wir nicht für die evtl. entstandenen Schäden.

This e-mail is…
```

</details>

---

### [AW-230991] — Zawartość folderu temp dla awspooler

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-230991]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 22.05.2025 12:52 |

**Description:**

> RE: [AW-230991] Zawartość folderu temp dla awspooler (2) Cześć, może to zostać usunięte, pamiętaj żeby w trakcie usuwania wyłączyć całkowicie spoolery i sysmany - tak aby nie blokowały Ci zawartości. Serdecznie pozdrawiam Radoslaw Jaruszewski ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, M...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Radoslaw Jaruszewski (support.cantor.pl@a-w.com)
To: szymon.kaczykowski@wiked.pl | Date: 22.05.2025 12:52
Type: Answer | 
RE: [AW-230991] Zawartość folderu temp dla awspooler (2)
Cześć,
może to zostać usunięte, pamiętaj żeby w trakcie usuwania wyłączyć całkowicie spoolery i sysmany - tak aby nie blokowały Ci zawartości.
Serdecznie pozdrawiam
Radoslaw Jaruszewski
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail…
```

</details>

---

### [AW-221969] — Encountered an improper argument error only when using CaFra.dll + 7.9

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-221969]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 20.05.2025 15:44 |

**Description:**

> RE: [AW-221969] Encountered an improper argument error only when using CaFra.dll (10) Hello, reported problem was fixed - the newest dlls are available on ftp server, please be aware that dlls were sent in version 7.9. Serdecznie pozdrawiam Radoslaw Jaruszewski ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmi...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Radoslaw Jaruszewski (support.cantor.pl@a-w.com)
To: chaouki.selama@oxxo.dz | Date: 20.05.2025 15:44
Type: Answer | 
RE: [AW-221969] Encountered an improper argument error only when using CaFra.dll (10)
Hello, reported problem was fixed - the newest dlls are available on ftp server, please be aware that dlls were sent in version 7.9.
Serdecznie pozdrawiam
Radoslaw Jaruszewski
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem e…
```

</details>

---

### [AW-230810] — Kopiowanie rabatów między dwoma komputerami

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-230810]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 20.05.2025 15:37 |

**Description:**

> Re: [AW-230810] Kopiowanie rabatów między dwoma komputerami (4) Niestety nie mamy funkcjonalności, która byłaby stworzona pod takie wymaganie. Ale być może opcje w CAEXPORT dałyby radę to ograć: Należałoby to najpierw przetestować, ponieważ ta funkcjonalność (CAEXPORT) została stworzona do przenoszenia danych pomiędzy ERP i Diler, więc opcja diler-->diler nie jest oficjalnie wspierana i należy mieć to na uwadze decydując się na używanie jej u dilerów do przenoszenia cen (nie ma opcji żeby przeni...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Radoslaw Jaruszewski (support.cantor.pl@a-w.com)
To: iiwanca@drutex.com.pl | Date: 20.05.2025 15:37
Type: Answer | 
Re: [AW-230810] Kopiowanie rabatów między dwoma komputerami (4)
Niestety nie mamy funkcjonalności, która byłaby stworzona pod takie wymaganie.
Ale być może opcje w CAEXPORT dałyby radę to ograć:

Należałoby to najpierw przetestować, ponieważ ta funkcjonalność (CAEXPORT) została stworzona do przenoszenia danych pomiędzy ERP i Diler, więc opcja diler-->diler nie jest oficjalnie wspierana i należy mieć to na uwadze decydując się na używanie jej u dilerów do przenoszenia cen (nie ma opcji żeby przenieść tylko rabaty).
 
Serdecznie pozdrawiam
Radoslaw Jaruszewski
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. …
```

</details>

---

### [AW-230647] — Preferowany termin

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-230647]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 20.05.2025 15:17 |

**Description:**

> RE: [AW-230647] Preferowany termin (2) Cześć Łukasz, niestety nie mamy takie opcji, potrzebne byłoby tu płatne rozwinięcie programu. Serdecznie pozdrawiam Radoslaw Jaruszewski ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan Amtsgericht Gießen/Gießen Local Court: ...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Radoslaw Jaruszewski (support.cantor.pl@a-w.com)
To: lukasz.urwanowicz@witraz.eu | Date: 20.05.2025 15:17
Type: Answer | 
RE: [AW-230647] Preferowany termin (2)
Cześć Łukasz,
niestety nie mamy takie opcji, potrzebne byłoby tu płatne rozwinięcie programu.
Serdecznie pozdrawiam
Radoslaw Jaruszewski
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus in Ihr System gelangen, hafte…
```

</details>

---

### [AW-230764] — Uprawnienia do tekstów wiel.

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-230764]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 20.05.2025 13:58 |

**Description:**

> RE: [AW-230764] Uprawnienia do tekstów wiel. (2) Cześć, uprawnienie do edycji to 253, a do wyświetlenia tekstów 252. Serdecznie pozdrawiam Radoslaw Jaruszewski ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan Amtsgericht Gießen/Gießen Local Court: HRB 7963 Diese E...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Radoslaw Jaruszewski (support.cantor.pl@a-w.com)
To: jkreft@drutex.com.pl | Date: 20.05.2025 13:58
Type: Answer | 
RE: [AW-230764] Uprawnienia do tekstów wiel. (2)
Cześć,
uprawnienie do edycji to 253, a do wyświetlenia tekstów 252.
Serdecznie pozdrawiam
Radoslaw Jaruszewski
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus in Ihr System gelangen, haften wir nicht für die evtl. …
```

</details>

---

### [AW-230687] — Cantor - zbyt mała czcionka

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-230687]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 19.05.2025 12:37 |

**Description:**

> RE: [AW-230687] Cantor - zbyt mała czcionka (2) Cześć, z tego co się orientuję to ustawienia wielkości czcionki (i formatowania tekstu ogólnie) można ustawiać w crystal reports Serdecznie pozdrawiam Radoslaw Jaruszewski ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘H...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Radoslaw Jaruszewski (support.cantor.pl@a-w.com)
To: iiwanca@drutex.com.pl | Date: 19.05.2025 12:37
Type: Answer | 
RE: [AW-230687] Cantor - zbyt mała czcionka (2)
Cześć,
z tego co się orientuję to ustawienia wielkości czcionki (i formatowania tekstu ogólnie) można ustawiać w crystal reports
Serdecznie pozdrawiam
Radoslaw Jaruszewski
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein …
```

</details>

---

### [AW-229774] — Fwd: Fwd: Firma drobiazg - Drukuj raport error

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-229774]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 16.05.2025 12:55 |

**Description:**

> Re: [AW-229774] Fwd: Fwd: Firma drobiazg - Drukuj raport error (6) Cześć, sprawdźcie proszę uprawnienia użytkownika do zapisu w danej lokalizacji: Serdecznie pozdrawiam Radoslaw Jaruszewski ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan Amtsgericht Gießen/Gießen...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Radoslaw Jaruszewski (support.cantor.pl@a-w.com)
To: iiwanca@drutex.com.pl | Date: 16.05.2025 12:55
Type: Answer | 
Re: [AW-229774] Fwd: Fwd: Firma drobiazg - Drukuj raport error (6)
Cześć,
sprawdźcie proszę uprawnienia użytkownika do zapisu w danej lokalizacji:

Serdecznie pozdrawiam
Radoslaw Jaruszewski
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus in Ihr System gelangen, haften wir nicht …
```

</details>

---

### [AW-230053] — SMTP Configuration with SSL and Authentication on CANTOR

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-230053]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 14.05.2025 08:45 |

**Description:**

> RE: [AW-230053] SMTP Configuration with SSL and Authentication on CANTOR (2) Hi Billel, SMTP is no longer supported by Microsoft so also by us For now In cantor there is only one option to use OAuth2. Whole documentation attached Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: billel.benmakhlouf@oxxo.dz | Date: 14.05.2025 08:45
Type: Answer | 
RE: [AW-230053] SMTP Configuration with SSL and Authentication on CANTOR (2)
Hi Billel,
SMTP is no longer supported by Microsoft so also by us 

For now In cantor there is only one option to use OAuth2. Whole documentation attached 
Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung die…
```

</details>

---

### [AW-227753] — Opisy szyb na ofercie

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-227753]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 13.05.2025 10:31 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet
To: | Date: 13.05.2025 10:31
Type: State changed | 
RE: [AW-227753] Opisy szyb na ofercie (22)
sesja zoom - rozwiązanie musi być wykonane na poziomie domyślnych - w AUFARTIK potrzebujemy wartość właściwości, nie jej opis
```

</details>

---

### [AW-225683] — Color description does not correspond with color code on the accessories list printout

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-225683]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 13.05.2025 08:19 |

**Description:**

> RE: [AW-225683] wydruk - lista akcesoriów PCV (13) Hej, Nowe DLL-ki są już na ftp. Serdecznie pozdrawiam Lukasz Lieske ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan Amtsgericht Gießen/Gießen Local Court: HRB 7963 Diese E-Mail ist ausschließlich für den Adressat...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Lukasz Lieske (support.cantor.pl@a-w.com)
To: robert.krampikowski@wiked.pl | Date: 13.05.2025 08:19
Type: Answer | 
RE: [AW-225683] wydruk - lista akcesoriów PCV (13)
Hej,
 
Nowe DLL-ki są już na ftp.
 
Serdecznie pozdrawiam
Lukasz Lieske
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus in Ihr System gelangen, haften wir nicht für die evtl. entstandenen Schäden.

This e-mail …
```

</details>

---

### [AW-229994] — Fwd: Fwd: USA - wydruk w j.polskim - jednostka mm

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-229994]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 13.05.2025 08:14 |

**Description:**

> RE: [AW-229994] Fwd: Fwd: USA - wydruk w j.polskim - jednostka mm (2) Cześć, Nie ma takiej możliwości, chyba że zamówicie taką funkcjonalność a my ją doprogramujemy Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan Amtsgericht ...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: iiwanca@drutex.com.pl | Date: 13.05.2025 08:14
Type: Answer | 
RE: [AW-229994] Fwd: Fwd: USA - wydruk w j.polskim - jednostka mm (2)
Cześć,
Nie ma takiej możliwości, chyba że zamówicie taką funkcjonalność a my ją doprogramujemy 
Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus in Ihr System gelangen, haften w…
```

</details>

---

### [AW-229856] — Iquote - pakiet instalacyjny

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-229856]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 12.05.2025 12:21 |

**Description:**

> RE: [AW-229856] Iquote - pakiet instalacyjny (2) Hej, Na ten moment nic nowszego nie mamy. Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan Amtsgericht Gießen/Gießen Local Court: HRB 7963 Diese E-Mail ist ausschließlich für de...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: G.Babicz@krispol.pl | Date: 12.05.2025 12:21
Type: Answer | 
RE: [AW-229856] Iquote - pakiet instalacyjny (2)
Hej,
Na ten moment nic nowszego nie mamy. 
Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus in Ihr System gelangen, haften wir nicht für die evtl. entstandenen Schäden.

This …
```

</details>

---

### [AW-229721] — CANTOR 7.8 (DLL 2023.1.0.69) - Odświeżanie danych na zleceniu

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-229721]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 09.05.2025 11:30 |

**Description:**

> RE: [AW-229721] CANTOR 7.8 (DLL 2023.1.0.69) - Odświeżanie danych na zleceniu (2) Cześć, Przy wprowadzaniu pozycji i pierwszej próbie wyboru właściwości np 5610 nie są wypełnione lub są błędnie wartości które używane są w funkcji dbo.krispol_brseg_DobAut_naped_I waga - bębny - ilość sprężyn Wartości te są prawidłowe po zapisie menu i ponownej próbie wyboru właściwości 5610 Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w....

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: L.Kempiak@krispol.pl | Date: 09.05.2025 11:30
Type: Answer | 
RE: [AW-229721] CANTOR 7.8 (DLL 2023.1.0.69) - Odświeżanie danych na zleceniu (2)
Cześć,
Przy wprowadzaniu pozycji i pierwszej próbie wyboru właściwości np 5610 nie są wypełnione lub są błędnie wartości które używane są w funkcji dbo.krispol_brseg_DobAut_naped_I

waga - bębny - ilość sprężyn 

Wartości te są prawidłowe po zapisie menu i ponownej próbie wyboru właściwości 5610

Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sow…
```

</details>

---

### [AW-229172] — zapytanie o przekroje

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-229172]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 08.05.2025 13:42 |

**Description:**

> RE: [AW-229172] zapytanie o przekroje (2) Cześć, Mowa tutaj o module CAD -> generowanie przekrojów poprzecznych? Tam możesz wstawiać tylko grafiki elementów na danym profilu, na ich podstawie jesteś w stanie odczytać np ilość, ale jeśli chodzi o typ i grubość to raczej nie Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsfüh...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: m.gwozdz@budvar.pl | Date: 08.05.2025 13:42
Type: Answer | 
RE: [AW-229172] zapytanie o przekroje (2)
Cześć,
Mowa tutaj o module CAD -> generowanie przekrojów poprzecznych? 
Tam możesz wstawiać tylko grafiki elementów na danym profilu, na ich podstawie jesteś w stanie odczytać np ilość, ale jeśli chodzi o typ i grubość to raczej nie 
Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbs…
```

</details>

---

### [AW-222371] — Incorrect average price calculation when transferring one material to another

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-222371]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 07.05.2025 09:42 |

**Description:**

> RE: RE: [AW-222371] Wrong CUMP Calculation when transferring from item to another (16) Hi Billel, DLL's for both versions on CANTOR are on ftp. Serdecznie pozdrawiam Lukasz Lieske ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan Amtsgericht Gießen/Gießen Local Cou...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Lukasz Lieske (support.cantor.pl@a-w.com)
To: zahir.azi@oxxo.dz, billel.benmakhlouf@oxxo.dz | Date: 07.05.2025 09:42
Type: Answer | 
RE: RE: [AW-222371] Wrong CUMP Calculation when transferring from item to another (16)
Hi Billel,
 
DLL's for both versions on CANTOR are on ftp.

Serdecznie pozdrawiam
Lukasz Lieske
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus in Ihr System gelangen, haften wir nicht für die evtl. entstandenen …
```

</details>

---

### [AW-229413] — odświeżanie zleceń starszych niż 24h

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-229413]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 07.05.2025 08:44 |

**Description:**

> RE: [AW-229413] odświeżanie zleceń starszych niż 24h (2) Cześć, Nie mamy takiej funkcjonalności Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan Amtsgericht Gießen/Gießen Local Court: HRB 7963 Diese E-Mail ist ausschließlich f...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: mtelega@drutex.com.pl | Date: 07.05.2025 08:44
Type: Answer | 
RE: [AW-229413] odświeżanie zleceń starszych niż 24h (2)
Cześć,
Nie mamy takiej funkcjonalności 
Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus in Ihr System gelangen, haften wir nicht für die evtl. entstandenen Schäden.

This e-m…
```

</details>

---

### [AW-229417] — MT - zakresy eksportowe

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-229417]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 07.05.2025 08:38 |

**Description:**

> [AW-229417] MT - zakresy eksportowe (1) Hej, Co jest przenoszone w danym zakresie sprawdzisz poprzez narzędzie sql dostępne na ERPie - jest to tabela CAEXPD W przypadku sqlek będzie to zakres nr 44 Serdecznie pozdrawiam Patryk Muszkiet ###EOM## ​ Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark T...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: radoslaw.kozlowski@domel.pl | Date: 07.05.2025 08:38
Type: Answer | 
[AW-229417] MT - zakresy eksportowe (1)
Hej,
Co jest przenoszone w danym zakresie sprawdzisz poprzez narzędzie sql dostępne na ERPie - jest to tabela CAEXPD

W przypadku sqlek będzie to zakres nr 44

Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##
​
Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendu…
```

</details>

---

### [AW-229276] — Terminal załadunkowy - błąd

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-229276]` |
| **Status** | 🟡 New |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 06.05.2025 10:59 |

**Description:**

> RE: Terminal załadunkowy - błąd (2) Dzień dobry Pani Paulino, Dziękuję za zgłoszenie. Dział suportu odezwie się w tej sprawie. Z poważaniem / Mit freundlichen Grüßen / Best regards Dawid Cegła From: PAGEN - Paulina Leżoń <p.lezon@pagen.pl> Sent: wtorek, 6 maja 2025 10:47 To: Cegla, Dawid <Dawid.Cegla@a-w.com> Cc: 'PAGEN | Marcin Plewniak' <m.plewniak@pagen.pl>; support.cantor.pl <support.cantor.pl@a-w.com>; informatyk <informatyk@pagen.pl>; d.bukowiec@pagen.pl Subject: Terminal załadunkowy - błą...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Dawid Cegła (Dawid.Cegla@a-w.com)
To: p.lezon@pagen.pl | Date: 06.05.2025 10:59
Type: Request | 
RE: Terminal załadunkowy - błąd (2)
Dzień dobry Pani Paulino,

Dziękuję za zgłoszenie. Dział suportu odezwie się w tej sprawie.
 
Z poważaniem / Mit freundlichen Grüßen / Best regards
 
Dawid Cegła

 
From: PAGEN - Paulina Leżoń <p.lezon@pagen.pl>
Sent: wtorek, 6 maja 2025 10:47
To: Cegla, Dawid <Dawid.Cegla@a-w.com>
Cc: 'PAGEN | Marcin Plewniak' <m.plewniak@pagen.pl>; support.cantor.pl <support.cantor.pl@a-w.com>; informatyk <informatyk@pagen.pl>; d.bukowiec@pagen.pl
Subject: Terminal załadunkowy - błąd

 
Panie Dawidzie,
 
Zgłaszam problem, gdzie nie przenoszą się informacje z dowodów dostaw na Terminal załadunkowy.
 
Przykład, trasa 1778.
Zlecenie 24841.
 
Dowód dostawy – poz 16 – 1 szt (poniżej screan i w załączeniu całość).
 

 
 
Poniżej widok z terminala załadunkowego, gdzie pozostałe 6 szt z pozycji 16 się pojawia – na strefie wyrobów gotowych.
 

 
To częsty problem w przypadku dzielonych dowodów dostaw. Prośba o weryfikacje.
 
 
#DoDzieła!
Pozdrawiam
Paulina Leżoń

Mana…
```

</details>

---

### [AW-229248] — blad

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-229248]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 06.05.2025 09:40 |

**Description:**

> RE: [AW-229248] blad (2) Cześć, Odsyłam do [AW-218436]: Problemem jest tu moment generowania osprzętu z 2226 - analiza - oznacza to że element dodaje się dopiero w momencie analizy technicznej I przez to powstaje błędne koło w przypadku zlecenia powtórzenia produkcji/reklamacji: system widzi że został wygenerowany nowy element, ale nie jest widoczny w polu wyboru w BOM, należy go wybrać a nie jesteśmy w stanie ponieważ w momencie gdy wchodzimy do zlecenia tego elementu tam nie ma Musicie zmienić...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: m.gwozdz@budvar.pl | Date: 06.05.2025 09:40
Type: Answer | 
RE: [AW-229248] blad (2)
Cześć,
Odsyłam do [AW-218436]:
Problemem jest tu moment generowania osprzętu z 2226 - analiza - oznacza to że element dodaje się dopiero w momencie analizy technicznej

I przez to powstaje błędne koło w przypadku zlecenia powtórzenia produkcji/reklamacji: system widzi że został wygenerowany nowy element, ale nie jest widoczny w polu wyboru w BOM, należy go wybrać a nie jesteśmy w stanie ponieważ w momencie gdy wchodzimy do zlecenia tego elementu tam nie ma 

Musicie zmienić sposób generowania tego elementu, koniecznie tak aby był dostępny przed analizą techniczną 
Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließ…
```

</details>

---

### [AW-228768] — Cantor Multitrade - kilka pytań

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-228768]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 05.05.2025 16:00 |

**Description:**

> RE: [AW-228768] Cantor Multitrade - kilka pytań (5) Hej, W sumie na wszystkie pytania odpowiedź to tak poza tym: Taka osoba powinna posiadać wgląd do przeglądu wszystkich zleceń, czy może jedynie tych, które były przesłane do działu technicznego? Tu wystarczy podgląd w te przesłane do działu technicznego Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: d.precht@pagen.pl | Date: 05.05.2025 16:00
Type: Answer | 
RE: [AW-228768] Cantor Multitrade - kilka pytań (5)
Hej,
W sumie na wszystkie pytania odpowiedź to tak poza tym:
Taka osoba powinna posiadać wgląd do przeglądu wszystkich zleceń, czy może jedynie tych, które były przesłane do działu technicznego? Tu wystarczy podgląd w te przesłane do działu technicznego 
Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist n…
```

</details>

---

### [AW-229115] — Blokada rabatu niewidocznego

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-229115]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 05.05.2025 11:17 |

**Description:**

> RE: [AW-229115] Blokada rabatu niewidocznego (2) Cześć, Nie ma takiego uprawnienia - jeśli jest możliwa edycja cen/rabatów to tyczy się wszystkiego Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan Amtsgericht Gießen/Gießen Loc...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: m.gwozdz@budvar.pl | Date: 05.05.2025 11:17
Type: Answer | 
RE: [AW-229115] Blokada rabatu niewidocznego (2)
Cześć,
Nie ma takiego uprawnienia - jeśli jest możliwa edycja cen/rabatów to tyczy się wszystkiego
Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus in Ihr System gelangen, hafte…
```

</details>

---

### [AW-228862] — Faktury kwoty - Empol S.A. , Empol BIS S.A

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-228862]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 30.04.2025 14:46 |

**Description:**

> RE: [AW-228862] Faktury kwoty - Empol S.A. , Empol BIS S.A (2) Cześć, Gdzie w cantorze znajdę te faktury? Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan Amtsgericht Gießen/Gießen Local Court: HRB 7963 Diese E-Mail ist aussch...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: mszkoda@empol.pl | Date: 30.04.2025 14:46
Type: Answer | 
RE: [AW-228862] Faktury kwoty - Empol S.A. , Empol BIS S.A (2)
Cześć,
Gdzie w cantorze znajdę te faktury?
Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus in Ihr System gelangen, haften wir nicht für die evtl. entstandenen Schäden.

This …
```

</details>

---

### [AW-228865] — Teksty nagłówków i stopek

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-228865]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 30.04.2025 13:45 |

**Description:**

> RE: [AW-228865] Teksty nagłówków i stopek (2) Cześć, W ramach płatnego developmentu być może tak. Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan Amtsgericht Gießen/Gießen Local Court: HRB 7963 Diese E-Mail ist ausschließlich...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: L.Nowak@krishome.eu | Date: 30.04.2025 13:45
Type: Answer | 
RE: [AW-228865] Teksty nagłówków i stopek (2)
Cześć,
W ramach płatnego developmentu być może tak. 
Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus in Ihr System gelangen, haften wir nicht für die evtl. entstandenen Schäden…
```

</details>

---

### [AW-226151] — Przekroje kontrukcji

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-226151]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 30.04.2025 11:10 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet
To: | Date: 30.04.2025 11:10
Type: State changed | 
RE: [AW-226151] Przekroje kontrukcji (3)
```

</details>

---

### [AW-224514] — Filtrowanie zamówień w zamówieniach magazynówek

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-224514]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 30.04.2025 11:06 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet
To: | Date: 30.04.2025 11:06
Type: State changed | 
RE: [AW-224514] Filtrowanie zamówień w zamówieniach magazynówek (3)
```

</details>

---

### [AW-225862] — Alternatywy w roletach

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-225862]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 30.04.2025 10:41 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet
To: | Date: 30.04.2025 10:41
Type: State changed | 
RE: [AW-225862] Alternatywy w roletach (4)
```

</details>

---

### [AW-223437] — Obiekty rysunkowe kolejność rysowania

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-223437]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 29.04.2025 12:13 |

**Description:**

> RE: [AW-223437] Obiekty rysunkowe kolejność rysowania (10) Cześć, Przeanalizowałem temat i wniosek jest nastepujący: W przypadku obiektów rysunkowych warstwy nie mają zastosowania, ponieważ wszystkie obrazy generują się na jednej, o oznaczeniu 0 Roleta jest elementem który jest wyżej w hierarchii niż moskitiera (grupy synów 2 (niebieski) oraz 3 (żółty)). Z tego co sprawdziłem ten element który na liście ma niższy numer grupy generuje się jako pierwszy na grafice (PAN_W przed PLISA_MO_W). Jeśli e...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: G.Sieradzki@krishome.eu | Date: 29.04.2025 12:13
Type: Answer | 
RE: [AW-223437] Obiekty rysunkowe kolejność rysowania (10)
Cześć,
Przeanalizowałem temat i wniosek jest nastepujący:
W przypadku obiektów rysunkowych warstwy nie mają zastosowania, ponieważ wszystkie obrazy generują się na jednej, o oznaczeniu 0 

Roleta jest elementem który jest wyżej w hierarchii niż moskitiera (grupy synów 2 (niebieski) oraz 3 (żółty)). Z tego co sprawdziłem ten element który na liście ma niższy numer grupy generuje się jako pierwszy na grafice (PAN_W przed PLISA_MO_W). Jeśli elementy są w obrębie jednej grupy jak np PAN_W oraz NAW to wtedy o hierarchii wyświetlania decyduje numer REF co widać na poniższym przykładzie gdzie nawijarka o wyższym ref# została przesunięta nad obraz rolety o niższym ref#

Rozwiązaniem na Twój problem jest generowanie grafiki PAN_W oraz PLISA_MO_W w obrębie jednej grupy, wtedy za pomocą indeksu sortowania będziemy w stanie wyciągnąć PLISA_MO_W nad PAN_W
Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
…
```

</details>

---

### [AW-228548] — Fwd: RYSUNEK NA WYDRUKU / RYSUNEK W CANTORZE

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-228548]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 28.04.2025 15:18 |

**Description:**

> Re: [AW-228548] Fwd: RYSUNEK NA WYDRUKU / RYSUNEK W CANTORZE (4) Cześć, ShowShadow? Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan Amtsgericht Gießen/Gießen Local Court: HRB 7963 Diese E-Mail ist ausschließlich für den Adres...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: jkreft@drutex.com.pl | Date: 28.04.2025 15:18
Type: Answer | 
Re: [AW-228548] Fwd: RYSUNEK NA WYDRUKU / RYSUNEK W CANTORZE (4)
Cześć,
ShowShadow?
Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus in Ihr System gelangen, haften wir nicht für die evtl. entstandenen Schäden.

This e-mail is for the intend…
```

</details>

---

### [AW-228531] — [Fwd: ##RE-68470## : 871021]

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-228531]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 28.04.2025 14:09 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet
To: | Date: 28.04.2025 14:09
Type: State changed | 
RE: [AW-228531] [Fwd: ##RE-68470## : 871021] (10)
```

</details>

---

### [AW-219689] — Problem z wyświetlaniem tekstury dekoru na IQuote

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-219689]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 25.04.2025 15:03 |

**Description:**

> RE: [AW-219689] Problem z wyświetlaniem tekstury dekoru na IQuote (15) Nie mam dostępu do instalki mojej wersji. Aktualizację iQuote mamy zawsze do najnowszej, to co wysłałem na FTPa to wersja z 20.03.2025. Koniecznie zróbcie to najpierw na poligonie Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors:...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: G.Babicz@krispol.pl | Date: 25.04.2025 15:03
Type: Answer | 
RE: [AW-219689] Problem z wyświetlaniem tekstury dekoru na IQuote (15)
Nie mam dostępu do instalki mojej wersji. Aktualizację iQuote mamy zawsze do najnowszej, to co wysłałem na FTPa to wersja z 20.03.2025.
Koniecznie zróbcie to najpierw na poligonie 
Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sol…
```

</details>

---

### [AW-228107] — zdefiniowana stopka na wydruku ofertowym

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-228107]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 24.04.2025 15:24 |

**Description:**

> Re: Fwd: [AW-228107] zdefiniowana stopka na wydruku ofertowym (6) Hej, Niestety nie w wersji dealerskiej. Spróbujcie może zaproponować umieszczenie tej formatki w tym miejscu to co tam wpiszesz ląduje do handconfa 20 i 21, na wydruku konieczne wyciągnięcie następującego pola: Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäfts...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: mtelega@drutex.com.pl, iiwanca@drutex.com.pl | Date: 24.04.2025 15:24
Type: Answer | 
Re: Fwd: [AW-228107] zdefiniowana stopka na wydruku ofertowym (6)
Hej,
Niestety nie w wersji dealerskiej. Spróbujcie może zaproponować umieszczenie tej formatki w tym miejscu 

to co tam wpiszesz ląduje do handconfa 20 i 21, na wydruku konieczne wyciągnięcie następującego pola:

Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verw…
```

</details>

---

### [AW-227872] — Wiki - link won't open

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-227872]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 24.04.2025 12:41 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet
To: | Date: 24.04.2025 12:41
Type: State changed | 
RE: [AW-227872] Wiki - link won't open (8)
waiting for ict
```

</details>

---

### [AW-218436] — Problem with article Z801 created for camplaint order

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-218436]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 24.04.2025 12:26 |

**Description:**

> FW: RE: [AW-218436] Problem z puszczeniem na produkcję 911726 (15) Cześć. Problemem jest tu moment generowania osprzętu z 2226 - analiza - oznacza to że element dodaje się dopiero w momencie analizy technicznej I przez to powstaje błędne koło w przypadku zlecenia powtórzenia produkcji/reklamacji: system widzi że został wygenerowany nowy element, ale nie jest widoczny w polu wyboru w BOM, należy go wybrać a nie jesteśmy w stanie ponieważ w momencie gdy wchodzimy do zlecenia tego elementu tam nie ...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: m.kosecka@budvar.pl | Date: 24.04.2025 12:26
Type: Answer | 
FW: RE: [AW-218436] Problem z puszczeniem na produkcję 911726 (15)
Cześć.
Problemem jest tu moment generowania osprzętu z 2226 - analiza - oznacza to że element dodaje się dopiero w momencie analizy technicznej

I przez to powstaje błędne koło w przypadku zlecenia powtórzenia produkcji/reklamacji: system widzi że został wygenerowany nowy element, ale nie jest widoczny w polu wyboru w BOM, należy go wybrać a nie jesteśmy w stanie ponieważ w momencie gdy wchodzimy do zlecenia tego elementu tam nie ma 

Musicie zmienić sposób generowania tego elementu, koniecznie tak aby był dostępny przed analizą techniczną 
Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten b…
```

</details>

---

### [AW-222722] — Obiekty rysunkowe

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-222722]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 24.04.2025 10:48 |

**Description:**

> RE: [AW-222722] Obiekty rysunkowe (2) Cześć, Uciekł mi przykład odnośnie tego zgłoszenia, możesz podrzucić nr zlecenia? Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan Amtsgericht Gießen/Gießen Local Court: HRB 7963 Diese E-M...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: przemyslaw.barthelke@wiked.pl | Date: 24.04.2025 10:48
Type: Answer | 
RE: [AW-222722] Obiekty rysunkowe (2)
Cześć,
Uciekł mi przykład odnośnie tego zgłoszenia, możesz podrzucić nr zlecenia? 
Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus in Ihr System gelangen, haften wir nicht für …
```

</details>

---

### [AW-227932] — [Urgent] Błąd przy imporcie zlecenia

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-227932]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 24.04.2025 09:26 |

**Description:**

> Re: [AW-227932] [Urgent] Błąd przy imporcie zlecenia (6) Cześć, Zatem wyeksportuj raz jeszcze zlecenie, jeśli problem się powtórzy to proszę w miarę możliwości o bazę z tej instancji. (backup można utworzyć jednym kliknięciem) Nr wersji master data musi się zgadzać podczas eksportu pomiędzy bazą a paczką. Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Wrześni...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: psuszko@drutex.com.pl | Date: 24.04.2025 09:26
Type: Answer | 
Re: [AW-227932] [Urgent] Błąd przy imporcie zlecenia (6)
Cześć,
Zatem wyeksportuj raz jeszcze zlecenie, jeśli problem się powtórzy to proszę w miarę możliwości o bazę z tej instancji.
(backup można utworzyć jednym kliknięciem)

Nr wersji master data musi się zgadzać podczas eksportu pomiędzy bazą a paczką.
Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nic…
```

</details>

---

### [AW-228067] — CANTOR 7.8 (DLL 2023.1.0.69) - Problem z generowaniem danych na wydruk

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-228067]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 23.04.2025 15:58 |

**Description:**

> RE: [AW-228067] CANTOR 7.8 (DLL 2023.1.0.69) - Problem z generowaniem danych na wydruk (4) Zgadza się, jeśli te artykuły są z tych dwóch wymienionych klas to taki będzie efekt uboczny Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: L.Kempiak@krispol.pl | Date: 23.04.2025 15:58
Type: Answer | 
RE: [AW-228067] CANTOR 7.8 (DLL 2023.1.0.69) - Problem z generowaniem danych na wydruk (4)
Zgadza się, jeśli te artykuły są z tych dwóch wymienionych klas to taki będzie efekt uboczny 
Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus in Ihr System gelangen, haften wir …
```

</details>

---

### [AW-227774] — oPTYMALIZACJA

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-227774]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 22.04.2025 11:54 |

**Description:**

> Re: [AW-227774] oPTYMALIZACJA (4) Cześć, Musisz jeszcze wskazać ID listy o której mowa bo jeśli chodzi o  centrum to rozumiem że terminal 2099 pliki na maszyny? W ustawieniach etykiety możesz definiować tryb cięcia i może być on różny od tego na maszynie, stąd może wynikać różnica Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Gesc...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: przemyslaw.barthelke@wiked.pl | Date: 22.04.2025 11:54
Type: Answer | 
Re: [AW-227774] oPTYMALIZACJA (4)
Cześć,
Musisz jeszcze wskazać ID listy o której mowa

bo jeśli chodzi o  centrum to rozumiem że terminal 2099 pliki na maszyny?

W ustawieniach etykiety możesz definiować tryb cięcia i może być on różny od tego na maszynie, stąd może wynikać różnica

Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist n…
```

</details>

---

### [AW-227838] — data ważności oferty

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-227838]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 22.04.2025 10:29 |

**Description:**

> Re: [AW-227838] data ważności oferty (4) Niestety nie, tylko dni robocze Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan Amtsgericht Gießen/Gießen Local Court: HRB 7963 Diese E-Mail ist ausschließlich für den Adressaten besti...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: mtelega@drutex.com.pl | Date: 22.04.2025 10:29
Type: Answer | 
Re: [AW-227838] data ważności oferty (4)
Niestety nie, tylko dni robocze 
Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus in Ihr System gelangen, haften wir nicht für die evtl. entstandenen Schäden.

This e-mail is f…
```

</details>

---

### [AW-227768] — Zdjęcia klamek/smartlock na ofercie

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-227768]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 18.04.2025 14:00 |

**Description:**

> Re: [AW-227768] Zdjęcia klamek/smartlock na ofercie (4) To jak najbardziej jest to możliwe, aby osprzęt jako pozycja drukował się na potwierdzeniu należy zaznaczyć na nim opcję mapa bitowa: Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, T...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: jkreft@drutex.com.pl | Date: 18.04.2025 14:00
Type: Answer | 
Re: [AW-227768] Zdjęcia klamek/smartlock na ofercie (4)
To jak najbardziej jest to możliwe, aby osprzęt jako pozycja drukował się na potwierdzeniu należy zaznaczyć na nim opcję mapa bitowa:

Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein…
```

</details>

---

### [AW-223698] — Błąd przy przenoszeniu rabatów

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-223698]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 18.04.2025 12:41 |

**Description:**

> Re: [AW-223698] Re: Błąd przy przenoszeniu rabatów (7) Hej, Na ERPie reguła podatkowa nie bierze się z klienta, a z domyślej wartości ustawionej w tax rules Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan Amtsgericht Gießen/G...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: jkreft@drutex.com.pl | Date: 18.04.2025 12:41
Type: Answer | 
Re: [AW-223698] Re: Błąd przy przenoszeniu rabatów (7)
Hej,
Na ERPie reguła podatkowa nie bierze się z klienta, a z domyślej wartości ustawionej w tax rules 

Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus in Ihr System gelangen,…
```

</details>

---

### [AW-227754] — Tłum. tekstów nagłówek i stopek :)

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-227754]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 18.04.2025 09:55 |

**Description:**

> RE: [AW-227754] Tłum. tekstów nagłówek i stopek :) (2) Hej, Tak: SELECT * FROM DRUTEX_ERP.TEXTE WHERE SYSTEMMANDANT=0 AND Auftyp <> '#AP' AND POSITIONSTEXT=0 ORDER BY AUFTYP, IND, LFDNR, POSITIONSTEXT Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark ...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: jkreft@drutex.com.pl | Date: 18.04.2025 09:55
Type: Answer | 
RE: [AW-227754] Tłum. tekstów nagłówek i stopek :) (2)
Hej,
Tak:
SELECT * FROM DRUTEX_ERP.TEXTE WHERE SYSTEMMANDANT=0 AND Auftyp <> '#AP' AND POSITIONSTEXT=0 ORDER BY AUFTYP, IND, LFDNR, POSITIONSTEXT

 
Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-…
```

</details>

---

### [AW-227688] — skrót klawiszowy na status workflow

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-227688]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 18.04.2025 08:29 |

**Description:**

> RE: [AW-227688] skrót klawiszowy na status workflow (2) Cześć, Nie ma takiej opcji, skróty klawiszowe możemy przypisać tylko do funkcji z paska górnego menu w danym oknie, a niestety nie jesteśmy w stanie odwołać się do konkretnego statusu Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Eric Herrm...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: mtelega@drutex.com.pl | Date: 18.04.2025 08:29
Type: Answer | 
RE: [AW-227688] skrót klawiszowy na status workflow (2)
Cześć,
Nie ma takiej opcji, skróty klawiszowe możemy przypisać tylko do funkcji z paska górnego menu w danym oknie, a niestety nie jesteśmy w stanie odwołać się do konkretnego statusu 

Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramm…
```

</details>

---

### [AW-222096] — CaImport - Inconsistency between delete and insert statement: artprschema vs preisschema

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-222096]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 17.04.2025 12:22 |

**Description:**

> FW: Re: [AW-222096] Błąd przy imporcie paczki drugi raz w ciągu jednego dnia (11) Cześć, Problem tu powoduje delete na preise który wrzuciliście do SQL przed importem Oto skrypt który usuwa dane z tabeli źródłowej: Ma 660 rezultatów Więc spod bazy wygląda wszystko ok, natomiast fakt że w SQL przed importem robicie delete from preise całkowicie niszczy logikę powyższego zapytania, co za tym idzie część danych nie jest usuwana i tworzą się duplikaty podczas kolejnego importu Oto przykład co dzieje...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: dpradzinski@drutex.com.pl | Date: 17.04.2025 12:22
Type: Answer | 
FW: Re: [AW-222096] Błąd przy imporcie paczki drugi raz w ciągu jednego dnia (11)
Cześć,
Problem tu powoduje delete na preise który wrzuciliście do SQL przed importem

Oto skrypt który usuwa dane z tabeli źródłowej:

Ma 660 rezultatów 

Więc spod bazy wygląda wszystko ok, natomiast fakt że w SQL przed importem robicie delete from preise całkowicie niszczy logikę powyższego zapytania, co za tym idzie część danych nie jest usuwana i tworzą się duplikaty podczas kolejnego importu 
Oto przykład co dzieje się podczas importu:
1 delete
2 zamiast 660 rekordów nie usuwa się nic

Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtl…
```

</details>

---

### [AW-217526] — Lack of translation Italian - remake position 'Teile einer Position'

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-217526]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 17.04.2025 08:31 |

**Description:**

> FW: RE: [AW-217526] Tłumaczenie fragmentu kostrukcji (10) Cześć, Tłumaczenie zostało poprawione - dllki na ftpie Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Peter Dixen, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan Amtsgericht Gießen/Gießen Local Court: HRB 7963 Diese E-Mail ist a...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: m.gwozdz@budvar.pl | Date: 17.04.2025 08:31
Type: Answer | 
FW: RE: [AW-217526] Tłumaczenie fragmentu kostrukcji (10)
Cześć,
Tłumaczenie zostało poprawione - dllki na ftpie 
Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Peter Dixen, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus in Ihr System gelangen, haften wir nicht für die evtl. entstandenen Schäde…
```

</details>

---

### [AW-227340] — Update Article variable after updating property lable

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-227340]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 16.04.2025 11:54 |

**Description:**

> RE: [AW-227340] Update Article variable after updating property lable (4) Hi Billel, Unfortunately, at this time we do not have any solution or tool available to help solve this particular scenario. If, in the future, something changes or we develop an appropriate feature, we will certainly let you know. Of course, if you are interested, we can add some type of checking here on request for a additional fee Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +49641966...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: billel.benmakhlouf@oxxo.dz | Date: 16.04.2025 11:54
Type: Answer | 
RE: [AW-227340] Update Article variable after updating property lable (4)
Hi Billel,
Unfortunately, at this time we do not have any solution or tool available to help solve this particular scenario. 
If, in the future, something changes or we develop an appropriate feature, we will certainly let you know. Of course, if you are interested, we can add some type of checking here on request for a additional fee 
Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Peter Dixen, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu lö…
```

</details>

---

### [AW-227315] — Uprawnienia do sterowania wydruku

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-227315]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 15.04.2025 11:39 |

**Description:**

> RE: [AW-227315] Uprawnienia do sterowania wydruku (2) Cześć, Uprawnienie 2026 odblokowuje tą opcje: Serdecznie pozdrawiam Lukasz Lieske ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Peter Dixen, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan Amtsgericht Gießen/Gießen Local Court: HRB 7963 Diese E-Mail ist ausschließlich f...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Lukasz Lieske (support.cantor.pl@a-w.com)
To: jkreft@drutex.com.pl | Date: 15.04.2025 11:39
Type: Answer | 
RE: [AW-227315] Uprawnienia do sterowania wydruku (2)
Cześć,
 
Uprawnienie 2026 odblokowuje tą opcje:

Serdecznie pozdrawiam
Lukasz Lieske
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Peter Dixen, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus in Ihr System gelangen, haften wir nicht für die evtl. entstandenen Schäden.

T…
```

</details>

---

### [AW-225855] — Smart Companion Stock and Purchase service working only for site 1

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-225855]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 15.04.2025 11:30 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Dawid Rogacki
To: | Date: 15.04.2025 11:30
Type: State changed | 
RE: [AW-225855] Smart Companion Stock and Purchase service working only for site 1 (6)
channel
```

</details>

---

### [AW-225808] — RE: 19849 - okno nie przypisane do stojaka, ze statusem "w magazynie"

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-225808]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 14.04.2025 14:44 |

**Description:**

> RE: [AW-225808] RE: 19849 - okno nie przypisane do stojaka, ze statusem "w magazynie" (4) Dzień dobry, Zgadzam się z wnioskami przedstawionymi przez Pana Dawida – wskazani pracownicy nie mają możliwości jednoczesnego zalogowania się na ten sam terminal. Z mojej strony przeanalizowałem sytuację w kontekście danych dostępnych w bazie, jednak niestety nie udało się znaleźć żadnych przesłanek, które mogłyby wyjaśnić zaistniały problem. Obawiam się, że obecnie nie dysponujemy narzędziami pozwalającym...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: p.lezon@pagen.pl, d.precht@pagen.pl | Date: 14.04.2025 14:44
Type: Answer | 
RE: [AW-225808] RE: 19849 - okno nie przypisane do stojaka, ze statusem "w magazynie" (4)
Dzień dobry,
Zgadzam się z wnioskami przedstawionymi przez Pana Dawida – wskazani pracownicy nie mają możliwości jednoczesnego zalogowania się na ten sam terminal.
Z mojej strony przeanalizowałem sytuację w kontekście danych dostępnych w bazie, jednak niestety nie udało się znaleźć żadnych przesłanek, które mogłyby wyjaśnić zaistniały problem. Obawiam się, że obecnie nie dysponujemy narzędziami pozwalającymi na dokładne ustalenie przyczyn tego zdarzenia.
Proponuję rozważyć przeprowadzenie rozmów z pracownikami wskazanymi w zgłoszeniu. Być może posiadają wiedzę na temat sposobów obejścia zabezpieczeń, które pozwoliłyby na zalogowanie się na terminal już używany przez innego użytkownika.
Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Peter Dixen, Julia Schmidt, D…
```

</details>

---

### [AW-227067] — Brak zamówienia od klienta

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-227067]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 11.04.2025 15:54 |

**Description:**

> RE: [AW-227067] Brak zamówienia od klienta (2) Hej, Najpierw tabela mailjob z parametrem aufnrold = nr_zlec_z_mt/dealera Jeśli będzie rezultat to aufnrnew to nr zlecenia w ERP Jeśli powyższa tabela nie będzie miała rezultatów to tabelę errorlog przejrzeć Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Direct...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: jkreft@drutex.com.pl | Date: 11.04.2025 15:54
Type: Answer | 
RE: [AW-227067] Brak zamówienia od klienta (2)
Hej,
Najpierw tabela mailjob z parametrem aufnrold = nr_zlec_z_mt/dealera
Jeśli będzie rezultat to aufnrnew to nr zlecenia w ERP
Jeśli powyższa tabela nie będzie miała rezultatów to tabelę errorlog przejrzeć
Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Peter Dixen, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir…
```

</details>

---

### [AW-226517] — Zlecenie nie zmienia statusy na PO_OK

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-226517]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 10.04.2025 14:36 |

**Description:**

> RE: [AW-226517] Zlecenie nie zmienia statusy na PO_OK (2) Cześć, Sprawdziłem u nas na wersji 7.8 ten status zmienia się prawidłowo po wydrukowaniu potwierdzenia oferty. Możesz potwierdzić czy zadanie wydrukowania potwierdzenia oferty zapisuje się w historii zlecenia? Serdecznie pozdrawiam Lukasz Lieske ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Mana...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Lukasz Lieske (support.cantor.pl@a-w.com)
To: mtelega@drutex.com.pl | Date: 10.04.2025 14:36
Type: Answer | 
RE: [AW-226517] Zlecenie nie zmienia statusy na PO_OK (2)
Cześć,
 
Sprawdziłem u nas na wersji 7.8 ten status zmienia się prawidłowo po wydrukowaniu potwierdzenia oferty.

 
Możesz potwierdzić czy zadanie wydrukowania potwierdzenia oferty zapisuje się w historii zlecenia?

Serdecznie pozdrawiam
Lukasz Lieske
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Peter Dixen, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verw…
```

</details>

---

### [AW-226423] — Fwd: Błąd ramki dystansowej

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-226423]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 07.04.2025 11:16 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet
To: | Date: 07.04.2025 11:16
Type: State changed | 
RE: [AW-226423] Fwd: Błąd ramki dystansowej (4)
```

</details>

---

### [AW-225617] — Błąd podczas aktualizacji DLL

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-225617]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 01.04.2025 08:17 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Radoslaw Jaruszewski
To: | Date: 01.04.2025 08:17
Type: State changed | 
RE: [AW-225617] Błąd podczas aktualizacji DLL (4)
```

</details>

---

### [AW-225642] — nie da się zlecenia przeliczyc

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-225642]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 31.03.2025 14:27 |

**Description:**

> RE: [AW-225642] nie da się zlecenia przeliczyc (2) Cześć Marku, pobrałem zlecenia (oryginał i reklamację) przekalkulowałem i przeszło poprawnie: Nie chcę działać na waszym "żywym systemie", czy mógłbyś podegrać to na bazę testową i podać mi tylko dostęp do niej (pliki ini oraz dll-ki) Serdecznie pozdrawiam Radoslaw Jaruszewski ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Radoslaw Jaruszewski (support.cantor.pl@a-w.com)
To: m.gwozdz@budvar.pl | Date: 31.03.2025 14:27
Type: Answer | 
RE: [AW-225642] nie da się zlecenia przeliczyc (2)
Cześć Marku,
pobrałem zlecenia (oryginał i reklamację) przekalkulowałem i przeszło poprawnie:

Nie chcę działać na waszym "żywym systemie", czy mógłbyś podegrać to na bazę testową i podać mi tylko dostęp do niej (pliki ini oraz dll-ki)
Serdecznie pozdrawiam
Radoslaw Jaruszewski
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Peter Dixen, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet.…
```

</details>

---

### [AW-224180] — Canotr źle liczy robociznę  po kalkulacji terminy dostawy

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-224180]` |
| **Status** | 🔵 In Progress |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 31.03.2025 10:38 |

**Description:**

> RE: RE: [AW-224180] Canotr źle liczy robociznę  po kalkulacji terminy dostawy (9) Jak wyłączyłem tego prodconfa to przestały pojawiać się te blokady Pozdrawiam, Marek Gwozdz IT Manager Dział IT mobile: 663 442 325 email: m.gwozdz@budvar.pl tel.: +48 43 824 31 32 wew. 262 <https://www.budvar.pl/> <https://www.budvarcentrum.pl/typ-produktu/drzwi-wejsciowe-aluminiowe/> <https://www.budvarcentrum.pl> <https://www.budvarcentrum.pl/> <https://www.budvarcentrum.pl/> <https://www.budvarcentrum.pl/><http...

<details>
<summary>View Full Conversation Thread</summary>

```
From: BUDVAR SPÓLKA Z OGRANICZONA ODPOWIE (m.gwozdz@budvar.pl)
To: support.cantor.pl@a-w.com | Date: 31.03.2025 10:38
Type: Request | 
RE: RE: [AW-224180] Canotr źle liczy robociznę  po kalkulacji terminy dostawy (9)
Jak wyłączyłem tego prodconfa to przestały pojawiać się te blokady

       Pozdrawiam,

Marek Gwozdz
IT Manager
Dział IT

mobile: 663 442 325
email: m.gwozdz@budvar.pl
tel.: +48 43 824 31 32 wew. 262

<https://www.budvar.pl/>

<https://www.budvarcentrum.pl/typ-produktu/drzwi-wejsciowe-aluminiowe/>

<https://www.budvarcentrum.pl>

<https://www.budvarcentrum.pl/>

<https://www.budvarcentrum.pl/>

<https://www.budvarcentrum.pl/><https://www.budvarcentrum.pl/>

<https://www.budvarcentrum.pl/><https://www.budvarcentrum.pl/produkt/okna-pvc/t-passive-perfekt/><https://katalog.grupamtp.pl/pl?oid=1588647&ec=T132301&ec=T992301><https://www.budvarcentrum.pl/typ-produktu/okna-aluminiowe/>

Administratorem danych osobowych jest BUDVAR CENTRUM Sp. z o.o. z siedzibą w Warszawie, Przetwarzamy dane osobowe w celu kontaktu lub realizacji usługi. Kontakt w sprawach ochrony danych osobowych możliwy jest pod adresem: iod@budvar.p…
```

</details>

---

### [AW-223135] — RE: Worng commercial site assignement (Invoice)

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-223135]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 20.03.2025 09:41 |

**Description:**

> RE: [AW-223135] RE: Worng commercial site assignement (Invoice) (6) Hi Billel, I have carefully reviewed the entire process of creating an invoice using the workflow, and everything appears to be correct. Specifically, the most critical page was neither incorrect nor altered when opening the invoice preview. At this point, I am unsure how to proceed further to address this issue. To identify a solution, we may need to understand how to manually replicate such an example. Could you kindly provide...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: billel.benmakhlouf@oxxo.dz | Date: 20.03.2025 09:41
Type: Answer | 
RE: [AW-223135] RE: Worng commercial site assignement (Invoice) (6)
Hi Billel,
I have carefully reviewed the entire process of creating an invoice using the workflow, and everything appears to be correct. Specifically, the most critical page was neither incorrect nor altered when opening the invoice preview.
At this point, I am unsure how to proceed further to address this issue. To identify a solution, we may need to understand how to manually replicate such an example. Could you kindly provide additional details or guidance on this matter?
Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Peter Dixen, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informatione…
```

</details>

---

### [AW-223518] — automatyczne liczenie terminów dostaw

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-223518]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 14.03.2025 08:17 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet
To: | Date: 14.03.2025 08:17
Type: State changed | 
RE: [AW-223518] automatyczne liczenie terminów dostaw (4)
```

</details>

---

### [AW-223166] — Dealer - duplikat klucza przy imporcie

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-223166]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 11.03.2025 14:52 |

**Description:**

> Re: [AW-223166] Dealer - duplikat klucza przy imporcie (4) to proszę podeślij plik z masterdata :) Serdecznie pozdrawiam Radoslaw Jaruszewski ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Peter Dixen, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan Amtsgericht Gießen/Gießen Local Court: HRB 7963 Diese E-Mail ist ausschließ...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Radoslaw Jaruszewski (support.cantor.pl@a-w.com)
To: jkreft@drutex.com.pl | Date: 11.03.2025 14:52
Type: Answer | 
Re: [AW-223166] Dealer - duplikat klucza przy imporcie (4)
to proszę podeślij plik z masterdata :)
Serdecznie pozdrawiam
Radoslaw Jaruszewski
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Peter Dixen, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus in Ihr System gelangen, haften wir nicht für die evtl. entstandenen Schäden.

This e…
```

</details>

---

### [AW-221515] — Wydajność canor-a i archiwizacja zleceń

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-221515]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 06.03.2025 15:32 |

**Description:**

> FW: [AW-221515] Wydajność canor-a i archiwizacja zleceń (4) Cześć Kuba, dosyłam skrypt w załączniku, najpewniej w trakcie wykonania pojawią się błędy jak ponizej, niestety nie byłem w stanie tego obejść, finalnie rezultat jednak jest prawidłowy: Weź jeszcze pod uwagę, że skrypty dla ERP i CIM były zrobione w oparciu o nasze bazy, najpewniej ich nazwy pokrywają się z tym co jest u Was na serwerze, ale sprawdź proszę to zanim je wykonasz: ERP=DOMEL, CIM=DOMEL_PRODU I jeszcze jedna sprawa, sprawdź ...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Radoslaw Jaruszewski (support.cantor.pl@a-w.com)
To: jakub.alachamowicz@domel.pl | Date: 06.03.2025 15:32
Type: Answer | 
FW: [AW-221515] Wydajność canor-a i archiwizacja zleceń (4)
Cześć Kuba,
dosyłam skrypt w załączniku, najpewniej w trakcie wykonania pojawią się błędy jak ponizej, niestety nie byłem w stanie tego obejść, finalnie rezultat jednak jest prawidłowy:

Weź jeszcze pod uwagę, że skrypty dla ERP i CIM były zrobione w oparciu o nasze bazy, najpewniej ich nazwy pokrywają się z tym co jest u Was na serwerze, ale sprawdź proszę to zanim je wykonasz: ERP=DOMEL, CIM=DOMEL_PRODU
I jeszcze jedna sprawa, sprawdź zawartość tabeli na CIM[[UEBFILTD], jest tam zmieniane collation, więc dane z kolumny WERT są przenoszone do tabeli temp a potem ponownie wykonywany jest update dla tej kolumny - na mojej bazie jest ona pusta, ale jeśli u Was coś jest to warto sprawdzić czy zawartość po wykonaniu skryptu w kolumnie WERT jest taka sama jak przed.
 
Serdecznie pozdrawiam
Radoslaw Jaruszewski
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska …
```

</details>

---

### [AW-222100] — Dostęp do customer portal

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-222100]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 03.03.2025 10:39 |

**Description:**

> RE: [AW-222100] Customer portal - problem with ticket access after registration (7) Hello Frank, Customer has a problem with accessing tickets tab in customer portal. I asked if he did all listed steps in this case, and he confirmed. He registered to the portal on friday 28th of february, can login into portal main page, but cannot access tickets list - he is using correct username and password His access is active Could you please check on your side? Serdecznie pozdrawiam Patryk Muszkiet ###EOM...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: frank.agel@a-w.com | Date: 03.03.2025 10:39
Type: Answer | 
RE: [AW-222100] Customer portal - problem with ticket access after registration (7)
Hello Frank,
Customer has a problem with accessing tickets tab in customer portal. I asked if he did all listed steps in this case, and he confirmed.

 He registered to the portal on friday 28th of february, can login into portal main page, but cannot access tickets list - he is using correct username and password 

His access is active 

Could you please check on your side?
Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##
​
Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Peter Dixen, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns …
```

</details>

---

### [AW-221501] — Fwd: Fwd:

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-221501]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 25.02.2025 08:42 |

**Description:**

> RE: [AW-221501] Fwd: Fwd: (2) Hej ma być 2 czy 1? Serdecznie pozdrawiam Patryk Muszkiet ###EOM## Phone:  +48 61 438 47 44 Mobile:  +4964196620-0 Email: support.cantor.pl@a-w.com A+W Software Polska Sp. z o. o. ul. Sikorskiego 44 62-300 Września Polska www.a-w.com Geschäftsführer/Managing Directors: Peter Dixen, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan Amtsgericht Gießen/Gießen Local Court: HRB 7963 Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet (support.cantor.pl@a-w.com)
To: jkreft@drutex.com.pl | Date: 25.02.2025 08:42
Type: Answer | 
RE: [AW-221501] Fwd: Fwd: (2)
Hej ma być 2 czy 1?
Serdecznie pozdrawiam
Patryk Muszkiet
###EOM##

Phone:  +48 61 438 47 44
Mobile:  +4964196620-0
Email: support.cantor.pl@a-w.com
A+W Software Polska Sp. z o. o.
ul. Sikorskiego 44
62-300 Września
Polska

www.a-w.com

Geschäftsführer/Managing Directors: Peter Dixen, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus in Ihr System gelangen, haften wir nicht für die evtl. entstandenen Schäden.

This e-mail is for the intended…
```

</details>

---

### [AW-220659] — iQuote błąd

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-220659]` |
| **Status** | 🔵 In Progress |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 21.02.2025 15:49 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet
To: | Date: 21.02.2025 15:49
Type: State changed | 
RE: [AW-220659] iQuote błąd (12)
```

</details>

---

### [AW-218890] — URGENT - zatrzymana integracja - zawieszony SpMan

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-218890]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 03.02.2025 12:22 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Radoslaw Jaruszewski
To: | Date: 03.02.2025 12:22
Type: State changed | 
RE: [AW-218890] URGENT - zatrzymana integracja - zawieszony SpMan (7)
Problem pokazany na sesji, po kilku nieudanych próbach sysman z kolejką 2039 zaczął działać poprawnie, brak konkluzji, brak materiału do analizy.
Czekamy na ponowne wystapienie problemu.
```

</details>

---

### [AW-217641] — 64 bit CANTOR version

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-217641]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support Poland - Cantor |
| **Last Action** | 23.01.2025 14:53 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Patryk Muszkiet
To: | Date: 23.01.2025 14:53
Type: State changed | 
RE: [AW-217641] 64 bit CANTOR version (6)
waiting for 64-bit to be available
```

</details>

---

## Support US - Cantor

### [AW-238209] — Variable Descriptions for KundeFld.Bereich...

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-238209]` |
| **Status** | 🟡 New |
| **Category** | Support Cantor / Support US - Cantor |
| **Last Action** | 25.07.2025 18:04 |

**Description:**

> Variable Descriptions for KundeFld.Bereich... (2) Hello Support, I need the variable list and variable descriptions for KundeFld.Bereich: Please also update the Cantor data dictionary with this information. Thanks, - Mike T.

<details>
<summary>View Full Conversation Thread</summary>

```
From: Mike Tetzlaff (Mike.Tetzlaff@a-w.com)
To: support.cantor.us@a-w.com | Date: 25.07.2025 18:04
Type: Request | 
Variable Descriptions for KundeFld.Bereich... (2)
Hello Support,
 
I need the variable list and variable descriptions for KundeFld.Bereich:
 

 
Please also update the Cantor data dictionary with this information.
 
Thanks,
 
- Mike T.
```

</details>

---

### [AW-237923] — Cantor 7.9: Error message when changing supplier in material management

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-237923]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support US - Cantor |
| **Last Action** | 25.07.2025 14:56 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Darius Porumb
To: Darius Porumb | Date: 25.07.2025 14:56
Type: State changed | 
RE: [AW-237923] Cantor 7.9: Error message when changing supplier in material management (6)
Need to talk with PS team. Sites master data missing.
```

</details>

---

### [AW-238070] — Cantor _ System Variable _ Define "... Boundary Edge"

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-238070]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support US - Cantor |
| **Last Action** | 25.07.2025 10:58 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Darius Porumb
To: Darius Porumb | Date: 25.07.2025 10:58
Type: State changed | 
Cantor _ System Variable _ Define "... Boundary Edge" (3)
Darius Porumb has taken the ticket
```

</details>

---

### [AW-237920] — Value Windows | Report Definition - Mat. Mgmt /Purchasing

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-237920]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support US - Cantor |
| **Last Action** | 25.07.2025 10:53 |

**Description:**

> Re: [AW-237920] Value Windows | Report Definition - Mat. Mgmt /Purchasing (9) Good morning, Please see attached. Also I add one more that I found out. Thank you, Mit freundlichen Grüßen | Best regards Darius Porumb ###EOM## Phone:  +49 641 96620 393 A+W Software GmbH Siemensstraße 3 35463 Fernwald Germany www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan Amtsgericht Gießen/Gießen Local Court: HRB 7963 Diese E-Mail ist ausschl...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Darius Porumb (support.cantor.us@a-w.com)
To: christyw@valuewds.com, it@valuewds.com | Date: 25.07.2025 10:53
Type: Answer | 
Re: [AW-237920] Value Windows | Report Definition - Mat. Mgmt /Purchasing (9)
Good morning,
Please see attached. Also I add one more that I found out.
Thank you,
Mit freundlichen Grüßen | Best regards
Darius Porumb
###EOM##

Phone:  +49 641 96620 393
 
A+W Software GmbH
Siemensstraße 3
35463 Fernwald
Germany

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus in Ihr System gelangen, haften wir nicht für die evtl. entstandenen Schäden.

This e-mail is for …
```

</details>

---

### [AW-237882] — Regarding 4012 API credentials not working.

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-237882]` |
| **Status** | 🔵 In Progress |
| **Category** | Support Cantor / Support US - Cantor |
| **Last Action** | 24.07.2025 14:05 |

**Description:**

> [AW-237882] FW: Regarding 4012 API credentials not working. (23) From: Daniel D Connors <daniel.connors@cornerstone-bb.com> Sent: Wednesday, July 23, 2025 7:45 PM To: Joe M Noel <Joe.Noel@cornerstone-bb.com>; Renaud Schmitt <Renaud.Schmitt@cornerstone-bb.com>; Michael Prestera <michael.prestera@cornerstone-bb.com>; Renaud Schmitt <Renaud.Schmitt2@cornerstone-bb.com>; Diego Garcia <Diego.Garcia2@cornerstone-bb.com>; Tim K Adams <Tim.Adams@cornerstone-bb.com> Cc: Roxanne Johnston <Roxanne.Johnston...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Loren Powell (Loren.Powell@a-w.com)
To: support.cantor.us@a-w.com | Date: 24.07.2025 14:05
Type: Request | 
[AW-237882] FW: Regarding 4012 API credentials not working. (23)
From: Daniel D Connors <daniel.connors@cornerstone-bb.com>
Sent: Wednesday, July 23, 2025 7:45 PM
To: Joe M Noel <Joe.Noel@cornerstone-bb.com>; Renaud Schmitt <Renaud.Schmitt@cornerstone-bb.com>; Michael Prestera <michael.prestera@cornerstone-bb.com>; Renaud Schmitt <Renaud.Schmitt2@cornerstone-bb.com>; Diego Garcia <Diego.Garcia2@cornerstone-bb.com>; Tim K Adams <Tim.Adams@cornerstone-bb.com>
Cc: Roxanne Johnston <Roxanne.Johnston@cornerstone-bb.com>; Luis E Gamboa <Luis.Gamboa@cornerstone-bb.com>
Subject: RE: Regarding 4012 API credentials not working.

 
All files successfully processed in PRD!

 
Thank you,
 
Daniel Connors | Integration Support Lead | CBB – Aperture Solutions
Cell: 219-309-0890 | Daniel.Connors@cornerstone-bb.com
 

 
From: Daniel D Connors
Sent: Wednesday, July 23, 2025 8:34 PM
To: Joe M Noel <Joe.Noel@cornerstone-bb.com>; Renaud Schmitt <Renaud.Schmitt@cornerstone-bb.com>; Michael Prestera <michael.prestera@cornerstone-bb.com>; Renaud Schmitt…
```

</details>

---

### [AW-237749] — Changed system label variable length

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-237749]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support US - Cantor |
| **Last Action** | 23.07.2025 08:29 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Darius Porumb
To: Mike Tetzlaff | Date: 23.07.2025 08:29
Type: State changed | 
RE: [AW-237749] Changed system label variable length (3)
set for today 23.07
General North American Support Meeting
```

</details>

---

### [AW-228945] — USWG | Add Evaluation Started/Running Indicator...

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-228945]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support US - Cantor |
| **Last Action** | 22.07.2025 14:24 |

**Description:**

> Automatic reply: [AW-228945] USWG | Add Evaluation Started/Running Indicator... (40) I am currently traveling. My responses will be delayed. 609 374 4066

<details>
<summary>View Full Conversation Thread</summary>

```
From: Joe Noel (Joe.Noel@cornerstone-bb.com)
To: support.cantor.us@a-w.com | Date: 22.07.2025 14:24
Type: Request | 
Automatic reply: [AW-228945] USWG | Add Evaluation Started/Running Indicator... (40)
I am currently traveling. My responses will be delayed.
609 374 4066
```

</details>

---

### [AW-237300] — USWG Spooler not updating Barcode to Status E

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-237300]` |
| **Status** | 🔵 In Progress |
| **Category** | Support Cantor / Support US - Cantor |
| **Last Action** | 22.07.2025 13:46 |

**Description:**

> RE: [AW-237300] USWG Spooler not updating Barcode to Status E (10) Good Day Darius! To my knowledge, Renaud resolved this yesterday. We can discuss in the MES Workshop today to confirm that it can be closed. Best regards Loren Powell Director Professional Services Global Business Unit A+W Cantor ###EOM### Phone: +1 502.754.0862 Mobile: +1 502.706.1008 Email: loren.powell@a-w.com A+W Software USA Inc. C/O Vela US Holdco Inc 8770 West Bryn Mawr Ave, Suite 1300 Chicago Illinois 60631 USA www.a-w.co...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Loren Powell (Loren.Powell@a-w.com)
To: support.cantor.us@a-w.com | Date: 22.07.2025 13:46
Type: Request | 
RE: [AW-237300] USWG Spooler not updating Barcode to Status E (10)
Good Day Darius! To my knowledge, Renaud resolved this yesterday. We can discuss in the MES Workshop today to confirm that it can be closed.
 
Best regards
 
Loren Powell
Director Professional Services Global
Business Unit A+W Cantor
###EOM###

Phone: +1 502.754.0862
Mobile: +1 502.706.1008 
Email: loren.powell@a-w.com
 
A+W Software USA Inc.
C/O Vela US Holdco Inc
8770 West Bryn Mawr Ave, Suite 1300 
Chicago Illinois 60631
USA
 
www.a-w.com

 

 
From: support.cantor.us <support.cantor.us@a-w.com>
Sent: Tuesday, July 22, 2025 2:19 AM
To: Powell, Loren <Loren.Powell@a-w.com>
Cc: Brown, Cynthia <Cynthia.Brown@a-w.com>
Subject: RE: [AW-237300] USWG Spooler not updating Barcode to Status E

 
Good morning Loren,
Is this still open? I don't have visibility.
Last status for them:

Can I help somehow or we should close the ticket?
Thank you,
Mit freundlichen Grüßen | Best regards
Darius Porumb
###EOM##
​
Phone:  +49 641 96620 393
 
A+W Software…
```

</details>

---

### [AW-234059] — North Star | Profile Technology Glazing bead adjustment not working as expected

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-234059]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support US - Cantor |
| **Last Action** | 22.07.2025 11:16 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Sascha Hermann
To: Ann Cypressi | Date: 22.07.2025 11:16
Type: State changed | 
RE: [AW-234059] North Star | Profile Technology Glazing bead adjustment not working as expected (20)
AC
```

</details>

---

### [AW-236287] — Job creation error

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-236287]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support US - Cantor |
| **Last Action** | 21.07.2025 10:49 |

**Description:**

> Automatic reply: [AW-236287] Ticket confirmation / Job creation error (9) ﻿ ﻿Hello, I am out of office, returning Aug 5. For immediate assistance please contact itservices.nst@cornerstone-bb.com Thanks! Steve Lock

<details>
<summary>View Full Conversation Thread</summary>

```
From: Steve Lock (Steve.Lock@cornerstone-bb.com)
To: support.cantor.us@a-w.com | Date: 21.07.2025 10:49
Type: Request | 
Automatic reply: [AW-236287] Ticket confirmation / Job creation error (9)
﻿

﻿Hello,

I am out of office, returning Aug 5.

For immediate assistance please contact itservices.nst@cornerstone-bb.com

Thanks!

Steve Lock
```

</details>

---

### [AW-231056] — USWG | Pick Ticket Report

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-231056]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support US - Cantor |
| **Last Action** | 18.07.2025 16:51 |

**Description:**

> RE: [AW-231056] USWG | Pick Ticket Report (24) Hello Joe, I was about to send this to R&D when I realized that I sent you the wrong DR.  The correct DR is attached.  I am so sorry for the confusion.  The attached is just to add a few fields to the Order Confirmation.  Please look over and respond back to all Approved if it is approved. Again, my apologies for sending the wrong one. Mit freundlichen Grüßen | Best regards Ann Cypressi ###EOM## ​ Phone:  +49 641 96620 393 A+W Software GmbH Siemenss...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Ann Cypressi (support.cantor.us@a-w.com)
To: joe.noel@cornerstone-bb.com | Date: 18.07.2025 16:51
Type: Answer | 
RE: [AW-231056] USWG | Pick Ticket Report (24)
Hello Joe,
I was about to send this to R&D when I realized that I sent you the wrong DR.  The correct DR is attached.  I am so sorry for the confusion.  The attached is just to add a few fields to the Order Confirmation.  Please look over and respond back to all Approved if it is approved.
Again, my apologies for sending the wrong one.
Mit freundlichen Grüßen | Best regards
Ann Cypressi
###EOM##
​
Phone:  +49 641 96620 393
 
A+W Software GmbH
Siemensstraße 3
35463 Fernwald
Germany

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Wei…
```

</details>

---

### [AW-234347] — FW: PO emailing process - next step - how to include EDI data in the email?

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-234347]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support US - Cantor |
| **Last Action** | 17.07.2025 19:52 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Sachin Bhangale
To: Sachin Bhangale | Date: 17.07.2025 19:52
Type: State changed | 
RE: [AW-234347] FW: PO emailing process - next step - how to include EDI data in the email? (14)
Alan is testing the solution.
```

</details>

---

### [AW-236001] — Value Window | iQuote installation

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-236001]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support US - Cantor |
| **Last Action** | 16.07.2025 14:50 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Darius Porumb
To: Lukasz Lieske | Date: 16.07.2025 14:50
Type: State changed | 
RE: [AW-236001] Value Window | iQuote installation (7)
Waiting for more details on customer side.
Status change to waiting for customer.
```

</details>

---

### [AW-224866] — ON-CUT AND OFF-CUT ANGLE

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-224866]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support US - Cantor |
| **Last Action** | 14.07.2025 15:48 |

**Description:**

> Re: Re: [AW-224866] ON-CUT AND OFF-CUT ANGLE (20) Hello Kawser, Nice to hear back from you. Can you please help us with an example order? Not sure why is not covering your needs. What should be the goal on this shape? Thank you, Mit freundlichen Grüßen | Best regards Darius Porumb ###EOM## Phone:  +49 641 96620 393 A+W Software GmbH Siemensstraße 3 35463 Fernwald Germany www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan Amtsg...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Darius Porumb (support.cantor.us@a-w.com)
To: kawserH@valuewds.com | Date: 14.07.2025 15:48
Type: Answer | 
Re: Re: [AW-224866] ON-CUT AND OFF-CUT ANGLE (20)
Hello Kawser,
Nice to hear back from you. Can you please help us with an example order? Not sure why is not covering your needs.
What should be the goal on this shape?
Thank you,
Mit freundlichen Grüßen | Best regards
Darius Porumb
###EOM##

Phone:  +49 641 96620 393
 
A+W Software GmbH
Siemensstraße 3
35463 Fernwald
Germany

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus in …
```

</details>

---

### [AW-235423] — PREMIUM | Picking List Printing Failure at CIM Station 9970

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-235423]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support US - Cantor |
| **Last Action** | 14.07.2025 07:43 |

**Description:**

> Re: [AW-235423] PREMIUM | Picking List Printing Failure at CIM Station 9970 (19) Good morning Claudio, Yes please, all the details to reproduce it. Mit freundlichen Grüßen | Best regards Darius Porumb ###EOM## Phone:  +49 641 96620 393 A+W Software GmbH Siemensstraße 3 35463 Fernwald Germany www.a-w.com Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan Amtsgericht Gießen/Gießen Local Court: HRB 7963 Diese E-Mail ist ausschließlich für de...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Darius Porumb (support.cantor.us@a-w.com)
To: claudio@premiumwindows.com | Date: 14.07.2025 07:43
Type: Answer | 
Re: [AW-235423] PREMIUM | Picking List Printing Failure at CIM Station 9970 (19)
Good morning Claudio,
Yes please, all the details to reproduce it.
Mit freundlichen Grüßen | Best regards
Darius Porumb
###EOM##

Phone:  +49 641 96620 393
 
A+W Software GmbH
Siemensstraße 3
35463 Fernwald
Germany

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zusendung dieser E-Mail trotzdem ein Virus in Ihr System gelangen, haften wir nicht für die evtl. entstandenen Schäden.

This e-mail is for the intended recip…
```

</details>

---

### [AW-226802] — VPI | Glazing Insert Codes _ Valid Exchange Glass Combinations for Insert Codes

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-226802]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support US - Cantor |
| **Last Action** | 09.07.2025 15:09 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Ann Cypressi
To: Ann Cypressi | Date: 09.07.2025 15:09
Type: State changed | 
RE: [AW-226802] VPI | Glazing Insert Codes _ Valid Exchange Glass Combinations for Insert Codes (19)
Discussed with the team and I am setting up a simple example in my demo to be able to get generic screen shots to send to Duran with some explanation.  AC
```

</details>

---

### [AW-229383] — USWG Paris Assessment | Make Cantor not allow Orders with a Qty of Zero

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-229383]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support US - Cantor |
| **Last Action** | 08.07.2025 17:03 |

**Description:**

> [AW-229383] USWG Paris Assessment | Make Cantor not allow Orders with a Qty of Zero (23) Hello, This bug has been fixed and was available in the 06/25/2025 dlls, and is of course available in the newest dlls from 07/07/2025.  This will need to be testing using your standard procedures for importing via AccuQuote.  Please let us know your feedback. Kind Regards, Ann Cypressi Support and Implementation Consultant A+W Cantor USA Email: ann.cypressi@a-w.com A+W Software USA Inc. C/O Vela US Holdco I...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Ann Cypressi (Ann.Cypressi@a-w.com)
To: genesisreleasenotice@cornerstone-bb.com | Date: 08.07.2025 17:03
Type: Request | 
[AW-229383] USWG Paris Assessment | Make Cantor not allow Orders with a Qty of Zero (23)
Hello,
This bug has been fixed and was available in the 06/25/2025 dlls, and is of course available in the newest dlls from 07/07/2025.  This will need to be testing using your standard procedures for importing via AccuQuote.  Please let us know your feedback.

 
Kind Regards,
 
Ann Cypressi
Support and Implementation Consultant
A+W Cantor USA
 

Email: ann.cypressi@a-w.com
 
A+W Software USA Inc.
C/O Vela US Holdco Inc
8770 West Bryn Mawr Ave, Suite 1300 
Chicago Illinois 60631
USA
 
www.a-w.com

 
Cantor Support Inbox: support.cantor.us@a-w.com
```

</details>

---

### [AW-229382] — USWG Paris Assessment | Order Overview/Back Order Overview Column for Order Note Flag

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-229382]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support US - Cantor |
| **Last Action** | 07.07.2025 20:12 |

**Description:**

> RE: [AW-229382] USWG Paris Assessment | Order Overview/Back Order Overview Column for Order Note Flag (16) Hello Tim, This view is now set up and available in the Stage environment.  In order to see it, from the Home page, go into Order/Quotation Overview.  Right click anywhere on the overview to bring up the User settings menu.  Choose Columns, and scroll to the very bottom to find 'Text'. Double click it to move it into the Columns to Show section, and use the up/down arrows to place it where ...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Ann Cypressi (support.cantor.us@a-w.com)
To: Tim.Adams@cornerstone-bb.com | Date: 07.07.2025 20:12
Type: Answer | 
RE: [AW-229382] USWG Paris Assessment | Order Overview/Back Order Overview Column for Order Note Flag (16)
Hello Tim,
This view is now set up and available in the Stage environment.  In order to see it, from the Home page, go into Order/Quotation Overview.  Right click anywhere on the overview to bring up the User settings menu.  Choose Columns, and scroll to the very bottom to find 'Text'.  

Double click it to move it into the Columns to Show section, and use the up/down arrows to place it where you would like that column to appear.  Click Ok to save that configuration.  You can now see in the first Column if an order contains any type of text notes.

Please copy this view to PROD and let me know if you have any questions.
Thank you!
Mit freundlichen Grüßen | Best regards
Ann Cypressi
###EOM##
​
Phone:  +49 641 96620 393
 
A+W Software GmbH
Siemensstraße 3
35463 Fernwald
Germany

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail is…
```

</details>

---

### [AW-228661] — USWG | Automate sending of Cantor reports

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-228661]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support US - Cantor |
| **Last Action** | 03.07.2025 20:57 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Cynthia Brown
To: Curtis Gabriel | Date: 03.07.2025 20:57
Type: State changed | 
RE: [AW-228661] USWG | Automate sending of Cantor reports (20)
Curtis - This is still needed. Please reach out to Joe Noel with your questions. Thank you!
```

</details>

---

### [AW-233567] — Can we change job status from E to another (e.g. U)

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-233567]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support US - Cantor |
| **Last Action** | 23.06.2025 15:31 |

**Description:**

> RE: [AW-233567] Can we change job status from E to another (e.g. U) (6) Hello Edvin, It is technically possible to change the status in Cantor but the status E triggers some integrations to other 3rd party software such as JDE or BLUE YONDER so you have to be carefull with changing the status. Mit freundlichen Grüßen | Best regards Lukasz Lieske ###EOM## Phone:  +49 641 96620 393 A+W Software GmbH Siemensstraße 3 35463 Fernwald Germany www.a-w.com Geschäftsführer/Managing Directors: Eric Herrman...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Lukasz Lieske (support.cantor.us@a-w.com)
To: edvin.eshagh@cornerstone-bb.com | Date: 23.06.2025 15:31
Type: Answer | 
RE: [AW-233567] Can we change job status from E to another (e.g. U) (6)
Hello Edvin,
It is technically possible to change the status in Cantor but the status E triggers some integrations to other 3rd party software such as JDE or BLUE YONDER so you have to be carefull with changing the status.
Mit freundlichen Grüßen | Best regards
Lukasz Lieske
###EOM##

Phone:  +49 641 96620 393
 
A+W Software GmbH
Siemensstraße 3
35463 Fernwald
Germany

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme. Sollte durch Zuse…
```

</details>

---

### [AW-227452] — Pick list

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-227452]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support US - Cantor |
| **Last Action** | 23.06.2025 10:58 |

**Description:**

> Re: [AW-227452] Pick list (23) Hello Claudio, I hope this week starts as well as possible for you. As I mentioned last week, your request was sent to R&D. An analysis was performed. Please read the response below and help us with a complex example that covers your cases. "When we are talking about grid and glass type. This can be difficult. For example if the grid is a macro or different grid pictures in different glass field. Similar with the glass type, if you have multiple fields or mulled un...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Darius Porumb (ps.cantor.us@a-w.com)
To: claudio@premiumwindows.com | Date: 23.06.2025 10:58
Type: Answer | 
Re: [AW-227452] Pick list (23)
Hello Claudio,
I hope this week starts as well as possible for you. As I mentioned last week, your request was sent to R&D. An analysis was performed. Please read the response below and help us with a complex example that covers your cases.
"When we are talking about grid and glass type. This can be difficult. For example if the grid is a macro or different grid pictures in different glass field. Similar with the glass type, if you have multiple fields or mulled units.
Please create some complex units and work out example.
That we can understand, what the customer required in cases with multiple fields and different grids."
Thank you,
Mit freundlichen Grüßen | Best regards
Darius Porumb
###EOM##

Phone:  +49 641 96620 393
 
A+W Software GmbH
Siemensstraße 3
35463 Fernwald
Germany

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail…
```

</details>

---

### [AW-231859] — PRODUKTTYP 5202 AND ARTIKEL="ASPW" 45° miter cut at BOTTOM

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-231859]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support US - Cantor |
| **Last Action** | 19.06.2025 14:33 |

**Description:**

> Re: [AW-231859] PRODUKTTYP 5202 AND ARTIKEL="ASPW" 45° miter cut at BOTTOM (6) Hello Kawser, I apologize for the delayed response, but we have finally identified the issue affecting our second position. Please refer to the screenshots for further information. Your profile record is A102C Using Corner Exchange - rule no 1 Corner Exchange And here you can see under type 1 -> Seq 4 -> Additional Condition in the bottom part. To test I comment the condition and add 1=0 to have a failure in condition...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Darius Porumb (support.cantor.us@a-w.com)
To: kawserH@valuewds.com | Date: 19.06.2025 14:33
Type: Answer | 
Re: [AW-231859] PRODUKTTYP 5202 AND ARTIKEL="ASPW" 45° miter cut at BOTTOM (6)
Hello Kawser,
 
I apologize for the delayed response, but we have finally identified the issue affecting our second position. Please refer to the screenshots for further information.
Your profile record is A102C
Using Corner Exchange - rule no 1

 
Corner Exchange
And here you can see under type 1 -> Seq 4 -> Additional Condition in the bottom part.

 
To test I comment the condition and add 1=0 to have a failure in condition
 

 
And with this you can see that the condition is not true so we will not have any corner exchange.
 

 
Now my question is, why you create this condition? I'm sure that you are using somewhere this, so maybe we can go further and to expend the condition.
 
Thank you,
Mit freundlichen Grüßen | Best regards
Darius Porumb
###EOM##

Phone:  +49 641 96620 393
 
A+W Software GmbH
Siemensstraße 3
35463 Fernwald
Germany

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, T…
```

</details>

---

### [AW-230143] — XML Export – Item Description Inclusion for NetSuite Integration

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-230143]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support US - Cantor |
| **Last Action** | 12.06.2025 15:00 |

**Description:**

> Re: [AW-230143] XML Export – Item Description Inclusion for NetSuite Integration (28) Hi Claudio, ItemNo would just give you the number of the item. Since there is no reference to the item description in this XML file I will speak today with my colleagues from support to check if it's possible to export the item description too. Mit freundlichen Grüßen | Best regards Lukasz Lieske ###EOM## Phone:  +49 641 96620 393 A+W Software GmbH Siemensstraße 3 35463 Fernwald Germany www.a-w.com Geschäftsfüh...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Lukasz Lieske (support.cantor.us@a-w.com)
To: claudio@premiumwindows.com, claudio@qos-net.com | Date: 12.06.2025 15:00
Type: Answer | 
Re: [AW-230143] XML Export – Item Description Inclusion for NetSuite Integration (28)
Hi Claudio,
 
ItemNo would just give you the number of the item. Since there is no reference to the item description in this XML file I will speak today with my colleagues from support to check if it's possible to export the item description too.
 
Mit freundlichen Grüßen | Best regards
Lukasz Lieske
###EOM##

Phone:  +49 641 96620 393
 
A+W Software GmbH
Siemensstraße 3
35463 Fernwald
Germany

www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutz…
```

</details>

---

### [AW-229372] — USWG Paris Assessment | Soft Warning for Other  users when Scheduling is occuring

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-229372]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support US - Cantor |
| **Last Action** | 03.06.2025 14:54 |

<details>
<summary>View Full Conversation Thread</summary>

```
From: Ann Cypressi
To: Ann Cypressi | Date: 03.06.2025 14:54
Type: State changed | 
RE: [AW-229372] USWG | Soft Warning for Other  users when Scheduling is occuring (11)
I provided 2 options for solution to the USWG, and I waiting to hear back on which way they would like to try.  Both ways will require testing on their part, or we could offer to test for them - they would need to provide us with very detailed information about user rights and specific scenarios, and we can test it in their Stage system.  AC
```

</details>

---

### [AW-231306] — Angle Rotation for left and right profile from 45 to 90 and 90 to 45

| Field | Value |
|-------|-------|
| **Ticket ID** | `[AW-231306]` |
| **Status** | ⚪ Unknown |
| **Category** | Support Cantor / Support US - Cantor |
| **Last Action** | 03.06.2025 13:27 |

**Description:**

> Re: [AW-231306] Angle Rotation for left and right profile from 45 to 90 and 90 to 45 (8) Good morning, A new profiles will not change angles. Any changes to the interface may be generated by R&D. We cannot work inside the database - profiles. At the same time, I studied the interface documentation and found the following section there: Are there any special machinings for units that open outwards (e.g. angles that are exchanged)? How are units that open outwards recognized (flag at hardware vari...

<details>
<summary>View Full Conversation Thread</summary>

```
From: Darius Porumb (support.cantor.us@a-w.com)
To: kawserH@valuewds.com | Date: 03.06.2025 13:27
Type: Answer | 
Re: [AW-231306] Angle Rotation for left and right profile from 45 to 90 and 90 to 45 (8)
Good morning,
 
A new profiles will not change angles.
Any changes to the interface may be generated by R&D. We cannot work inside the database - profiles.
 
At the same time, I studied the interface documentation and found the following section there:
 
Are there any special machinings for units that open outwards (e.g. angles that are exchanged)? How are units that open outwards recognized (flag at hardware variant or via sash profiles)?
Angle exchange

 
Therefore, according to this description, the angles should be changed according to certain parameters.
 
My question now would be, what are the rules for change? For all profiles, depending on whether there is external opening?
Or only for certain profiles?
Does anything change depending on the existence of a threshold?
(These are cases known from our customers)
Please specify the specific cases.
At the same time, I would like you to place an order for two units. One in which this change occurs and one in whi…
```

</details>

---

