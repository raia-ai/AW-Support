---
title: "EN CONFIG A+W Smart Companion"
category: "configuration"
product: "A+W Smart Companion"
doc_type: "Configuration"
language: "EN"
tags: ["CONFIG", "A+W Smart Companion"]
version: "1.0"
last_updated: "2025-12-10"
description: "Configuration   A+W Smart Companion                                   english                           - -INTERNAL- Change history          Date      Author   Remarks                                             Version         2019-05-09 PK      Beta release                                        0.1         2019-11-27 PK      Installation via AppStore or PlayStore              1.0         2022-07-22 ABE     Content split into configuration and installation   2.0"
source_file: "EN-CONFIG-A+W Smart Companion.pdf"
---


# EN CONFIG A+W Smart Companion

    Configuration


A+W Smart Companion




                              english




                      - -INTERNAL-
Change history

        Date      Author   Remarks                                             Version
        2019-05-09 PK      Beta release                                        0.1
        2019-11-27 PK      Installation via AppStore or PlayStore              1.0
        2022-07-22 ABE     Content split into configuration and installation   2.0
                           Information about token switches and other
        2023-11-07 SWI                                                         3.0
                           innovations added
        2025-02-20 DIH     New test devices and discontinuation of TC20        4.0
Content

1.   Introduction                                                    4
     1.1. Benefits                                                   4
     1.2. Limitations                                                4
2.   Hardware requirements                                           5
3.   Installation of the back end                                    6
4.   Licensing                                                      7
     4.1. Applying for license in the administration                7
     4.2. Entering license in the back end                          7
     4.3. Establishing connection to the back end                   7
          4.3.1. Demo mode                                          8
     4.4. Confirming end user device in the back end                8
     4.5. Configuration of the devices in the back end              9
5.   Installation on the end user device                            14




A+W Software GmbH              EN-CONFIG-A+W Smart Companion.docx        3
1. Introduction
A+W Smart Companion is a scanner solution that was developed to use a smartphone as
hardware. Because handling the camera as barcode scanner may be something that users have
not done before, the A+W Smart Companion also supports a scanner (Zebra TC20), which is
equipped with both a camera and a 2D barcode scanner. The user can decide which method he
would like to use to read barcodes.


1.1. Benefits
   •   The application is independent of the hardware as long as you use the camera as barcode
       reader and the hardware requirements described below are fulfilled.
   •   Currently the iOS and Android operating systems are supported
   •   Easy configuration and installation
   •   Communication is bidirectional (scanner -> back end, back end -> scanner)
   •   Better user guidance
   •   Fewer errors
   •   Connection of various barcode systems planned in the future (AWP, AWB, AWE)


1.2. Limitations
   •   For installation, the device requires an internet connection
   •   No support for QuantityPDC (A+W Serial Manager)
   •   For initial authentication and verification at least once a year, requires an internet
       connection




A+W Software GmbH              EN-CONFIG-A+W Smart Companion.docx                               4
2. Hardware requirements
The A+W Smart Companion makes the following minimum requirements of the hardware:
                                                                 iOS                  Android
        Operating system                                       iOS 13                    6.0
        Minimum display size [pixels]                        1136 x 640               800 x 480
        Minimum screen resolution [pixels/inch]                  326                     217
        Minimum computing power [MHz]                           1840                     1400


Current test devices:

                            Height Width         Display     with Camera         Test
             Device                                                                                 OS
                            [mm] [mm]            [pixel]     [ppi] [Mpixel]     device

    iPhone 8                  138.1     67.0   1334 x 750     326          12     C        iOS 16
    iPhone SE2                138.3     67.1   1334 x 750     326          12     C        iOS 18
    iPhone XR                 150.9     75.7   1792 x 828     326          12     C        iOS 18
    iPhone 12                 146.7     71.5   2532 x 1170    460          12     D        iOS 18
    iPhone 13                 146.7     71.5   2532 x 1170    460          12     D        iOS 17
    Samsung S22 Ultra         163.3     77.9   3088 x 1440    500         108     D        Android 14
    OnePlus 7T                160.9     74.4   2400 x 1080    402          48     D        Android 12
    OnePlus 9Pro              163.2     73.6   2960 x 1440    525          48     D        Android 13
    Pixel 8Pro                162.6     76.5   2992 x 1344    489          48     D        Android 14
    Zebra TC20                134.0     73.1    800 x 480     217           8     C        Android 8.1
    Zebra TC21                158.0     79.0   1280 x 720     294          13     D        Android 11
    Zebra TC22                165.0     76.3   2160 x 1080    402          16     D        Android 13
    •     Test device: D = Daily, C = Compatibility


Note: Since both the Android versions (6/7/8) will be
discontinued by Google in the next few years and the display and
CPU of the TC20 are no longer up to date, support for this device
will end in 2026 from our side. Please do not actively deploy the
TC20 to customers and encourage them to update existing
devices promptly.



