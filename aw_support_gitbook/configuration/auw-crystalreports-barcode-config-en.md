---
title: "AUW_Configuration_Barcode_CrystalReports"
source: "AUW_Configuration_Barcode_CrystalReports.docx"
tags: ["Crystal Reports", "Barcode", "Configuration", "AUW", "Report Design", "Barcode Font", "SAP Crystal Reports", "Printing", "Technical Guide"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "Barcodes with CrystalReports History Content IDAutomation A+W has licensed the IDAutomation package “TrueType 1D Barcode Font Package” in our software. In this package we have function for Interleave 2/5 Barcodes which we use in our Software. Other barcode function are part of other packages. If a customer needs this he can buy it, but he can’t get support from A+W for this. Universal Barcode Font Package: includes e.g. IDAutomation_Uni_C128 or IDAutomation_Uni_C128C QR Code Font & Encoder Suite: includes e.g. IDAutomationQRCodeEncoderQRSet This information may be outdated, check for actual information. In Crystal Reports use our functions AWIDAutomationWrapper+. In this function we"
long_description: "Barcodes with CrystalReports History Content IDAutomation A+W has licensed the IDAutomation package “TrueType 1D Barcode Font Package” in our software. In this package we have function for Interleave 2/5 Barcodes which we use in our Software. Other barcode function are part of other packages. If a customer needs this he can buy it, but he can’t get support from A+W for this. Universal Barcode Font Package: includes e.g. IDAutomation_Uni_C128 or IDAutomation_Uni_C128C QR Code Font & Encoder Suite: includes e.g. IDAutomationQRCodeEncoderQRSet This information may be outdated, check for actual information. In Crystal Reports use our functions AWIDAutomationWrapper+. In this function we execute the IDAutomation functions and write a trace files in our trace structure. This will help our support. Interleave 2of5 with IDAutomation Since version 6.2 we provide a new Crystal-Report runtime and a new font-package from IDAutomation. The new Crystal Report runtime was necessary, because SAP solved some serious bugs in the runtime, and we can only open a service case at SAP, when we use the latest version. To change the fonts from IDAutomation the reason was similar. Our old font is out of maintenance and in some cases the checkdigit of the barcode will be calculated wrong, so that the barcode isn’t readable. (see: ) Behaviour with CrystalReports Runtime 2008 Behaviour with CrystalReports Runtime 2013 QR Code with IDAutomation **What is a QR Code?** How can a QR Code printed on a report? The in A+W products embedded IDAutomation barcode functions does not include QR codes. If a customer wants to use them, they must to purchase a separate license directly from IDAutomation for its company. He gets an installation package from IDAutomation with the font and a DLL that can be accessed via CrystalReports. **A+W will not give support for such a solution!** **Demo version: **License** version: Download and install the ZIP-File of IDAutomation. In the demo version the file has the name „IDAutomation_QRCodeWindowsFontEncoderDEMO.exe“. In CrystalReports you find now 2 additional functions in “COM- und.NET-UFLs (u212com.dll)”: IDAutomationQRCodeEncoderQRSet IDAutomationQRCodeEncoderQRGet Enter a new CrystalReports formula with the following syntax: stringVar DataToEncode:= {Datenbankfeld}; stringVar CompleteBarcodeString:=\"\"; numberVar i:=0; numberVar Segments:= IDAutomationQRCodeEncoderQRSet(DataToEncode,0,0,0,0 ); For i:=0 to Segments Do ( CompleteBarcodeString:= CompleteBarcodeString + IDAutomationQRCodeEncoderQRGet(i); ); CompleteBarcodeString Finally, include the formula on the report with the new TrueType-Font „IDAutomation2D“. Parameter of function IDAutomationQRCodeEncoderQRSet Parameter of function IDAutomationQRCodeEncoderQRSet (<Data>, <Process Tilde>, <Error Correction>, <Encoding Mode>, <Version>): Process Tilde: 1 = True; Ehen true, ~d013 = return and ~d009=tab Error Correction: 0=M, 1=H, 2=L and 3=Q Encoding Mode: 0=Byte, 1=Alpha-Numeric and 2=Numeric Version: 0=Auto Tools Calculate Checksum for an Interleave 2/5 Barcode Wirth the follow INFORMIX Function you can calculate the checksum of your Interleave 2/5 Barcode with 9 digits. CREATE FUNCTION cu_CheckSumInterleaved2of5 (spBarcode CHAR(9)) RETURNING CHAR(1); DEFINE spDigit CHAR(1); DEFINE spChecksum CHAR(1); DEFINE spCounter, spSum INTEGER; LET spSum = 0; IF LENGTH(spBarcode) = 9 THEN FOR spCounter = 1 TO LENGTH(spBarcode) STEP 1 LET spDigit=SUBSTR(spBarcode, spCounter, 1); --rechnet die Summe von allen Zeichen mit Koeffizienten LET spSum=spSum + (1+2*MOD(spCounter,2))*spDigit;"
---

## Barcodes with CrystalReports

## History

| Date | Author | Modification/remarks | Version |
| --- | --- | --- | --- |
| 27.01.2015 | DLA | QR Code (nach Erfahrungen von AS) | 1.0 |
| 06.12.2017 | DLA | Unsere Standard Barcodes | 1.1 |
| 24.01.2018 | DLA | Beispiel CODE128 in CR | 1.2 |
|  |  |  |  |

## Content

## IDAutomation

A+W has licensed the IDAutomation package “TrueType 1D Barcode Font Package” in our software. In this package we have function for Interleave 2/5 Barcodes which we use in our Software.

Other barcode function are part of other packages. If a customer needs this he can buy it, but he can’t get support from A+W for this.

Universal Barcode Font Package: includes e.g. IDAutomation_Uni_C128 or IDAutomation_Uni_C128C

QR Code Font & Encoder Suite: includes e.g. IDAutomationQRCodeEncoderQRSet

This information may be outdated, check  for actual information.

In Crystal Reports use our functions AWIDAutomationWrapper+. In this function we execute the IDAutomation functions and write a trace files in our trace structure. This will help our support.

## Interleave 2of5 with IDAutomation

Since version 6.2 we provide a new Crystal-Report runtime and a new font-package from IDAutomation.

The new Crystal Report runtime was necessary, because SAP solved some serious bugs in the runtime, and we can only open a service case at SAP, when we use the latest version.

To change the fonts from IDAutomation the reason was similar. Our old font is out of maintenance and in some cases the checkdigit of the barcode will be calculated wrong, so that the barcode isn’t readable.
(see:  )

### Behaviour with CrystalReports Runtime 2008

### Behaviour with CrystalReports Runtime 2013

## QR Code with IDAutomation

**What is a QR Code?**

### How can a QR Code printed on a report?

The in A+W products embedded IDAutomation barcode functions does not include QR codes. If a customer wants to use them, they must to purchase a separate license directly from IDAutomation for its company. He gets an installation package from IDAutomation with the font and a DLL that can be accessed via CrystalReports. **A+W will not give support for such a solution!**

**Demo version:

**License** version:

Download and install the ZIP-File of IDAutomation. In the demo version the file has the name „IDAutomation_QRCodeWindowsFontEncoderDEMO.exe“.

In CrystalReports you find now 2 additional functions in “COM- und.NET-UFLs (u212com.dll)”:

- IDAutomationQRCodeEncoderQRSet

- IDAutomationQRCodeEncoderQRGet

Enter a new CrystalReports formula with the following syntax:

stringVar DataToEncode:= {Datenbankfeld};

stringVar CompleteBarcodeString:="";

numberVar i:=0;

numberVar Segments:= IDAutomationQRCodeEncoderQRSet(DataToEncode,0,0,0,0 );

For i:=0 to Segments Do

(

CompleteBarcodeString:= CompleteBarcodeString + IDAutomationQRCodeEncoderQRGet(i);

);

CompleteBarcodeString

Finally, include the formula on the report with the new TrueType-Font „IDAutomation2D“.

#### Parameter of function IDAutomationQRCodeEncoderQRSet

Parameter of function IDAutomationQRCodeEncoderQRSet (<Data>, <Process Tilde>, <Error Correction>, <Encoding Mode>, <Version>):

- Process Tilde: 1 = True; Ehen true, ~d013 = return and ~d009=tab

- Error Correction: 0=M, 1=H, 2=L and 3=Q

- Encoding Mode: 0=Byte, 1=Alpha-Numeric and 2=Numeric

- Version: 0=Auto

## Tools

### Calculate Checksum for an Interleave 2/5 Barcode

Wirth the follow INFORMIX Function you can calculate the checksum of your Interleave 2/5 Barcode with 9 digits.

CREATE FUNCTION cu_CheckSumInterleaved2of5 (spBarcode CHAR(9))

RETURNING CHAR(1);

DEFINE spDigit CHAR(1);

DEFINE spChecksum CHAR(1);

DEFINE spCounter, spSum INTEGER;

LET spSum = 0;

IF LENGTH(spBarcode) = 9 THEN

FOR spCounter = 1 TO LENGTH(spBarcode) STEP 1

LET spDigit=SUBSTR(spBarcode, spCounter, 1);

--rechnet die Summe von allen Zeichen mit Koeffizienten

LET spSum=spSum + (1+2*MOD(spCounter,2))*spDigit;

END FOR;

LET spSum=MOD(spSum,10);

IF spSum<>0 then LET spSum=10-spSum; END IF;

LET spChecksum=spSum;

ELSE

LET spChecksum='0';

END IF;

RETURN spChecksum;

End FUNCTION;

### Calculate CODE 128 with CR Report Function

*Example from WT*

Function  (stringVar TheLabel)

TheLabel:= TrimLeft (TheLabel);

Local NumberVar TheLabelLen:= Length (TheLabel);

Local NumberVar i;

Local NumberVar TarDigit:= 104;

Local NumberVar CheckSum:= TarDigit;

Local StringVar Target:= CHR (32+TarDigit);

Local NumberVar TarPos:= 1;

For i:= 1 To TheLabelLen Do

(

Local NumberVar SrcDigit;

SrcDigit:= ASC (TheLabel [i]);

If SrcDigit < 32 OR SrcDigit >= 122 THEN SrcDigit = 32;

SrcDigit:= SrcDigit -32;

Target:= Target + CHR (32 + SrcDigit);

CheckSum:= CheckSum + TarPos * SrcDigit;

TarPos:= TarPos + 1;

);

Target:= Target + CHR (32 + CheckSum MOD 103);

Target:= Target + CHR(32 + 106);

Target;

## Troubleshooting

### Barcode troubles on a PDF export

If you export your report into a PDF, it could happen that the barcode is too small or is missing.

Create the registry DWORD parameter [.\Crystal Reports\Export\PDF\ForceLargerFonts] in HKLM and HKCU and set value to 1. Where the parameter is stored depends on the crystal reports version, e.g:

[.\Business Objects\Suite 11.0\Crystal Reports\Export\PDF]
[.\Business Objects\Suite 11.5\Crystal Reports\Export\PDF]
[.\Business Objects\Suite 12.0\Crystal Reports\Export\PDF]
[.\SAP BusinessObjects\Crystal Reports for.NET Framework 4.0\Crystal Reports\Export\PDF]