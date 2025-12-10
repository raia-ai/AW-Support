---
title: "Wireless Dome Button"
source: "Wireless_Dome_Button.pdf"
tags: ["wireless button", "dome button", "USB dongle", "H0730", "Key Configurator", "user manual", "hardware", "CompuPhase"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A user manual for the CompuPhase Wireless Dome Button. It covers first-time setup, configuration using the Key Configurator utility, battery replacement, mounting options, and technical specifications."
long_description: "This document provides comprehensive instructions for the CompuPhase 'Wireless Dome Button,' a large mushroom-style button that transmits press and release operations to a PC via a 'Wireless Dongle.' The manual details the initial setup process, which involves pairing the button with an H0730 model dongle using a specific pin code. It explains how to use the 'Key Configurator' software to customize the button's function, including setting it to 'Auto-repeat,' 'Pulse,' or 'Macro' mode to transmit single keystrokes, repeated keys, or complex key sequences. The guide also covers practical aspects such as replacing the CR123 battery, mounting the button temporarily on a tripod or permanently with screws, and resetting the dongle. Technical specifications are provided, covering mechanical dimensions, electronic interface details (battery life, power consumption), operating conditions, and conformity with EU directives (RED, EMC, RoHS)."
---

# Wireless Dome Button

*Image of a red dome button and a USB wireless dongle.*

**CompuPhase**  
Eerste Industriestraat 19  
1401VL Bussum, Netherlands

*FC CE Compliance Marks*

---
## Introduction

The "wireless Dome Button" is a large mushroom/dome button that transmits press and release operations to a workstation or PC, with the help of a "Wireless Dongle". Up to six Wireless Buttons may be attached to a dongle.

The Wireless Button requires a H0730 model dongle for reception.

The dongle is inserted in a USB port, and reports itself as a "Human Interface Device" (HID). Microsoft Windows and other operating systems have intrinsic support for HIDs. No drivers are necessary.

Specifically, the Wireless Dome Button implements a "keyboard" HID function. The key to transmit to the PC is configured via a configuration utility (see the section "Configuring the Wireless Button").

## First time use

Before the Wireless Button can be used, it must be attached to a Dongle. Please follow these steps:

1.  Insert the Dongle in the PC.
2.  Launch the "Key Configurator" utility. Download the Key Configurator from: [http://www.compuphase.com/usbkey/](http://www.compuphase.com/usbkey/)
3.  Verify that the utility detects the Dongle.
4.  Press and release the Wireless Button.
5.  The utility scans for buttons. For a new Wireless Button, it pops up a dialog.
6.  Enter the pin code for the Button. The pin-code is printed at the bottom of the Button.

The Wireless Button is now attached to the Dongle. You may proceed configuring the Button.

## Configuring the Wireless Button

The "Key Configurator" utility is available from [http://www.compuphase.com/usbkey/](http://www.compuphase.com/usbkey/).

*[Image of the Key Configurator 2.0 utility interface, showing options for Model, Button, Layout, Mode, Key, Shift keys, and LED mode.]*

The utility configures only a single button at a time. The serial number, at the top right, shows which button is being configured.

You may need to press a Wireless Button before the Key Configurator detects and recognizes it.

If not using a US keyboard layout, please select the appropriate layout of the keyboard (QWERTY/AZERTY).

The mode can be "Auto-repeat", "Pulse" or "Macro".
- In **auto-repeat mode**, the key-code is repeated when the Wireless Button is kept pressed down (just like a key on the keyboard repeats when you hold it down).
- In **pulse mode**, the key-code is transmitted once; it does not repeat.
- In **macro mode**, you can specify a sequence of keys to be transmitted. For the syntax of macro mode, please see the Help function in the Key Configurator application.

After changing the configuration, you must click on **Apply** to store the settings in the USB button.

To test a Wireless Button, the Key Configurator must first be closed, so that the buttons toggle back from configuration mode to normal mode.

## Re-attach buttons / reset dongle

To reset a Wireless Dongle to factory defaults or to attach a Button previously attached to a different Dongle, please see the Help function in the Key Configurator.

## Starting programs or commands

In Microsoft Windows, the `Win` + `R` key combination shows the "Run" dialog. In "macro" mode, you can pop up this dialog with the key sequence `"#R"`. You can follow this by a command and then `"{ENTER}"` at the end to execute it. Other operating systems support similar functions, but may require a different key combination to pop up a "Run" dialog.

In addition, the Wireless Button supports several consumer control functions, like play, pause and others. These require auto-repeat or pulse modes.

## Replacing the battery

The indicator at the front briefly flashes at each button press. If the indicator flashes red (instead of green), the battery is low.

*[Diagram showing how to unscrew the top dome part from the base of the button.]*

Unscrew the top part of the button from the base to get access to the battery. Replace the battery with a Lithium Metal 3V CR123 size battery (also called 123A or A123 size).

## Temporary or permanent mount

The Wireless Button has a 1/4-20 UNC thread for mounting on a (camera) tripod or a (microphone) stand.

Alternatively, the base of the button has two mounting holes/slots for a permanent mounting (see the arrows in the picture below).

*[Diagram showing the underside of the button base with two mounting holes indicated by arrows.]*

To get access to the two mounting holes in the base, the first step is to unscrew the top part of the button from the base (see the picture on page 6).

The mounting holes are suitable for 4 to 4.5 mm screws. After the base is fixed on the table or wall, remount the top part of the button.

## Specifications

### Mechanical
- **Dimensions:** Base: 85×85 mm, height: 45 mm, dome diameter: 94 mm; total height: 101 mm.
- **Colour:** Base: black & grey; dome: red, black, green, yellow or white.
- **Mechanical lifespan:** > 10⁶ operations.
- **Protection level:** IEC/EN 60529: IP65, IP67.
- **Actuation force:** 20 to 25 N.

### Operating conditions
- **Operating temperature:** -25 °C to +40 °C.
- **Humidity:** 5% to 95% non-condensing.

### Electronic interface
- **Operating voltage:** 3.0 V, battery powered (CR123 Lithium battery).
- **Battery lifetime:** > 5 years in normal use.
- **Current:** 5 µA nominal while idle; 35 mA nominal during transmission.
- **Debounce criterion:** 20 ms stable period.
- **Switch latency:** 50 ms maximum, 35 ms average.
- **Radio frequency:** 868 MHz or 915 MHz, depending on model.
- **Transmission range:** > 30 meters outdoors (unobstructed line of sight).

### Conformity
- **Radio Equipment Directive (RED):** Compliant with EU Directive 2014/53/EU:
  - ETSI EN 301 489-3:2002 V1.4.1
  - ETSI EN 300 220-2:2012 V2.4.1
  - ETSI EN 300 220-1:2012 V2.4.1
- **EMC:** Compliant with EU Directive 2014/30/EU: EN 55022 and EN 55024 + A1 (2001) + A2 (2003).
- **Electrical safety:** Compliant with EU Directive 2014/35/EU: EN 60950-1.
- **RoHS:** Compliant with EU Directive 2011/65/EU: EN 50581:2012.

## Legal disclaimer

CompuPhase shall not be liable for the incidental or consequential losses or damage to tangible property, injury or death of a person in connection with the use of this device.
