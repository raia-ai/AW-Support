---
description: "EN CONFIG QR Code Integration"
---



# EN CONFIG QR Code Integration

     Configuration


QR Code Integration




                             english




                      - INTERN -
Änderungshistorie

Date      Author    Modification/remarks                     Version
27.01.2015 DLA      First draft (after experience from AS)   1.0
11.05.2022 PK       Update for new fonts and parameter       2.0
20.05.2022 PK       Configuration A+W Production             3.0
11.10.2023 PK       Update for SMC                           4.0
Content

1.   What is a QR Code?                                               4
2.   Installation                                                     5
3.   Usage in Crystal Reports                                         6
     3.1. Example Code                                                6
     3.2. Parameter                                                   6
          3.2.1. DataToEncode                                         6
          3.2.2. ProcTilde                                            6
          3.2.3. EncMode                                              7
          3.2.4. Version                                              7
          3.2.5. ErrorCorrectionLevel                                 7
          3.2.6. BestMask                                             8
          3.2.7. QuietZone                                            8
     3.3. Swiss Cross                                                 8
4.   Usage in A+W Production                                         10
     4.1. Prerequisites                                              10
     4.2. Barcoding Masterdata                                       10
     4.3. QR Code Scanner                                            11
     4.4. A+W Production Terminal                                    12
     4.5. A+W Smart Companion                                        12




A+W Software GmbH               EN-CONFIG-QR Code Integration.docx        3
1. What is a QR Code?
http://de.wikipedia.org/wiki/QR-Code
http://en.wikipedia.org/wiki/QR_code




A+W Software GmbH              EN-CONFIG-QR Code Integration.docx   4
2. Installation
In standard package of A+W products there is only one font package for linear barcodes. To create
a QR code, the “Reporting Extension”:


 786010       QR Barcode Integration


Need to be purchased from A+W.
Necessary Setup: “A+W IDAutomation QR Code”
After the installation there are 2 new functions in the Crystal Reports (in “COM- und .NET-UFLs
(u212com.dll))”:
    •   IDAutomationQRCodeEncoderQRSet
    •   IDAutomationQRCodeEncoderQRGet




A+W Software GmbH                EN-CONFIG-QR Code Integration.docx                               5
3. Usage in Crystal Reports
3.1. Example Code
        stringVar DataToEncode:= "{Database-fields};
        numberVar ProcTilde := 1;
        numberVar EncMode := 0;
        numberVar Version := 0;
        numberVar ErrorCorrectionLevel := 0;
        numberVar BestMask := 0;
        numberVar QuietZone := 0;


        stringVar CompleteBarcodeString:="";
        numberVar i:=0;
        numberVar Segments:= IDAutomationQRCodeEncoderQRSet(DataToEncode, ProcTilde,
        EncMode, Version, ErrorCorrectionLevel, BestMask, QuietZone);
        For i:=0 to Segments Do
        (
        CompleteBarcodeString := CompleteBarcodeString +
        IDAutomationQRCodeEncoderQRGet(i);
        );
        CompleteBarcodeString


Finally, include the formula on the report with the new TrueType-Font „IDAutomation2D“.


3.2. Parameter
3.2.1. DataToEncode
This text parameter contains the content of the QR code. As more content in the code, as larger
the code will be at the end and die decoding in the scanner takes longer!


3.2.2. ProcTilde
This parameter need to set to 1 if there are any control characters use within the QR code, such as
    •   ~1 represents the GS1 FNC1 in first position (in supporting products).
    •   ~2 represents the AIM FNC1 in second position (in supporting products).



