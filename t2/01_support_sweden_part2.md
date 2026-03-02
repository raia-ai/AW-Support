# 01\_support\_sweden\_part2

**Category:** Support Clarity / Support Sweden | **Tickets:** 165 | **Part 2 of 3**

***

### \[AW-233935]

**Subject:** Regarding the manual decoating\
**Status:** Unknown | **Category:** Support Clarity / Support Sweden | **Last Action:** 30.06.2025 16:11

RE: Regarding the manual decoating \[AW-233935] (7) Hello Linas, The problem is that the Manual Decoating is still included in the calculation of the total edge decoating. The cutting driver will use the value in pool\_entschichtung for decoating. This is controlled via the product class in AWB master data. I think you have a few alternatives here. Two standard options, and one custom. It is possible for you to change the product class to 420 - Decoating. This will let you add it on the tempered ...

<details>

<summary>Full conversation</summary>

```
From: Adam Grimberg (support.se@a-w.com)
To: support@stronglasas.lt, adam.grimberg@a-w.com | Date: 30.06.2025 16:11
Type: Answer | 
RE: Regarding the manual decoating [AW-233935] (7)
Hello Linas, 
The problem is that the Manual Decoating is still included in the calculation of the total edge decoating. The cutting driver will use the value in pool_entschichtung for decoating.  This is controlled via the product class in AWB master data. 
I think you have a few alternatives here. Two standard options, and one custom.  
It is possible for you to change the product class to 420 - Decoating. This will let you add it on the tempered glass and would not transfer to the cutting code. But, it means that the input parameters for sales would be different, see picture 1 below. 
The second option is to disable BOM Breakdown on the tempered Master data (BOM tab) article, for edge stripping product class. See second picture below.  Then you put the automatic decoating on the cut glass, and manual decoating on tempered glass in the BOM. Your order entry persons will need to take care where in the BOM, each decoating is entered. 
Third option is that I investigate if I can c…
```

</details>

***

### \[AW-235228]

**Subject:** Sekurit support\
**Status:** New | **Category:** Support Clarity / Support Sweden | **Last Action:** 30.06.2025 15:16

Sekurit support (2) You don't often get email from Learn why this is important[https://aka.ms/LearnAboutSenderIdentification](https://aka.ms/LearnAboutSenderIdentification) Hej Vi har installerat A-W på två nya datorer med Win11 och har stött på lite problem. Allt verkar funka till vi ska skicka koden till maskinen då kommer detta upp: Tacksam för support. Mvh/Best regards Mattias Lundgren IT Responsible SAINT-GOBAIN SEKURIT SCANDINAVIA AB Bruksgatan 18 241 38 Eslöv \* Sweden Tel: +46 (0) 413 64 390 E-mail:m...

<details>

<summary>Full conversation</summary>

```
From: Lundgren, Mattias - SG Sekurit AB (Mattias.Lundgren@saint-gobain.com)
To: support.se@a-w.com | Date: 30.06.2025 15:16
Type: Request | 
Sekurit support (2)
You don't often get email from mattias.lundgren@saint-gobain.com. Learn why this is important<https://aka.ms/LearnAboutSenderIdentification>
Hej
Vi har installerat A-W på två nya datorer med Win11 och har stött på lite problem.
Allt verkar funka till vi ska skicka koden till maskinen då kommer detta upp:

Tacksam för support.

Mvh/Best regards

Mattias Lundgren
IT Responsible

SAINT-GOBAIN SEKURIT SCANDINAVIA AB
Bruksgatan 18
241 38 Eslöv * Sweden
Tel: +46 (0) 413 64 390
E-mail:mattias.lundgren@saint-gobain.com
www.saint-gobain sekurit.com<https://urldefense.com/v3/__http:/www.saint-gobain-sekurit.com/sekurit-experience__;!!Mj5yV84exmbMMB4!r_Tq-KpQLbbJclHasyT4CmPkVNKxGvoWM76MfcmrYrqdE0Mu7hXtgTitVjLMKbX9GUH3xv45bTUXQ5oMZuwkjPj1tAehO-k4$>
```

</details>

***

### \[AW-220345]

**Subject:** Rack location tracking\
**Status:** In Progress | **Category:** Support Clarity / Support Sweden | **Last Action:** 27.06.2025 17:26

<details>

<summary>Full conversation</summary>

```
From: Jens Thorsen
To: Jens Thorsen | Date: 27.06.2025 17:26
Type: State changed | 
Rack location tracking (13)
```

</details>

***

### \[AW-225844]

**Subject:** Questions regarding racks\
**Status:** In Progress | **Category:** Support Clarity / Support Sweden | **Last Action:** 27.06.2025 17:22

<details>

<summary>Full conversation</summary>

```
From: Jens Thorsen
To: Adam Grimberg | Date: 27.06.2025 17:22
Type: State changed | 
Questions regarding racks (8)
```

</details>

***

### \[AW-225387]

**Subject:** Capacity planning and Fomula workshop\
**Status:** In Progress | **Category:** Support Clarity / Support Sweden | **Last Action:** 27.06.2025 14:14

RE: \[AW-225387] Capacity planning (6) Hello To me there are 2 thigs \* Planning (I mean moving orders between dates) actual examples - so It really works in our Production, and we know how to use it and what makes it to crash. +Where in TTV-s we can actually see the result of this planning. \* Formulas for allow-d times \* There are multiple things \* The end goal is that we can use it freely by ourselves - without calling you every time we want to change something \* Main formulas that we ...

<details>

<summary>Full conversation</summary>

```
From: Andres Parts (Andres.Parts@glassense.com)
To: support.se@a-w.com | Date: 27.06.2025 14:14
Type: Request | 
RE: [AW-225387] Capacity planning (6)
Hello

To me there are 2 thigs

 *   Planning (I mean moving orders between dates) actual examples - so It really works in our Production, and we know how to use it and what makes it to crash. +Where in TTV-s we can actually see the result of this planning.
 *   Formulas for allow-d times
    *   There are multiple things
    *   The end goal is that we can use it freely by ourselves - without calling you every time we want to change something
       *   Main formulas that we are missing - that has the greatest impact Plan vs reality
          *   Are deletion with 10, 20, 30, 40, 50, 60, 80, 90, over 100
             *   To be able to use it in cutting allowed times formulas
          *   TPF and Eazy Pro (sun protective glass Temperable) - in combination with wide area delition  - one lite can take up to 1 hour.
          *   Max side, number of layers, thickness
             *   To be used in Lamination formulas
          *   Sealing depth + U - profiles ty…
```

</details>

***

### \[AW-234579]

**Subject:** Rack scanned in production added to the order in business\
**Status:** In Progress | **Category:** Support Clarity / Support Sweden | **Last Action:** 27.06.2025 14:11

SV: \[AW-234579] Rack scanned in production added to the order in business (4) Hi Henrik, Yes – Order 1372102 – According to business it’s a wooden frame (article 4755), but it is packed and scanned in production on a steel frame (article 4721) The order is due to be delivered Monday, so it has not yet been invoiced. Let me know if You need anything else 😊 Venlig hilsen / Regards / Grüssen Peter Rostrup Hebo Regnskabschef M: +45 28 97 85 49 E: W: www.glaseksperten.dk Fra: Sup...

<details>

<summary>Full conversation</summary>

