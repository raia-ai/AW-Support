---
description: "EN INST A+W Smart Companion"
---



# EN INST A+W Smart Companion

    Installation Instructions


A+W Smart Companion




                                english
Change history

          Date      Author   Remarks            Version
          2022-07-22 ABE     Original version   0.1
Contents

1.   Establishing connection to the back end                         4
2.   Installation on the end user device                            5
     2.1. Zebra TC20                                                5
                  WLAN                                              5
                  Barcode types                                     6
     2.2. Installation of the A+W Smart Companion                   8
                  Smart Device iOS                                  8
                  Smart Device Android                              9
                  Smart Device Android via USB                      9
3.   Troubleshooting                                                13
     3.1. Trace files on the device                                 13
                 Android (Zebra)                                    13
                 iPhone                                             13




A+W Software GmbH                EN-INST-A+W Smart Companion.docx        3
1. Establishing connection to the back end
In order to connect to the back end, of course the A+W Smart Companion must be installed on
the device. The installation is described starting from Chapter 2.
When the A+W Smart Companion is started for the first time, first you have to connect to the
back end.




The "Device name" must be a unique name for the location of the end user device. This is not yet
the "ScannerID," which is used later for the PDC bookings.


In the "Service locator" field, you enter the IP address for the back end. Generally, this is the IP
address of the process server. After that, the device waits for confirmation from the back end:




Note 1: If you enter only the IP address in the Service locator field, the port 12003 is used as
default.
After you have installed A+W Smart Companion and entered a valid backend service, A+W Smart
Companion waits for a license assignment for the device. To do this, simply contact your PS
employee. If you are in the project status, it is a service case then please contact a CS employee.




The scanner was activated. It continues automatically and the app is available.


A+W Software GmbH                 EN-INST-A+W Smart Companion.docx                                     4
2. Installation on the end user device
The installation is a little different depending on the device type. The supported device types will
be described below.


A few basic settings are necessary on each end user device:


    -   WLAN: Must be set up so that the scanner has access to the A+W Process-Server on
        which the infrastructure services are running. Since these settings are very different for
        most end user devices and depend heavily on the customer's network structure, these
        settings will only be described roughly here.



2.1. Zebra TC20
The advantage of the Zebra TC20 is that it can enter barcodes both with an installed camera as
well as with a 2D laser scanner. Furthermore, in addition to the A+W Smart Companion, the
device can also be used for the CimBarcoding solution as well as for the A+W Barcode Manager
(EL) (in A+W Business).


         WLAN
                                                 Select gear for "Settings"




                                                 Select desired WiFi connection




                                                 Enter Password.

                                            CAUTION: There is a "slider" on the right edge of this
                                            field. If you have to enter additional network settings
                                            such as encryption, pass phrase, etc. manually, you
                                            can scroll upwards in this dialog (type on Password
                                            and swipe up).




A+W Software GmbH                 EN-INST-A+W Smart Companion.docx                                     5
                                           You can also reach this dialog by pressing longer on
                                           an existing WLAN connection and selecting "modify
                                           network" from the context menu.


         Barcode types
With this setting, the scanner is restricted to the barcode types that are supported by the A+W
software. This section describes only the minimum settings that must be activated or set.


                                               If you swipe from bottom to top on the
                                                scanner display, an overview of the available
                                                APPs appears.
                                               Here, select the "Data Wedge" app




                                               Select default profile Profile 0




A+W Software GmbH                EN-INST-A+W Smart Companion.docx                                 6
                               Activate Profile enabled
                               Activate Barcode input




                               Select Decoders menu and activate the
                                following barcode types:
                                Code 128
                                Code 39
                                Interleaved 2/5
                               On the Decoder params menu, make the
                                following settings for the code Interleaved 2/5


                                Barcode Input
                               Checkdigit = USS Check Digit
                               Length1 = 8
                               Length2 = 10
                               Redundancy = activated
                               Report Check Digit = deactivated




A+W Software GmbH   EN-INST-A+W Smart Companion.docx                              7
                                          As of Android version 8, this setting is also
                                          required

                                          Keystroke output
                                           Inter character delay = 10 ms




