---
description: "AUW_Configuration_HEGLA_Remaster"
---
 | --- | --- | --- | | 08.06.2012 | Eike Luh | Issue first release
  | 1.0 | | 26.02.2019 | Peter Kühn | Add information about TCP IT communication |
  1.1 | Content ## Introduction The Hegla Remaster system has become one of the most
  efficient systems out there in the market to be able to reduce glass yields in very
  efficient und uncomplicated way. The installation process is also pretty easy as
  you will see within the next chapter. ## ReMaster Installation'
long_description: 'Configuration HEGLA ReMaster History | Date | Author | Modification/remarks
  | Version | | --- | --- | --- | --- | | 08.06.2012 | Eike Luh | Issue first release
  | 1.0 | | 26.02.2019 | Peter Kühn | Add information about TCP IT communication |
  1.1 | Content ## Introduction The Hegla Remaster system has become one of the most
  efficient systems out there in the market to be able to reduce glass yields in very
  efficient und uncomplicated way. The installation process is also pretty easy as
  you will see within the next chapter. ## ReMaster Installation The ReMaster module
  is part of the setup XStockmaster. In addition to that you will need to get a revised
  license file that has the ReMaster license included. Please make sure you select
  the XStockMaster module out of the installation tree during the XOPT-ON installation
  since it needs to be installed on the XOPT-ON machine in order to be able to communicate
  to the ReMaster Server. Once installed there are a couple of areas that need to
  be tweaked: a) DCOM settings (are handled in a separate document) b) XRemasterEditor.INI
  and XStockMaster.INI c) Xopton.cfg b) Within the xremastereditor.ini you can specify
  language and server information as to where the main ReMaster application is running.
  The editor will allow you to view and edit the contents of the ReMaster. ### XRemasterEditor.INI
  [COMMON] Language=gb ServerName=HEGLA ; ; #167048: Several columns in list are now
  configureable ;Show_DoppelOpt=No ;Show_InclusionTime=Yes ;Show_Priority=Yes [DIMENSIONS]
  ; 0=mm, 1=1/32 inch, 2=0.1 mm Measurement=1 ### XStockMaster.INI This file is mainly
  used on the ReMaster Server itself which is the Hegla PC – so on the A+W side it
  doesn’t need to be configured. [GLOBALS] Language=gb ; Mode=1 1=HEGLA (Remaster)
  DefaultDataFileName=Remaster.dat ; Default data filename, for example for HEGLA:
  Remaster.dat DataFilePath=%ALLUSERSPROFILE%\A+W\Techsoft\Remaster\ ; Path for the
  DataFileName [DIMENSIONS] ; 0=mm, 1=1/32 inch, 2=0.1 mm Length/Height=1 Thickness=1
  ### Xopton.cfg The settings themselves are documented pretty well within the xopton.cfg
  so I will just point out the key ones you will have to do. - Remaster=Y turns on
  the Remaster function itself - Remaster1= Heg1, HEGLA ALCIM table name and name
  of the Remaster server (Hegla PC) - MinremasterLength=1270 value is in mm even for
  the inch version – defines the minimum width as to when the ReMaster will store
  a piece or when it is considered waste. [Remaster] Remaster=Y NumberOfRemasters=1
  Remaster1=HEG1,HEGLA ;Remaster2=HEVG,PC-Name2 RemasterMode=0 MaxRemasterPlatesToUse=10
  MinRemasterLength=1270 SortAscending=N UseArticleCodeForRemaster=Y HeglaArticleCodeIsLeftJustified=Y
  RemasterDim=1 ; 0=mm, 1=1/32 inch, 2=0.1 mm CheckGlassArticle=N ;NumberOfRemasterGlasArticle=3
  ;----- Use this Format for the Hegla Remaster with Hegla Articlecode ;-----See also
  the description of this section. ;GlassArticle0=01003-1270 ;GlassArticle1=00206-1000
  ;GlassArticle2=02010-1000 ;-Use this Format if the flag ''UseArticleCodeForRemaster=N''
  is set. ;-Then you don''t need any Articlecode in Masterdata. The Articlcode ;-or
  the XStockmaster will be created by GLASART*DICKE from table ;-XOPT_ART. See also
  the description of this section. ;GlassArticle0=30000 ;GlassArticle1=100003*6000-500
  ;GlassArticle2=100003*10000-500 UseRemasterForResidualPlate=N ShowInfoForResidualPlate=Y
  ;MinNewResidualLength= ;MaxResidualLengthToUse ShowTimeStamp=0 ### Remaster with
  TCP/IP To run the Hegla Remaster with a TCP/IP communication (instead of DCOM),
  there are several setting'
---

Configuration HEGLA ReMaster

History

| Date | Author | Modification/remarks | Version |
| --- | --- | --- | --- |
| 08.06.2012 | Eike Luh | Issue first release | 1.0 |
| 26.02.2019 | Peter Kühn | Add information about TCP IT communication | 1.1 |

Content

## Introduction

The Hegla Remaster system has become one of the most efficient systems out there in the market to be able to reduce glass yields in very efficient und uncomplicated way.

The installation process is also pretty easy as you will see within the next chapter.