A+W Software GmbH                 EN-CONFIG-QR Code Integration.docx                              6
    •   ~CO is a center override function → see also chapter about the “swiss cross”
    •   ^| enables TLV (Tag-Length-Value) encoding. When the first two characters are ^| TLV
        values separated by | are encoded.
    •   | enables TLV in Base64 encoding. This allows TLV fields to be encoded in Base64 when
        the first character is |. For example:
    •   |IDAutomation|123456789012345|2022-11-30 06:04:31|92435.33|2692.22″
    •   = enables Base 64 encoding. When the first character is “=” all data is encoded in Base64.
    •   ~dNNN represents the ASCII character encoded by the 3 digits NNN.
               o   For example:
                   ~d009 represents a tab,
                   ~d013 represents a return,
                   ~d029 represents the <GS> character and
                   ~d065 represents the character ‘A’.


3.2.3. EncMode
Defines the content of the QR Code.
    •   0 = Byte (default - most used)
    •   1=Alpha-Numeric (Encodes only numbers, uppercase letters, the space and the following
        symbols (&%*+-./:)
    •   2 = Numeric (Encodes only numbers)
Even if the mode “Byte” is the most common one, the other modes can make the QR Code a bit
smaller.
Choosing the correct encoding mode and the lowest error correction of “L” (or parameter 2) will
help ensure the symbol size is as small as possible.


3.2.4. Version
Define the size of the QR Code
    •   0 = automatic (default)
    •   1 = 21x21
    •   ....
    •   40 = 177x177


3.2.5. ErrorCorrectionLevel
The error correction levels allow verification of data and recovery in the event that part of the
symbol is damaged. Increasing the error correction level increases the symbol size and reduces
data capacity.
    •   0:M = 15% (default - most used)
    •   1:H = 30%


A+W Software GmbH                 EN-CONFIG-QR Code Integration.docx                                7
    •   2:L = 7%
    •   3:Q = 25%


3.2.6. BestMask
0 = default
The mask pattern determines which modules are dark and which are light to make it as easy as
possible for a QR Code scanner to decode the data.


3.2.7. QuietZone
0 = default
According to the specification, a quiet zone of four times the size of one module is required on all
sides of the QR Code symbol. The quiet zone should be the same color as the background within
the symbol.


3.3. Swiss Cross
In Switzerland invoices need to have the swiss cross in the middle of the barcode. This can be
achieved, by raising up the ErrorCorrectionLevel (makes the QR Code larger) and put a jpg in the
middle of the code.




But our code-fonts from IDAutomation have also a functionality to place this swiss cross (or other
pictures in the middle of the code.
This functionality is called “Center Overwrite Function” (see also chapter “ProcTilde”). The
necessary “~CO” string should be placed at the very end of the data being encoded:
Example:
stringVar DataToEncode:= "123456789-Swiss Cross " & "~CO77,007C6C446C7C00";
To calculate this “~CO” String, there is an Excel available. The Excel-Sheet and an example report
can be downloaded from here.


Hint:
With this example, it was possible to create the QR Code from above, but it was not readably by
several scanners. Reason: the ratio between size of the code and size of the swiss cross was in a
bad relationship. So, there are 3 ways getting out of that problem:
    •   Set the parameter “Version” to a higher value. This lead to a larger QR Code, by same size
        of the swiss cross
    •   Put more content into the encoded data (lead also to a larger QR Code)


A+W Software GmbH                 EN-CONFIG-QR Code Integration.docx                                 8
   •   Increase the parameter “ErrorCorrectionLevel” – of course this also lead to a larger QR
       Code.




A+W Software GmbH               EN-CONFIG-QR Code Integration.docx                               9
4. Usage in A+W Production
4.1. Prerequisites
In principle, QR codes can be processed in A+W Production. You only have to make sure that the
content of the QR Code is writable by a regular expression. In addition, the QR Code must contain
the label number with which the A+W Production will later work. All other information contained
in the QR Code will be truncated and not used further.
Additionally, the script awupdate_alcim_Nr.389903_-1_-1.xml must be executed for the new
master data table awbar_barcodetypes to exist


More information about this, you can find in the release notes to the following AWDesk Cases (in
DevOps Wiki!):


229434: Alphanumerische Gestellbarcodes (Feature)
389903: A+W Production Terminal – Custom barcodes (Feature)
443290: Verwendung der Barcodes von Gestellpool Europe in A+W Production (Feature)


4.2. Barcoding Masterdata
A new entry must be created in the awbar_barcodetypes table.


Column Description awbar_barcodetypen
 Column                Description
 Nummer                increasing number for the entries. So if the last number is 2, the next
                       value should be 3
 Typ                   0; always the same for sheets
 Name                  EINHEIT; always the same for sheets
 Laenge                Length of the sheetbarcode
 Pruefziffer           0 = there is no checkdigit to be checked by the scanner
                       1 = there is a checkdigit to be checked by the scanner (only WLAN CE-
                       Scanner)
 Codetyp               0; Irrelevant
 Status                0; always the same
 Regex                 0 = column “prefix” is used as barcode-prefix
                       1 = column “prefix” is used as regular expression
 Praefix               prefix or regular expression depending on column “regex”



A+W Software GmbH                EN-CONFIG-QR Code Integration.docx                              10
 Ersetzungsmuster        Define the part of the praefix, which is used from the QR Code


Example (for sheet-barcode):
       Praefix =         "(0[0-9]{8})( *- *)(.*)"
                              •   the praefix is grouped with brackets into 3 groups
                              •   first group describes out etikettnr (only numbers, 8 digits)
                              •   second group is just a delimiter between etikettnr and other
                                  content (optional)
                              •   third group means: everything and unlimited amount of
                                  characters
       Ersetzungsmuster = “$1”
               ($1 means, that only the first group (or etikettnr) is used and everything else will
       be truncated)


Content of the QR Code:
       000071046 – Order: 2609 – Pos: 1 – PartNo: 0
                     ▪   Only the yellow part is used


New entry (only as example; finally, it depends on the content of the QR Code!):
       insert into awbar_barcodetypen (nummer, typ, name, laenge, pruefziffer, codetyp, status,
       regex, praefix, ersetzungsmuster)
        values (2, 1, 'EINHEIT', 9,0,0,0,1,'(0[0-9]{8})( *- *)(.*)','$1');


4.3. QR Code Scanner
Of course, the setting of the scanner depends on the manufacturer and scanner type. We’ve
tested our system with the Datalogic Gryphon GM4500 (which is on the pricelist) and it is possible
to configure this scanner, just with the following configuration code:




A+W Software GmbH                  EN-CONFIG-QR Code Integration.docx                             11
Communication Interface: USB KBD, Keyboard Country Mode: German, Aztec Code
Enable/Disable: Disable, Data Matrix Enable/Disable: Disable, PDF 417 Enable/Disable: Disable, QR
Code ECI Identifier transmission Enable/Disable: Disable, Global Prefix:
5300000000000000000000000000000000000000
~3$P,HA35,CKBCO05,CAZEN00,CDMEN00,CP4EN00,CQRET00,
CLFPR5300000000000000000000000000000000000000,P<CR>


4.4. A+W Production Terminal
To connect a USB QR Code scanner to a A+W Production Terminal, you need the following
settings:




The language has to match to the language which is setup in the scanner!


4.5. A+W Smart Companion
The A+W Smart Companion is also now able to read the QR Codes. The QR code must also be set
with a regular expression in the infrastructure.web. Details can be found in the configuration
manual of the A+W Smart Companion.
The entry here might look something like this:
{
     "$type":
“AWSOA.Infrastructure.Config.ServiceContracts.DataTransferObject.BarcodeClassificationDto,
AWSOA.Infrastructure.Config.ServiceContracts",
       "Sequence": 19,
       "BarcodeType": 5,
       "BarcodeSymbology": 256,
       "Application": 1,
       "RegularExpression": "^(0[0-9]{8})( *- *)(.*)$",
       "Substitution": "$1",
       "Description": "QR Product Barcode"
},




A+W Software GmbH                EN-CONFIG-QR Code Integration.docx                           12

