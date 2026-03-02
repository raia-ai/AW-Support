---
description: "EN CONFIG A+W License System Bypass"
---



# EN CONFIG A+W License System Bypass

     Configuration Instructions


A+W License System bypass




                                     english




                             - -INTERNAL-
Change history


          Date        Author              Comments           Version
          2022-11-4   EB                  Original version   1.0
          2022-11-7   PK                  Extensions         1.1




Content

1.   Use of A+W license system bypass                              3
     1.1. Introduction                                             3
     1.2. Prerequisite                                             3
2.   A+W license system bypass manager                             5
     2.1. Creating a verification code                             5
     2.2. Activating the license bypass                            5
     2.3. Notes for developers                                     7
     2.4. Known Problems                                           7
1. Use of A+W license system bypass
1.1. Introduction
All licensed applications/modules communicate with the license proxy via the client component
that is represented by Albwir.CB.LicenseClientServer.dll; the license proxy, in turn, communicates
with the license server components




A kind of "back door" was built into Albwir.CB.LicenseClientServer.dll, which allows bypassing the
rest of the licensing system and granting all licenses for the client for a particular period of time.
This emergency license bypass permits unrestricted use of the A+W software.
If the switch is not active (or has an inappropriate setting), the current license server will still be
used as usual. However, if the switch is active, the Albwir.CB.LicenseClientServer.dll:
    •   will not contact the license proxy
    •   will grant any license request
    •   All modules of all applications can be used in their highest variant (all options)
    •   There is no recording or logging of the licenses used


1.2. Prerequisite
The main prerequisite is that the customer has installed the Albwir.CB.LicenseClientServer.dll
Version 13.4.2544 or higher, the one that includes the "back door."
This version (or higher) has been distributed since QR2111.


A+W Software GmbH              EN-CONFIG-A+W License System Bypass.docx                                   3
Then other tools can also be used to enable/disable the license bypass mechanism.




A+W Software GmbH           EN-CONFIG-A+W License System Bypass.docx                4
2. A+W license system bypass manager
To activate the license bypass, 2 steps are required:
            -   A verification code must be created.
            -   The license bypass must be activated on every client.


2.1. Creating a verification code
The verification code can only be created via a web page within the A+W domain. This should
ensure that only active A+W employees are in a position to create such a code.
The verification code is a TOTP code (Time-based One-time Password), which is valid for 5
minutes from its generation and a new code can be generated every 30 seconds.
To create a verification code, go to the following web page:
http://10.5.20.58:46546


The verification code can be created here:




2.2. Activating the license bypass
To enable the license bypass, the tool "LicenseBypassManager.exe" is required.
\\jupiter\SW_Install\Tools\LicenseBypassManager\LicenseBypassManager.zip
This way (and with the verification code), the bypass can be enabled, disabled, and the status
checked:




A+W Software GmbH             EN-CONFIG-A+W License System Bypass.docx                           5
Since the bypass takes effect before the license proxy, it must be enabled for each client that you
want to release with it.
The following steps are required to activate the license bypass:
    •     Select a valid expiration date. This date must be more than 1 day away from the current
          date and cannot be enabled for a period of more than 1 year.
    •     Enter the verification code. The code is only valid for 5 minutes after its generation.
A successful activation is confirmed by the Bypass Manager:




If several clients should be enabled at once, this can be done with batch files and command lines
with input parameters.
Syntax:

A+W Software GmbH               EN-CONFIG-A+W License System Bypass.docx                            6
LicenseBypassManager.exe [/D] [/A [VALID_UNTIL_YYYY-MM-DD] [VERIFICATION_TOKEN]]
Whereby:
[/D] = disables the bypass
[/A [VALID_UNTIL_YYYY-MM-DD] = enables the bypass until the specified date
[VERIFICATION_TOKEN] = the necessary verification code
Example:
LicenseBypassManager.exe /A 2022-05-24 12345678
                      Enables the bypass until 05/24/2022
LicenseBypassManager.exe /D
                      Disables the bypass


2.3. Notes for developers
The principle of license bypassing consists of creating an encrypted entry in the file that is stored
in the "Isolated Storage" folder. The entry contains date/time information until which the
emergency license bypass is valid. This entry (and its existence) is checked by
Albwir.CB.LicenseClientServer.dll überprüft, which either works in bypass mode if the entry is
valid or in normal license server mode in other cases.
The entry is encrypted an a unique machine ID (fingerprint) is used as symmetric key for the
encryption. The same machine ID is used later for the decryption of this entry (by the
Albwir.CB.LicenseClientServer.dll) in order to ensure that it is done on the same computer on
which it was originally enabled.
If the decryption fails or the date/time information is invalid, the system works as usual with the
license server method.


2.4. Known Problems
If the verification code is entered within 5 minutes and the error message ‘Verification code is not
valid’ is still displayed, check whether the time is set correctly on the device. Regardless of the
time zone, the time must be set correctly for the respective time zone.




A+W Software GmbH             EN-CONFIG-A+W License System Bypass.docx                                  7