A+W Software GmbH                 EN-CONFIG-A+W Smart Companion.docx                                5
3. Installation of the back end
The following A+W modules are required in order to use the A+W Smart Companion:
The following infrastructure set-ups must be present somewhere on the network (normally on the
process server). These set-ups are included in the "A+W Infrastructure Process Server" diskset.
    •   A+W Infrastructure 6 Collector Services
    •   A+W Infrastructure 6 Middleware
    •   A+W Infrastructure 6 Service Locator
    •   A+W Infrastructure 6 Services
    •   A+W Infrastructure 6 Web
    •   A+W Infrastructure 6 Workflow Studio

In addition, the following set-ups must be installed in order to execute the scanner software
(normally also on the process server):
    •   A+W Infrastructure 6 Collector Services
    •   A+W Infrastructure 6 Middleware
    •   A+W CIM 6 Barcoding Services
    •   A+W CIM 6 Web
    •   A+W Planning 6 Job Services

If the Stock Module should also be used, then the following services are added in the Unix/Linux
or AWB environment:
    •   A+W Commercial Purchase
    •   A+W Commercial Stock


Follow the installation instructions for these set-ups and set the correct database connection in
A+W Infrastructure 6 Web (start A+W Infrastructure 6 Web, configuration, A+W Production,
database connection).




A+W Software GmbH               EN-CONFIG-A+W Smart Companion.docx                                  6
4. Licensing
Start-up is done in several steps:
      a) apply for license in the administration
      b) enter license in the back end
      d) establish connection to the back end
      e) confirm end device in the back end


4.1. Applying for license in the administration
For a new order of the module: "264101 A+W Smart Companion Basic License," a license key
must be requested from F&A via e-mail to sw-contractmanagement@a-w.com. The license key
consists of a very long cryptic text. Example:
„AQBs7RzoA1B+AW7EzBYuwvM1s1vGFrY/HXtGbIxHzWR5Mh44AkStk1R6eq6kFsxMkRHsjjBS+tgQL
euqHFtS7mFgXaoQUPc3ngAjeb428fSLcf7rRkc58O5MP+y7CYOlvEaW+otZfgFFAKFDhB7URpMS0yz1
l/c5REcCzSH6iyfUt/LQwKjYRGdo5Xq7UT7CZxzHRPqh80h6zwOYMbjCogZPOOup+FVu8f6s2Q9OweJ
AxnT2sWMO90lL1aJhcgZ7nZK/xIoknejsiuYC0T29YgyDyITM4j2rhxl1W3eDDtzgySda+1qttAZyUeXVS
GQa48HpBlvbieZNKcYF9MnvhdjpNksDp3BZNNZYuwi/eqqQpNqhYzLo35cSyNV846F1ggADm7buwV
wPVqY7gfVyLYqZHNvtMZWOXm5KKvtPREjdM1MNgFwd004BNf/+4TBl8MGTpPXNPeW0VoSOpuH
E7W5cn3FT9xw3L6QRLgMrBB3LKRi5NRhk+2vdboTqACWo0wXhSDbWsDgvtHbLNohN/tPbqmx5VJ
ZDZr33vQ4/pbFP4SHJDY9NSG1y2sujtAkEQ3oHQVYY3VNH9IS1rcggtfKJi0xf5uuEWMc6gguAj0cUDz
mXUihbsHMxG7Dfu/Zm8dYXvbyJ7ctsDViKBL7pgGGmhpVqpRaiSRceuO6g780WkyU++OmMO880a
nzKOMgxO+sHWqSfp+jjEfwgUWSxcES0W3C5/Ym2OB+WE2bPxnMCdmtlcJuvyhEENw6+mlAXssNy
KpVh29SbQiiL2pL3JpKVK+7JdvlPzQJTtwAv3ZoJoHuuGedGewajlO72Gz2b/fhVzp2dSD+++Q==).


4.2. Entering license in the back end
The customer-specific license key is entered in the infrastructure web. For this, open
A+W Infrastructure 6 Web > License > Foreign License. The following fields must be filled out
here:
     Client            Selection of the correct client.
     Variant           Always "Scandit – (1)" for the Smart Companion.
     Description       Here the <client number> - <customer name> is entered.
     Serial Number     The license key is copied in here.


When everything has been entered, the changes must be confirmed with [Save].


4.3. Establishing connection to the back end
How to connect to the backend is described in detail in the Installation Instructions.



A+W Software GmbH                EN-CONFIG-A+W Smart Companion.docx                             7
4.3.1. Demo mode
If you enter the IP address 0.0.0.0 under Service locator, the scanner is in a demo mode. That is, it
does not need a back end and can only scan specified barcodes. This mode should help Sales
demonstrate the full functional scope of the A+W Smart Companion without establishing a
complete infrastructure. This mock mode is only available in the preview versions (Microsoft
AppCenter) with camera scan. In the live/store version, otherwise an invalid license key is
depicted as an error. This is a security feature, not an error.


