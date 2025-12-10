---
title: "Wireless Button Dongle"
source: "Wireless_Button_Dongle.pdf"
tags: ["Wireless Button", "USB Dongle", "Key Configurator", "HID", "Macro", "ITB CompuPhase", "User Manual"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A user guide for the ITB CompuPhase Wireless Button Dongle. It explains how to connect the dongle and button, configure the button's function using the Key Configurator utility, and details the device's specifications and compliance information."
long_description: "This document serves as a comprehensive user manual for the Wireless Button Dongle from ITB CompuPhase. It details the setup and configuration process for the device, which functions as a Human Interface Device (HID) keyboard. The guide covers the initial introduction, explaining that the dongle requires no special drivers and can be paired with up to six wireless buttons. It provides step-by-step instructions on connecting a button to the dongle using the 'Key Configurator' utility, which is available for download. The manual explains how to configure each button's behavior, including setting the mode to 'Standard' (repeats key press), 'Pulse' (single key press), or 'Macro' (a sequence of keys). It also includes information on starting programs or commands using key combinations, re-attaching buttons, or resetting the dongle. The document concludes with detailed specifications covering mechanical, operating, and electronic aspects, as well as compatibility, conformity, and legal disclaimers."
---

# Wireless Button Dongle

*Image of a red wireless button and a USB dongle.*

**ITB CompuPhase**
Eerste Industriestraat 19-21
1401VL Bussum, The Netherlands
FC CE

---

---
## Introduction

The Wireless Dongle is inserted in a USB port. The workstation recognizes it as a "Human Interface Device” (HID), and specifically as a keyboard. Microsoft Windows and other operating systems have intrinsic support for HIDs. No drivers are necessary.

The key to transmit to the PC is configured via a configuration utility (see the section "Configuring the Wireless Button").

Up to six Wireless Buttons may be attached to a dongle. Each button is configured separately.

---

## Connect a button to the dongle

1.  Insert the Dongle in the PC.
2.  Launch the "Key Configurator" utility. (http://www.compuphase.com/usbkey/)
3.  Verify that the utility detects the Dongle.
4.  Press and release the Wireless Button.
5.  The utility scans for buttons. For a new Wireless Button, it pops up a dialog.
6.  Enter the pin code for the button. The pin-code is printed at the bottom of the button.

The Wireless Button is now attached to the Dongle. You may proceed with configuring the Button.

---

## Configuring the Wireless Button

*Image of the Key Configurator utility interface.*

The "Key Configurator” utility is available from http://www.compuphase.com/usbkey/.

The utility configures only a single button at a time. The serial number at the top right shows which button is being configured. This number is also at the bottom of each Wireless Button.

If not using a US keyboard layout, please select the appropriate layout of the keyboard (QWERTY/AZERTY).

The mode can be "Standard", "Pulse" or "Macro".
- In **standard mode**, the Wireless Button repeats a key-code when the button is kept pressed down (just like a key on the keyboard repeats when you hold it down).
- In **pulse mode**, the button automatically releases the key-code; it therefore does not repeat.
- In **macro mode**, you can specify a sequence of keys to be transmitted. For the syntax of macro mode, please see the help file in the application.

After changing the configuration, you must click on **Apply** to store the settings in the USB button.

To test a Wireless Button, the Key Configurator must first be closed, so that the buttons toggle back from configuration mode to normal mode.

---

## Re-attach buttons / reset dongle

To reset a Wireless Dongle to factory defaults or to attach a Button previously attached to a different Dongle, please see the Help function in the Key Configurator.

---

## Starting programs or commands

In Microsoft Windows, the `Win` + `R` key combination shows the "Run" dialog. In "macro" mode, you can pop up this dialog with the key sequence "#R". You can follow this by a command and then “{ENTER}” at the end to execute it. Other operating systems support similar functions, but may require a different key combination to pop up a “Run” dialog.

In addition, the Wireless Button supports several consumer control functions, like play, pause and others. These require standard or pulse modes.

---

## Specifications

### Mechanical
- **Dimensions**: 67×23×9 mm
- **Colour**: Off-white (light gray)

### Operating conditions
- **Operating temperature**: -25 °C to +40 °C
- **Humidity**: 5% to 95% non-condensing

### Electronic interface
- **Operating voltage**: 5.0 V, powered through USB
- **Current**: 35 mA nominal
- **USB interface**: 2.0, full-speed
- **Radio frequency**: 868 MHz or 915 MHz, depending on model
- **Transmission range**: > 30 meters outdoors (unobstructed line of sight)

---

## Compatibility

Compatible with Microsoft Windows® XP and later, Macintosh®, and Linux. No client-side software is needed. (Free configuration software requires Windows® operating system).

---

## Conformity

- **Radio Equipment Directive (RED)**: Compliant with EU Directive 2014/53/EU:
  - ETSI EN 301 489-3:2002 V1.4.1
  - ETSI EN 300 220-2:2012 V2.4.1
  - ETSI EN 300 220-1:2012 V2.4.1
- **EMC**: Compliant with EU Directive 2014/30/EU: EN 55022 and EN 55024 + A1 (2001) + A2 (2003).
- **Electrical safety**: Compliant with EU Directive 2014/35/EU: EN 60950-1
- **RoHS**: Compliant with EU Directive 2011/65/EU: EN 50581:2012.

---

## Legal disclaimer

ITB CompuPhase shall not be liable for the incidental or consequential losses or damage to tangible property, injury or death of a person in connection with the use of this device.