```
From: Peter Rostrup Hebo (prh@glaseksperten.dk)
To: support.se@a-w.com | Date: 27.06.2025 14:11
Type: Request | 
SV: [AW-234579] Rack scanned in production added to the order in business (4)
Hi Henrik,

Yes – Order 1372102 – According to business it’s a wooden frame (article 4755), but it is packed and scanned in production on a steel frame (article 4721)

The order is due to be delivered Monday, so it has not yet been invoiced.

Let me know if You need anything else 😊

Venlig hilsen / Regards / Grüssen
Peter Rostrup Hebo
Regnskabschef

M: +45 28 97 85 49
E: prh@glaseksperten.dk
W: www.glaseksperten.dk

Fra: Support Mailbox Sweden <support.se@a-w.com>
Sendt: 24. juni 2025 16:25
Til: Peter Rostrup Hebo <prh@glaseksperten.dk>
Emne: RE: [AW-234579] Rack scanned in production added to the order in business

CAUTION: External Sender. Please do not click on links or open attachments from senders you do not trust.

Hi Peter,

Do you have an example here that I can use to check the data? A real order that is already invoiced would be OK, I just want to compare the data in AWP to AWB. I have a good idea already as to …
```

</details>

***

### \[AW-221054]

**Subject:** Purchase lables are printed 2 times...\
**Status:** In Progress | **Category:** Support Clarity / Support Sweden | **Last Action:** 27.06.2025 08:00

RE: \[AW-221054] Purchase lables are printed 2 times... (4) Hello, I released one batch and there I got also double labels. Order 155662-1 Batch 9205 Our Tartu plant send 4 pcs of glass to Kolu plant. Order entry inserted new order for this and changed this procurement type to – customer owned glass. Maybe we do something wrong, but I don’t have any other idea how we should produce this kind of orders. We get labels from both boxes: Cutting labels and Purchase labels. Please take a look what sh...

<details>

<summary>Full conversation</summary>

```
From: Rain Aava (Rain.Aava@glassense.com)
To: support.se@a-w.com, Andres.Parts@glassense.com | Date: 27.06.2025 08:00
Type: Request | 
RE: [AW-221054] Purchase lables are printed 2 times... (4)
Hello,

I released one batch and there I got also double labels.
Order 155662-1   Batch 9205
Our Tartu plant send 4 pcs of glass to Kolu plant.
Order entry inserted new order for this and changed this procurement type to – customer owned glass.

Maybe we do something wrong, but I don’t have any other idea how we should produce this kind of orders.

We get labels from both boxes:
Cutting labels and Purchase labels.

Please take a look what should we do differently next time.

Rain Aava
Production planner
+372 5358 6369

Glassense AS
Kose vald Kolu
75121 Estonia

From: Support Mailbox Sweden <support.se@a-w.com>
Sent: Tuesday, June 24, 2025 11:55
To: Andres Parts <Andres.Parts@glassense.com>
Cc: Oleksandr Prutas <Oleksandr.Prutas@glassense.com>; Rain Aava <Rain.Aava@glassense.com>
Subject: RE: [AW-221054] Purchase lables are printed 2 times...
…
```

</details>

***

### \[AW-226321]

**Subject:** MGA AW Rack management.\
**Status:** Unknown | **Category:** Support Clarity / Support Sweden | **Last Action:** 26.06.2025 13:40

<details>

<summary>Full conversation</summary>

```
From: Jens Thorsen
To: Jens Thorsen | Date: 26.06.2025 13:40
Type: State changed | 
MGA AW Rack management. (4)
This will be kept open during the entire process until this is in live production
This was discussed during the meeting
Hur rack ordrar skapas för att fakturera rack
 
Pallvärde behövs fyllas i där artikelnummret skrivs in för att koppla
Packat och lev kommer tillbaka som feedback till Business
 
Kunddata klassifikatorer PallFakt eft X dagar 0 så stängs den av
Finns på alla kunder för att aktivera
Flöde körs varje natt som kan följas i Monitorn under customizings
Boxen Bortappad blir ibockad på Pallar
Produktion och palltyper eller pallar
Om något är fel så kan man bock aur denna så tar flödet om körningen
Filen hamnar under Export EDI
Importera EDI filer via Importera
Dokument order och sedan Importera
Detta fel kommer om inte artikel är inlagd på pallvärde

 
Sedan behöver man skicka en pall faktura precis som vanligt när man skapar en order faktura
Spara och sedan spara igen
 
De vill ha ordernummer kopplat toll pallordern
```

</details>

***

### \[AW-227512]

**Subject:** Vertmax automatic file generation error\
**Status:** In Progress | **Category:** Support Clarity / Support Sweden | **Last Action:** 25.06.2025 19:54

