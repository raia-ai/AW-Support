# 03\_professional\_services\_clarity\_emea\_part6

**Category:** PS Clarity / Professional Services Clarity EMEA | **Tickets:** 370 | **Part 6 of 7**

***

## \[AW-225350]

**Subject:** WG: (E) AW: Improvements to RELEASE\_SP\_INDIVIDUAL functionality\
**Status:** New | **Category:** PS Clarity / Professional Services Clarity EMEA | **Last Action:** 27.03.2025 13:32

WG: (E) AW: Improvements to RELEASE\_SP\_INDIVIDUAL functionality (2) Hi Dieter So we have this development that is controlled by the alenv var RELEASE\_SP\_INDIVIDUAL. If it’s enabled then intauf will call the SP and check for the return. The SP returns two fields, an integer with values 0 or 1, and a char. If the integer is 0 then intauf carries on as normal, but if it is a 1 then it puts the order into freitek, with the text contained in the char field. The way I have set it to work is that t...

<details>

<summary>Full conversation</summary>

```
From: Dieter Büchsenschütz (Dieter.Buechsenschuetz@a-w.com)
To: projects.emea@a-w.com | Date: 27.03.2025 13:32
Type: Request | 
WG: (E) AW: Improvements to RELEASE_SP_INDIVIDUAL functionality (2)
Hi Dieter
 
So we have this development that is controlled by the alenv var RELEASE_SP_INDIVIDUAL.  If it’s enabled then intauf will call the SP and check for the return.  The SP returns two fields, an integer with values 0 or 1, and a char.  If the integer is 0 then intauf carries on as normal, but if it is a 1 then it puts the order into freitek, with the text contained in the char field.  The way I have set it to work is that the order can cycle through freitek a number of times, being released for different reasons each time (generally relating to whether the hold is financial or commercial).  Also, there are some absolute stop checks that must be satisfied before the order can be released, so the order can be stuck in freitek until those conditions are met (e.g. if the order contains a shape 99 item, then the shape MUST have an SN filename against it).
 
So far so good.
 
However, one of the developments I would like is for there to be a third possible return code.  “0” sho…
```

</details>

***

## \[AW-225306]

**Subject:** AW: Einschulung neuer IT Systemadministrator - AWE -Schulungen\
**Status:** New | **Category:** PS Clarity / Professional Services Clarity EMEA | **Last Action:** 27.03.2025 11:13