2.2. Installation of the A+W Smart Companion
        Smart Device iOS
The A+W Smart Companion can be downloaded for iOS devices from the Appstore with the
following barcode.




A+W Software GmbH             EN-INST-A+W Smart Companion.docx                            8
         Smart Device Android
The A+W Smart Companion can be downloaded for Android devices from the Playstore with the
following barcode.




         Smart Device Android via USB
Installation
On Android devices, the A+W Smart Companion can also be installed via USB. For this, the scanner
must be connected with a USB cable to a PC/notebook. As soon as the scanner is connected, you
will see a small TC20 symbol in the Explorer:



So that you can also transfer data, you first have to activate this on the scanner:

                                                 Swipe from top to bottom on the display
                                                 Touch the Device will be loaded via USB
                                                  message




A+W Software GmbH                 EN-INST-A+W Smart Companion.docx                            9
                                                Activate Transfer files


                                           After that, you should also recognize the drives on
                                           the scanner in the Explorer of the PC/notebook:




                                                In the folder:
                                                 Interner gemeinsamer Speicher
                                                 or
                                                 internal shared storage
                                                 the file Smart Companion.apk is copied (the
                                                 file name plays no role here)
                                                 (apk=Android Package)

                                                From the app view (swipe from bottom to
                                                 top), select the File browser.


                                                Select the internal folder here



                                                Now start the SmartCompanion.apk file and
                                                 follow the instructions



                                                After successful installation, you will find the
                                                 A+W Smart Companion in the APP overview
                                                By touching and holding, you can store it on
                                                 the scanner's desktop. From there, you can
                                                 start the A+W Smart Companion.

                                                Answer the question Allow Smart
                                                 Companion to Phone with ALLOW.
                                                 Otherwise, the device-ID will not be
                                                 transferred to the back end and the device
                                                 cannot be used.



After successful installation, the connection to the back end must be established.

Update



A+W Software GmbH                EN-INST-A+W Smart Companion.docx                                   10
If the A+W Smart Companion was installed via USB, an update must be done manually. The
following steps are required for this:


                                               Note the Device name. This is important since
                                                you have to assign the same Device name
                                                after the new installation! You can find the
                                                device name in the A+W Smart Companion on
                                                the Settings page under Configuration




                                               Then the already installed A+W Smart
                                                Companion has to be uninstalled. You can do
                                                this by pressing and holding the A+W Smart
                                                Companion icon and dragging it to the trash
                                                can in the upper right corner.




The installation in the new version is then done according to Installation of the A+W Smart
Companion.
Reset
This chapter describes possibilities for resetting the A+W Smart Companion.


                                                Select gear for "Settings"




                                                Select APPS entry


                                                Select the A+W Smart Companion app




A+W Software GmbH                EN-INST-A+W Smart Companion.docx                             11
                                UNINSTALL: Uninstalls the application
                                 (necessary for a manual reinstallation)

                                FORCE STOP: Ends the application
                                 (necessary in case the application hangs)

                                With Storage, you can manage the storage:




                                CLEAR DATA: Deletes all data stored by the
                                 A+W Smart Companion (logs, offline
                                 readings, PDC master data, settings (Service
                                 Locator), etc.)

                                CLEAR CACHE: Deletes only the data in the
                                 cache (logs, offline readings, PDC master
                                 data, etc.)




A+W Software GmbH   EN-INST-A+W Smart Companion.docx                            12
3. Troubleshooting
3.1. Trace files on the device
Starting with Version 2.1, trace files are written on the devices. Depending on the type of the
device, these can be read out differently.



         Android (Zebra)
File Explorer application on the device
Internal Storage -> Android/data/com.aw.smartcompanion[.development]/files/Logging


20210304.txt
20210303.txt
…



         iPhone
Accessible only via iTunes




A+W Software GmbH                EN-INST-A+W Smart Companion.docx                                 13
A+W Software GmbH   EN-INST-A+W Smart Companion.docx   14

