---
title: "EN-INST-AW_Smart_Companion"
source: "EN-INST-AW_Smart_Companion.pdf"
tags: ["A+W", "Smart Companion", "Installation", "Zebra TC20", "Android", "iOS", "Software", "Glass Industry", "Barcode Scanner", "Troubleshooting"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "An installation guide for the A+W Smart Companion application on various end-user devices, including Zebra TC20, iOS, and Android. It covers initial setup, backend connection, device-specific configurations, and troubleshooting steps."
long_description: "This document provides comprehensive installation instructions for the A+W Smart Companion software, a tool designed for the glass industry. It details the entire process from establishing a connection to the backend server to installing the application on different types of devices. The guide offers specific instructions for the Zebra TC20 scanner, including WLAN setup and barcode type configuration. It also explains how to install the app on iOS devices via the App Store and on Android devices through the Google Play Store or via a direct USB connection. The manual includes step-by-step procedures with screenshots for clarity. Additionally, it covers updating a manually installed application, resetting the app to its default state, and troubleshooting common issues, such as accessing trace files on both Android and iPhone devices for support purposes."
---

# A+W Installation Instructions: A+W Smart Companion

**A+W - Software for Glass**

---
### Change history

| Date       | Author | Remarks          | Version |
| :--------- | :----- | :--------------- | :------ |
| 2022-07-22 | ABE    | Original version | 0.1     |

## 1. Establishing connection to the back end

In order to connect to the back end, the A+W Smart Companion must be installed on the device. The installation is described starting from Chapter 2.

When the A+W Smart Companion is started for the first time, you must first connect to the back end.

*   **Device Name**: The "Device name" must be a unique name for the location of the end user device. This is not yet the "ScannerID," which is used later for the PDC bookings.
*   **Service locator**: In the "Service locator" field, you enter the IP address for the back end. Generally, this is the IP address of the process server.

After entering the details and tapping "Connect", the device waits for confirmation from the back end, displaying a "Pending Access Request" status.

> **Note 1:** If you enter only the IP address in the **Service locator** field, the port 12003 is used as default.

After you have installed A+W Smart Companion and entered a valid backend service, A+W Smart Companion waits for a license assignment for the device. To do this, simply contact your PS employee. If you are in the project status, it is a service case; then please contact a CS employee.

Once approved, the status changes to "Access Request Approved". The scanner is then activated, it continues automatically, and the app becomes available.

## 2. Installation on the end user device

The installation is a little different depending on the device type. The supported device types will be described below.

A few basic settings are necessary on each end user device:
*   **WLAN**: Must be set up so that the scanner has access to the A+W Process-Server on which the infrastructure services are running. Since these settings are very different for most end user devices and depend heavily on the customer's network structure, these settings will only be described roughly here.

### 2.1. Zebra TC20

The advantage of the Zebra TC20 is that it can enter barcodes both with an installed camera as well as with a 2D laser scanner. Furthermore, in addition to the A+W Smart Companion, the device can also be used for the CimBarcoding solution as well as for the A+W Barcode Manager (EL) (in A+W Business).

#### 2.1.1. WLAN

1.  Select the gear icon to open "Settings".
2.  Select the desired WiFi connection.
3.  Enter the Password.

> **CAUTION:** There is a "slider" on the right edge of this field. If you have to enter additional network settings such as encryption, pass phrase, etc. manually, you can scroll upwards in this dialog (tap on Password and swipe up).
> You can also reach this dialog by long-pressing on an existing WLAN connection and selecting "modify network" from the context menu.

#### 2.1.2. Barcode types

With this setting, the scanner is restricted to the barcode types that are supported by the A+W software. This section describes only the minimum settings that must be activated or set.

1.  If you swipe from bottom to top on the scanner display, an overview of the available APPs appears.
2.  Here, select the **"Data Wedge"** app.
3.  Select the default profile **Profile 0**.
4.  Activate **Profile enabled**.
5.  Activate **Barcode input**.
6.  Select the **Decoders** menu and activate the following barcode types:
    *   Code 128
    *   Code 39
    *   Interleaved 2/5
7.  In the **Decoder params** menu, make the following settings for the code **Interleaved 2/5**:
    *   **Barcode Input**
    *   **Checkdigit** = USS Check Digit
    *   **Length1** = 8
    *   **Length2** = 10
    *   **Redundancy** = activated
    *   **Report Check Digit** = deactivated
8.  As of Android version 8, this setting is also required under **Keystroke output**:
    *   **Inter character delay** = 10 ms

### 2.2. Installation of the A+W Smart Companion

#### 2.2.1. Smart Device iOS

The A+W Smart Companion can be downloaded for iOS devices from the App Store. You can find it by scanning the provided QR code or searching for it directly.

#### 2.2.2. Smart Device Android

The A+W Smart Companion can be downloaded for Android devices from the Play Store. You can find it by scanning the provided QR code or searching for it directly.

#### 2.2.3. Smart Device Android via USB

**Installation**

On Android devices, the A+W Smart Companion can also be installed via USB. For this, the scanner must be connected with a USB cable to a PC/notebook.

1.  As soon as the scanner is connected, you will see a small TC20 symbol in the PC's Explorer.
2.  To enable data transfer, you first have to activate this on the scanner:
    *   Swipe from top to bottom on the display.
    *   Touch the "Device will be loaded via USB" message.
3.  In the "Use USB to" dialog, select **Transfer files**.
4.  After that, you should recognize the drives on the scanner in the Explorer of the PC/notebook.
5.  In the folder `Interner gemeinsamer Speicher` or `internal shared storage`, copy the `Smart Companion.apk` file (the file name plays no role here).
6.  From the app view on the device (swipe from bottom to top), select the **File browser**.
7.  Select the **internal** folder.
8.  Now start the `SmartCompanion.apk` file and follow the installation instructions.
9.  After successful installation, you will find the A+W Smart Companion in the app overview. By touching and holding, you can add it to the scanner's desktop. From there, you can start the A+W Smart Companion.
10. Answer the question **Allow Smart Companion to Phone?** with **ALLOW**. Otherwise, the device-ID will not be transferred to the back end and the device cannot be used.

After successful installation, the connection to the back end must be established.

**Update**

If the A+W Smart Companion was installed via USB, an update must be done manually. The following steps are required for this:

1.  Note the **Device name** from the A+W Smart Companion settings page under `Configuration`. This is important since you have to assign the same Device name after the new installation.
2.  Then the already installed A+W Smart Companion has to be uninstalled. You can do this by pressing and holding the A+W Smart Companion icon and dragging it to the trash can in the upper right corner.
3.  The installation of the new version is then done according to the instructions in **Installation of the A+W Smart Companion**.

**Reset**

This chapter describes possibilities for resetting the A+W Smart Companion.

1.  Select the gear icon for "Settings".
2.  Select the **APPS** entry.
3.  Select the **A+W Smart Companion** app.
4.  In the `App info` screen, you have several options:
    *   **UNINSTALL**: Uninstalls the application (necessary for a manual reinstallation).
    *   **FORCE STOP**: Ends the application (necessary in case the application hangs).
    *   **Storage**: Tap this to manage the storage.
5.  In the `Storage` screen, you can manage the data:
    *   **CLEAR DATA**: Deletes all data stored by the A+W Smart Companion (logs, offline readings, PDC master data, settings (Service Locator), etc.).
    *   **CLEAR CACHE**: Deletes only the data in the cache (logs, offline readings, PDC master data, etc.).

## 3. Troubleshooting

### 3.1. Trace files on the device

Starting with Version 2.1, trace files are written on the devices. Depending on the type of the device, these can be read out differently.

#### 3.1.1. Android (Zebra)

Using the File Explorer application on the device, navigate to:
`Internal Storage -> Android/data/com.aw.smartcompanion[.development]/files/Logging`

You will find log files named by date, such as `20210304.txt`.

#### 3.1.2. iPhone

Trace files are accessible only via iTunes on a computer.

1.  Connect the iPhone to a computer with iTunes.
2.  Select the device icon in iTunes.
3.  In the left sidebar, click on **File Sharing**.
4.  From the list of Apps, select **A+W Smart Companion**.
5.  The documents will appear on the right. Select the **Logging** folder.
6.  Click **Save...** to copy the trace files to your computer.