4.4. Confirming end user device in the back end
For this, you open: A+W Infrastructure 6 Web > License > Foreign License.
The new device (here Scanner 3) now appears in the lower area under "Devices." The following
fields must be filled:


    Foreign License       Selection of the license to be used from the upper part of the screen.
    Variant               Here always "Scandit – (1)" for the Smart Companion.
    Activation            "Granted – (2)" This confirms or revokes the activation.
    Device Type           None - (0) = Default
                          Camera - (1) = for smartphones
                          HardwareScanner - (2) = for Zebra TC20, if you only want to use the
                          laser scanner
                          Mixed - (3) = for Zebra TC20, the user can set on the settings page
                          whether he wants to use the camera or the scanner.


                          Essentially, this setting only controls whether or not the switch on the
                          settings page is visible to the user.
    Station ID            This is the id that will be used for the bookings in the PDC.
    Device Token          Is the unique identifier for a device and cannot be changed. This
                          identifier can also be queried in the Smart Companion on the settings
                          page under "Info."
    Device Name           The name of the device appears here, as you entered it for the
                          connection to the back end. This entry also cannot be changed.
    Description           Is a text that can be helpful for the identification of the device
    Date                  Is updated by the system for each inquiry. Here, for example, you can
                          see whether a device has not been used for a longer time.


If all fields are filled out correctly and you have confirmed this with the [Save] button, you only
have to enter a password and then, after a brief while, the following message will appears in the
A+W Smart Companion:



A+W Software GmbH               EN-CONFIG-A+W Smart Companion.docx                                    8
Then you can start selecting the actual application.
CAUTION: An A+W employee can apply for the password via e-mail to sw-
contractmanagement@a-w.com and it should in no case be given to the customer!




4.5. Configuration of the devices in the back end




The scanners can be configured differently for each site. For this, select Client at the top right and
then click on the CIM Smart Companion item in the A+W Production area.




A+W Software GmbH               EN-CONFIG-A+W Smart Companion.docx                                   9
   Applications                     Different applications that should be activated in the
                                    SmartCompanion, e.g. Production, Stock, Inventory, etc.
   BackEnd Modes                    Which back-end systems are addressed by the
                                    CIM/Commercial service, e.g. Production, AWE, Cantor,
                                    etc.
   Number of Logs                   How many booking entries are saved on the device per
                                    user (default normal is sufficient)
   ProductionDataAquisitionTypes Which types of RegistrationPoints should be
                                 displayed/used on the device (default normal is sufficient)
   RegistrationPoints Whitelist     If a customer has too displayed many RegistrationPoints
                                    on his device, a "positive" whitelist can be kept here. That
                                    is, only what is entered here is available on the device.
                                    (Can be left blank)
   Rack Inventory Interval          After how many days does a rack inspection conducted
                                    have to be repeated. (Default 730 days)
   Label Printer Group              In which ProcessManager printer group should the rack
                                    labels be printed.
   Label Print Report Path          Complete path to the report with which the rack label is
                                    printed
   Label Print Printer              Which printer should print the rack label
   Tracing Level                    Select between Debug, Info, and Error in order to define
                                    which entries should be written to the logs on the device
   Is Rack Scan Required            If switched on, the user of the Smart Companion must
                                    always scan a rack in the Production module first before a
                                    product can be scanned.
   Barcode Settings                 Which different barcode types are activated (e.g.
                                    Interleave2of5, Code128 etc.) – currently can only be
                                    changed via JSON Down/Upload
   Barcode Classification           Which regular expressions are used for which input types
                                    (Person, RegPoint, Rack, etc.) - currently can only be
                                    changed via JSON Down/Upload




A+W Software GmbH            EN-CONFIG-A+W Smart Companion.docx                                10
   Token Switches         Opens token switches view
   Download               Download all Smart Companion settings as .awconfig file
                          in JSON format
   Upload                 Upload an .awconfig file in order to take over the settings
                          it contains
   Add                    Add new barcode settings or barcode classification
                          entries
   Edit                   Edit an entry under barcode settings or barcode
                          classification directly in the web interface




A+W Software GmbH   EN-CONFIG-A+W Smart Companion.docx                              11
   Delete                 Delete an entry under barcode settings or barcode
                          classification directly in the web interface




A+W Software GmbH   EN-CONFIG-A+W Smart Companion.docx                        12
In the system token management view, settings for the Smart Companion can be made for
individual devices under a site. With Add, new user tokens can be added. Under System Switch,
you can select CIM Smart Companion. In order to assign the settings to a specific device, the
device ID of the device in question must be specified under user token. It can be found under
License > Foreign License. All other settings are the same as the settings on the main page of the
Smart Companion configuration. You can switch back to this view with System Switch.




A+W Software GmbH               EN-CONFIG-A+W Smart Companion.docx                               13
5. Installation on the end user device
How to install the A+W Smart Companion on the end device is described in detail in the
Installation Instructions. Also troubleshooting.




A+W Software GmbH              EN-CONFIG-A+W Smart Companion.docx                        14