## ReMaster Installation

The ReMaster module is part of the setup XStockmaster.

In addition to that you will need to get a revised license file that has the ReMaster license included. Please make sure you select the XStockMaster module out of the installation tree during the XOPT-ON installation since it needs to be installed on the XOPT-ON machine in order to be able to communicate to the ReMaster Server.

Once installed there are a couple of areas that need to be tweaked:

a) DCOM settings (are handled in a separate document)

b) XRemasterEditor.INI and XStockMaster.INI

c) Xopton.cfg

b) Within the xremastereditor.ini you can specify language and server information as to where the main ReMaster application is running. The editor will allow you to view and edit the contents of the ReMaster.

### XRemasterEditor.INI

[COMMON]

Language=gb

ServerName=HEGLA

;

; #167048: Several columns in list are now configureable

;Show_DoppelOpt=No

;Show_InclusionTime=Yes

;Show_Priority=Yes

[DIMENSIONS]

; 0=mm, 1=1/32 inch, 2=0.1 mm

Measurement=1

### XStockMaster.INI

This file is mainly used on the ReMaster Server itself which is the Hegla PC – so on the A+W side it doesn’t need to be configured.

[GLOBALS]

Language=gb

;

Mode=1

1=HEGLA (Remaster)

DefaultDataFileName=Remaster.dat

; Default data filename, for example for HEGLA: Remaster.dat

DataFilePath=%ALLUSERSPROFILE%\A+W\Techsoft\Remaster\

; Path for the DataFileName

[DIMENSIONS]

; 0=mm, 1=1/32 inch, 2=0.1 mm

Length/Height=1

Thickness=1

### Xopton.cfg

The settings themselves are documented pretty well within the xopton.cfg so I will just point out the key ones you will have to do.

- Remaster=Y
turns on the Remaster function itself

- Remaster1= Heg1, HEGLA
ALCIM table name and name of the Remaster server (Hegla PC)

- MinremasterLength=1270
value is in mm even for the inch version – defines the minimum width as to when the ReMaster will store a piece or when it is considered waste.

[Remaster]

Remaster=Y

NumberOfRemasters=1

Remaster1=HEG1,HEGLA

;Remaster2=HEVG,PC-Name2

RemasterMode=0

MaxRemasterPlatesToUse=10

MinRemasterLength=1270

SortAscending=N

UseArticleCodeForRemaster=Y

HeglaArticleCodeIsLeftJustified=Y

RemasterDim=1

; 0=mm, 1=1/32 inch, 2=0.1 mm

CheckGlassArticle=N

;NumberOfRemasterGlasArticle=3

;----- Use this Format for the Hegla Remaster with Hegla Articlecode

;-----See also the description of this section.

;GlassArticle0=01003-1270

;GlassArticle1=00206-1000

;GlassArticle2=02010-1000

;-Use this Format if the flag 'UseArticleCodeForRemaster=N' is set.

;-Then you don't need any Articlecode in Masterdata. The Articlcode

;-or the XStockmaster will be created by GLASART*DICKE from table

;-XOPT_ART. See also the description of this section.

;GlassArticle0=30000

;GlassArticle1=100003*6000-500

;GlassArticle2=100003*10000-500

UseRemasterForResidualPlate=N

ShowInfoForResidualPlate=Y

;MinNewResidualLength=

;MaxResidualLengthToUse

ShowTimeStamp=0

### Remaster with TCP/IP

To run the Hegla Remaster with a TCP/IP communication (instead of DCOM), there are several setting s necessary.

### XT_rcutf32

[Options]

UseXMLHeader=Y

### Opt2TXT

Record 98 Byte 34 = 1

Plate ID in NC Header (AW172664)

Record 98 Byte 46 = 1

Cutcode with a XML Header

### Xopton.cfg

[REMASTER]

Remastermode = 4

Remaster1=TB1,172.17.41.11,10010,5

Where:

TB1 = Tablename

172.17.41.11 = IP Address to the Remaster

10010 = Portnumber

5 = Client ID

You can get these Values if you click on the Remaster Server on the Hegla icon in the taskbar:

## Facts in and around Xopton & ReMaster

- The content of the Hegla ReMaster is not stored in any ALCIM database table so there is unfortunately no way of creating a Crystal report showing the contents.

- The contents of the ReMaster cannot be accessed during detail scheduling from ALCIM – the only way to access it is through xopt-on via a table optimization

### Other ReMaster Systems

Besides the Hegla ReMaster system Bystronic had developed one of their own which was mainly used with their vertical cutting table. Unfortunately their only exist about two or three installs of these tables worldwide. One is in Switzerland and the other one in the United States (Salt Lake City) – this one is actually our customer. I believe the third one was installed in Florida but as far as I know the company went out of business. The configuration is very similar to the one used for the Hegla ReMaster.

Despite being mainly used for the Vertical Cutting tables which Bystronic stopped producing due to too many issues the Bystronic version of the Remaster can also be used for any regular table. I haven’t seen this in that configuration yet and the fact that Bystronic and & Hegla have merged their cutting table operation I will doubt that we will ever see any new installations of that.