RE: \[AW-227512] Vertmax automatic file generation error (4) Hello Only Vermax is using automatic file generation for CNC. So this is the place to fix it. Andres Parts Development manager +372 50 12 981 Glassense AS Kose vald Kolu 75121 Estonia www.glassense.com[http://www.glassense.com/](http://www.glassense.com/) From: Support Mailbox Sweden Sent: Tuesday, June 24, 2025 4:54 PM To: Andres Parts Cc: Oleksandr Prutas Subject: RE: \[AW-227512]...

<details>

<summary>Full conversation</summary>

```
From: Andres Parts (Andres.Parts@glassense.com)
To: support.se@a-w.com | Date: 25.06.2025 19:54
Type: Request | 
RE: [AW-227512] Vertmax automatic file generation error (4)
Hello

Only Vermax is using automatic file generation for CNC.

So this is the place to fix it.

Andres Parts
Development manager
+372 50 12 981

Glassense AS
Kose vald Kolu
75121 Estonia

www.glassense.com<http://www.glassense.com/>

From: Support Mailbox Sweden <support.se@a-w.com>
Sent: Tuesday, June 24, 2025 4:54 PM
To: Andres Parts <Andres.Parts@glassense.com>
Cc: Oleksandr Prutas <Oleksandr.Prutas@glassense.com>
Subject: RE: [AW-227512] Vertmax automatic file generation error

Do you have this issue somewhere else or is it only on Vertmax?

Do you have a similar that works for Vertmax

Best regards
Jens Thorsen
###EOM##

A+W Support Sweden +46 (0) 35 175 417
A+W Support UK + 44 (0) 560348 8606
A+W Support Poland +48 61 436 63 74

A+W Helpdesk Tool and other ways of contacts
https://www.a-w.com/uk/service/

A+W Software GmbH
Siemensstraße 3
35463 Fernwald
German…
```

</details>

***

### \[AW-233539]

**Subject:** Patching the live system and setting up test\
**Status:** Unknown | **Category:** Support Clarity / Support Sweden | **Last Action:** 25.06.2025 15:16

<details>

<summary>Full conversation</summary>

```
From: Jens Thorsen
To: Jens Thorsen | Date: 25.06.2025 15:16
Type: State changed | 
Patching the live system and setting up test (3)
The Production terminal is starting but it can't load the surfacedialogue
```

</details>

***

### \[AW-233196]

**Subject:** AWB long loading on certain account\
**Status:** In Progress | **Category:** Support Clarity / Support Sweden | **Last Action:** 25.06.2025 07:31

Re: \[AW-233196] AWB long loading on certain account (12) Hi Henrik, Yes, it will by great if you look at this function if it cleans this data automatically. Please give more information about it. Best regards / Pagarbiai Regimantas Graževičius CIO / IT vadovas \[signature\_540931018]+370 620 41450 \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_ From: Support Mailbox Sweden Sent: Tuesday, June 24, 2025 11:05 To: Regimantas Graževičius Lukas Aleksejevas

<details>

<summary>Full conversation</summary>

```
From: Regimantas Graževičius (regimantas@glasslt.com)
To: support.se@a-w.com, lukas@glasslt.com | Date: 25.06.2025 07:31
Type: Request | 
Re: [AW-233196] AWB long loading on certain account (12)
Hi Henrik,

Yes, it will by great if you look at this function if it cleans this data automatically.
Please give more information about it.

Best regards / Pagarbiai

Regimantas Graževičius
CIO / IT vadovas
[signature_540931018]+370 620 41450

________________________________
From: Support Mailbox Sweden <support.se@a-w.com>
Sent: Tuesday, June 24, 2025 11:05
To: Regimantas Graževičius <regimantas@glasslt.com>; Lukas Aleksejevas <lukas@glasslt.com>
Subject: Re: [AW-233196] AWB long loading on certain account

Hi Regimantas,

The table where this data is stored is SYSADM.AD_TERMIN, you can review the database documentation for some details regarding this table. I think we have a function that can be setup manage clean-up of this data if you would like us to have a look at this for you.

Please let me know how you would like us to proceed.

Best regards
Henrik Johansson
###EOM##

A+W Support Sweden +46 (0) 35 175 417
A+W Support UK + 44 …
```

</details>

***

### \[AW-228756]

**Subject:** FW: Erikujud terava tipuga (Kolmanurgad)\
**Status:** In Progress | **Category:** Support Clarity / Support Sweden | **Last Action:** 24.06.2025 15:49

<details>

<summary>Full conversation</summary>

```
From: Jens Thorsen
To: Vladimir Iljin | Date: 24.06.2025 15:49
Type: State changed | 
FW: Erikujud terava tipuga (Kolmanurgad) (4)
```

</details>

***

### \[AW-233039]

**Subject:** SN-fil som visas i PT Intermac\
**Status:** New | **Category:** Support Clarity / Support Sweden | **Last Action:** 23.06.2025 14:47

Sv: \[AW-233039] Ticket confirmation / SN-fil som visas i PT Intermac (3) Hej, Har Ni hittat något svar på detta? \[Logo] Med vänlig hälsning Per-Inge Aleräng Forserum Safety Glass AB Direkt: +46 380 295 26 Sommar 2025 Vi stänger v29-31. Med reducerad bemanning v28 & 32 Från: Support Mailbox Sweden Skickat: den 9 juni 2025 11:11 Till: Intermac 2 Per-Inge Aleräng Ämne: \[AW-233039] Ticket confirmation / SN-fil som visas i PT Inte...

<details>

<summary>Full conversation</summary>

```
From: Per-Inge Aleräng (per-inge.alerang@fsglass.se)
To: support.se@a-w.com, inter@fsglass.se | Date: 23.06.2025 14:47
Type: Request | 
Sv: [AW-233039] Ticket confirmation / SN-fil som visas i PT Intermac (3)
Hej,

Har Ni hittat något svar på detta?

[Logo]
Med vänlig hälsning
Per-Inge Aleräng
Forserum Safety Glass AB
Direkt: +46 380 295 26

Sommar 2025
Vi stänger v29-31. Med reducerad bemanning v28 & 32

Från: Support Mailbox Sweden <support.se@a-w.com>
Skickat: den 9 juni 2025 11:11
Till: Intermac 2 <inter@fsglass.se>; Per-Inge Aleräng <per-inge.alerang@fsglass.se>
Ämne: [AW-233039] Ticket confirmation / SN-fil som visas i PT Intermac

Dear Mr. Aleräng,

Ticket ID [AW-233039]

Tack för att ni kontaktar A+W Support Team.

Om ert ärende är brådskande. Vänligen kontakta oss på nedanstående nummer.

Ert ärende har nått oss och en ticket har skapits automatiskt i vårt support system.

Vi kommer att bearbeta ert ärende så fort som möjligt.

Vid fortsatt kontakt i detta ärende, vänligen använd bifogat ticket id.

-------------------------------------------------------------------------------------------------------------------------------

Thank you for contact…
```

</details>

***

### \[AW-224373]

**Subject:** P-2025-237 - (IT-600) Request to create new label with QR code for Velux Commercial\
**Status:** In Progress | **Category:** Support Clarity / Support Sweden | **Last Action:** 23.06.2025 10:05

\[AW-224373] (IT-600) Ny label til Velux Commercial (63) Issue is comments: Thomas Abildgaard Skelly - I dag 10:03 AM Hi Henrik This is the last message she sent: Hej Det går fint. Det eneste problem er, at det kun er Bjarne der kan udskrive den, men det tænker jeg i kan fikse?

<details>

<summary>Full conversation</summary>

```
From: Glaseksperten Itservicedesk (it@glaseksperten.dk)
To: support.se@a-w.com | Date: 23.06.2025 10:05
Type: Request | 
[AW-224373]   (IT-600) Ny label til Velux Commercial (63)
Issue is comments:
 

Thomas Abildgaard Skelly - I dag 10:03 AM
Hi Henrik
This is the last message she sent:
Hej
Det går fint.
Det eneste problem er, at det kun er Bjarne der kan udskrive den, men det tænker jeg i kan fikse?
```

</details>

***

### \[AW-230009]

**Subject:** SmartFactory - SJ3 Furnace outwall request window issue\
**Status:** In Progress | **Category:** Support Clarity / Support Sweden | **Last Action:** 20.06.2025 11:29

RE: \[AW-230009] Ticket confirmation / SJ3 Furnace outwall request window issue (6) Hello Jens, Yes, this is still happening. Currently we have many completed batches which are booked for the packing. But today I can still see one batch which is also with booked packing, but it is still visible in SJ3 outwall 207: Linas Liaudinskas • Process Engineer mobile +370 697 98934 secretary's number +370 697 58904 \[Summer break - Ka...

<details>

<summary>Full conversation</summary>

```
From: Linas Liaudinskas (linas.liaudinskas@pressglass.com)
To: support.se@a-w.com | Date: 20.06.2025 11:29
Type: Request | 
RE: [AW-230009] Ticket confirmation / SJ3 Furnace outwall request window issue (6)
Hello Jens,

Yes, this is still happening.
Currently we have many completed batches which are booked for the packing. But today I can still see one batch which is also with booked packing, but it is still visible in SJ3 outwall 207:

Linas Liaudinskas • Process Engineer
mobile +370 697 98934
secretary's number +370 697 58904
linas.liaudinskas@pressglass.com<mailto:linas.liaudinskas@pressglass.com>
[Summer break - Kaunas.gif]
[logo-pg-172x38.png]
________________________________
PRESS GLASS UAB • The Division in Kaunas • Aviacijos g.3, LT-54460, Sergeičikų I k. Karmėlavos sen., Kauno raj.• Lithuania • phone +370 697 58904
VAT LT100013866714 • Company Register No.: 305710904 • Before printing, think about the environment.

From: Support Mailbox Sweden <support.se@a-w.com>
Sent: 2025 m. birželio 18 d., trečiadienis 12:19
To: Linas Liaudinskas <linas@glasslt.com>
```

</details>

***

### \[AW-234216]

**Subject:** Längre utskrifter av CR-rapporter efter patch - KLJ\
**Status:** Unknown | **Category:** Support Clarity / Support Sweden | **Last Action:** 19.06.2025 11:29

RE: \[AW-234216] Längre utskrifter av CR-rapporter efter patch - KLJ (3) Hej Andreas MGA är patchat för inte så längesedan ca a månad sedan så versions mässigt är de inte så olika Best regards Jens Thorsen ###EOM## A+W Support Sweden +46 (0) 35 175 417 A+W Support UK + 44 (0) 560348 8606 A+W Support Poland +48 61 436 63 74 A+W Helpdesk Tool and other ways of contacts https://www.a-w.com/uk/service/ A+W Software GmbH Siemensstraße 3 35463 Fernwald Germany www.a-w.com Geschäftsführer/Managing Direc...

<details>

<summary>Full conversation</summary>

```
From: Jens Thorsen (support.se@a-w.com)
To: andreas.persson@glasgruppen.se | Date: 19.06.2025 11:29
Type: Answer | 
RE: [AW-234216] Längre utskrifter av CR-rapporter efter patch - KLJ (3)
Hej Andreas
MGA är patchat för inte så längesedan ca a månad sedan så versions mässigt är de inte så olika
Best regards
Jens Thorsen
###EOM##

A+W Support Sweden +46 (0) 35 175 417
A+W Support UK + 44 (0) 560348 8606
A+W Support Poland +48 61 436 63 74

A+W Helpdesk Tool and other ways of contacts
https://www.a-w.com/uk/service/
A+W Software GmbH
Siemensstraße 3
35463 Fernwald
Germany
www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-Schutzprogramme…
```

</details>

***

### \[AW-234206]

**Subject:** Fw: AW kinnitus / hinnad\
**Status:** New | **Category:** Support Clarity / Support Sweden | **Last Action:** 19.06.2025 08:17

Fw: AW kinnitus / hinnad (2) Hello We cannot get purchase order price maching with order confirmation EUR sum. What can be done there? More digits after comma? Andres Parts Development manager +372 50 12 981 Glassense AS Kose vald Kolu 75121 Estonia www.glassense.com[http://www.glassense.com/](http://www.glassense.com/) \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_ From: Marju Mustimets Sent: Wednesday, June 18, 2025 10:20 AM To: Andres Parts Cc: Karin Riisalu \<Karin.Riisalu...

<details>

<summary>Full conversation</summary>

```
From: Andres Parts (Andres.Parts@glassense.com)
To: support.se@a-w.com | Date: 19.06.2025 08:17
Type: Request | 
Fw: AW kinnitus / hinnad (2)
Hello

We cannot get purchase order price maching with order confirmation EUR sum.

What can be done there? More digits after comma?

Andres Parts

Development manager

+372 50 12 981

Glassense AS

Kose vald Kolu

75121 Estonia

www.glassense.com<http://www.glassense.com/>

________________________________
From: Marju Mustimets <Marju.Mustimets@glassense.com>
Sent: Wednesday, June 18, 2025 10:20 AM
To: Andres Parts <Andres.Parts@glassense.com>
Cc: Karin Riisalu <Karin.Riisalu@glassense.com>
Subject: AW kinnitus / hinnad

Hei

Hinnavahe 116,93 €

Ehk saab seda veic „näppida“. Võiks olla 3-4 kohta peale koma.

AW-st ostukas:

Tarnija TK:

Tnx 😊

Glassense on kollektiivpuhkusel:

Tartu ja Mäo tehas puhkavad N28 - N29 (07.07-20.07)

Kolu tehas puhkab N29 - N30 (14.07-27.07)

Glassense will be on summer holidays:

Tar…
```

</details>

***

### \[AW-233993]

**Subject:** Incorrect VAT calculated for invoice.\
**Status:** In Progress | **Category:** Support Clarity / Support Sweden | **Last Action:** 18.06.2025 14:29

Sv: Sv: \[AW-233993] Ticket confirmation / VB: Alfak fel belopp (5) Hej Då det troligen inte beror på oss eller vårt handhavande, så är det just hjälp med att hitta felet som jag vill. Är det så att det är något handhavandefel hos oss, så är ju ett fel i systemet som gör det möjligt. Tänker att det kanske inte är vi som ska hitta problemet?! Hälsningar Håkan Från: Support Mailbox Sweden Skickat: den 18 juni 2025 14:23 Till: Håkan Johnsson Kopia: Samra Mala...

<details>

<summary>Full conversation</summary>

```
From: Håkan Johnsson (hakan@osbyglas.se)
To: support.se@a-w.com | Date: 18.06.2025 14:29
Type: Request | 
Sv: Sv: [AW-233993] Ticket confirmation / VB: Alfak fel belopp (5)
Hej
Då det troligen inte beror på oss eller vårt handhavande, så är det just hjälp med att hitta felet som jag vill.
Är det så att det är något handhavandefel hos oss, så är ju ett fel i systemet som gör det möjligt.

Tänker att det kanske inte är vi som ska hitta problemet?!

Hälsningar
Håkan

Från: Support Mailbox Sweden <support.se@a-w.com>
Skickat: den 18 juni 2025 14:23
Till: Håkan Johnsson <hakan@osbyglas.se>
Kopia: Samra Malagic <samra@osbyglas.se>
Ämne: RE: Sv: [AW-233993] Ticket confirmation / VB: Alfak fel belopp

Hej Håkan,

Jag kan inte se att någon tittat på detta än, du kan kontrollera detta via kundportalen på A-W's hemsida<https://portal.a-w.com/us/member-login/> där du kan skapa in inloggning om du inte redan har access.

Detta är inte ett problem jag sett tidigare, är detta ett problem ni kan återskapa? Är det ett problem även i testsystemet där allt är uppdaterat? Om vi inte kan reproducera detta så tror jag det blir svårt att hitta källan till de…
```

</details>

***

### \[AW-231365]

**Subject:** Production start date calculations\
**Status:** In Progress | **Category:** Support Clarity / Support Sweden | **Last Action:** 18.06.2025 14:18

RE: \[AW-231365] Ticket confirmation / Production start date calculations (4) Hello, Is there any news on how to achieve the previous behaviour of prod. Start calculations? Best regards Linas Vaičiūnas Process engineer \[signature\_540931018]+370 688 34696 From: Support Mailbox Sweden Sent: Monday, May 26, 2025 11:09 AM To: Linas Vaičiūnas Lukas Aleksejevas Subject: \[AW-231365] Ticket confirmation / Production star...

<details>

<summary>Full conversation</summary>

```
From: Linas Vaiciunas (linas@glasslt.com)
To: support.se@a-w.com, lukas@glasslt.com, adam.grimberg@a-w.com | Date: 18.06.2025 14:18
Type: Request | 
RE: [AW-231365] Ticket confirmation / Production start date calculations (4)
Hello,

Is there any news on how to achieve the previous behaviour of prod. Start calculations?

Best regards

Linas Vaičiūnas
Process engineer
[signature_540931018]+370 688 34696

From: Support Mailbox Sweden <support.se@a-w.com>
Sent: Monday, May 26, 2025 11:09 AM
To: Linas Vaičiūnas <linas@glasslt.com>; Lukas Aleksejevas <lukas@glasslt.com>; adam.grimberg@a-w.com
Subject: [AW-231365] Ticket confirmation / Production start date calculations

Dear Mr. Vaiciunas,

Ticket ID [AW-231365]

Tack för att ni kontaktar A+W Support Team.

Om ert ärende är brådskande. Vänligen kontakta oss på nedanstående nummer.

Ert ärende har nått oss och en ticket har skapats automatiskt i vårt support system.

Vi kommer att bearbeta ert ärende så fort som möjligt.

Vid fortsatt kontakt i detta ärende, vänligen använd bifogat ticket id.

-------------------------------------------------------------------------------------------------------------------------------
```

</details>

***

### \[AW-224751]

**Subject:** How to adjust minimum order value for customers in AWB\
**Status:** Unknown | **Category:** Support Clarity / Support Sweden | **Last Action:** 18.06.2025 11:38

<details>

<summary>Full conversation</summary>

```
From: Henrik Johansson
To: Erik Berggren | Date: 18.06.2025 11:38
Type: State changed | 
RE: [AW-224751] How to adjust minimum order value for customers in AWB (10)
Waiting for feedback from customer...
```

</details>

***

### \[AW-226737]

**Subject:** Did not bring the glasses for the Line2\
**Status:** In Progress | **Category:** Support Clarity / Support Sweden | **Last Action:** 17.06.2025 16:31

Re: \[AW-226737] Did not bring the glasses for the Line2 (7) Hello, It happens very rarely. I think it might happen after servers restarts during monthly Windows updates, but not every time and I'm not sure. Is there anything else we could check or look into to help identify the cause? Best regards / Pagarbiai Regimantas Graževičius CIO / IT vadovas \[signature\_540931018]+370 620 41450 \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_ From: Support Mailbox Sweden Sent: Monday, June 02, 2025 10...

<details>

<summary>Full conversation</summary>

```
From: Regimantas Graževičius (regimantas@glasslt.com)
To: support.se@a-w.com | Date: 17.06.2025 16:31
Type: Request | 
Re: [AW-226737] Did not bring the glasses for the Line2 (7)
Hello,

It happens very rarely.
I think it might happen after servers restarts during monthly Windows updates, but not every time and I'm not sure.
Is there anything else we could check or look into to help identify the cause?

Best regards / Pagarbiai

Regimantas Graževičius
CIO / IT vadovas
[signature_540931018]+370 620 41450

________________________________
From: Support Mailbox Sweden <support.se@a-w.com>
Sent: Monday, June 02, 2025 10:22
To: Regimantas Graževičius <regimantas@glasslt.com>
Cc: Linas Vaičiūnas <linas@glasslt.com>
Subject: RE: [AW-226737] Did not bring the glasses for the Line2

Greetings,

did it happen only once or more times?

If yes, when was the most recent time ?

Best regards
Vladimir Iljin
###EOM##

A+W Support Sweden +46 (0) 35 175 417
A+W Support UK + 44 (0) 560348 8606
A+W Support Poland +48 61 436 63 74

A+W Helpdesk Tool and other ways of contacts
https://www.a-w.com/uk/service/

A+W Software Gm…
```

</details>

***

### \[AW-231235]

**Subject:** PT changes, "HQ" PT adjustments and breakage status configuration.\
**Status:** Unknown | **Category:** Support Clarity / Support Sweden | **Last Action:** 17.06.2025 13:28

<details>

<summary>Full conversation</summary>

```
From: Henrik Johansson
To: Henrik Johansson | Date: 17.06.2025 13:28
Type: State changed | 
RE: [AW-231235] PT changes, "HQ" PT adjustments and breakage status configuration. (6)
Time scheduled via email, first session to be 30/6 @ 10:00.
```

</details>

***

### \[AW-233871]

**Subject:** SMF tickets set to be archived, batch 8807\
**Status:** In Progress | **Category:** Support Clarity / Support Sweden | **Last Action:** 17.06.2025 09:58

Sv: \[AW-233871] Arkiverade tickets, batch 8807 (5) Hej Henrik, Det stämmer att packningen antagligen har lagt in fel glas på en pall via deras Tool TV, misstag händer då och då och är inget jag tror vi kommer kunna eliminera. Däremot så tror jag att vi kan ändra hur den arkiverar tickets genom att kolla först kolla om det finns kvar i OSBSOA.dbo.Stock\_StockSheets. Gör den det så ska den inte arkiveras förrän den har försvunnit från denna tabellen. Jag har inte koll på hur denna arkivering görs, ...

<details>

<summary>Full conversation</summary>

```
From: Robin Johnsson (robin@osbyglas.se)
To: support.se@a-w.com | Date: 17.06.2025 09:58
Type: Request | 
Sv: [AW-233871] Arkiverade tickets, batch 8807 (5)
Hej Henrik,

Det stämmer att packningen antagligen har lagt in fel glas på en pall via deras Tool TV, misstag händer då och då och är inget jag tror vi kommer kunna eliminera. Däremot så tror jag att vi kan ändra hur den arkiverar tickets genom att kolla först kolla om det finns kvar i OSBSOA.dbo.Stock_StockSheets.
Gör den det så ska den inte arkiveras förrän den har försvunnit från denna tabellen.

Jag har inte koll på hur denna arkivering görs, är den triggad på tidpunkter där den kollar vad som är packat eller är det när processen packning är görs?

Vi kan vänta på att Anders eller Adam är tillgängliga men jag vill ta tag i detta så snart som möjligt, i alla fall senast i början på nästa vecka.

Här kommer en lista på enheter som jag tror detta har hänt på tidigare:

Select * from
(
SELECT
SheetId,
Info,
ManufacturerSlot,
ManufacturerStation,
Source,
(Select MAX(ArchiveStatus) from alcimdb.dbo.Maps_Tickets where SheetId = Stock_StockSheets.SheetId) AS Archived
F…
```

</details>

***

### \[AW-233584]

**Subject:** RE: GLASSENSE : Batch 8203 - didnt get cutting labels for 44.2 Premium2 lami\
**Status:** New | **Category:** Support Clarity / Support Sweden | **Last Action:** 17.06.2025 09:19

RE: GLASSENSE : Batch 8203 - didnt get cutting labels for 44.2 Premium2 lami \[AW-233584] (9) Hello, I have tried to do again some batches with PMO optimizer. Seems that some IGU batches were ok. Now I did some batches where is Ral-Tempering-Heat soak tested glass and there I can’t print rack list for cutting. PMO were put this to the harp rack list again. Can’t you just remove those harp rack lists from everywhere ? Rain Aava Production planner +372 5358 6369 Glassense AS Kose vald Kolu 75121 E...

<details>

<summary>Full conversation</summary>

```
From: Rain Aava (Rain.Aava@glassense.com)
To: Adam.Grimberg@a-w.com, Andres.Parts@glassense.com, support.se@a-w.com, Marc.Emieux@a-w.com, Xavier.Thevenin@a-w.com | Date: 17.06.2025 09:19
Type: Request | 
RE: GLASSENSE :  Batch 8203 - didnt get cutting labels for 44.2 Premium2 lami [AW-233584] (9)
Hello,

I have tried to do again some batches with PMO optimizer. Seems that some IGU batches were ok.

Now I did some batches where is Ral-Tempering-Heat soak tested glass and there I can’t print rack list for cutting.
PMO were put this to the harp rack list again.
Can’t you just remove those harp rack lists from everywhere ?

Rain Aava
Production planner
+372 5358 6369

Glassense AS
Kose vald Kolu
75121 Estonia

From: Rain Aava
Sent: Monday, June 16, 2025 09:07
To: 'Grimberg, Adam' <Adam.Grimberg@a-w.com>; Andres Parts <andres.parts@glassense.com>; support.se <support.se@a-w.com>; Emieux, Marc <Marc.Emieux@a-w.com>; Thevenin, Xavier <Xavier.Thevenin@a-w.com>
Subject: RE: GLASSENSE : Batch 8203 - didnt get cutting labels for 44.2 Premium2 lami [AW-233584]

Good morning,

I don’t know if you already did something, but I tried to release this batch again and today I got production lis…
```

</details>

***

### \[AW-233311]

**Subject:** Ordrer transferred directly to Alcim\
**Status:** New | **Category:** Support Clarity / Support Sweden | **Last Action:** 16.06.2025 11:49

SV: \[AW-233311] Ticket confirmation / Ordrer transferred directly to Alcim (3) Hvordan går det med denne sag? Venlig hilsen / Regards / Grüssen Jette Gern Madsen Kundecenter M: +45 96 23 47 27 E: W: www.glaseksperten.dk Fra: Support Mailbox Sweden Sendt: 11. juni 2025 13:17 Til: Jette Gern Madsen Emne: \[AW-233311] Ticket confirmation / Ordrer transferred directly to Alcim CAUTION: External Sender. Please do not click on links or op...

<details>

<summary>Full conversation</summary>

```
From: Jette Gern Madsen (jgm@glaseksperten.dk)
To: support.se@a-w.com | Date: 16.06.2025 11:49
Type: Request | 
SV: [AW-233311] Ticket confirmation / Ordrer transferred directly to Alcim (3)
Hvordan går det med denne sag?

Venlig hilsen / Regards / Grüssen
Jette Gern Madsen
Kundecenter

M: +45 96 23 47 27
E: jgm@glaseksperten.dk
W: www.glaseksperten.dk

Fra: Support Mailbox Sweden <support.se@a-w.com>
Sendt: 11. juni 2025 13:17
Til: Jette Gern Madsen <jgm@glaseksperten.dk>
Emne: [AW-233311] Ticket confirmation / Ordrer transferred directly to Alcim

CAUTION: External Sender. Please do not click on links or open attachments from senders you do not trust.

Dear Ms. Madsen,

Ticket ID [AW-233311]

Tack för att ni kontaktar A+W Support Team.

Om ert ärende är brådskande. Vänligen kontakta oss på nedanstående nummer.

Ert ärende har nått oss och en ticket har skapits automatiskt i vårt support system.

Vi kommer att bearbeta ert ärende så fort som möjligt.

Vid fortsatt kontakt i detta ärende, vänligen använd bifogat ticket id.

---------------------------------------------------------------------------------…
```

</details>

***

### \[AW-231347]

**Subject:** Macotec RTO, no product number\
**Status:** In Progress | **Category:** Support Clarity / Support Sweden | **Last Action:** 16.06.2025 11:29

RE: \[AW-231347] Macotec RTO, no product number (9) Hello, guys. This issue is urgent. This issue has been registered almost half of the month ago. We need to a solution to this issue. What are the options? When you can solve it ? Pagarbiai / Faithfully, Gen. Direktorius / CEO Darius Puzinovas Tel. +37068744937 El. paštas / e-mail: UAB/JSC ,,Gravera” Draugystės g. 19, LT-51230, Kaunas, Lietuva www.gravera.com[http://www.gravera.com/](http://www.gravera.com/) From: Darius ...

<details>

<summary>Full conversation</summary>

```
From: JSC Gravera (dariuspu@gravera.com)
To: support.se@a-w.com | Date: 16.06.2025 11:29
Type: Request | 
RE: [AW-231347] Macotec RTO, no product number (9)
Hello, guys.

This issue is urgent. This issue has been registered almost half of the month ago.

We need to a solution to this issue. What are the options? When you can solve it ?

Pagarbiai / Faithfully,
Gen. Direktorius / CEO
Darius Puzinovas
Tel. +37068744937
El. paštas / e-mail: dariuspu@gravera.com<mailto:dariuspu@gravera.com>

UAB/JSC ,,Gravera”
Draugystės g. 19, LT-51230, Kaunas, Lietuva
www.gravera.com<http://www.gravera.com/>

From: Darius Puzinovas
Sent: Friday, June 6, 2025 3:23 PM
To: Support Mailbox Sweden <support.se@a-w.com>
Subject: RE: [AW-231347] Macotec RTO, no product number

Hello,

Do you have any news regarding this issue?

There are almost two weeks pasted since we have this issue.

Do you have any option how can we solve it? It is urgent already.

Perhaps you could reinstall RTO on macotec user?

If yes, we would plan a time window for the next week. Please let me ASAP what is the plan her…
```

</details>

***

### \[AW-233627]

**Subject:** Daily Reset of Negative 0x0 Stock to Zero\
**Status:** Unknown | **Category:** Support Clarity / Support Sweden | **Last Action:** 16.06.2025 11:27

<details>

<summary>Full conversation</summary>

```
From: Henrik Johansson
To: Henrik Johansson | Date: 16.06.2025 11:27
Type: State changed | 
RE: [AW-233627] Daily Reset of Negative 0x0 Stock to Zero (8)
Waiting for customer
```

</details>

***

### \[AW-221951]

**Subject:** 8912 prod. sequence wrong\
**Status:** In Progress | **Category:** Support Clarity / Support Sweden | **Last Action:** 16.06.2025 08:18

RE: \[AW-221951] 8912 prod. sequence wrong (6) Hello, To explain in more detail: Usually, the files go in sequence 89120240, 89120241, 89120242, 89120243 and 89120244. In these files the production sequence should be from 1 to 58 (58 units in batch total). However, if you check 1st file 89120240 contains items from 31 to 44 2nd file 89120241 contains item 1 and then items 45 to 58 3rd file 89120242 contains items 2 to 15 4th file 89120243 contains items 16 to 29 5th file 89120244 contains item 30...

<details>

<summary>Full conversation</summary>

```
From: Linas Vaiciunas (linas@glasslt.com)
To: regimantas@glasslt.com, support.se@a-w.com | Date: 16.06.2025 08:18
Type: Request | 
RE: [AW-221951] 8912 prod. sequence wrong (6)
Hello,

To explain in more detail:

Usually, the files go in sequence 89120240, 89120241, 89120242, 89120243 and 89120244.
In these files the production sequence should be from 1 to 58 (58 units in batch total).
However, if you check
1st file 89120240 contains items from 31 to 44
2nd file 89120241 contains item 1 and then items 45 to 58
3rd file 89120242 contains items 2 to 15
4th file 89120243 contains items 16 to 29
5th file 89120244 contains item 30

And expected is:
1st file items 1 to 14
2nd file items 15 to 28
3rd file items 29 to 42
4th file items 43 to 57
5th file items 58

Or something similar, based on the rule that there can be max 42 sheets in a single TRF file and of course based on the PMO.

Best regards

Linas Vaičiūnas
Process engineer
[signature_540931018]+370 688 34696

From: Regimantas Graževičius <regimantas@glasslt.com>
Sent: Friday, June 6, 2025 4:55 PM
To: Support Mailbox Sweden <support.se@a-w.com>
Cc: Linas Vaičiūvas <linas@glass…
```

</details>

***

### \[AW-233050]

**Subject:** Stock for grill\
**Status:** Unknown | **Category:** Support Clarity / Support Sweden | **Last Action:** 13.06.2025 17:05

<details>

<summary>Full conversation</summary>

```
From: Jens Thorsen
To: Jens Thorsen | Date: 13.06.2025 17:05
Type: State changed | 
Stock for grill (3)
Test batch that has been used is 7137
we modified the stored procedure which was executed from the vorfein STP
```

</details>

***

### \[AW-233116]

**Subject:** Feature request, increase price based on weight of article\
**Status:** In Progress | **Category:** Support Clarity / Support Sweden | **Last Action:** 13.06.2025 16:32

RE: Prishöjning per kg. \[AW-233116] (3) Hej Ola, Beskrivning av formatet osv. är det tyvärr sämre med, jag pratade med en kollega tittat lite närmare på detta för något år sedan som konstaterat att denna integration skapades för en kund för 20 – 25 år sedan och min kollega var inte medveten om någon kund som idag använder denna funktion. Det ser alltså ut som att det inte är ett bra alternativ att försöka använda denna gamla funktion för import av pris. Hur ser priserna ut som ni jobbar med här,...

<details>

<summary>Full conversation</summary>

```
From: Henrik Johansson (Henrik.Johansson@a-w.com)
To: Ola.Anvegard@glasgruppen.se | Date: 13.06.2025 16:32
Type: Request | 
RE: Prishöjning per kg. [AW-233116] (3)
Hej Ola,
 
Beskrivning av formatet osv. är det tyvärr sämre med, jag pratade med en kollega tittat lite närmare på detta för något år sedan som konstaterat att denna integration skapades för en kund för 20 – 25 år sedan och min kollega var inte medveten om någon kund som idag använder denna funktion. Det ser alltså ut som att det inte är ett bra alternativ att försöka använda denna gamla funktion för import av pris.
 
Hur ser priserna ut som ni jobbar med här, är det enkelpriser eller är det mycket matris / vektor priser? Jag fick lite info om att vi har en kund där vi skapat en lösning där vi kan läsa en csv fil i databasen med hjälp av en customizing för att underlätta stora uppdateringar av priser men då är det enkelpris som används då dessa inte är like komplexa att hantera på detta sätt.
 
Jag har pratat lite med Anders om andra möjlig lösningar utöver utvecklingsförslag via R&D, vi ska diskutera det vidare i början på nästa vecka och jag återkopplar när jag har lite mer in…
```

</details>

***

### \[AW-226368]

**Subject:** Goods receipt local currency differs when exchange rate and price is the same\
**Status:** Unknown | **Category:** Support Clarity / Support Sweden | **Last Action:** 13.06.2025 11:21

<details>

<summary>Full conversation</summary>

```
From: Henrik Johansson
To: Henrik Johansson | Date: 13.06.2025 11:21
Type: State changed | 
RE: [AW-226368] Goods receipt local currency differs when exchange rate and price is the same (8)
Reminder sent to Therése:
From: Johansson, Henrik
Sent: den 13 juni 2025 11:20
To: 'Therése Cederqvist' <therese@osbyglas.se>; Grimberg, Adam <Adam.Grimberg@a-w.com>; 'Ola Holmgren' <ola@osbyglas.se>
Cc: Joel Rosenqvist <joel@osbyeksperten.dk>; Levin, Pontus <Pontus.Levin@a-w.com>; Mason, Stephen <Stephen.Mason@a-w.com>
Subject: RE: Osby Glas - Lager - Goods receipt local currency differs when exchange rate and price is the same [AW-226368]
Hej Therése,
Har det varit något mer problem gällande detta eller har det fungerat sedan detta senast diskuterades? Om detta är något vi behöver jobba vidare med så behöver vi ett nytt exempel enligt föregående email. Om vi behöver en längre tidsperiod bakåt för giltiga exempel så kan vi se om vi kan justera hur många databas backuper för A+W Business vi sparar på er databasserver, detta är idag konfigurerat till att spara backuper sju dagar bakåt men kan utökas givet att det finns utrymme på databas servern för detta.
Återkoppla gärna till mig …
```

</details>

***

### \[AW-230039]

**Subject:** Booking of stock sheets and boxes (end-caps)\
**Status:** Unknown | **Category:** Support Clarity / Support Sweden | **Last Action:** 13.06.2025 11:20

<details>

<summary>Full conversation</summary>

```
From: Erik Berggren
To: Erik Berggren | Date: 13.06.2025 11:20
Type: State changed | 
RE: [AW-230039] Booking of stock sheets and boxes (end-caps) (5)
Sent email to Ola, regarding which solution to use for booking boxes
```

</details>

***

### \[AW-233605]

**Subject:** AWB : Stock control even without document type Stock P.O.\
**Status:** Unknown | **Category:** Support Clarity / Support Sweden | **Last Action:** 13.06.2025 11:07

<details>

<summary>Full conversation</summary>

```
From: Henrik Johansson
To: Henrik Johansson | Date: 13.06.2025 11:07
Type: State changed | 
RE: [AW-233605] AWB : Stock control even without document type Stock P.O. (3)
Awaiting feedback from customer to see if this should be enabled in live. Active in test system so it can be reviewed there.
```

</details>

***

### \[AW-233213]

**Subject:** 275261\
**Status:** Unknown | **Category:** Support Clarity / Support Sweden | **Last Action:** 12.06.2025 16:48

<details>

<summary>Full conversation</summary>

```
From: Jens Thorsen
To: Jens Thorsen | Date: 12.06.2025 16:48
Type: State changed | 
275261 (3)
Made some tests in the test system to see what the issue can be. I will need to investigate this a little bit more
```

</details>

***

### \[AW-232876]

**Subject:** Step på tool\_tv\
**Status:** In Progress | **Category:** Support Clarity / Support Sweden | **Last Action:** 12.06.2025 09:43

\[AW-232876] Step på tool\_tv (4) Hej Oscar Jag har kopierat det som KJ har uppsatt på på deras iso lina bara för att vi ska ha något att gå på, där blir det så här på step. detta är från test systemet. Hur vill ni att det ska visas? Best regards Jens Thorsen ###EOM## A+W Support Sweden +46 (0) 35 175 417 A+W Support UK + 44 (0) 560348 8606 A+W Support Poland +48 61 436 63 74 A+W Helpdesk Tool and other ways of contacts https://www.a-w.com/uk/service/ A+W Software GmbH Siemensstraße 3 35463 Fernwa...

<details>

<summary>Full conversation</summary>

```
From: Jens Thorsen (support.se@a-w.com)
To: oscar.carlsson@glasgruppen.se | Date: 12.06.2025 09:43
Type: Answer | 
[AW-232876] Step på tool_tv (4)
Hej Oscar
Jag har kopierat det som KJ har uppsatt på på deras iso lina bara för att vi ska ha något att gå på, där blir det så här på step.
detta är från test systemet. 
Hur vill ni att det ska visas? 

Best regards
Jens Thorsen
###EOM##

A+W Support Sweden +46 (0) 35 175 417
A+W Support UK + 44 (0) 560348 8606
A+W Support Poland +48 61 436 63 74

A+W Helpdesk Tool and other ways of contacts
https://www.a-w.com/uk/service/
A+W Software GmbH
Siemensstraße 3
35463 Fernwald
Germany
www.a-w.com

Geschäftsführer/Managing Directors: Eric Herrmann, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich med…
```

</details>

***

### \[AW-233428]

**Subject:** Ändring av priser på stativ.\
**Status:** New | **Category:** Support Clarity / Support Sweden | **Last Action:** 12.06.2025 09:36

Ändring av priser på stativ. (2) Hej! Vi skall justera våra priser som vi fakturerar på ej returnerade stativ. Frågan är då vad som händer om kunderna får kreditfaktura där det gamla priser är faktureras, när kreditfakturan görs hämtas priset från prislistan eller från den gamla fakturan? OM den hämtar från prislitan kommer ju kunden få en kredit på högre belopp än vad som fakturerats, vilket ju är väldigt olyckligt. /Ola Ola Anvegård, Chef Affärs- & Verksamhetsutveckling Phone: +46(0)705 269034...

<details>

<summary>Full conversation</summary>

```
From: Ola Anvegard (Ola.Anvegard@glasgruppen.se)
To: Support.se@a-w.com | Date: 12.06.2025 09:36
Type: Request | 
Ändring av priser på stativ. (2)
Hej!
Vi skall justera våra priser som vi fakturerar på ej returnerade stativ. Frågan är då vad som händer om kunderna får kreditfaktura där det gamla priser är faktureras, när kreditfakturan görs hämtas priset från prislistan eller från den gamla fakturan? OM den hämtar från prislitan kommer ju kunden få en kredit på högre belopp än vad som fakturerats, vilket ju är väldigt olyckligt.

/Ola

Ola Anvegård, Chef Affärs- & Verksamhetsutveckling
Phone: +46(0)705 269034| Adress: Box 1736,70117 Örebro, Sweden
www.glasgruppen.se<http://www.glasgruppen.se/>
```

</details>

***

### \[AW-231081]

**Subject:** Removable Remakes and Assemly terminals lagging\
**Status:** In Progress | **Category:** Support Clarity / Support Sweden | **Last Action:** 11.06.2025 12:04

Re: \[AW-231081] Removable Remakes and Assemly terminals lagging (7) Hello, Lisec autofab server is not lagging and we have no complaints from our production about it. I have created login for you to ig in 1: Id: 576 617 693 Psw: awadmin Best regards / Pagarbiai Lukas Aleksejevas IT specialist / IT specialistas \[signature\_991271617][https://glasslt.com/](https://glasslt.com/) \[signature\_857976224] \[signature\_1049242110]www.glasslt.com[http://www.glasslt.com/](http://www.glasslt.com/) \[signature\_1056612673]Verslo g. 10, 621...

<details>

<summary>Full conversation</summary>

```
From: Lukas Aleksejevas (lukas@glasslt.com)
To: support.se@a-w.com | Date: 11.06.2025 12:04
Type: Request | 
Re: [AW-231081] Removable Remakes and Assemly terminals lagging (7)
Hello,

Lisec autofab server is not lagging and we have no complaints from our production about it. I have created login for you to ig in 1:

Id: 576 617 693
Psw: awadmin

Best regards / Pagarbiai

Lukas Aleksejevas
IT specialist /  IT specialistas

[signature_991271617]<https://glasslt.com/>

[signature_857976224]  lukas@glasslt.com
[signature_1049242110]www.glasslt.com<http://www.glasslt.com/>

[signature_1056612673]Verslo g. 10, 62175 Alytus

________________________________
From: Support Mailbox Sweden <support.se@a-w.com>
Sent: Tuesday, June 10, 2025 5:52 PM
To: Lukas Aleksejevas <lukas@glasslt.com>
Subject: Re: [AW-231081] Removable Remakes and Assemly terminals lagging

Hello Lukas,

Could you share a TeamViewer password?

Seems the documented password might have changed.

When I check the log files it looks like it takes 30-45 seconds - but I need to see it to live and check what is take the most time. There are no single SQL or loading that is t…
```

</details>

***

### \[AW-233184]

**Subject:** Spacer text restrictions\
**Status:** Unknown | **Category:** Support Clarity / Support Sweden | **Last Action:** 10.06.2025 15:11

<details>

<summary>Full conversation</summary>

```
From: Adam Grimberg
To: Jens Thorsen | Date: 10.06.2025 15:11
Type: State changed | 
RE: [AW-233184] Spacer text restrictions (3)
@Jens - can you check?
```

</details>

***

### \[AW-233190]

**Subject:** Errors in process manager again\
**Status:** Unknown | **Category:** Support Clarity / Support Sweden | **Last Action:** 10.06.2025 15:11

<details>

<summary>Full conversation</summary>

```
From: Adam Grimberg
To: Vladimir Iljin | Date: 10.06.2025 15:11
Type: State changed | 
RE: [AW-233190] Errors in process manager again (3)
@Vlad - looks like there is a configuration error in the release screen. Printer name says "OFF". Can you check?
```

</details>

***

### \[AW-233036]

**Subject:** Orders have old sperrstation set in pool\_teile that is preventing order from archiving\
**Status:** In Progress | **Category:** Support Clarity / Support Sweden | **Last Action:** 09.06.2025 09:48

Orders have old sperrstation set in pool\_teile that is preventing order from archiving (1) Noticed some messages about batches that could not archive due to sperrstation set in Pool\_teile, this will need to be reviewed. We can likely just remove the sprrstation where sperrzeit is > one year or something like this.

<details>

<summary>Full conversation</summary>

```
From: Henrik Johansson on behalf of Darius Puzinovas
To: Henrik Johansson | Date: 09.06.2025 09:48
Type: Request | 
Orders have old sperrstation set in pool_teile that is preventing order from archiving (1)
Noticed some messages about batches that could not archive due to sperrstation set in Pool_teile, this will need to be reviewed. We can likely just remove the sprrstation where sperrzeit is > one year or something like this.
```

</details>

***

### \[AW-218439]

**Subject:** Surcharge "Stelhåndtering og kilometerafgift" article 8997 not set for article when copying to a new document.\
**Status:** In Progress | **Category:** Support Clarity / Support Sweden | **Last Action:** 05.06.2025 10:50

SV: \[AW-218439] Stelhåndtering og kilometerafgift varenr. 8997 kommer ikke med over, når vi kopierer ordre fra arkiv. (6) Det virker, når prisberegning är ”vinget” af. Venlig hilsen / Regards / Grüssen Jette Gern Madsen Kundecenter M: +45 96 23 47 27 E: W: Fra: Support Mailbox Sweden Sendt: 3. juni 2025 11:48 Til: Jette Gern Madsen Cc: Karen Nielsen Emne: RE: \[AW-218439] Stelhåndtering og kilometerafgift varen...

<details>

<summary>Full conversation</summary>

```
From: Jette Gern Madsen (jgm@glaseksperten.dk)
To: support.se@a-w.com | Date: 05.06.2025 10:50
Type: Request | 
SV: [AW-218439] Stelhåndtering og kilometerafgift varenr. 8997 kommer ikke med over, når vi kopierer ordre fra arkiv. (6)
Det virker, när prisberegning är ”vinget” af.

Venlig hilsen / Regards / Grüssen
Jette Gern Madsen
Kundecenter

M: +45 96 23 47 27
E: jgm@glaseksperten.dk
W:

Fra: Support Mailbox Sweden <support.se@a-w.com>
Sendt: 3. juni 2025 11:48
Til: Jette Gern Madsen <jgm@glaseksperten.dk>
Cc: Karen Nielsen <kn@glaseksperten.dk>
Emne: RE: [AW-218439] Stelhåndtering og kilometerafgift varenr. 8997 kommer ikke med over, når vi kopierer ordre fra arkiv.

CAUTION: External Sender. Please do not click on links or open attachments from senders you do not trust.

Hej Jette,

Har du märkt om detta fungerar bättre efter uppdateringen? Är detta fortfarande är ett problem fungerar det nu som förväntat?

Best regards
Henrik Johansson
###EOM##

A+W Support Sweden +46 (0) 35 175 417
A+W Support UK + 44 (0) 560348 8606
A+W Support Poland +48 61 436 63 74

A+W Helpdesk Tool and other ways of contacts
htt…
```

</details>

***

(continued in Part 3)