AW: Einschulung neuer IT Systemadministrator - AWE -Schulungen (2) Hallo Herr Holzinger, Danke für die Hinweise. Gerne können drei Personen an der Schulung teilnehmen. Es ist auch möglich, das Coaching-Budget separat zu bestellen, wozu ich abraten würde, da Sie sehr wahrscheinlich noch Fragen dann in der täglichen Praxis haben werden. Bei Wunsch, ändern wir das sehr gerne ab. 😊 Zu Ihren Fragen: • Ja, wir gehen die AWE-Anwendervorgänge in einem unserer Testsysteme durch (darin befinden sich natür...

<details>

<summary>Full conversation</summary>

```
From: Dr. Paul Hohmann (Paul.Hohmann@a-w.com)
To: manfred.holzinger@vandaglas.ch, samir.uznik@vandaglas.ch | Date: 27.03.2025 11:13
Type: Request | 
AW: Einschulung neuer IT Systemadministrator - AWE -Schulungen (2)
Hallo Herr Holzinger,
 
Danke für die Hinweise. Gerne können drei Personen an der Schulung teilnehmen. Es ist auch möglich, das Coaching-Budget separat zu bestellen, wozu ich abraten würde, da Sie sehr wahrscheinlich noch Fragen dann in der täglichen Praxis haben werden. Bei Wunsch, ändern wir das sehr gerne ab. 😊
 
Zu Ihren Fragen:
 • Ja, wir gehen die AWE-Anwendervorgänge in einem unserer Testsysteme durch (darin befinden sich natürlich nur Testdaten).
 • Ja, die Themen hatte ich Ihnen ins Angebot geschrieben:
 • Datenbankenstrukturen und wichtigste Tabellen,
 • Tabellen-Dokumentation,
 • Backend-Services (Hintergrund/Starten/Stoppen/Logging),
 • Verzeichnisstrukturen,
 • Wichtige Skripte (Individualskripte, vorgangssql etc.),
 • Wichtige Eingriffsmöglichkeiten als Backend-User,
 • Wichtige Befehle zum orientieren im Backend,
 • CSV Import/Export,
 • Windowsdienste inkl. Logging,
 • Weiteres?
 • Sie können Ihre Crystal Reports auch mit dem Traine…
```

</details>

***

## \[AW-225276]

**Subject:** Support Ticket für Niklas P.\
**Status:** In Progress | **Category:** PS Clarity / Professional Services Clarity EMEA | **Last Action:** 27.03.2025 09:08

Support Ticket für Niklas P. (1) Allgemeines Support Ticket Niklas P.

<details>

<summary>Full conversation</summary>

```
From: Niklas Pietzsch
To: Niklas Pietzsch | Date: 27.03.2025 09:08
Type: Request | 
Support Ticket für Niklas P. (1)
Allgemeines Support Ticket Niklas P.
```

</details>

***

## \[AW-219087]

**Subject:** Remontée Coutras sur environnement de test SGVB (AWB et AWP)\
**Status:** Unknown | **Category:** PS Clarity / Professional Services Clarity EMEA | **Last Action:** 26.03.2025 18:10

RE: \[AW-219087] Devis base TEST AWB/AWP Coutras (15) Bonjour, François a paramétré les comptes suivants : \* CFRGEN-COU-MK \* CFRGEN-COU-DEC1 \* UFRGEN-COU-TTVVIENT Ces comptes peuvent ouvrir une session sur le serveur ALT2, accès au disque P:\Trans du serveur ABT1 Cdlt Arnaud BOURREAU IT régional +33 6 12 45 33 52 \[signatureImage] De : Palluy, Sylviane Envoyé : mercredi 26 mars 2025 10:05 À : projects.ga Bourreau, Arnaud

<details>

<summary>Full conversation</summary>

```
From: DSI Sgvb-dsi (sgvb-dsi@saint-gobain.com)
To: sylviane.palluy@a-w.com, David.Cousido@a-w.com | Date: 26.03.2025 18:10
Type: Request | 
RE: [AW-219087] Devis base TEST AWB/AWP Coutras (15)
Bonjour,
François a paramétré les comptes suivants :

 *   CFRGEN-COU-MK
 *   CFRGEN-COU-DEC1
 *   UFRGEN-COU-TTVVIENT
Ces comptes peuvent ouvrir une session sur le serveur ALT2, accès au disque P:\Trans du serveur ABT1
Cdlt

Arnaud BOURREAU
IT régional
+33 6 12 45 33 52
[signatureImage]

De : Palluy, Sylviane <Sylviane.Palluy@a-w.com>
Envoyé : mercredi 26 mars 2025 10:05
À : projects.ga <projects.ga@a-w.com>; Bourreau, Arnaud <Arnaud.Bourreau@saint-gobain.com>; David Cousido <David.Cousido@a-w.com>
Cc : Pfisterer, Simon <Simon.Pfisterer@saint-gobain.com>; Renault, Samuel <Samuel.Renault@saint-gobain.com>; SGVB-DSI <sgvb-dsi@saint-gobain.com>; Costecalde, Muriel <Muriel.Costecalde@saint-gobain.com>
Objet : RE: [AW-219087] Devis base TEST AWB/AWP Coutras

Bonjour

L'installation de Coutras pour la partie AWB est maintenant terminée.
Est-ce que vous pourriez donner les éléments demandés dans le mail ci-dessous pour que la partie AWP puisse également être finali…
```

</details>

***

## \[AW-225209]

**Subject:** New comment - \[#INC-15917] Eilt. S2S Tunnel mit A\&W aufbauen\
**Status:** New | **Category:** PS Clarity / Professional Services Clarity EMEA | **Last Action:** 26.03.2025 16:39

New comment - \[#INC-15917] Eilt. S2S Tunnel mit A\&W aufbauen (1) Sie erhalten nicht häufig E-Mails von Erfahren Sie, warum dies wichtig ist[https://aka.ms/LearnAboutSenderIdentification](https://aka.ms/LearnAboutSenderIdentification) Hi, There is a new comment in the ticket submitted by Tim Lehnert to DENWERIT Support Comment added by : Frank Christian Comment Content : Hallo Herr Lehnert Ich habe unsere IT informiert. Die werden sich mit ihnen in Verbindung setzen, um die Verbindung zu etablieren. Mit freundlichen G...

<details>

<summary>Full conversation</summary>

```
From: Support Denwerit (it-support@denwerit.com)
To: projects.emea@a-w.com, dieter.buechsenschuetz@a-w.com, frank.christian@a-w.com | Date: 26.03.2025 16:39
Type: Request | 
New comment - [#INC-15917] Eilt. S2S Tunnel mit A&W aufbauen (1)
Sie erhalten nicht häufig E-Mails von it-support@denwerit.com. Erfahren Sie, warum dies wichtig ist<https://aka.ms/LearnAboutSenderIdentification>

Hi,

There is a new comment in the ticket submitted by Tim Lehnert to DENWERIT Support

Comment added by : Frank Christian

Comment Content :

Hallo Herr Lehnert
Ich habe unsere IT informiert.
Die werden sich mit ihnen in Verbindung setzen, um die Verbindung zu etablieren.

Mit freundlichen Grüßen | Best regards

Frank Christian
Director Customer Support EMEA / APAC
A+W Business Unit Clarity

[Ein Bild, das Text, Schrift, Logo, Grafiken enthält.    Automatisch generierte Beschreibung]<http://www.a-w.com/>
Phone:  +49 641 96620-330
Mobile: +49 151 16228-822
Email: frank.christian@a-w.com

A+W Software GmbH
Siemensstraße 3
35463 Fernwald
Germany

www.a-w.com<http://www.a-w.com/>

Geschäftsführer/Managing Directors: Peter Dixen, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gieße…
```

</details>

***

## \[AW-224932]

**Subject:** P-2024-224 - NSG Bad Bentheim - Dynopt\
**Status:** In Progress | **Category:** PS Clarity / Professional Services Clarity EMEA | **Last Action:** 26.03.2025 12:15

AW: \[AW-224932] P-2024-224 - NSG Bad Bentheim - Dynopt (3) Hi Xavier, interesting, you are right. But Wolfgang started with investigation and found a gap. Regards Dieter Von: Thevenin, Xavier Gesendet: Mittwoch, 26. März 2025 11:47 An: Büchsenschütz, Dieter Cc: Dr. Hohmann, Paul support.production.de Betreff: RE: \[AW-224932] P-2024-224 - NSG Bad Bentheim - Dynopt Hello Dieter, Fyi, ...

<details>

<summary>Full conversation</summary>

```
From: Dieter Büchsenschütz (Dieter.Buechsenschuetz@a-w.com)
To: Xavier.Thevenin@a-w.com | Date: 26.03.2025 12:15
Type: Request | 
AW: [AW-224932] P-2024-224 - NSG Bad Bentheim - Dynopt (3)
Hi Xavier,
 
interesting, you are right.
But Wolfgang started with investigation and found a gap.
 
Regards Dieter
 
Von: Thevenin, Xavier <Xavier.Thevenin@a-w.com>
Gesendet: Mittwoch, 26. März 2025 11:47
An: Büchsenschütz, Dieter <Dieter.Buechsenschuetz@a-w.com>
Cc: Dr. Hohmann, Paul <Paul.Hohmann@a-w.com>; support.production.de <support.production.de@a-w.com>
Betreff: RE: [AW-224932] P-2024-224 - NSG Bad Bentheim - Dynopt

 
Hello Dieter,
Fyi, I cannot find your cirtical ticket in devops:  [AW-224413]
Br
Xavier
 
Br
Xavier Thevenin
###EOM###
BU A+W Clarity – Director Key Account Management – EMEA/APAC
+ 33 6 80591728
 
 

 
From: Büchsenschütz, Dieter <Dieter.Buechsenschuetz@a-w.com>
Sent: 25 March 2025 12:41
To: Tiegs, Dennis <Dennis.Tiegs@a-w.com>; Cortisse, Alfred <Alfred.Cortisse@a-w.com>
Cc: Thevenin, Xavier <Xavier.Thevenin@a-w.com>; Dr. Hohmann, Paul <Paul.Hohmann@a-w.com>
Subject: WG: [AW-224932] P-2024-224 - NSG Bad Bentheim - Dynopt

 
H…
```

</details>

***

## \[AW-216261]

**Subject:** Sperrstatus setzen bei PMO\
**Status:** Unknown | **Category:** PS Clarity / Professional Services Clarity EMEA | **Last Action:** 26.03.2025 09:29

<details>

<summary>Full conversation</summary>

```
From: Jürgen Möller
To: | Date: 26.03.2025 09:29
Type: Note | 
Hotfix was created (35)
An hotfix was created for this ticket
Product-Target: A+W Production 6 Import
Publish: \\jupiter\SW_INSTALL\Hotfix\12026_A+W Production 6 Import_19330.zip
Customer: AGC Glass Europe SA
UpdateDate: 30/03/2025 00:00:00

--- This is an automatically generated message ---
```

</details>

***

## \[AW-224740]

**Subject:** Glas Herzog Log-Files Corporate Tracking Service\
**Status:** Unknown | **Category:** PS Clarity / Professional Services Clarity EMEA | **Last Action:** 25.03.2025 08:56

<details>

<summary>Full conversation</summary>

```
From: Niklas Pietzsch
To: | Date: 25.03.2025 08:56
Type: State changed | 
RE: [AW-224740] Glas Herzog Log-Files Corporate Tracking Service (3)
Sicherung der Log-Dateien
```

</details>

***

## \[AW-220720]

**Subject:** Caleoglas Murr in Semco Projekt Momentum\
**Status:** Unknown | **Category:** PS Clarity / Professional Services Clarity EMEA | **Last Action:** 24.03.2025 08:54

AW: Freigabe AWB in MUR / Standort Murr \[AW-220720] (12) Auftrag 1164 auch ohne Probleme reingelaufen. Mit freundlichen Grüßen / Best regards Norbert Gardemann Tel: +49 (0) 281 / 47 57 205 Mobil: +49 (0) 151/ 162 28 – 797 Von: Gardemann, Norbert Gesendet: Montag, 24. März 2025 08:46 An: Abeska, Paul Graf, Thomas Cc: Projects EMEA Betreff: AW: Freigabe AWB in MUR / Standort Murr \[AW-220720] Moin moin, ich habe Auftrag 1194 erfa...

<details>

<summary>Full conversation</summary>

```
From: Norbert Gardemann (Norbert.Gardemann@a-w.com)
To: Paul.Abeska@a-w.com, T.Graf@semcoglas.de | Date: 24.03.2025 08:54
Type: Request | 
AW: Freigabe AWB in MUR / Standort Murr [AW-220720] (12)
Auftrag 1164 auch ohne Probleme reingelaufen.
 
Mit freundlichen Grüßen / Best regards
Norbert Gardemann
Tel:  +49 (0) 281 / 47 57 205
Mobil: +49 (0) 151/ 162 28 – 797
 
 

 
Von: Gardemann, Norbert
Gesendet: Montag, 24. März 2025 08:46
An: Abeska, Paul <Paul.Abeska@a-w.com>; Graf, Thomas <T.Graf@semcoglas.de>
Cc: Projects EMEA <projects.emea@a-w.com>
Betreff: AW: Freigabe AWB in MUR / Standort Murr [AW-220720]

 
Moin moin,
 
ich habe Auftrag 1194 erfasst und der ist ohne Probleme reingelaufen 😊
 
Mit freundlichen Grüßen / Best regards
Norbert Gardemann
Tel:  +49 (0) 281 / 47 57 205
Mobil: +49 (0) 151/ 162 28 – 797
 
 

 
Von: Abeska, Paul <Paul.Abeska@a-w.com>
Gesendet: Freitag, 21. März 2025 18:29
An: Graf, Thomas <Thomas.Graf@semcoglas.de>
Cc: Gardemann, Norbert <Norbert.Gardemann@a-w.com>; Projects EMEA <projects.emea@a-w.com>
Betreff: Freigabe AWB in MUR / Standort Murr [AW-220720]

 
Hallo Thomas,
 
ich habe AWB in MUR nach bestem Wissen und Ge…
```

</details>

***

## \[AW-224469]

**Subject:** CEV: Projet Dynopt - Pré-buffer\
**Status:** New | **Category:** PS Clarity / Professional Services Clarity EMEA | **Last Action:** 20.03.2025 16:38

CEV: Projet Dynopt - Pré-buffer \[AW-224469] (2) Bonjour Christophe, J’ai bien eu ton message sur mon portable et je pense que le mieux serait d’en discuter en intégrant Xavier dans un premier temps afin de voir le concept global. Ensuite nous en discuterons avec les experts en interne et pourrons te dire ce qu’il est possible ou non de faire. Pourrais-tu organiser une réunion Teams quand tu as un moment ? Ce qui sera intéressant pour nous au cour de cette réunion c’est évidemment que tu nous exp...

<details>

<summary>Full conversation</summary>

```
From: David Cousido (David.Cousido@a-w.com)
To: Christophe.Ruaux@saint-gobain.com | Date: 20.03.2025 16:38
Type: Request | 
CEV: Projet Dynopt - Pré-buffer [AW-224469] (2)
Bonjour Christophe,
 
J’ai bien eu ton message sur mon portable et je pense que le mieux serait d’en discuter en intégrant Xavier dans un premier temps afin de voir le concept global. Ensuite nous en discuterons avec les experts en interne et pourrons te dire ce qu’il est possible ou non de faire.
 
Pourrais-tu organiser une réunion Teams quand tu as un moment ?
 
Ce qui sera intéressant pour nous au cour de cette réunion c’est évidemment que tu nous expliques ce que vous voulez faire mais également savoir si vous en avez déjà discuté avec Hegla ou un autre fournisseur de machines ? si vous avez un layout ?
 
Merci
 
Cordialement | Best regards
 
David COUSIDO
Director Business Development France
Business Unit A+W Clarity – EMEA/APAC
 

Phone:  +33 (0) 4 72 23 68 60
Email: david.cousido@a-w.com
 
A+W Software France SAS
62 Avenue des Frères Montgolfier
69740 Genas
France
 
www.a-w.com

 

Managing Directors: Peter Dixen, Julia Schmidt

This e-mail is …
```

</details>

***

## \[AW-224419]

**Subject:** Eko-Okna - delayed change of rack status in Request dialog\
**Status:** New | **Category:** PS Clarity / Professional Services Clarity EMEA | **Last Action:** 20.03.2025 13:52

Eko-Okna - delayed change of rack status in Request dialog (2) Customer complained that rack is shown in green colour in Request dialog for some time AFTER the rack had been requested and sheets are already coming from the sorter. The line goes blue eventually, but after a very long time. Z poważaniem | Best regards Patrik Pytlak Senior Consultant Professional Services A+W Clarity Phone: +48 61 438 47 45 Email: A+W Software Polska sp.z.o.o. ul. Sikorskiego 44 62-300 Wrzesn...

<details>

<summary>Full conversation</summary>

```
From: Patrik Pytlak (Patrik.Pytlak@a-w.com)
To: projects.emea@a-w.com | Date: 20.03.2025 13:52
Type: Request | 
Eko-Okna - delayed change of rack status in Request dialog (2)
Customer complained that rack is shown in green colour in Request dialog for some time AFTER the rack had been requested and sheets are already coming from the sorter. The line goes blue eventually, but after a very long time.
 

 
 
 
Z poważaniem | Best regards
 
Patrik Pytlak
Senior Consultant Professional Services
A+W Clarity
 

Phone:  +48 61 438 47 45
Email: patrik.pytlak@a-w.com
 
A+W Software Polska sp.z.o.o.
ul. Sikorskiego 44
62-300 Wrzesnia
Polska
 
www.a-w.com
```

</details>

***

## \[AW-224263]

**Subject:** A+W Enterprise - Update des zentralen Stammdatenmandanten\
**Status:** Unknown | **Category:** PS Clarity / Professional Services Clarity EMEA | **Last Action:** 20.03.2025 11:24

<details>

<summary>Full conversation</summary>

```
From: Judith Alexandra Schäfer
To: Dieter Büchsenschütz | Date: 20.03.2025 11:24
Type: | 
Ticketprojekt erstellt (4)
Ticketprojekt erstellt.
```

</details>

***

## \[AW-221712]

**Subject:** WG: A+W Schnittstelle für Lombarda Rahmenbieger - \[Ticket#1046966]\
**Status:** In Progress | **Category:** PS Clarity / Professional Services Clarity EMEA | **Last Action:** 19.03.2025 15:12

RE: \[AW-221712] WG: A+W Schnittstelle für Lombarda Rahmenbieger - \[Ticket#1046966] (6) Hallo Zusammen, Herr Fleischmann hat eine Dateiversion 3.0 gesendet. Wir haben aktuell aber schon eine Version 3.5 im Einsatz, siehe Ergebnis von Beppo. @Alfred willst Du das HErrn Fleischmann mitteilen? Ich kenne den Hintergrund der Anfrage nicht. Mit freundlichen Grüßen | Best regards Dieter Büchsenschütz ###EOM## Phone: +49 641 96620 391 A+W Software GmbH Siemensstraße 3 35463 Fernwald Germany www.a-w.com ...

<details>

<summary>Full conversation</summary>

```
From: Dieter Büchsenschütz (projects.emea@a-w.com)
To: alfred.cortisse@a-w.com, frank.christian@a-w.com | Date: 19.03.2025 15:12
Type: Answer | 
RE: [AW-221712] WG: A+W Schnittstelle für Lombarda Rahmenbieger - [Ticket#1046966] (6)
Hallo Zusammen,
Herr Fleischmann hat eine Dateiversion 3.0 gesendet.
Wir haben aktuell aber schon eine Version 3.5 im Einsatz, siehe Ergebnis von Beppo.
@Alfred willst Du das HErrn Fleischmann mitteilen? Ich kenne den Hintergrund der Anfrage nicht.
Mit freundlichen Grüßen | Best regards
Dieter Büchsenschütz
###EOM##

Phone:  +49 641 96620 391
 
A+W Software GmbH
Siemensstraße 3
35463 Fernwald
Germany

www.a-w.com

Geschäftsführer/Managing Directors: Peter Dixen, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/oder rechtlich geschützte Informationen enthalten. Sollten Sie nicht der Adressat dieser Mitteilung sein, bitten wir Sie sich mit uns in Verbindung zu setzen und diese E-Mail zu löschen. Das unerlaubte Kopieren sowie die unbefugte Weitergabe dieser E-Mail ist nicht gestattet. Selbstverständlich verwenden wir Viren-S…
```

</details>

***

## \[AW-224252]

**Subject:** RE: EKo-Okna - dostęp do środowiska testowego\
**Status:** New | **Category:** PS Clarity / Professional Services Clarity EMEA | **Last Action:** 19.03.2025 10:50

RE: EKo-Okna - dostęp do środowiska testowego (2) Dzięki Radku. Ja jednak nie mogę się zalogować na konto kornice\awkier. Mógłbyś zresetować hasło? Z poważaniem | Best regards Patrik Pytlak Senior Consultant Professional Services A+W Clarity From: Radosław Damiec Sent: środa, 19 marca 2025 09:35 To: Pytlak, Patrik Cc: Łukasz Burek Seweryn Witosz Wojciech Zaporowski

<details>

<summary>Full conversation</summary>

```
From: Patrik Pytlak (Patrik.Pytlak@a-w.com)
To: radoslaw.damiec@ekookna.pl | Date: 19.03.2025 10:50
Type: Request | 
RE: EKo-Okna - dostęp do środowiska testowego (2)
Dzięki Radku.
Ja jednak nie mogę się zalogować na konto kornice\awkier. Mógłbyś zresetować hasło?
 
Z poważaniem | Best regards
 
Patrik Pytlak
Senior Consultant Professional Services
A+W Clarity
 
From: Radosław Damiec <radoslaw.damiec@ekookna.pl>
Sent: środa, 19 marca 2025 09:35
To: Pytlak, Patrik <Patrik.Pytlak@a-w.com>
Cc: Łukasz Burek <lukasz.burek@ekookna.pl>; Seweryn Witosz <seweryn.witosz@ekookna.pl>; Wojciech Zaporowski <wojciech.zaporowski@ekookna.pl>; Blejwas, Lukasz <Lukasz.Blejwas@a-w.com>; Projects EMEA <projects.emea@a-w.com>
Subject: Re: EKo-Okna - dostęp do środowiska testowego

 
Cześć,
 

Przetestowałem, skrót na pulpicie także utworzony. Powinno wszystko działać ale w razie problemów proszę o kontakt. 

wt., 18 mar 2025 o 14:31 Pytlak, Patrik <Patrik.Pytlak@a-w.com> napisał(a):

» Cześć,
» Proszę o skonfigurowanie dostępu do środowiska testowego A+W dla Wojtka i Seweryna. Powinni oni móc się podłączyć przez RDP ze swoich komputerów do serwer…
```

</details>

***

## \[AW-223891]

**Subject:** AW: Liefertermin in AWP für Kunde vorziehen\
**Status:** New | **Category:** PS Clarity / Professional Services Clarity EMEA | **Last Action:** 19.03.2025 08:31

WG: Liefertermin in AWP für Kunde vorziehen \[AW-223891] (3) Hallo Sascha, ich habe zu diesem Punkt bei Dir nachgefragt, so wie es aussieht hat der Kunde selbst eine Lösung gefunden und wir müssen hier nichts mehr machen 😊 … ich werde das Ticket schießen … Gruß Darius Von: Beckers Daniel Gesendet: Mittwoch, 19. März 2025 08:15 An: Krol, Darius Betreff: AW: Liefertermin in AWP für Kunde vorziehen Sie erhalten nicht häufig E-Mails von beckers....

<details>

<summary>Full conversation</summary>

```
From: Darius Krol (Darius.Krol@a-w.com)
To: Sascha.Schmidt@a-w.com | Date: 19.03.2025 08:31
Type: Request | 
WG: Liefertermin in AWP für Kunde vorziehen [AW-223891] (3)
Hallo Sascha,
ich habe zu diesem Punkt bei Dir nachgefragt, so wie es aussieht hat der Kunde selbst eine Lösung gefunden und wir müssen hier nichts mehr machen 😊 … ich werde das Ticket schießen …
 
Gruß
Darius
 
Von: Beckers Daniel <beckers.daniel@kermi-design.com>
Gesendet: Mittwoch, 19. März 2025 08:15
An: Krol, Darius <Darius.Krol@a-w.com>
Betreff: AW: Liefertermin in AWP für Kunde vorziehen

 
Sie erhalten nicht häufig E-Mails von beckers.daniel@kermi-design.com. Erfahren Sie, warum dies wichtig ist

Hallo Herr Krol,
 
wir vermuten, dass wir durch diese Anpassung große Probleme bei Nachläufern erhalten werden. Dann hätte u.U. eine Position zwei verschiedene Liefertermine.

Das ist bei unseren Kunden nicht gewünscht, zudem organisieren wir derzeit unseren Versand auf Basis der Wunschliefertermin der Kunden.
Desweiteren würden die bestehenden Rückstandsauswertungen nicht passen, wenn der Liefertermin immer weiter nach vorne geschoben werden kann.
 
De…
```

</details>

***

## \[AW-224167]

**Subject:** Eko-Okna - brak szkiców PMO\
**Status:** New | **Category:** PS Clarity / Professional Services Clarity EMEA | **Last Action:** 18.03.2025 15:48

\[AW-224167] RE: błąd w stojakach (3) Szkice już są Z poważaniem | Best regards Patrik Pytlak Senior Consultant Professional Services A+W Clarity From: Danuta Chrystof Sent: czwartek, 13 marca 2025 20:30 To: Pytlak, Patrik Blejwas, Lukasz Cc: Beata Obiegała Żaneta Skowronek Wojciech Zaporowski Subject: błąd w stojakach Dzień do...

<details>

<summary>Full conversation</summary>

```
From: Patrik Pytlak (Patrik.Pytlak@a-w.com)
To: danuta.chrystof@ekookna.pl, Lukasz.Blejwas@a-w.com | Date: 18.03.2025 15:48
Type: Request | 
[AW-224167] RE: błąd w stojakach (3)
Szkice już są
 

 
Z poważaniem | Best regards
 
Patrik Pytlak
Senior Consultant Professional Services
A+W Clarity
 
From: Danuta Chrystof <danuta.chrystof@ekookna.pl>
Sent: czwartek, 13 marca 2025 20:30
To: Pytlak, Patrik <Patrik.Pytlak@a-w.com>; Blejwas, Lukasz <Lukasz.Blejwas@a-w.com>
Cc: Beata Obiegała <beata.obiegala@ekookna.pl>; Żaneta Skowronek <zaneta.skowronek@ekookna.pl>; Wojciech Zaporowski <wojciech.zaporowski@ekookna.pl>
Subject: błąd w stojakach

 
 

 

Dzień dobry,

Moment temu udostepniając laufa zauwazyłam iz nie mam grafiki na rozpisce stelaży, mimo to iz zaznaczyłam aby były:

 

 

 

 

 

 

 

 

Jak równiez optymalizacja ta mi wisi dalej w PMO:

 

 

 

 

 

Dodatkowo jeszcze jak chciałam nadac nowy nr nastepnej optymalizacji to system pozwalał mi nadac ten sam 4351.

--
Pozdrawiam / Best Regards

Danuta Chrystof

Specjalista ds. przygotowania produkcji Szyb Zespolonych Wodzisław Śl.

 
danuta…
```

</details>

***

## \[AW-224107]

**Subject:** Fehler Marktpartner-Anlage + Replikation\
**Status:** New | **Category:** PS Clarity / Professional Services Clarity EMEA | **Last Action:** 18.03.2025 10:54

Fehler Marktpartner-Anlage + Replikation (2) Hallo Frau Schmid, lange nichts voneinander gehört, ich hoffe mal sie sind gut ins neue Jahr gestartet. Wir haben diese Woche angefangen weitere Mitarbeiter auf der neuen Version arbeiten zu lassen. Dabei ist uns aufgefallen, dass die Marktpartneranlage Probleme macht. Zunächst funktioniert die Bezugnahme auf einen bestehenden Marktpartner nicht (s. Bilder). -> -> Außerdem ist danach ebenfalls aufgefallen, dass auch die Replikation nicht durchgeführt...

<details>

<summary>Full conversation</summary>

```
From: Klaas Tietjen (tietjen@frerichs-glas.de)
To: monika.schmid@a-w.com | Date: 18.03.2025 10:54
Type: Request | 
Fehler Marktpartner-Anlage + Replikation (2)
Hallo Frau Schmid,

lange nichts voneinander gehört, ich hoffe mal sie sind gut ins neue Jahr gestartet.

Wir haben diese Woche angefangen weitere Mitarbeiter auf der neuen Version arbeiten zu lassen. Dabei ist uns aufgefallen, dass die Marktpartneranlage Probleme macht. Zunächst funktioniert die Bezugnahme auf einen bestehenden Marktpartner nicht (s. Bilder).
 ->  -> 

Außerdem ist danach ebenfalls aufgefallen, dass auch die Replikation nicht durchgeführt wird.

Ein anderer Punkt der mir erst beim schreiben dieser Mail aufgefallen ist, dass wir ja keine Steuerkreis-Meetings in diesem Jahr hatten. Wie Sie ja auch daran erkennen, dass eine lange Zeit keine Fragen und Probleme unsererseits gemeldet wurden, ist das Projekt aktuell etwas in den Hintergrund gerückt worden. Ich weiß nicht, ob es dazu eine Absprache mit Herrn Cordes gab, ich war gerade nur e…
```

</details>

***

## \[AW-223932]

**Subject:** Anpassung der Crystal Reports nach Vorgabe\
**Status:** In Progress | **Category:** PS Clarity / Professional Services Clarity EMEA | **Last Action:** 18.03.2025 10:33

AW: \[AW-223932] Anpassung der Crystal Reports nach Vorgabe (2) Hallo Herr Mannhaupt, sie können die Arbeiten wie besprochen durchführen. Die Vorlagen aus dem alten System für Angebote, Rechnungen etc. sende ich Ihnen per Mail. Mit freundlichen Grüßen W. Steenebrügge GmbH & Co. KG i. V. Robert Flammersfeld Marienburger Str. 1 56566 Neuwied Tel: 0 26 31 / 83 86 - 17 Hier finden Sie unsere Datenschutzerklärung gem. DSGVO www.glas-steenebruegge.de\<http://www.glas-steenebruegge.de/datenschutzerklae...

<details>

<summary>Full conversation</summary>

```
From: Robert Flammersfeld (robert.flammersfeld@glas-steenebruegge.de)
To: projects.emea@a-w.com | Date: 18.03.2025 10:33
Type: Request | 
AW: [AW-223932] Anpassung der Crystal Reports nach Vorgabe (2)
Hallo Herr Mannhaupt,

sie können die Arbeiten wie besprochen durchführen.

Die Vorlagen aus dem alten System für Angebote, Rechnungen etc.
sende ich Ihnen per Mail.

Mit freundlichen Grüßen

W. Steenebrügge GmbH & Co. KG

i. V.
Robert Flammersfeld

Marienburger Str. 1
56566 Neuwied

Tel:   0 26 31 / 83 86 - 17

Hier finden Sie unsere Datenschutzerklärung gem. DSGVO
www.glas-steenebruegge.de<http://www.glas-steenebruegge.de/datenschutzerklaerung>
Die Information in dieser E-Mail ist vertraulich und ist ausschließlich für den Adressaten bestimmt.
Jeglicher Zugriff auf diese E-Mail durch andere Personen als den Adressaten ist untersagt.
Sollten Sie nicht der für diese E-Mail bestimmte Adressat sein, ist Ihnen jede Veröffentlichung,
Vervielfältigung oder Weitergabe wie auch das Ergreifen oder Unterlassen von Maßnahmen
im Vertrauen auf erlangte Informationen untersagt.
Angehängte Dateien unterliegen dem Copyright und dürfen ohne unsere vorherige Zustimmung
weder…
```

</details>

***

## \[AW-216440]

**Subject:** AGC KG: AGC KG: Breakage on IG Assembly / IG Out Stations with reset of ticket chain\
**Status:** Unknown | **Category:** PS Clarity / Professional Services Clarity EMEA | **Last Action:** 17.03.2025 14:08

<details>

<summary>Full conversation</summary>

```
From: Frank Christian
To: Alexander Trenin | Date: 17.03.2025 14:08
Type: State changed | 
RE: [AW-216440] AGC KG: AGC KG: Breakage on IG Assembly / IG Out Stations with reset of ticket chain (12)
```

</details>

***

## \[AW-223906]

**Subject:** WG: Ticket#1037007 — Arbeitsschritt Gehrung in Production nicht ersichtlich (Trennung über Orga)\
**Status:** New | **Category:** PS Clarity / Professional Services Clarity EMEA | **Last Action:** 17.03.2025 13:20

\[AW-223906] Support-Ticket / WG: Ticket#1037007 — Arbeitsschritt Gehrung in Production nicht ersichtlich (Trennung über Orga) (3) Sehr geehrte Damen und Herren, Vielen Dank, dass Sie sich an das A+W-Support-Team gewandt haben. Ihre Anfrage ist in unserem Ticket-System unter der Nummer \[AW-223906] und dem Stichwort "WG: Ticket#1037007 — Arbeitsschritt Gehrung in Production nicht ersichtlich (Trennung über Orga)" erfasst worden. Unser Support-Team wird sich so schnell wie möglich um die Bearbeitun...

<details>

<summary>Full conversation</summary>

```
From: Projects EMEA (projects.emea@a-w.com)
To: support.production.de@a-w.com | Date: 17.03.2025 13:20
Type: Request | 
[AW-223906] Support-Ticket / WG: Ticket#1037007 — Arbeitsschritt Gehrung in Production nicht ersichtlich (Trennung über Orga) (3)
Sehr geehrte Damen und Herren, 
Vielen Dank, dass Sie sich an das A+W-Support-Team gewandt haben.
Ihre Anfrage ist in unserem Ticket-System unter der Nummer [AW-223906] und dem Stichwort "WG: Ticket#1037007 — Arbeitsschritt Gehrung in Production nicht ersichtlich (Trennung über Orga)" erfasst worden.
 
Unser Support-Team wird sich so schnell wie möglich um die Bearbeitung Ihres Tickets kümmern.
Bei Rückfragen beziehen Sie sich bitte immer auf diese Ticket-Nummer.
 
-------------------------------------------------------------------------------------------------------------------------------
Dear Customer, 
 
Thank you for contacting A+W Support Team.
Your request has reached us and a ticket has been created automatically in our support system with ticket-number [AW-223906] and ticket subject "WG: Ticket#1037007 — Arbeitsschritt Gehrung in Production nicht ersichtlich (Trennung über Orga)".
 
We will process your request as soon as possible.
In case of any further commu…
```

</details>

***

## \[AW-216267]

**Subject:** Klärung der aktuellen Projekte( Schulungskontingent Trösch)\
**Status:** New | **Category:** PS Clarity / Professional Services Clarity EMEA | **Last Action:** 17.03.2025 10:22

AW: Kontingent von Trösch V-2025-008 V-2021-012 1.2 \[AW-216267] (12) Hallo Darius, alles klar, bin ich mit einverstanden. Danke für die Info und Gruß - Dieter Von: Krol, Darius Gesendet: Montag, 17. März 2025 10:16 An: Büchsenschütz, Dieter Cc: Abeska, Paul Projects EMEA Betreff: Kontingent von Trösch V-2025-008 V-2021-012 1.2 \[AW-216267] Hallo Dieter, ich habe eben erfahren, dass Paul die PL fü...

<details>

<summary>Full conversation</summary>

```
From: Dieter Büchsenschütz (Dieter.Buechsenschuetz@a-w.com)
To: Darius.Krol@a-w.com | Date: 17.03.2025 10:22
Type: Request | 
AW: Kontingent von Trösch V-2025-008 V-2021-012 1.2 [AW-216267] (12)
Hallo Darius,
 
alles klar, bin ich mit einverstanden.
 
Danke für die Info und Gruß - Dieter
 
Von: Krol, Darius <Darius.Krol@a-w.com>
Gesendet: Montag, 17. März 2025 10:16
An: Büchsenschütz, Dieter <Dieter.Buechsenschuetz@a-w.com>
Cc: Abeska, Paul <Paul.Abeska@a-w.com>; Projects EMEA <projects.emea@a-w.com>
Betreff: Kontingent von Trösch V-2025-008 V-2021-012 1.2 [AW-216267]

 
Hallo Dieter,
ich habe eben erfahren, dass Paul die PL für das Update bei Trösch übernimmt .. da es wenig Sinn macht die aktuellen Projekte von dem großen Update zu trennen haben wir vereinbart, dass he PL auch für die anderen Punkte übernimmt bzw. die Ansprechperson für Trösch bleibt ( er hat mich bis jetzt nur vertreten ) …  
 
Gruß
Darius
 
Mit freundlichen Grüßen
 
Darius Krol
Senior Consultant
Software Implementation
 

Phone:  +49 641 96620-0
Mobile: +49 151 16228- 799
Email: darius.krol@a-w.com 
 
A+W Software GmbH
Siemensstraße 3
35463 Fernwald
Germany
 
ww…
```

</details>

***

## \[AW-222604]

**Subject:** Informix Error beim DB Update\
**Status:** Unknown | **Category:** PS Clarity / Professional Services Clarity EMEA | **Last Action:** 13.03.2025 08:43

<details>

<summary>Full conversation</summary>

```
From: Dirk Holzapfel
To: | Date: 13.03.2025 08:43
Type: State changed | 
RE: [AW-222604] Informix Error beim DB Update (2)
Ggf. ist das Skript schon ausgeführt, bzw. die Funktion schon durchgeführt.
```

</details>

***

## \[AW-223376]

**Subject:** WG: Verifica sovra materiale taglio bolla test 1001938\
**Status:** New | **Category:** PS Clarity / Professional Services Clarity EMEA | **Last Action:** 12.03.2025 17:10

\[AW-223376] Verifica sovra materiale taglio bolla test 1001938 (3) Hello Andrea, the reason is following: the 1st picture shows pos 1 , there is (1) header and (2)+(3) processings on floats the 2st picture shows pos 2 , there is no header processing header entered and (1)+(4) processings on floats , because its entered twice(wrong) . in the 2nd position the AWP calculates only (1) and (2), other ones will be ignored. Conclusion: the order entry has to be in “balance” with production system to ...

<details>

<summary>Full conversation</summary>

```
From: Ilja Scheinker (Ilja.Scheinker@a-w.com)
To: a.vergori@galvolux.com | Date: 12.03.2025 17:10
Type: Request | 
[AW-223376] Verifica sovra materiale taglio bolla test 1001938 (3)
Hello Andrea,
 
the reason is following:
the 1st picture shows pos 1 , there is (1)  header and (2)+(3) processings on floats
the 2st picture shows pos 2 , there is no header processing  header entered and (1)+(4) processings on floats , because its entered twice(wrong) .
in the 2nd position the AWP calculates only (1) and (2), other ones will be ignored.
 
Conclusion: the order entry has to be in “balance” with production system to be able to work with a new way.
 
àPlease let Gabriella change this order in the old matter to do not produce wrong glas.
 
 

 

 
Mit freundlichen Grüßen | Best regards
Ilja Scheinker
 

Phone:  +49 641 96620-391
Email: ilja.scheinker@a-w.com
 
Siemensstraße 3
35463 Fernwald
Germany
 
www.a-w.com

 
 
Geschäftsführer/Managing Directors: Peter Dixen, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963

This e-mail is for the intended recipient only and may contain …
```

</details>

***

## \[AW-223363]

**Subject:** WG: Neue Dynopt\
**Status:** New | **Category:** PS Clarity / Professional Services Clarity EMEA | **Last Action:** 12.03.2025 14:43

WG: Neue Dynopt (1) Moin Stefan, darf ich Dir das geben ? Mit freundlichen Grüßen | Best regards Andreas Schwarz Consultant Customer Support Business Unit A+W Clarity Phone: +49 641 96620-392 Mobile: Email: A+W Software GmbH Siemensstraße 3 35463 Fernwald Germany www.a-w.com Geschäftsführer/Managing Directors: Peter Dixen, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan Amtsgericht Gießen/Gießen Local Court: HRB 7963 This e-mail is for the intended recipient on...

<details>

<summary>Full conversation</summary>

```
From: Andreas Schwarz
To: Stefan Beppler | Date: 12.03.2025 14:43
Type: Request | 
WG: Neue Dynopt (1)
Moin Stefan,
 
darf ich Dir das geben ?

 
Mit freundlichen Grüßen | Best regards
 
Andreas Schwarz
Consultant Customer Support
Business Unit A+W Clarity
 

Phone:  +49 641 96620-392
Mobile:
Email: andreas.schwarz@a-w.com
 
A+W Software GmbH
Siemensstraße 3
35463 Fernwald
Germany
 
www.a-w.com

Geschäftsführer/Managing Directors: Peter Dixen, Julia Schmidt, Dennis Tiegs, Mark Thompson, Tyler O‘Hagan
Amtsgericht Gießen/Gießen Local Court: HRB 7963

This e-mail is for the intended recipient only and may contain confidential and/or legally protected information. If you have received it by mistake please contact us and delete it from your system. Copying as well as unauthorized relaying is strictly prohibited. Of course we use anti virus programs. Should a virus have reached your system through this e-mail we do not accept any liability for damages resulting from it.
 
Diese E-Mail ist ausschließlich für den Adressaten bestimmt und kann vertrauliche und/ode…
```

</details>

***

## \[AW-223338]

**Subject:** RE: REPONSE DE OPTIMA\
**Status:** New | **Category:** PS Clarity / Professional Services Clarity EMEA | **Last Action:** 12.03.2025 13:37

RE: REPONSE DE OPTIMA (2) Bonjour Mr David,Vous allez bien?Si hous pourriez me rappeler svp Merci.Cordialement.SafdarEnvoyé de mon mobile -------- Message d'origine --------De : "Cousido, David" Date : 10/03/2025 19:34 (GMT+04:00) À : hassambay "projects.ga" Objet : RE: REPONSE DE OPTIMA Bonjour, Je pense que l’option 1 suffira pour charger nos optimisations directement sur les tables de découpe. David De : hassambay \<has...

<details>

<summary>Full conversation</summary>

```
From: Safdar Hassambay (hassambay@miroglass.net)
To: David.Cousido@a-w.com, projects.ga@a-w.com | Date: 12.03.2025 13:37
Type: Request | 
RE: REPONSE DE OPTIMA (2)
 Bonjour Mr David,Vous allez bien?Si hous pourriez me rappeler svp Merci.Cordialement.SafdarEnvoyé de mon mobile
-------- Message d'origine --------De : "Cousido, David" <David.Cousido@a-w.com> Date : 10/03/2025  19:34  (GMT+04:00) À : hassambay <hassambay@miroglass.net>, "projects.ga" <projects.ga@a-w.com> Objet : RE: REPONSE DE OPTIMA

Bonjour,
 
Je pense que l’option 1 suffira pour charger nos optimisations directement sur les tables de découpe.
 
David
 

De : hassambay <hassambay@miroglass.net>

Envoyé : vendredi 7 mars 2025 12:39
À : Cousido, David <David.Cousido@a-w.com>; projects.ga <projects.ga@a-w.com>
Objet : RE: REPONSE DE OPTIMA

 
Bonjour David,
 
Voici les deux propositions qu’il m’a transmis.
 
Vous lire.
 
 

 

Cordialement / Best regards,

SAFDAR HASSAMBAY |
Président

hassambay@miroglass.net
+262 692 67 22 28
+262 262 42 01 54
2 bis rue Charles Darwin 
ZAC 2000 – 97420 LE PORT REUNION

Miroglass : 32 ans de vitrages innovants et décoratifs à La…
```

</details>

***

## \[AW-222855]

**Subject:** GLS: Additional access to Guacamole\
**Status:** In Progress | **Category:** PS Clarity / Professional Services Clarity EMEA | **Last Action:** 11.03.2025 16:01

RE: GLS: Accès complémentaires Guacamole \[AW-222855] (6) David, OK, bien noté pour Abdallah 😉 Tous les autres comptes sont créés sur la nouvelle infra tels que : - Nigar ANUM M001\ext.nanum - Tayyab AFTAB M001\ext.taftab - Mughees AHSAN M001\ext.mahsan - Ahmed AMIN M001\ext.aamin \* Holger NEISES M001\ext.hneises \* Frank CHRISTIAN M001\ext.fchristian A+ Cyril ROUSSELOT Service informatique IT BUMI Mob.: + 33 7 88 27 95...

<details>

<summary>Full conversation</summary>

```
From: Rousselot, Cyril (Cyril.Rousselot@saint-gobain.com)
To: David.Cousido@a-w.com | Date: 11.03.2025 16:01
Type: Request | 
RE: GLS: Accès complémentaires Guacamole [AW-222855] (6)
David,

OK, bien noté pour Abdallah 😉
Tous les autres comptes sont créés sur la nouvelle infra tels que :

              - Nigar ANUM                  M001\ext.nanum
- Tayyab AFTAB              M001\ext.taftab
- Mughees AHSAN        M001\ext.mahsan
- Ahmed AMIN                M001\ext.aamin

 *   Holger NEISES               M001\ext.hneises
 *   Frank CHRISTIAN          M001\ext.fchristian

A+

Cyril ROUSSELOT
 Service informatique IT BUMI

Mob.: + 33 7 88 27 95 73
Tel.: (+33) 5 49 82 06 23
cyril.rousselot@saint-gobain.com<mailto:cyril.rousselot@saint-gobain.com>
GLASSOLUTIONS BUMI
Glassver
ZI Le Vivier
79700, St-Pierre-Des-Echaubrognes
France
www.saint-gobain-glass.fr<http://www.saint-gobain-glass.fr/>

De : Cousido, David <David.Cousido@a-w.com>
Envoyé : mardi 11 mars 2025 13:22
À : Rousselot, Cyril <Cyril.Rousselot@saint-gobain.com>
C…
```

</details>

***

(continued in next part)
